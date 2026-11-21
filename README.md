# Skills Antigravity

Coleção modular de **23 skills diretas** (com `SKILL.md` na raiz) e **4 repositórios/pacotes externos** para o ecossistema **Google Antigravity**, organizados por domínio: Engenharia de Software & Game Dev, Web & Design, Fluxo de Engenharia & TDD, Segurança & QA, Escrita e Meta-Skills.

Todas as skills autorais seguem o padrão de *Progressive Disclosure* do Antigravity (`SKILL.md` com frontmatter YAML + diretórios auxiliares `references/`, `scripts/` e `data/` quando aplicável) e entregam respostas e comentários de código em **Português do Brasil (`pt-BR`)**.

---

## Visão Geral Rápida (23 Skills Diretas)

| Skill | Categoria | Foco Principal | Invocação |
|-------|-----------|----------------|-----------|
| [`dev-flutter-senior`](./dev-flutter-senior/SKILL.md) | Engenharia de Software | Apps Flutter/Dart com Clean Architecture, estado escalável e APIs REST | `/dev-flutter-senior` |
| [`dev-dotnet-senior`](./dev-dotnet-senior/SKILL.md) | Engenharia de Software | APIs e microsserviços em C# 12+ / .NET 8 e 9 no Linux (`dotnet CLI`) | `/dev-dotnet-senior` |
| [`dev-cpp-senior`](./dev-cpp-senior/SKILL.md) | Engenharia de Software | Sistemas de alta performance em C (C99/C11) e C++ Moderno (C++11-23) | `/dev-cpp-senior` |
| [`dev-godot3d-senior`](./dev-godot3d-senior/SKILL.md) | Game Dev 3D | Jogos 3D na Godot 4.x, GDScript 2.0/C#, `AnimationTree` e Vulkan | `/dev-godot3d-senior` |
| [`frontend-expert`](./frontend-expert/SKILL.md) | Web & Frontend | Arquitetura React + TypeScript, Suspense, TanStack Query e performance | `/frontend-expert` |
| [`frontend-design`](./frontend-design/SKILL.md) | Web & Design | Direção visual autoral, tipografia e identidade estética distinta para UI | `/frontend-design` |
| [`3d-web-experience`](./3d-web-experience/SKILL.md) | Web & 3D | Three.js, React Three Fiber (R3F), Spline, WebGL e otimização GLB | `/3d-web-experience` |
| [`uiux-designer`](./uiux-designer/SKILL.md) | Design & UX | Design systems, paletas, tipografia, acessibilidade e revisão UX | `/uiux-designer` |
| [`setup-matt-pocock-skills`](./setup-matt-pocock-skills/SKILL.md) | Fluxo de Engenharia | Configura tracker de issues, rótulos de triagem e docs (`GLOSSARY.md`/ADRs) | `/setup-matt-pocock-skills` |
| [`grill-me`](./grill-me/SKILL.md) | Fluxo de Engenharia | Entrevista rigorosa para lapidar planos e decisões de arquitetura | `/grill-me` |
| [`to-spec`](./to-spec/SKILL.md) | Fluxo de Engenharia | Sintetiza a conversa atual em uma spec e publica no issue tracker | `/to-spec` |
| [`to-tickets`](./to-tickets/SKILL.md) | Fluxo de Engenharia | Quebra planos/specs em tickets verticais (*tracer-bullet*) com bloqueios | `/to-tickets` |
| [`implement`](./implement/SKILL.md) | Fluxo de Engenharia | Implementa uma spec ou conjunto de tickets usando `tdd` e `code-review` | `/implement` |
| [`tdd`](./tdd/SKILL.md) | Testes & Qualidade | Ciclo *red-green-refactor* testando comportamento em *seams* públicos | `/tdd` |
| [`diagnosing-bugs`](./diagnosing-bugs/SKILL.md) | Debugging | Loop disciplinado de reprodução e diagnóstico para bugs e lentidões | `/diagnosing-bugs` |
| [`code-review`](./code-review/SKILL.md) | Revisão de Código | Revisão paralela em 2 eixos (*Standards* e *Spec*) desde um ponto fixo | `/code-review` |
| [`web-launch-auditor`](./web-launch-auditor/SKILL.md) | Qualidade & SEO | Auditoria pré-deploy em 9 pilares (CWV, PageSpeed, SEO, Pixels, IA) | `/web-launch-auditor` |
| [`ciberseguranca`](./ciberseguranca/SKILL.md) | Segurança (AppSec) | Auditoria defensiva multiplataforma (OWASP/MASVS) + Prompt de Remediação | `/ciberseguranca` |
| [`humanizar`](./humanizar/SKILL.md) | Escrita & Revisão | Remoção de padrões de escrita por IA (guia da Wikipédia) em textos/arquivos | `/humanizar` |
| [`criar-txt`](./criar-txt/SKILL.md) | Documentação | Registro cronológico de alterações em `explicacoes.txt` na raiz do projeto | `/criar-txt` |
| [`criarskill`](./criarskill/SKILL.md) | Meta-Skill | Entrevista, arquitetura e criação de novas skills no padrão Antigravity | `/criarskill` |
| [`orquestradora`](./orquestradora/SKILL.md) | Meta-Skill / Roteamento | Análise de contexto, escolha da(s) melhor(es) skill(s) e ordem segura de execução | `/orquestradora` |
| [`find-skills`](./find-skills/SKILL.md) | Meta-Skill / Descoberta | Descobre e instala skills do ecossistema aberto via Skills CLI (`npx skills`) | `/find-skills` |

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

