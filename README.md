# Emilio Melis

CS engineering student at Polytech Tours and AI research intern at HEC Montréal (Summer 2026). I focus on native systems, edge AI runtimes, and low-level performance.

[Portfolio](https://aatricks.github.io/Portfolio/) / [LinkedIn](https://www.linkedin.com/in/emilio-melis-14a801338)

---

I build software that runs directly on constrained hardware:

## Projects

### AI and on-device inference

* **[llmedge](https://github.com/Aatricks/llmedge)** – Android wrapper for llama.cpp, stable-diffusion.cpp, whisper.cpp, and ONNX. Handles native runtime pooling and OpenCL/Vulkan/CPU fallback logic to prevent crashes on device-specific drivers.
* **[LightDiffusion-Next](https://github.com/Aatricks/LightDiffusion-Next)** – Stable Diffusion pipeline and desktop GUI built in PyTorch. Uses custom batching and memory layout optimization to squeeze inference speed out of low-VRAM GPUs.
* **[EasyReader](https://github.com/Aatricks/EasyReader)** – Manga and PDF reader for Android. Integrates `llmedge` to run chapter summaries and text-to-speech entirely offline.

### Systems and low-level

* **[Pilotrs](https://github.com/Aatricks/Pilotrs)** – A `no_std` Rust flight simulator and autopilot. Implements MEKF/complementary filters for state estimation and PID/LQR loops for attitude control.
* **[FrameLimiter](https://github.com/Aatricks/FrameLimiter)** – macOS frame pacer for Metal games. Hooks `CAMetalLayer`'s `nextDrawable` via DYLD injection to apply backpressure, reducing GPU power draw and heat.
* **[CChess](https://github.com/Aatricks/CChess)** – A chess engine written in C using bitboards, alpha-beta pruning, and iterative deepening.

---

## Technical stack

* **Languages**: C/C++, Rust, Python, Kotlin, Objective-C
* **Domains**: On-device ML, sensor fusion, graphics (Metal), system hooks, control loops
* **Tools**: NixOS (Flakes), Git, ADB, PyTorch, Android NDK
