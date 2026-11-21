# Skills Antigravity

Coleção modular de **12 skills especializadas** para o ecossistema **Google Antigravity**, organizadas por domínio (Engenharia de Software, Web & Design, Segurança & QA, Escrita e Meta-Skills).

Todas as skills seguem o padrão de *Progressive Disclosure* do Antigravity (`SKILL.md` com frontmatter YAML + diretórios auxiliares `references/`, `scripts/` e `data/` quando aplicável), possuem instruções otimizadas para raciocínio determinístico e entregam respostas e comentários de código estritamente em **Português do Brasil (`pt-BR`)**.

---

## Visão Geral Rápida

| Skill | Categoria | Foco Principal | Invocação |
|-------|-----------|----------------|-----------|
| [`dev-flutter-senior`](./dev-flutter-senior/SKILL.md) | Engenharia de Software | Apps Flutter/Dart com Clean Architecture, estado escalável e APIs REST | `/dev-flutter-senior` |
| [`dev-dotnet-senior`](./dev-dotnet-senior/SKILL.md) | Engenharia de Software | APIs e microsserviços em C# 12+ / .NET 8 e 9 no Linux (`dotnet CLI`) | `/dev-dotnet-senior` |
| [`dev-cpp-senior`](./dev-cpp-senior/SKILL.md) | Engenharia de Software | Sistemas de alta performance em C (C99/C11) e C++ Moderno (C++11-23) | `/dev-cpp-senior` |
| [`dev-godot3d-senior`](./dev-godot3d-senior/SKILL.md) | Game Dev 3D | Jogos 3D na Godot 4.x, GDScript 2.0/C#, `AnimationTree` e Vulkan | `/dev-godot3d-senior` |
| [`frontend-expert`](./frontend-expert/SKILL.md) | Web & Frontend | Arquitetura React + TypeScript, Suspense, TanStack Query e performance | `/frontend-expert` |
| [`3d-web-experience`](./3d-web-experience/SKILL.md) | Web & 3D | Three.js, React Three Fiber (R3F), Spline, WebGL e otimização GLB | `/3d-web-experience` |
| [`uiux-designer`](./uiux-designer/SKILL.md) | Design & UX | Design systems, paletas, tipografia, acessibilidade e revisão UX | `/uiux-designer` |
| [`web-launch-auditor`](./web-launch-auditor/SKILL.md) | Qualidade & SEO | Auditoria pré-deploy em 9 pilares (CWV, PageSpeed, SEO, Pixels, IA) | `/web-launch-auditor` |
| [`ciberseguranca`](./ciberseguranca/SKILL.md) | Segurança (AppSec) | Auditoria defensiva multiplataforma (OWASP/MASVS) + Prompt de Remediação | `/ciberseguranca` |
| [`humanizar`](./humanizar/SKILL.md) | Escrita & Revisão | Remoção de padrões de escrita por IA (guia da Wikipédia) em textos/arquivos | `/humanizar` |
| [`criar-txt`](./criar-txt/SKILL.md) | Documentação | Registro cronológico de alterações em `explicacoes.txt` na raiz do projeto | `/criar-txt` |
| [`criarskill`](./criarskill/SKILL.md) | Meta-Skill | Entrevista, arquitetura e criação de novas skills no padrão Antigravity | `/criarskill` |

---

## O Que Cada Skill Faz

### Engenharia de Software e Game Dev

#### 1. `dev-flutter-senior` ([SKILL.md](./dev-flutter-senior/SKILL.md))
Atua como **Engenheiro Mobile Sênior em Flutter e Dart**.
- **O que faz:** Projeta aplicativos do zero (*Full-Cycle*) ou refatora bases existentes em **Feature-First Clean Architecture**, implementa integrações RESTful (`dio`/`http`), modelagem imutável (`freezed`/`json_serializable`), gerenciamento de estado (`Riverpod`, `Bloc/Cubit`, `Provider`) e injeção de dependências (`get_it`).
- **Diferenciais:** Bloqueia widgets monolíticos ("spaghetti widgets"), trabalha com diffs cirúrgicos em arquivos existentes e trata payloads JSON incompletos sinalizando os campos inferidos.

#### 2. `dev-dotnet-senior` ([SKILL.md](./dev-dotnet-senior/SKILL.md))
Atua como **Senior .NET Backend Developer e Cloud Architect** focado em desenvolvimento multiplataforma no **Arch Linux (`dotnet CLI`)**.
- **O que faz:** Desenvolve APIs escaláveis e microsserviços em **C# 12+ e .NET 8/9** com ASP.NET Core, Entity Framework Core, PostgreSQL, SQL Server, Redis, Dockerfiles multi-stage não-root e testes em `xUnit`/`Moq`.
- **Diferenciais:** Escala automaticamente a arquitetura conforme o escopo (**Minimal APIs** para serviços enxutos; **Clean Architecture + CQRS/MediatR** para domínios complexos), proíbe *Fat Controllers*, evita *Captive Dependencies* na DI e exige I/O 100% assíncrono com `CancellationToken`.