#### 6. `frontend-design` ([SKILL.md](./frontend-design/SKILL.md))
Atua como **Diretor de Design Visual para Interfaces Web**.
- **O que faz:** Orienta escolhas estéticas autorais e intencionais ao criar ou redesenhar interfaces web — direção visual ancorada no assunto do produto, tipografia expressiva, composição de hero e fuga de templates genéricos gerados por IA.

#### 7. `3d-web-experience` ([SKILL.md](./3d-web-experience/SKILL.md))
Atua como **3D Web Experience Architect**.
- **O que faz:** Projeta configuradores 3D, portfólios imersivos, animações sincronizadas com scroll e cenas interativas com **Three.js, React Three Fiber (R3F), `@react-three/drei`, Spline e WebGL**.
- **Diferenciais:** Inclui pipeline de compressão `.glb` com `gltf-transform` (Draco + WebP), orçamento de triângulos/FPS por dispositivo, proteção de SSR no Next.js, fallback para ausência de WebGL e controle de `dpr` em dispositivos móveis.

#### 8. `uiux-designer` ([SKILL.md](./uiux-designer/SKILL.md))
Atua como **Senior UI/UX Designer e Especialista em Design Systems**.
- **O que faz:** Gera sistemas de design completos (estilo, paleta de cores, tipografia, efeitos e antipadrões) e realiza revisões de ergonomia, responsividade e acessibilidade (WCAG) para web e mobile.
- **Diferenciais:** Consulta uma base local pesquisável via [`scripts/search.py`](./uiux-designer/scripts/search.py) e datasets em [`data/`](./uiux-designer/data/) com 50+ estilos, 97 paletas, 57 combinações tipográficas e diretrizes para 12 stacks.

---

### Fluxo de Engenharia, Testes e Debugging

#### 9. `setup-matt-pocock-skills` ([SKILL.md](./setup-matt-pocock-skills/SKILL.md))
Configura o repositório para o conjunto de skills de engenharia: define o issue tracker (GitHub ou markdown local), vocabulário de rótulos de triagem e layout de documentação de domínio (`GLOSSARY.md` e ADRs).

#### 10. `grill-me` ([SKILL.md](./grill-me/SKILL.md))
Conduz uma entrevista técnica rigorosa sobre um plano ou design para expor lacunas, premissas implícitas e decisões em aberto antes de escrever código.

#### 11. `to-spec` ([SKILL.md](./to-spec/SKILL.md))
Sintetiza o contexto da conversa atual e do repositório diretamente em uma especificação técnica estruturada (incluindo *seams* de teste) e publica no issue tracker configurado, sem entrevista adicional.

#### 12. `to-tickets` ([SKILL.md](./to-tickets/SKILL.md))
Quebra um plano, spec ou conversa em tickets verticais (*tracer-bullet slices*), declarando explicitamente as dependências de bloqueio entre tickets e publicando no tracker configurado.

