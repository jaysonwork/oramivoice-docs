# Self-Hosted GPU & Colab Integration

OramiVoice provides **Self-Hosted GPU Acceleration** for high-volume creators, production studios, and power users. This allows you to route speech synthesis, voice cloning, audio transcription, and image generation requests directly to your own GPU hardware or free/cloud notebooks with **zero cloud credit consumption**.

---

## Access & Eligibility

Self-Hosted GPU access is an advanced feature reserved for:
- **Unlimited Neural Engine (OTO 1)** tier members.
- **Unlimited Image Generation** tier members.
- Custom Enterprise & Dedicated Infrastructure plans.

> **Note**: Free and Starter (500K credits) tiers run exclusively on OramiVoice's managed high-speed cloud clusters. To unlock Self-Hosted GPU privileges, upgrade to **OTO 1 (Unlimited Neural Engine)** on the [Subscription Page](/subscription.php).

---

## Supported Endpoints & Models

When connected to your self-hosted GPU endpoint, OramiVoice can offload the following workloads:

| Workload | Supported Models | Endpoint Type |
| :--- | :--- | :--- |
| **Speech-to-Text (STT)** | Fast Whisper Large-v3, Faster-Whisper | `/v1/audio/transcriptions` |
| **Neural Text-to-Speech** | CosyVoice 2, F5-TTS, MeloTTS, ChatTTS | `/v1/audio/speech` |
| **Voice Cloning** | Instant Zero-Shot Cloning (3s reference) | `/v1/voices/clone` |
| **Image Generation** | SDXL Turbo, FLUX.1 Schnell, Realistic Vision | `/v1/images/generations` |

---

## Setup Methods

### Method 1: Google Colab GPU (1-Click Free / Pro Setup)
1. Open the official **OramiVoice Colab Notebook** (link available in [Account Settings -> Colab GPU](/profile.php?tab=colab)).
2. Select runtime hardware: **Runtime -> Change runtime type -> T4 GPU / A100 GPU**.
3. Run Step 1 to install the lightweight OramiVoice GPU Agent and Cloudflare Tunnel / Ngrok.
4. Copy the public tunnel URL provided at the end of the notebook (e.g., `https://your-session.trycloudflare.com`).
5. Open [Self-Hosted Servers](/servers.php), click **Connect New Server**, paste the URL, and click **Verify Connection**.

### Method 2: Cloud GPU Providers (RunPod, Vast.ai, Lambda Labs)
1. Launch an Ubuntu 22.04 template with an NVIDIA RTX 3090, 4090, or A6000 GPU.
2. Clone and run the OramiVoice worker container:
   ```bash
   git clone https://github.com/jaysonwork/oramivoice-worker.git
   cd oramivoice-worker && bash start.sh
   ```
3. Expose the worker port via Cloudflare Tunnel or an open reverse proxy.
4. Register your server endpoint in [Self-Hosted Servers](/servers.php).

### Method 3: Local Desktop GPU (RTX 3060 12GB or higher)
1. Launch the **OramiVoice Desktop App** on your local machine.
2. Go to **Settings -> Local GPU Engine -> Start Worker**.
3. The desktop app will bind to `http://localhost:8000` or broadcast a secure local tunnel for your account.

---

## Verifying Server Status

Once connected, navigate to **Self-Hosted Servers** (`/servers.php`):
- **Health Check**: OramiVoice sends a heartbeat ping every 30 seconds to monitor GPU VRAM, temperature, and latency.
- **Auto Fallback**: If your self-hosted server goes offline, OramiVoice automatically routes urgent requests back to cloud clusters without interrupting your workflow.
- **Credit Saving Indicator**: All generations processed through your self-hosted server display a **`0 Credits`** badge in your history logs.
