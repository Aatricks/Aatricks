# Emilio Melis

I'm a CS engineering student at Polytech Tours and an AI research intern at HEC Montréal (Summer 2026). I build systems around constrained hardware, low-level performance, and on-device ML inference.

[Portfolio](https://aatricks.github.io/Portfolio/) / [LinkedIn](https://www.linkedin.com/in/emilio-melis-14a801338)

---

I write mostly in C/C++, Python, Kotlin, and Rust. Since GitHub only lets you pin 6 repos, here's a list of the projects I actually work on:

## AI & Mobile Inference

* **llmedge** ([github](https://github.com/Aatricks/llmedge)) - A Kotlin wrapper that lets you run LLMs, Stable Diffusion, Whisper, and ONNX models locally on Android. I built this because juggling native C++ runtimes and JNI lifecycles on mobile is painful. It handles engine pooling and GPU backend fallbacks (OpenCL -> Vulkan -> CPU) so the app doesn't crash on device-specific drivers.
* **LightDiffusion-Next** ([github](https://github.com/Aatricks/LightDiffusion-Next)) - A fast, memory-optimized Stable Diffusion execution pipeline and GUI written from scratch using PyTorch. Built specifically to squeeze high performance and low VRAM footprint out of desktop GPUs.
* **EasyReader** ([github](https://github.com/Aatricks/EasyReader)) - A lightweight Android manga and PDF reader. It uses my `llmedge` library to generate offline chapter summaries and run text-to-speech, keeping all user data completely on the phone.
* **LightDiffusion** ([github](https://github.com/Aatricks/LightDiffusion)) - An ultra-minimal Stable Diffusion GUI and pipeline in a single Python script.
* **Newelle-Light-Diffusion** ([github](https://github.com/Aatricks/Newelle-Light-Diffusion)) - Extension to use LightDiffusion as an image-generation backend for the Newelle chat GUI.

## Systems & Low-Level

* **Pilotrs** ([github](https://github.com/Aatricks/Pilotrs)) - A 6DOF flight simulator and autopilot core written in Rust (`no_std`). Autopilot estimates state using complementary filters / MEKF and controls them via LQR/PIDs.
* **FrameLimiter** ([github](https://github.com/Aatricks/FrameLimiter)) - macOS frame pacer for Metal games. Hooks `CAMetalLayer`'s `nextDrawable` using DYLD injection to apply backpressure, cutting down real GPU power draw and heat.
* **Atoll** ([github](https://github.com/Aatricks/Atoll)) - A macOS system monitor menu bar app. I forked the original and added a standalone volume mixer, custom EQ, a Spotify controller, a file explorer, and custom resource graphs.
* **PoSubmarine** ([github](https://github.com/Aatricks/PoSubmarine)) - Control stack for an autonomous submarine prototype. Wrote the sensor fusion Kalman filters to get clean heading estimates out of noisy IMU data.
* **CChess** ([github](https://github.com/Aatricks/CChess)) - A lightweight chess engine written in pure C.

## Android Utilities & Automation

* **Android-battery-optimizer** ([github](https://github.com/Aatricks/Android-battery-optimizer)) - A script that runs customized battery saving rules on Android devices via automated ADB calls.
* **Novel-Scraper** ([github](https://github.com/Aatricks/Novel-Scraper)) - Lightweight Android light novel reader with automated web parsers.
* **Boubou** ([github](https://github.com/Aatricks/Boubou)) - Discord bot cycling statuses with Stable Diffusion image generation support.

## Configs & Tools

* **NixOS-EasyConfig** ([github](https://github.com/Aatricks/NixOS-EasyConfig)) - My personal flake-based NixOS config.
* **Arch-Matebook-X-Pro** ([github](https://github.com/Aatricks/Arch-Matebook-X-Pro)) - Scripts to automate setting up Arch Linux on my Matebook.
* **pixcii** ([github](https://github.com/Aatricks/pixcii)) - CLI tool to convert images to colorized ASCII art with optional ML matting (U2Net/BiRefNet).
* **Julia_Set** ([github](https://github.com/Aatricks/Julia_Set)) - Interactive Julia Set fractal renderer using a Python frontend and a Rust backend.
