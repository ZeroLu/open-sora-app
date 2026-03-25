<div align="center">

# 🌌 OpenSoraApp
**They shut down Sora. We're opening it up.**

[![License: MIT](https://img.shields.io/badge/License-MIT-purple.svg)](https://opensource.org/licenses/MIT)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg)](http://makeapullrequest.com)
[![Discord](https://img.shields.io/discord/1234567890?color=5865F2&label=Discord&logo=discord&logoColor=white)](https://discord.gg/opensoraapp)
[![Website](https://img.shields.io/badge/Website-opensoraapp.com-black?logo=vercel)](https://opensoraapp.com)[Website](https://opensoraapp.com) • [The Manifesto](#-the-manifesto) • [Roadmap](#-roadmap) • [Contributing](#-join-the-rebellion-how-to-contribute) • [Discord](https://discord.gg/opensoraapp)

</div>

---

## 📜 The Manifesto

On March 24, 2026, OpenAI pulled the plug on Sora. Citing the need to prioritize compute power for "lucrative enterprise robotics," they effectively abandoned the millions of creators who helped popularize their platform. 

They treated human creativity as a disposable side quest. **We disagree.**

The future of AI video generation shouldn't be locked behind a walled garden, heavily censored by a corporation, or shut down overnight. We are building **OpenSoraApp**—an open-source sanctuary for filmmakers, creators, and developers. Bring your own models. Own your creations. Never lose your work again.

---

## ✨ Features (What we are building)

- 🔌 **Bring Your Own Model (BYOM):** Agnostic architecture. Plug in any open-weights video model (Stable Video, Open-Sora, etc.), local AI, or API. If a new model drops tomorrow, you can use it here today.
- 🔄 **Remix & Evolve ("Git for Video"):** True social creation. Easily branch, remix, and iterate on prompts and videos shared by the community. 
- 🎭 **Consistent Avatars & Characters:** Built-in pipelines utilizing ControlNet and IP-Adapter equivalents to maintain character consistency across multiple shots and generations.
- 🌍 **Social feature:** Comment, like, share. Don't create alone, create with other creators.
---

## 🗺️ Roadmap

We are moving fast. Here is our roadmap to build the ultimate open-source text-to-video framework.

### Phase 1: Foundation (We are here 📍)
- [x] Launch the community hub & Manifesto.
- [ ] Release core UI/UX framework (React/Next.js + Tailwind).
- [ ] Define standardized API schemas for text-to-video inference.
- [ ] Basic integration with initial open-weight video models (via Hugging Face integrations).

### Phase 2: The Creator Engine 
- [ ] One-click local deployment (Docker/RunPod/ComfyUI backend support).
- [ ] Implement the "Remix" branching timeline UI.
- [ ] Launch the Prompt & Output Gallery for community sharing.
- [ ] Add the `thesorawatermarkremover.com` upscaling & cleaning node.

### Phase 3: Advanced Filmmaking
- [ ] Native Director's Timeline (multi-clip stitching and audio generation syncing).
-[ ] Release the "Consistent Avatar" training loop UI.
- [ ] P2P distributed inference (share GPU compute power with the community).

---

## 🛠️ Tech Stack

OpenSoraApp is built to be modular, allowing the frontend UI to operate seamlessly with various local or cloud AI backends.
*   **Frontend:** Next.js, React, Tailwind CSS, Zustand
*   **Backend/API:** Python, FastAPI, WebSockets (for streaming generation progress)
*   **AI Integration:** Diffusers, PyTorch, ComfyUI API wrappers

---

## 🚀 Quick Start (Pre-Alpha)

*Note: The repository is currently in rapid active development. Instructions below are for setting up the development environment.*

```bash
# 1. Clone the repo
git clone https://github.com/OpenSoraApp/OpenSoraApp.git
cd OpenSoraApp

# 2. Setup the Frontend (Web UI)
cd frontend
npm install
npm run dev

# 3. Setup the Backend (Python FastAPI)
cd ../backend
python -m venv venv
source venv/bin/activate  # On Windows: venv\Scripts\activate
pip install -r requirements.txt
uvicorn main:app --reload