#### 13. `implement` ([SKILL.md](./implement/SKILL.md))
Executa a implementação de uma spec ou conjunto de tickets de ponta a ponta: busca o contexto do ticket, aplica `tdd` nos *seams* acordados, roda typechecking/testes continuamente, aciona `code-review` ao final e realiza o commit na branch atual.

#### 14. `tdd` ([SKILL.md](./tdd/SKILL.md))
Guia o desenvolvimento orientado a testes (*red-green-refactor*) testando comportamento através de interfaces públicas (*seams* pré-acordados), evitando acoplamento a detalhes internos de implementação.

#### 15. `diagnosing-bugs` ([SKILL.md](./diagnosing-bugs/SKILL.md))
Aplica um loop estruturado de diagnóstico para bugs complexos e regressões de performance: redação rigorosa de segredos (`<REDACTED>`), construção de um loop de feedback rápido e reproduzível (vermelho/verde), bissecção e verificação de hipóteses.

#### 16. `code-review` ([SKILL.md](./code-review/SKILL.md))
Executa revisão do diff entre `HEAD` e um ponto fixo (commit, branch, tag ou merge-base) em dois eixos paralelos via subagentes independentes: **Standards** (aderência aos padrões documentados do repo) e **Spec** (fidelidade à issue/spec original).

---

### Segurança, Qualidade e Pré-Lançamento

#### 17. `web-launch-auditor` ([SKILL.md](./web-launch-auditor/SKILL.md))
Atua como **Senior Web Performance, Technical SEO e QA Engineer**.
- **O que faz:** Executa uma auditoria pré-deploy (*Pre-Flight Check*) em **9 pilares técnicos**: *Delayed Pixel Loading*, otimização de imagens e proteção de LCP (`fetchpriority="high"` sem `loading="lazy"` na hero), prevenção de CLS (`font-display: swap`), Meta tags individuais, Open Graph (`og:image` absoluta), Schema.org (JSON-LD), responsividade cross-device, limpeza de rastros de IA/placeholders e Core Web Vitals/WCAG AA.
- **Diferenciais:** Entrega tabela de status (`[APROVADO]`, `[ALERTA]`, `[CRÍTICO]`) acompanhada do código exato pronto para substituir.

#### 18. `ciberseguranca` ([SKILL.md](./ciberseguranca/SKILL.md))
Atua como **Engenheiro de Cibersegurança e AppSec Sênior** (postura estritamente defensiva).
- **O que faz:** Audita repositórios, manifestos e código contra a Matriz de Ameaças 2026: **Mobile/OWASP MASVS** (`FLAG_SECURE`, overlays, storage seguro contra stealers, SSL Pinning), **Web/OWASP Top 10** (IDOR, SQLi, XSS, JWT, Rate Limit, CSP/SRI) e **Desktop/Infra** (Path Traversal, menor privilégio, memória segura).
- **Diferenciais:** Classifica achados por severidade (`Crítico`, `Alto`, `Médio`, `Baixo`), aponta arquivo/linha exatos, evita alucinação de CVEs e gera um **Prompt de Remediação** pronto para a skill desenvolvedora correspondente.

---

### Escrita, Documentação e Meta-Skills

#### 19. `humanizar` ([SKILL.md](./humanizar/SKILL.md))
Atua como **Editor Sênior de Humanização Textual** (100% em Português do Brasil).
- **O que faz:** Detecta e elimina os 7 grupos de sinais de texto gerado por IA catalogados pela Wikipédia (*Wikipedia:Signs of AI writing* / *Wikipédia:Sinais de texto gerado por inteligência artificial*), ajustando o texto para os tons **Técnico**, **Acadêmico**, **Neutro/Enciclopédico** ou **Conversacional**.
- **Diferenciais:** Preserva blocos de código, LaTeX (`$...$`, `\cite{}`) e citações diretas, limpa parâmetros `utm_source=` de URLs e sinaliza afirmações vagas sem inventar fontes falsas.

