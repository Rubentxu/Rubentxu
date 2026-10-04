<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:6E56CF,50:4C7EF3,100:38BDF8&height=200&section=header&text=Rub%C3%A9n%20Dar%C3%ADo%20Cabrera&fontSize=40&fontColor=ffffff&fontAlignY=34&desc=Cloud%20Solutions%20Architect%20%C2%B7%20DevOps%20Lead&descSize=17&descAlignY=55&animation=fadeIn" width="100%" alt="Rubén Darío Cabrera — Cloud Solutions Architect & DevOps Lead" />

<img src="https://readme-typing-svg.demolab.com?font=Fira+Code&weight=600&size=22&pause=1000&color=6E56CF&center=true&vCenter=true&width=760&lines=Cloud+Solutions+Architect+%26+DevOps+Lead;Platform+Engineer+%E2%86%92+AI+Agent+Tooling;Construyo+herramientas+de+desarrollo+en+Rust;Rethinking+how+AI+agents+earn+trust&height=110" alt="Rubén Darío Cabrera — typing" />

[![Followers](https://img.shields.io/github/followers/Rubentxu?style=for-the-badge&logo=github&label=Followers&color=6E56CF)](https://github.com/Rubentxu?tab=followers)
[![Stars](https://img.shields.io/github/stars/Rubentxu?style=for-the-badge&logo=github&label=Stars&color=orange)](https://github.com/Rubentxu?tab=repositories)
[![Repos](https://img.shields.io/github/repos/Rubentxu?style=for-the-badge&logo=github&label=Repos&color=blue)](https://github.com/Rubentxu?tab=repositories)
[![Forks](https://img.shields.io/github/forks/Rubentxu?style=for-the-badge&logo=github&label=Forks&color=8B949E)](https://github.com/Rubentxu?tab=repositories)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rubentxu)
[![Email](https://img.shields.io/badge/Email-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rubentxu74@gmail.com)

**📍 Vitoria-Gasteiz, País Vasco, España** · 15+ años construyendo software · 92 repos públicos

[⬇️ Saltar al contenido](#índice)

</div>

---

## 📑 Índice

| | | |
|---|---|---|
| [🧭 Lo que construyo](#-lo-que-construyo) | [🧬 Ecosistema y derivados](#-ecosistema-y-derivados) | [💼 Experiencia](#-experiencia) |
| [🚀 Proyectos bandera](#-proyectos-bandera) | [🧪 Más herramientas](#-m%C3%A1s-herramientas) | [🛠️ Stack](#%EF%B8%8F-stack) |
| | [📊 En números](#-en-n%C3%BAmeros) | [📫 Contacto](#-contacto) |

---

## 🧭 Lo que construyo

No tengo 40 proyectos sueltos: tengo **un stack**. Cada pieza responde a una pregunta distinta sobre cómo un
agente de IA gana **autoridad** sobre el software que toca, y todas se componen en un mismo harness gobernado.

```text
                                                           ▼
                                                           │
┌────────────────┐  ┌────────────────┐  ┌────────────────┐  ┌────────────────┐
│  SDDK          │  │  CogniCode     │  │  Bastion       │  │  Chronos       │
├────────────────┤  ├────────────────┤  ├────────────────┤  ├────────────────┤
│                │  │                │  │                │  │                │
│¿QUÉ PUEDO      │  │¿QUÉ ES EL      │  │¿DÓNDE SE       │  │¿QUÉ PASÓ       │
│HACER, Y CON    │  │CÓDIGO?         │  │EJECUTA?        │  │DE VERDAD?      │
│QUÉ EVIDENCIA   │  │                │  │                │  │                │
│LO RESPALDA?    │  │73 MCP tools    │  │Podman          │  │evidence        │
│                │  │30 lenguajes    │  │Firecracker     │  │ejecutable      │
│gates · ledger  │  │call graphs     │  │gVisor · K8s    │  │519+ tests      │
│6 lentes de     │  │safe refactor   │  │aislamiento     │  │no silent lies  │
│verificación    │  │                │  │                │  │                │
└────────────────┘  └────────────────┘  └────────────────┘  └────────────────┘
         │                   │                   │                   │
         ┌                   ┴                   ┴                   ┐
                                                           ▼
       ┌────────────────────────────────────────────┐
       │  PipelineK — ejecución local y durable     │
       └────────────────────────────────────────────┘
```

Cada capa tiene **una única autoridad**. SDDK no sabe qué es un símbolo; CogniCode no decide si algo puede
publicarse; Bastion no interpreta políticas. Separar las autoridades es lo que hace que el sistema sea
auditable en lugar de una caja negra con un LLM dentro.

---

## 🚀 Proyectos bandera

<table>
<tr>
<td width="50%" valign="top">

<b>🧠 SDDK — Software Development Decision Kernel</b><br><br>
<b>Kernel de decisión y workflow para desarrollo asistido por IA.</b><br><br>
<i>No es otro framework de agentes: es la capa que decide qué se puede hacer y con qué evidencia se cierra.</i><br><br>
• 🔀 Pipeline gobernado de <b>exploración → release</b><br>
• 🚦 <b>Quality gates</b> + auditoría de deuda técnica<br>
• 🕸️ Grafo de conocimiento que rastrea <b>cada decisión, requisito e incidencia</b> entre ciclos<br>
• 🔍 <b>6 lentes de verificación</b> en paralelo + síntesis: spec, arquitectura, calidad de test, coherencia de diseño y 2 jueces adversariales<br>
• 🔐 Efectos Git gobernados · <b>MIT</b> · compatible con OKF v0.2 y Obsidian Properties<br>
• 🇪🇸🇬🇧 README bilingüe<br><br>
<a href="https://github.com/Rubentxu/software-development-decision-kernel"><b>Rubentxu/software-development-decision-kernel</b></a>

</td>
<td width="50%" valign="top">

<b>🔍 CogniCode — Code Intelligence para agentes</b><br><br>
<b>Un Super-LSP en Rust que expone IntelliJ como herramientas MCP.</b><br><br>
<i>Piensa IntelliJ IDEA, pero invocado por un agente vía Model Context Protocol.</i><br><br>
• 🧰 <b>73 herramientas MCP</b><br>
• 🌍 <b>30 lenguajes</b> vía Tree-sitter (18 soportados + 12 experimentales)<br>
• 🕸️ Call graphs, análisis de impacto, búsqueda semántica<br>
• 🧬 Refactor seguro: rename, extract, inline, move, change signature <b>con preview de impacto</b><br>
• 💾 Caché de grafo persistente (embedded <code>redb</code>) que sobrevive entre sesiones<br>
• 🏛️ Detección de ciclos con <b>SCC de Tarjan</b>, hot paths y código muerto<br>
• 📈 Export a Mermaid · compresión de contexto · OpenTelemetry<br>
• 🧱 DDD + Clean Architecture<br><br>
<a href="https://github.com/Rubentxu/CogniCode"><b>Rubentxu/CogniCode</b></a>

</td>
</tr>
<tr>
<td width="50%" valign="top">

<b>🏰 Bastion — MCP Gateway para ejecución aislada</b><br><br>
<b>Ejecuta las tools de un agente en una sandbox, no en tu máquina.</b><br><br>
<i>El problema: los MCP servers existentes ejecutan comandos en el mismo proceso. Sin aislamiento, sin límites, sin limpieza.</i><br><br>
• 🧱 <b>Aislamiento real</b> por ejecución: contenedor o microVM<br>
• 📦 Backends intercambiables: <b>Podman · Firecracker · gVisor · Kubernetes</b><br>
• ⏱️ Límites de CPU, memoria y tiempo por sandbox<br>
• 🧹 Estado limpio: nada se filtra entre ejecuciones<br>
• 🤝 MCP nativo — funciona con OpenCode, Claude Code, Goose<br>
• 🦀 Rust · DDD + Clean Architecture · Apache-2.0<br><br>
<a href="https://github.com/Rubentxu/Bastion"><b>Rubentxu/Bastion</b></a>

</td>
<td width="50%" valign="top">

<b>⚙️ PipelineK — CI/CD local-first con DSL de Kotlin</b><br><br>
<b>Binario único. Pipelines duraderos. Sin controlador, sin estado remoto, sin phone-home.</b><br><br>
• 📄 DSL Kotlin tipado (<code>.pipeline.kts</code>), familiar al de Jenkins<br>
• ♻️ Ejecución <b>durable y reanudable</b> tras un crash<br>
• 🔎 Cada paso emite un <b>evento tipado</b>; cada shell queda registrado con huella <b>SHA-256</b> de sus entradas<br>
• 🏠 100% local — los datos no salen de tu máquina<br>
• 🔐 Releases firmados con SHA-256 verificable · <code>pipelinek doctor</code> para preflight<br>
• 🐧 Linux · macOS · Windows (WSL) · Java 21+ · <b>MIT</b><br><br>
<a href="https://github.com/Rubentxu/pipeline-kotlin"><b>Rubentxu/pipeline-kotlin</b></a>

</td>
</tr>
</table>

---

## 🧬 Ecosistema y derivados

El trabajo no son 4 repos: es un sistema con capas, y cada una tiene su propio ritmo.

**Un pipeline real de PipelineK se lee casi como Jenkins, pero escrito en Kotlin — un lenguaje más tipado y seguro — y se ejecuta en tu máquina:**

```kotlin
pipeline {
    stages {
        stage("build") {
            sh("./gradlew build")
        }
        stage("verify") {
            retry(count = 3) {
                sh("./gradlew test")
            }
        }
    }
}
```

<table>
<tr>
<th align="left">Capa</th>
<th align="left">Proyecto</th>
<th align="left">Qué resuelve</th>
</tr>
<tr>
<td valign="top"><b>Configuración</b></td>
<td><a href="https://github.com/Rubentxu/pipelattice"><b>Pipelattice</b></a><br><sub>Kotlin 2.4 · MIT</sub></td>
<td valign="top">Control-plane <b>GitOps</b> que compila configuración tipada y versionada en un <code>ResolvedPipelinePlan</code> <b>inmutable y explicable</b>. No ejecuta: produce el plan; el runtime lo consume.</td>
</tr>
<tr>
<td valign="top"><b>Decisión</b></td>
<td><a href="https://github.com/Rubentxu/software-development-decision-kernel"><b>SDDK</b></a> · <a href="https://github.com/Rubentxu/vistalith"><b>Vistalith</b></a><br><sub>Kernel · workspace visual</sub></td>
<td valign="top">SDDK gobierna el ciclo. Vistalith lo aplica a un <b>Semantic World Graph</b>: ingeniería visual agéntica construida <i>sobre</i> SDDK, no al lado.</td>
</tr>
<tr>
<td valign="top"><b>Estructura</b></td>
<td><a href="https://github.com/Rubentxu/arch-skillkit"><b>arch-skillkit</b></a><br><sub>Python</sub></td>
<td valign="top">Descubrimiento de arquitectura <b>agent-first</b> y limpio: evidencia determinista (ast-grep, Semgrep, metadatos de build) → agentes LLM → LikeC4 + Arrows. <b>Nunca escribe en el repo analizado.</b></td>
</tr>
<tr>
<td valign="top"><b>Contexto</b></td>
<td><a href="https://github.com/Rubentxu/skillgraph"><b>SkillGraph</b></a><br><sub>Python · H0..H7</sub></td>
<td valign="top">Orquestador de skills <b>local-first</b> basado en grafo. Blueprint v1: <b>16/16 UAT PASS</b> en 5 releases.</td>
</tr>
<tr>
<td valign="top"><b>Identidad</b></td>
<td><a href="https://github.com/Rubentxu/agent-secretless"><b>agent-secretless</b></a> · <a href="https://github.com/Rubentxu/agent-control-plane"><b>agent-control-plane</b></a><br><sub>Rust · TypeScript</sub></td>
<td valign="top">Un agente usa una identidad <b>sin recibir nunca el material de la credencial</b>. Control-plane declarativo <i>graph-first</i> con runtime Eve, grafo de recursos tipado, reconciliación y credential broker.</td>
</tr>
<tr>
<td valign="top"><b>Distribución</b></td>
<td><a href="https://github.com/Rubentxu/asdf-pipelinek"><b>asdf-pipelinek</b></a> · <a href="https://github.com/Rubentxu/homebrew-sddk"><b>homebrew-sddk</b></a></td>
<td valign="top">Canales de instalación verificados: plugin <b>asdf</b> y tap <b>Homebrew</b>. Instalables de una línea, con digest de release.</td>
</tr>
</table>

---

## 🧪 Más herramientas

<details>
<summary><b>Runtimes de agente, CI/CD agéntico y grafos</b> — <i>Rcode, Mentat, Quilt, a2a-protocol-rust, code-context-graph…</i></summary>

<br>

| Proyecto | Lenguaje | Qué es |
|---|---|---|
| [**Rcode**](https://github.com/Rubentxu/Rcode) ⭐5 | Rust | Coding agent de alto rendimiento: LLM en streaming, ejecución de tools, TUI, Web UI, MCP y LSP |
| [**Mentat**](https://github.com/Rubentxu/mentat) | Rust | CI/CD event-driven donde los agentes son ciudadanos de primera clase: actores Ractor, bus CloudEvents, LLM Router con caché semántico, motor de políticas **Cedar** |
| [**Quilt**](https://github.com/Rubentxu/quilt) ⭐7 | Rust | Knowledge graph **AI-first**: reimplementación en Rust del modelo de grafo de Logseq, arquitectura MCP-first, FTS5, local-first |
| [**a2a-protocol-rust**](https://github.com/Rubentxu/a2a-protocol-rust) | Rust | SDK del protocolo **A2A** (Agent-to-Agent) para comunicación fiable entre agentes |
| [**code-context-graph**](https://github.com/Rubentxu/code-context-graph) | Rust | Análisis semántico de código: representaciones en grafo para workflows de desarrollo asistidos por IA |
| [**agents-workflows**](https://github.com/Rubentxu/agents-workflows) | TypeScript | Sistema de workflows agénticos: binario único con Studio UI, servidor MCP, API REST y dashboard React |

</details>

<details>
<summary><b>Hodei — plataforma open source por piezas</b> — <i>la alternativa a Azure DevOps construida módulo a módulo</i></summary>

<br>

| Proyecto | Lenguaje | Qué es |
|---|---|---|
| [**hodei-jobs**](https://github.com/Rubentxu/hodei-jobs) ⭐2 | Rust | Ejecución de jobs distribuida con providers **Docker, Kubernetes y Firecracker** |
| [**hodei-artifacts**](https://github.com/Rubentxu/hodei-artifacts) | Rust | Registry de artefactos con IAM, políticas **Cedar** y analítica |
| [**hodei-authz**](https://github.com/Rubentxu/hodei-authz) | Rust | Motor de autorización multi-tenant basado en Cedar Policy |
| [**hodei-verified-permissions**](https://github.com/Rubentxu/hodei-verified-permissions) | Rust | Servicio de autorización Cedar multi-DB con caché en memoria — production-ready |
| [**hodei-audit-trail**](https://github.com/Rubentxu/hodei-audit-trail) | Rust | Centralized Audit Point con sistema HRN, enriquecimiento de eventos y query engine |
| [**hodei-scan**](https://github.com/Rubentxu/hodei-scan) | Rust | Motor de correlación de seguridad multi-dominio con DSL propio |
| [**hodei-dsl**](https://github.com/Rubentxu/hodei-dsl) | Kotlin | DSL declarativo de pipelines cloud-native, precursor del enfoque de PipelineK |
| [**hodei-pipelines**](https://github.com/Rubentxu/hodei-pipelines) | Rust | Procesamiento distribuido de jobs con integración de resource pools |
| [**pipeliner**](https://github.com/Rubentxu/pipeliner) ⭐1 | Rust | Biblioteca de orquestación de pipelines con **Arquitectura Hexagonal** |
| [**hodei-draw**](https://github.com/Rubentxu/hodei-draw) | Rust/WASM | Canvas interactivo estilo Excalidraw con física, animación y WebAssembly |

</details>

<details>
<summary><b>Rust, WASM, gráficos y motores</b> — <i>la capa de render y los motores</i></summary>

<br>

| Proyecto | Lenguaje | Qué es |
|---|---|---|
| [**archflow**](https://github.com/Rubentxu/archflow) | Rust | Motor de gráficos 2D con **Zero Trust**, curvas Bézier, sistema de estilos, puertos y conexiones, y export a WASM |
| [**arch-stack**](https://github.com/Rubentxu/arch-stack) ⭐1 | Rust + TS | `archctl` CLI sidecar para diagramas C4/UML + workbench SolidJS con G6 |
| [**bevy-2d-editor**](https://github.com/Rubentxu/bevy-2d-editor) | Rust | Editor de escenas 2D en navegador para juegos Bevy |
| [**bevy-libro-examples**](https://github.com/Rubentxu/bevy-libro-examples) | Rust | Patrones 2D y ECS con Bevy 0.19 — **38 crates, 197 tests** |
| [**grafos-bbdd-desde-cero**](https://github.com/Rubentxu/grafos-bbdd-desde-cero) | Rust | Obra técnica en 3 volúmenes: grafos, construcción de **LiraDB** (BBDD de grafos desde cero) y grafos en la era de la IA |

</details>

<details>
<summary><b>El inicio: donde empezó todo</b> — <i>ECS, motores de juego y automatización</i></summary>

<br>

| Proyecto | Lenguaje | Qué es |
|---|---|---|
| [**Entitas-Java**](https://github.com/Rubentxu/Entitas-Java) ⭐56 | Java 8 | **Entity Component System** en Java — mi proyecto más estrelas, y donde empezó la obsesión por los ECS |
| [**DreamsLibGdx**](https://github.com/Rubentxu/DreamsLibGdx) ⭐9 | Java | Juego de plataformas con **LibGDX** |
| [**pipeline-runtime**](https://github.com/Rubentxu/pipeline-runtime) ⭐2 | Groovy | Emulador de pipelines Jenkins — <b>el ancestro directo de PipelineK</b> |
| [**pipeline-kotlin**](https://github.com/Rubentxu/pipeline-kotlin) ⭐2 | Kotlin | Primer runner del DSL de pipelines en Kotlin — hoy <b>PipelineK</b> |
| [**lbricks**](https://github.com/Rubentxu/lbricks) | Go | Lógica de <i>logic bricks</i> reutilizable, puente entre los dos mundos |
| [**Artifex**](https://github.com/Rubentxu/artifex) | Rust + SvelteKit | Suite creativa IA para game devs: sprites, audio, música y voz con Tauri v2 |
| [**pkm-ai**](https://github.com/Rubentxu/pkm-ai) | Rust | Gestión de conocimiento personal potenciada con IA |

</details>

---

## 💼 Experiencia

<table>
<tr>
<td width="50%" valign="top">

<b>Paradigma Digital</b> — <i>2025 → presente</i><br>
<b>Cloud Solutions Architect &amp; DevOps Lead</b><br><br>
Arquitectura cloud y liderazgo de DevOps: automatización de plataformas, prácticas de seguridad y guardarraíles para equipos que entregan en producción. El punto donde el trabajo de plataforma se convierte en producto.

</td>
<td width="50%" valign="top">

<b>Viewnext</b> — <i>2024 → 2025</i><br>
<b>Cloud Solutions Architect &amp; DevOps Lead</b><br><br>
Modernización DevOps para <b>GISS / Seguridad Social</b>: virtualización de procesos, entornos y cadena de entrega en la Administración pública.

</td>
</tr>
<tr>
<td width="50%" valign="top">

<b>RealNaut</b> — <i>2021 → 2024</i><br>
<b>Platform Engineer</b><br><br>
Rediseño de CI/CD, cloud híbrido y mentoring de equipos de ingeniería. El salto de <i>usar</i> herramientas a <i>construir la plataforma</i> que las sostiene.

</td>
<td width="50%" valign="top">

<b>Accenture</b> — <i>2019 → 2020</i><br>
<b>DevOps Engineer</b><br><br>
Proyecto <b>Vodafone</b>: Kubernetes, observabilidad y automatización a escala de carrier.

</td>
</tr>
<tr>
<td colspan="2" valign="top">

<b>Ibermática</b> — <i>2016 → 2019</i><br>
<b>Software Architect</b><br><br>
Automatizaciones DevOps, microservicios y diseño de arquitecturas. Los años que enseñaron a pensar en sistemas antes que en servicios.

</td>
</tr>
</table>

**Clientes y programas:** Seguridad Social · Vodafone · Sanitas · RTVE · Gobierno Vasco · Servihabitat

<details>
<summary><b>📜 Certificaciones</b></summary>

<br>

- **AWS Certified** — Cloud Practitioner
- **Kubernetes for Developers** — LFD259 (CNCF)
- **Red Hat OpenShift Fundamentals** — DO081x
- **ITIL Foundation**

</details>

---

## 🛠️ Stack

<div align="center">

**Lenguajes & runtimes**

<img src="https://skillicons.dev/icons?i=rust,kotlin,go,python,typescript,javascript,java,groovy,bash,lua,c,cpp,zig" alt="Lenguajes" />

**AI, agentes & infraestructura**

<img src="https://skillicons.dev/icons?i=ai,mcp,ollama,langchain,openai,anthropic,linux,docker,kubernetes,githubactions,terraform,nginx" alt="AI e infraestructura" />

**Cloud, datos & observabilidad**

<img src="https://skillicons.dev/icons?i=aws,azure,gcp,k9s,helm,prometheus,grafana,postgresql,sqlite,redis,git,github" alt="Cloud y datos" />

</div>

<details>
<summary><b>Herramientas de plataforma que uso a diario</b></summary>

<br>

| Categoría | Herramientas |
|---|---|
| **CI/CD agéntico** | PipelineK · Mentat · Jenkins · ArgoCD · Spinnaker |
| **Ejecución aislada** | Podman · Firecracker · gVisor · Kubernetes · Docker |
| **Gobernanza** | Cedar Policy · OPA · GitOps · evidencia con receipts |
| **Observabilidad** | OpenTelemetry · Prometheus · Grafana · k9s |
| **Cloud** | AWS · Azure · GCP · Terraform · Helm |
| **Paradigma** | DDD · Clean Architecture · Hexagonal · TDD |

</details>

---

## 📊 En números

<div align="center">

<img height="165" alt="GitHub stats" src="https://github-readme-stats.vercel.app/api?username=Rubentxu&show_icons=true&theme=tokyonight&hide_border=true&rank_icon=github" />
<img height="165" alt="Top languages" src="https://github-readme-stats.vercel.app/api/top-langs/?username=Rubentxu&layout=compact&theme=tokyonight&hide_border=true&langs_count=10" />

<br>

<img height="150" alt="Streak stats" src="https://streak-stats.demolab.com?user=Rubentxu&theme=tokyonight&hide_border=true&locale=es" />

<br>

**🗂️ Los 4 bandera, en una tarjeta**

<a href="https://github.com/Rubentxu/pipeline-kotlin">
  <img height="150" alt="pipeline-kotlin" src="https://github-readme-stats.vercel.app/api/pin/?username=Rubentxu&repo=pipeline-kotlin&theme=tokyonight&hide_border=true" />
</a>
<a href="https://github.com/Rubentxu/CogniCode">
  <img height="150" alt="CogniCode" src="https://github-readme-stats.vercel.app/api/pin/?username=Rubentxu&repo=CogniCode&theme=tokyonight&hide_border=true" />
</a>
<br>
<a href="https://github.com/Rubentxu/Bastion">
  <img height="150" alt="Bastion" src="https://github-readme-stats.vercel.app/api/pin/?username=Rubentxu&repo=Bastion&theme=tokyonight&hide_border=true" />
</a>
<a href="https://github.com/Rubentxu/software-development-decision-kernel">
  <img height="150" alt="software-development-decision-kernel" src="https://github-readme-stats.vercel.app/api/pin/?username=Rubentxu&repo=software-development-decision-kernel&theme=tokyonight&hide_border=true" />
</a>

**🐍 La serpiente que se come mis contribuciones**

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/Rubentxu/Rubentxu/output/github-contribution-grid-snake-dark.svg" />
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/Rubentxu/Rubentxu/output/github-contribution-grid-snake.svg" />
  <img alt="Snake animation over the contribution graph" src="https://raw.githubusercontent.com/Rubentxu/Rubentxu/output/github-contribution-grid-snake.svg" />
</picture>

<br>

<a href="https://github.com/Rubentxu">
  <img src="https://komarev.com/ghpvc/?username=Rubentxu&label=Profile%20views&color=6E56CF&style=flat" alt="Profile views" />
</a>
&nbsp;&nbsp;
<a href="https://github.com/Rubentxu">
  <img src="https://img.shields.io/badge/Building%20with-Rust%20%E2%9A%A1%EF%B8%8F-202020?style=flat&logo=rust&logoColor=white" alt="Rust" />
</a>

</div>

---

## 📫 Contacto

<div align="center">

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Rub%C3%A9n%20Dario-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/rubentxu)
[![GitLab](https://img.shields.io/badge/GitLab-rubentxu74-FCA121?style=for-the-badge&logo=gitlab&logoColor=white)](https://gitlab.com/rubentxu74)
[![Email](https://img.shields.io/badge/Email-rubentxu74@gmail.com-D14836?style=for-the-badge&logo=gmail&logoColor=white)](mailto:rubentxu74@gmail.com)

</div>

> *"No enseñes al agente a recordar. Haz que el sistema materialice el estado correcto, limite lo que
> puede hacer y entregue contexto verificable antes de cada decisión."*

---

<details>
<summary><b>🗺️ Mi viaje</b></summary>

<br>

```text
2010–2013  Java · Spring · AppEngine · juegos Android
2014–2015  LibGDX · DreamsLibGdx · Entitas-Java (ECS) — 56 ⭐
2016–2017  Go · lbricks · automatización DevOps · Go real-time
2018–2020  DevOps de verdad — Jenkins · Terraform · Kubernetes · microservicios
2021–2024  Platform Engineering — cloud híbrido · CI/CD redesign · mentoring
2025       Cloud Solutions Architect & DevOps Lead
2026       AI agent tooling — SDDK · CogniCode · Bastion · PipelineK
```

**De escribir lógica a decidir qué lógica puede ejecutarse.**

</details>

<details>
<summary><b>🏔️ Fuera del código</b></summary>

<br>

- 🏔️ Montaña y senderismo — Pirineos, Gorbeia, Aizkorri
- 📚 Lectura técnica: sistemas distribuidos, arquitectura, IA
- ✍️ Escribiendo sobre Platform Engineering, Rust y MCP
- 👨‍🏫 Mentoring y formación de equipos
- 🎮 Game dev (histórico: LibGDX, Defold, Entitas)

</details>

---

<div align="center">

<sub>Este README cuenta la historia del stack, no solo la lista de repos. Si algo no encaja, probablemente
el cambio correcto es en el código, no aquí.</sub>

<img src="https://capsule-render.vercel.app/api?type=waving&color=0:38BDF8,50:4C7EF3,100:6E56CF&height=130&section=footer" width="100%" alt="" />

</div>
