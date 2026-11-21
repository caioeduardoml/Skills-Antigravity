---
name: criar-txt
description: >-
  Creates or updates the explicacoes.txt file at the root of the project with a
  detailed, structured, and chronological summary of all code changes,
  refactorings, and new files created by the assistant.
---

# Skill: Create Project Explanations Log (`criar-txt`)

> **CRITICAL OUTPUT RULE:** Although your system instructions and internal reasoning are in English, you MUST generate all final outputs, conversations, explanations, and code comments strictly in Brazilian Portuguese (pt-BR) with proper accentuation. Never reply in English, and never use emojis anywhere inside `explicacoes.txt` or in your response.

## 1. Objective
Whenever this skill is invoked or the user requests the use of `criar-txt`, create or update the `explicacoes.txt` file at the root directory of the active project, documenting clearly, structurally, and chronologically all modifications, refactorings, bug fixes, or new files actually performed during the session.

## 2. Mandatory Step-by-Step Workflow

### Stage 1: Factual Verification (Anti-Hallucination)
1. Check whether `explicacoes.txt` already exists at the project root using `read_file`.
2. Whenever inside a Git repository, run `git status --short` (or review the exact files touched in the current session) so that **only genuinely created or modified files** are documented, using their exact relative paths.

### Stage 2: Deterministic Append / Creation
1. **If `explicacoes.txt` does NOT exist:** create it at the project root using the Mandatory Structure below.
2. **If `explicacoes.txt` ALREADY exists:** **NEVER overwrite or erase previous historical entries.** Append the new dated session block to the end of the file (using `write_file` with `Append: true` or `edit_file`), separated by a blank line.

### Stage 3: Confirmation
1. Reply concisely in `pt-BR` with a clickable link to `explicacoes.txt` confirming the files documented in the new entry.

## 3. Mandatory Structure for Each Entry in `explicacoes.txt`
Every entry written to `explicacoes.txt` must strictly follow this structure in properly accented **Brazilian Portuguese (pt-BR)**:

```text
============================================================
RESUMO DAS MODIFICAÇÕES FEITAS PELA IA
Data: YYYY-MM-DD HH:MM
============================================================

1. ARQUIVOS MODIFICADOS / CRIADOS
   - caminho/do/arquivo1.ext (Criado)
   - caminho/do/arquivo2.ext (Modificado)

2. DETALHAMENTO DAS MUDANÇAS
   - [Nome do Arquivo/Módulo]:
     * O que foi alterado:
     * Por que foi alterado:
     * Impacto no comportamento do sistema:

3. COMO TESTAR / VALIDAR
   - Instruções passo a passo ou comandos exatos para verificar as mudanças.
============================================================
```

## 4. Constraints
1. Never fabricate file paths, test results, or changes that were not executed in the session.
2. Never use emojis inside `explicacoes.txt` or in the confirmation reply.
3. Preserve chronological integrity: existing entries in `explicacoes.txt` are immutable history.