#### 20. `criar-txt` ([SKILL.md](./criar-txt/SKILL.md))
Atua como **Registrador Cronológico de Alterações**.
- **O que faz:** Cria ou atualiza o arquivo `explicacoes.txt` na raiz do projeto documentando arquivos criados/modificados, motivação das mudanças, impacto no sistema e passos de validação, sempre anexando novas entradas sem apagar o histórico anterior.

#### 21. `criarskill` ([SKILL.md](./criarskill/SKILL.md))
Atua como **Arquiteto Especialista em Skills Antigravity (Meta-Skill)**.
- **O que faz:** Conduz a criação de novas skills em **3 Fases obrigatórias** (Descoberta e Entrevista -> Proposta de Arquitetura + Checagem Anti-Sobreposição -> Desenvolvimento Completo Plug & Play) seguindo os 8 passos oficiais do Codelab Antigravity.

#### 22. `orquestradora` ([SKILL.md](./orquestradora/SKILL.md))
Atua como **AI Skill Router & Workflow Orchestrator**.
- **O que faz:** Consulta este catálogo (`README.md` / `SKILL.md`), analisa a stack, a fase do projeto e a tarefa imediata para indicar a(s) skill(s) exata(s), a ordem mais segura de execução (pipeline), os riscos de escolha errada e um prompt pronto para acionar a skill recomendada.

#### 23. `find-skills` ([SKILL.md](./find-skills/SKILL.md))
Atua como **Descobridor de Skills do Ecossistema Aberto**.
- **O que faz:** Ajuda a buscar e instalar novas skills prontas da comunidade utilizando o Skills CLI (`npx skills`) quando o usuário precisa de uma capacidade ainda não instalada.

---

## Repositórios e Pacotes Externos Inclusos

As 4 pastas abaixo são repositórios externos completos presentes no diretório (não possuem `SKILL.md` direto na raiz, mas trazem ferramentas ou coleções internas de skills):

| Repositório | Descrição | Onde Estão os Recursos |
|-------------|-----------|------------------------|
| [`impeccable`](./impeccable/README.md) | Vocabulário de design para agentes de código (`polish`, `bolder`, `critique`, `audit`) focado em eliminar *AI slop* visual | [`.gemini/skills/impeccable/SKILL.md`](./impeccable/.gemini/skills/impeccable/SKILL.md) e [`.agents/skills/`](./impeccable/.agents/skills/) |
| [`hyperframes`](./hyperframes/README.md) | Coleção de 29 skills internas voltadas para vídeo, motion design e composição (`motion-doctrine`, `captions-overlay`, `changelog-video`, `cut-the-curve`, `oversized-cursor`, `seam-craft`) | [`.agents/skills/`](./hyperframes/.agents/skills/) |
| [`agent-browser`](./agent-browser/README.md) | Ferramenta de automação de navegador para agentes IA (Vercel Labs): abre páginas, lê a árvore de acessibilidade e executa ações pelo shell (12 skills internas) | [`skill-data/`](./agent-browser/skill-data/) e [`.agents/skills/`](./agent-browser/.agents/skills/) |
| [`MiroFish`](./MiroFish/README.md) | Motor de inteligência coletiva / simulação multiagente (projeto completo com `backend/` e `frontend/`, sem `SKILL.md` interno) | [`README.md`](./MiroFish/README.md) |

---

## Como as Skills Trabalham Juntas (Sem Sobreposição)

```text
Descoberta e Roteamento:
  orquestradora (Escolhe a skill certa e a ordem segura) | find-skills (Busca novas skills)

Planejamento e Entrega (Fluxo Estruturado):
  setup-matt-pocock-skills -> grill-me -> to-spec -> to-tickets -> implement (tdd + code-review)
  Em caso de bug difícil: diagnosing-bugs

Projeto Web:
  uiux-designer / frontend-design (Design System, direção estética e UX)
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
2. As skills diretas (`*/SKILL.md`) são descobertas automaticamente por *Progressive Disclosure* através do YAML frontmatter de cada `SKILL.md`.
3. Para acionar manualmente, utilize o comando slash correspondente no chat (ex.: `/orquestradora`, `/dev-flutter-senior`, `/ciberseguranca`, `/web-launch-auditor`, `/humanizar`, `/tdd`).