#### 3. `dev-cpp-senior` ([SKILL.md](./dev-cpp-senior/SKILL.md))
Atua como **Staff/Senior Software Engineer em C (C99/C11) e C++ Moderno (C++11 a C++23)**.
- **O que faz:** Arquiteta sistemas de alto desempenho, estruturas de dados otimizadas para cache de CPU, multithreading (`std::thread`/`pthreads`), integração com bibliotecas (STL, Boost, Qt, OpenCV), scripts modernos de build (`CMakeLists.txt` / `Makefile`) e diagnóstico de `SIGSEGV`, GDB, Valgrind e Sanitizers no Linux.
- **Diferenciais:** Proíbe "C com Classes" (exigindo RAII, Rule of 0/5/3 e Smart Pointers no C++), impõe structs opacos e funções seguras de string no C puro, declara complexidade Big-O + estratégia de cache e alerta sobre conflitos entre AddressSanitizer e Valgrind.

#### 4. `dev-godot3d-senior` ([SKILL.md](./dev-godot3d-senior/SKILL.md))
Atua como **Senior 3D Game Developer e Technical Artist especializado em Godot 4.x**.
- **O que faz:** Estrutura hierarquias de `Scene Tree`, scripts modulares fortemente tipados em **GDScript 2.0 ou C#**, física 3D (`CharacterBody3D`, `RigidBody3D`), navegação (`NavigationRegion3D`), iluminação Vulkan (`LightmapGI`/`VoxelGI`/`SDFGI`), `GridMap` e pipelines completos de animação (`AnimationPlayer`, `AnimationTree`, `BlendSpace2D`, `StateMachine`).
- **Diferenciais:** Aplica rigorosamente *Composition over Inheritance* ("Call Down, Signal Up"), bloqueia sintaxes legadas da Godot 3, fornece guia visual do `AnimationTree` + Inspector e integra-se ao servidor MCP `godot-ai` quando ativo.

---

### Web, Frontend e Design

#### 5. `frontend-expert` ([SKILL.md](./frontend-expert/SKILL.md))
Atua como **Senior React e TypeScript Frontend Engineer**.
- **O que faz:** Constrói e refatora componentes, hooks, rotas e camadas de consumo de dados com foco em `Suspense`, TanStack Query (`useSuspenseQuery`), lazy loading, TypeScript estrito (zero `any`) e otimização de renderização.
- **Diferenciais:** Inspeciona `package.json` e `tsconfig.json` antes de codificar para respeitar aliases e bibliotecas reais do projeto, e conta com 10 guias detalhados sob demanda na pasta [`references/`](./frontend-expert/references/).

#### 6. `3d-web-experience` ([SKILL.md](./3d-web-experience/SKILL.md))
Atua como **3D Web Experience Architect**.
- **O que faz:** Projeta configuradores 3D, portfólios imersivos, animações sincronizadas com scroll e cenas interativas com **Three.js, React Three Fiber (R3F), `@react-three/drei`, Spline e WebGL**.
- **Diferenciais:** Inclui pipeline de compressão `.glb` com `gltf-transform` (Draco + WebP), orçamento de triângulos/FPS por dispositivo, proteção de SSR no Next.js, fallback para ausência de WebGL e controle de `dpr` em dispositivos móveis.

#### 7. `uiux-designer` ([SKILL.md](./uiux-designer/SKILL.md))
Atua como **Senior UI/UX Designer e Especialista em Design Systems**.
- **O que faz:** Gera sistemas de design completos (estilo, paleta de cores, tipografia, efeitos e antipadrões) e realiza revisões de ergonomia, responsividade e acessibilidade (WCAG) para web e mobile.
- **Diferenciais:** Consulta uma base local pesquisável via [`scripts/search.py`](./uiux-designer/scripts/search.py) e datasets em [`data/`](./uiux-designer/data/) com 50+ estilos, 97 paletas, 57 combinações tipográficas e diretrizes para 12 stacks.

---

### Segurança, Qualidade e Pré-Lançamento

#### 8. `web-launch-auditor` ([SKILL.md](./web-launch-auditor/SKILL.md))
Atua como **Senior Web Performance, Technical SEO e QA Engineer**.
- **O que faz:** Executa uma auditoria pré-deploy (*Pre-Flight Check*) em **9 pilares técnicos**:
  1. *Delayed Pixel Loading* (carregamento assíncrono pós-interação para GA4, GTM, Meta Pixel, Clarity).
  2. Otimização de imagens (`.webp`/`.avif`, `width`/`height`, `fetchpriority="high"` na hero sem `loading="lazy"`).
  3. Prevenção de CLS (`font-display: swap` e dimensões reservadas).
  4. Meta tags individuais (`title`, `description`, `canonical`).
  5. Open Graph e Social Cards (`og:image` absoluta + `twitter:card`).
  6. Dados estruturados **Schema.org (JSON-LD)**.
  7. Responsividade cross-device (`320px` a `1440px+`).
  8. Limpeza de rastros de IA e placeholders (*Lorem Ipsum*, comentários robóticos, imports mortos).
  9. Core Web Vitals (LCP, INP, CLS), semântica de headings (`<h1>` único) e contraste WCAG AA.
