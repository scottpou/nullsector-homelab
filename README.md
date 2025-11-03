# 🖥️ NullSector — Home Lab AI & Container Server

**NullSector** is a high-performance 1U rackmount server configured for advanced AI workloads, container hosting, and lab-scale experimentation. Built around a Dell PowerEdge R630 with massive memory and dual NVIDIA T4 GPUs, it supports local deployment of LLMs, Stable Diffusion, Whisper, RVC, and more — all without the cloud.

## 🔧 Hardware Overview
| Component       | Specs |
|----------------|-------|
| **Server**      | Dell PowerEdge R630 (1U Rackmount) |
| **CPU**         | 2 × Intel Xeon E5-2697 v4 (36 cores / 72 threads total) |
| **Memory**      | 768GB DDR4-2133 ECC (24 × 32GB) |
| **GPU**         | 2 × NVIDIA T4 (16GB GDDR6 each) |
| **Storage**     | Samsung 990 Pro 4TB NVMe (via Supermicro AOC-SLG3-2M2) |
| **Power**       | Dual 750W Redundant PSUs |
| **Management**  | iDRAC8 Enterprise |
| **Networking**  | 2 × 10GbE + 4 × 1GbE NICs |

## 🚀 Use Cases
- 🧠 Local LLM inference (e.g. LLaMA 3 70B, Mixtral, DeepSeek)
- 🎨 Stable Diffusion XL + ControlNet image generation
- 🎤 Whisper Large-v3 transcription
- 🧬 RVC voice cloning + GPT-SoVITS
- 🐳 Docker Compose / K3s / Proxmox virtualization
- 📊 Grafana monitoring dashboards

## 🧪 Models Actively Tested
| Model                   | Type        | Runner              | Notes |
|-------------------------|-------------|----------------------|-------|
| LLaMA 3 70B (Q4_K_M)     | Chat LLM    | llama.cpp / Ollama   | Quantized, Claude-like reasoning |
| Mixtral 8x7B (MoE)       | Chat LLM    | Ollama / llama.cpp   | Fast Claude Instant alternative |
| DeepSeek-Coder 33B       | Coding LLM | GGUF (quantized)     | Best open-source coding model |
| SDXL + DreamShaper       | Diffusion  | Automatic1111        | Image generation & upscaling |
| Whisper Large-v3         | Audio      | faster-whisper       | Speech-to-text, 5× real-time |
| RVC + GPT-SoVITS         | Voice      | Local training/infer | Singing/voice cloning AI |

## 🛠️ Deployment Stack (WIP)
This server is being configured to support:
- Ollama + Open WebUI for chat LLMs
- Automatic1111 + ComfyUI for image generation
- Whisper + API endpoints for transcription
- Docker Compose orchestration
- Optional Proxmox VMs and K3s clusters

## 📸 Screenshots
> _Coming soon_: CLI stats, WebUI snapshots, sample outputs

## 📁 Goals
- Run GPT-4-class models entirely offline
- Host multi-user WebUIs for LLMs and SDXL
- Build a reproducible AI lab-in-a-box environment
- Share Docker configs and setup guides

## 📌 Status
✅ Hardware Installed  
✅ GPU + NVMe + RAM stress-tested  
🚧 LLM & Diffusion stack in progress  
📦 Docker Compose `.zip` bundle coming soon

## 🤝 Contributing / Forking
Once published, feel free to fork this repo or open issues. I'll be sharing model configs, benchmark results, and performance tuning notes.

## 🧾 License
This hardware/config documentation is provided freely under the [MIT License](LICENSE).

