<p align="center">
  <picture>
    <source media="(prefers-color-scheme: dark)" srcset="https://gist.githubusercontent.com/TSPstudio/e1cc8367a31f0e339947d86b64529143/raw/668ddbce0caca893ed857e035d69d9bb73f320a6/tsp-studio-logo-on-dark.svg">
    <img src="https://gist.githubusercontent.com/TSPstudio/e1cc8367a31f0e339947d86b64529143/raw/668ddbce0caca893ed857e035d69d9bb73f320a6/tsp-studio-logo-on-light.svg" alt="TSP Studio" width="400">
  </picture>
</p>

<p align="center">
  <b>Angel Arellano Rojas — Founder & Lead Software Engineer at TSP Studio.</b><br>
  Building pure-Kotlin ML runtimes, Android applications, and edge-native web systems — with zero unnecessary runtime overhead.
</p>

<p align="center">
  <a href="https://central.sonatype.com/artifact/io.github.tspstudio/kotensor"><img alt="Maven Central" src="https://img.shields.io/maven-central/v/io.github.tspstudio/kotensor?style=flat-square&label=Kotensor&color=364FC7"></a>
  <a href="https://play.google.com/store/apps/details?id=com.tsp.lecly"><img alt="Google Play: Lecly" src="https://img.shields.io/badge/Google%20Play-Lecly-16151C?style=flat-square&logo=google-play&logoColor=white"></a>
  <a href="https://dev.to/tspstudio"><img alt="Dev.to: @tspstudio" src="https://img.shields.io/badge/dev.to-%40tspstudio-364FC7?style=flat-square&logo=devdotto&logoColor=white"></a>
  <a href="https://www.linkedin.com/in/angel-arellano-758444405"><img alt="LinkedIn" src="https://img.shields.io/badge/LinkedIn-Angel%20Arellano-16151C?style=flat-square&logo=linkedin&logoColor=white"></a>
  <a href="mailto:angelarellano13510@gmail.com"><img alt="Email" src="https://img.shields.io/badge/email-angelarellano13510%40gmail.com-364FC7?style=flat-square"></a>
  <img alt="Location: Mexico City" src="https://img.shields.io/badge/Mexico%20City-CDMX-16151C?style=flat-square">
</p>

---

## Projects & Systems

| Project | Domain | Stack | Distribution |
| :--- | :--- | :--- | :--- |
| [**Kotensor**](https://github.com/TSPstudio/kotensor) | Pure-Kotlin Transformer & reverse-mode autograd engine | Kotlin, JVM 17+, Vector API (`jdk.incubator.vector`), Android API 24+ | [Maven Central (`io.github.tspstudio:kotensor:1.2.0`)](https://central.sonatype.com/artifact/io.github.tspstudio/kotensor) |
| [**Lecly**](https://play.google.com/store/apps/details?id=com.tsp.lecly) | AI study assistant (summaries, PDF notes, study courses, local AI) | Kotlin, Android SDK, Jetpack Compose, Kotensor (roadmap) | [Google Play Store](https://play.google.com/store/apps/details?id=com.tsp.lecly) |
| [**DatePlanner**](https://github.com/TSPstudio/DatePlanner) | Full-stack serverless web application | HTML5, CSS3, JavaScript SPA, Cloudflare Workers, Cloudflare D1 SQLite | [GitHub Pages + Cloudflare](https://tspstudio.github.io/DatePlanner/) |

- **Kotensor — On-device LLM inference and training in pure Kotlin.** Implements tensors, reverse-mode autograd, RMSNorm, SwiGLU, RoPE (with Llama 3 scaling), grouped-query attention, allocation-free `KVCache` decoding, and a zero-dependency byte-level `BPETokenizer` (`kotlin-stdlib` only — no C++, Python, or JNI).
- **Low-memory training & SIMD acceleration.** v1.1.0 and v1.2.0 introduced prompt loss masking (`IGNORE_INDEX = -100`), chunked `fusedCrossEntropyLoss` (16 MB cap), early backward termination via `requiresGrad`, no-copy transposed matmul backward, optional JVM Vector API FMA kernels, group-wise INT8/INT4 quantization, memory-mapped `.safetensors` loading, and on-device LoRA/QLoRA fine-tuning.
- **Lecly & edge systems.** Published Lecly on Google Play under TSP Studio; currently migrating local inference onto Kotensor and building cross-platform sync across mobile and web using Cloudflare Workers and D1 SQLite.

## Engineering Writing

- [**Cutting LLM Fine-Tuning Memory in Pure Kotlin: Fused Linear Cross-Entropy and the JVM Vector API**](https://dev.to/tspstudio/cutting-llm-fine-tuning-memory-in-pure-kotlin-fused-linear-cross-entropy-and-the-jvm-vector-api-1cj1) — Profiling and eliminating a 544 MB output-head bottleneck and 52B redundant FLOPs when fine-tuning `Qwen2-0.5B` inside a 6 GB JVM heap (`dev.to/tspstudio`).
- [**Kotensor Architecture Changelog (v0.1.0 to v1.2.0)**](https://github.com/TSPstudio/kotensor/blob/main/Engine/kotensor/CHANGELOG.md) — Detailed engineering notes, design rationale, and hardware measurements across desktop AVX-512 and Android ART.

## Stack & Credentials

| Category | Details |
| :--- | :--- |
| **Languages** | Kotlin, Java, C#, TypeScript, JavaScript, SQL, Lua, HTML5, CSS3 |
| **Platforms & Systems** | JVM (17+ / Vector API), Android SDK & Jetpack Compose, Cloudflare Workers & D1, Gradle (KTS), Maven Central, Dokka, Roblox Studio |
| **AI & Low-Level** | Transformer architectures, reverse-mode autograd, INT8/INT4 quantization, LoRA/QLoRA, memory-mapped I/O, cache-tiled concurrency (`ForkJoinPool`) |
| **Education & Awards** | **1st Place**, *Inter-Tec Programmer 2025* (Nov 2025) · Pursuing dual concurrent engineering degrees in **ICTs Engineering** (*Instituto Tecnológico de Tláhuac II*) and **Software Engineering** (*UnADM*) |