- **Diferenciais:** Entrega tabela de status (`[APROVADO]`, `[ALERTA]`, `[CRÍTICO]`) acompanhada do código exato pronto para substituir.

#### 9. `ciberseguranca` ([SKILL.md](./ciberseguranca/SKILL.md))
Atua como **Engenheiro de Cibersegurança e AppSec Sênior** (postura estritamente defensiva).
- **O que faz:** Audita repositórios, manifestos e trechos de código contra a Matriz de Ameaças 2026: **Mobile/OWASP MASVS** (`FLAG_SECURE`, overlays, storage seguro contra stealers, SSL Pinning), **Web/OWASP Top 10** (IDOR, SQLi, XSS, JWT, Rate Limit, CSP/SRI contra skimmers) e **Desktop/Infra** (Path Traversal, menor privilégio, memória segura).
- **Diferenciais:** Classifica achados por severidade (`Crítico`, `Alto`, `Médio`, `Baixo`), aponta arquivo/linha exatos, evita alucinação de CVEs exigindo ferramentas nativas de auditoria e gera um **Prompt de Remediação** pronto para a skill desenvolvedora correspondente.

---

### Escrita, Documentação e Meta-Skill

#### 10. `humanizar` ([SKILL.md](./humanizar/SKILL.md))
Atua como **Editor Sênior de Humanização Textual** (100% em Português do Brasil).
- **O que faz:** Detecta e elimina os 7 grupos de sinais de texto gerado por IA catalogados pela Wikipédia (*Wikipedia:Signs of AI writing* / *Wikipédia:Sinais de texto gerado por inteligência artificial*), ajustando o texto para os tons **Técnico**, **Acadêmico**, **Neutro/Enciclopédico** ou **Conversacional**.
- **Diferenciais:** Preserva intactos blocos de código, LaTeX (`$...$`, `\cite{}`) e citações diretas, limpa parâmetros `utm_source=` de URLs e sinaliza afirmações vagas sem nunca inventar fontes falsas.

#### 11. `criar-txt` ([SKILL.md](./criar-txt/SKILL.md))
Atua como **Registrador Cronológico de Alterações**.
- **O que faz:** Cria ou atualiza o arquivo `explicacoes.txt` na raiz do projeto documentando arquivos criados/modificados, motivação das mudanças, impacto no sistema e passos de validação.
- **Diferenciais:** Verifica as alterações reais via `git status --short` quando aplicável e sempre anexa novas entradas datadas sem apagar o histórico anterior.

#### 12. `criarskill` ([SKILL.md](./criarskill/SKILL.md))
Atua como **Arquiteto Especialista em Skills Antigravity (Meta-Skill)**.
- **O que faz:** Conduz a criação de novas skills em **3 Fases obrigatórias** (Descoberta e Entrevista -> Proposta de Arquitetura + Checagem Anti-Sobreposição -> Desenvolvimento Completo Plug & Play) seguindo os 8 passos oficiais do Codelab Antigravity.

---

## Como as Skills Trabalham Juntas (Sem Sobreposição)

```text
Projeto Web:
  uiux-designer (Design System / UX)
    -> frontend-expert (Arquitetura React/TS) + 3d-web-experience (Cenas WebGL/R3F)
    -> ciberseguranca (Auditoria OWASP + Prompt de Remediação)
    -> web-launch-auditor (PageSpeed, SEO, Pixels, Limpeza pré-deploy)

Projeto Mobile (Flutter):
  uiux-designer (Paleta/Tipografia/UX)
    -> dev-flutter-senior (Clean Architecture / Dart / APIs)
    -> ciberseguranca (Auditoria OWASP MASVS + Prompt de Remediação)

Sistemas / Backend / Games:
  dev-dotnet-senior | dev-cpp-senior | dev-godot3d-senior
    -> ciberseguranca (Auditoria de segurança específica da stack)
    -> criar-txt (Registro em explicacoes.txt)

Documentação e Textos:
  humanizar (Revisão estilística em chat ou arquivos .md/.txt/.tex)
```

---

## Instalação e Uso no Antigravity

1. Clone ou mantenha este repositório no diretório global de skills do Antigravity:
   ```bash
   ~/.gemini/config/skills/
   ```
2. As skills são descobertas automaticamente por *Progressive Disclosure* através do YAML frontmatter de cada `SKILL.md`.
3. Para acionar manualmente, utilize o comando slash ou menção correspondente no chat (ex.: `/dev-flutter-senior`, `/ciberseguranca`, `/web-launch-auditor`, `/humanizar`).
