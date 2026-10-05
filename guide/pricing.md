# Credit System, Plans & Pricing Reference

OramiVoice operates on a hybrid model offering generous credit balances for cloud clusters, as well as **Unlimited Neural Tiers** with dedicated **Self-Hosted GPU** capabilities.

---

## Membership Tiers & Packages

| Tier / Package | Price | Credits & Allocations | Key Privileges |
| :--- | :--- | :--- | :--- |
| **Starter Access (FE)** | **$17** (One-Time / Intro) | **500,000 Credits** | 5 Custom Voice Clone slots, Full Web & Desktop Studio Access, Standard Cloud Clusters |
| **Unlimited Neural Engine (OTO 1)** | **Subscription / Upgrade** | **Unlimited Speech & Cloning** | **Full Self-Hosted GPU Access**, Unlimited Zero-Shot Voice Clones, Priority Neural GPU Cluster |
| **Unlimited Image Studio (OTO 2)** | **Subscription / Upgrade** | **Unlimited Image Generation** | **Full Self-Hosted GPU Access**, 2K/4K Upscaling, Commercial Art License |
| **Enterprise Dedicated** | **Custom** | **Custom Quotas** | Private Dedicated Cluster, SLA Support, Custom Model Fine-Tuning |

> **Self-Hosted GPU Privilege**: Users on the **Unlimited Neural Engine (OTO 1)** and **Unlimited Image Studio** tiers can connect their own Google Colab GPU, RunPod, or local NVIDIA RTX hardware via `/servers.php`. All synthesis tasks routed to self-hosted GPUs consume **0 cloud credits**.

---

## Standard Cloud Credit Consumption

When utilizing OramiVoice's managed high-speed cloud clusters, credits are deducted per task according to the table below:

| Service / Action | Unit Measure | Credit Cost | Description |
| :--- | :--- | :--- | :--- |
| **Text to Speech (TTS)** | Per Character | `1 Credit` | Synthesizes 1 text character across 500+ neural voices in 40+ languages. |
| **Nano Banana Pro Image** | Per Image | `2,000 Credits` | High-fidelity photorealistic generation with intricate details. |
| **Nano Banana Image** | Per Image | `1,500 Credits` | Rapid generation for storyboarding and social graphics. |
| **Image Upscale 2K** | Per Image | `500 Credits` | Enhances image resolution to crisp 2K definition. |
| **Image Upscale 4K** | Per Image | `1,000 Credits` | Enhances image resolution to ultra-detailed 4K print quality. |
| **Speech Transcription (STT)**| Per Second | `15 Credits` | Transcribes spoken audio into timestamped subtitle cues (.srt / .vtt). |
| **Neural Subtitle Translation**| Per Character | `1 Credit` | Translates and synchronizes subtitles across multiple languages. |
| **Voice Cloning Slot** | Per Voice Model | Free in Plan (5 Slots in Starter, Unlimited in OTO 1) | Creates a persistent instant clone profile from 3-5s audio sample. |
| **Self-Hosted GPU Tasks** | Any Task | **0 Credits** | All workloads routed through your connected self-hosted GPU servers. |

---

## Checking Your Real-Time Balance

- Your remaining credit balance is displayed live in the top right navigation bar of the application.
- All generation tasks log credit transactions to your workspace history.
- If a task fails or is canceled before processing begins, zero credits are deducted.

---

## Upgrades & Credit Top-Ups

To upgrade your tier or add more on-demand credits:
1. Open the **Subscription** page (`/subscription.php`).
2. Select your desired package (e.g. Starter 500K or Unlimited Neural Engine).
3. Complete checkout to unlock new credits and permissions instantly.
