# VideoSDK X Neuphonic TTS Demo

This example demonstrates how to build a conversational AI Voice Agent using VideoSDK with **Neuphonic TTS** built using the [videosdk-neuphonic](https://pypi.org/project/videosdk-plugins-neuphonic/) plugin.

# Architecture Overview

The agent is built using VideoSDK’s Pipeline (Cascade Mode), which provides a flexible, modular approach to building AI agents by allowing you to mix and match different components for Speech-to-Text (STT), Large Language Models (LLM), Text-to-Speech (TTS), Voice Activity Detection (VAD), and Turn Detection.

<img width="3026" height="582" alt="videosdk_casading_pipeline" src="https://github.com/user-attachments/assets/cbdb6a40-efb4-41e9-b056-868b0f9ba287" />

## Prerequisites

- Python 3.11+
- A [VideoSDK Account](https://dub.sh/A1vscPp)
- A [Neuphonic API Key](https://app.neuphonic.com/apikey)
- A [Deepgram API Key](https://console.deepgram.com/apikeys)
- A [Google Gemini API Key](https://aistudio.google.com/apikey)

## Installation

1.  **Clone the repository:**

    ```bash
    git clone https://github.com/videosdk-community/videosdk-neuphonic-tts-demo.git
    cd videosdk-neuphonic-tts-demo
    ```

2.  **Create a virtual environment:**

    ```bash
    python -m venv .venv
    ```

    Activate the virtual environment:
    - MacOS/Linux: `source .venv/bin/activate`
    - Windows: `.venv\Scripts\activate`

3.  Install the required dependencies:

    ```bash
    pip install -r requirements.txt
    ```

4.  Set up environment variables:
    Copy `.env.example` to `.env` and fill in your keys.

    ```bash
    cp .env.example .env
    ```

    **Required Variables:**
    - `NEUPHONIC_API_KEY`
    - `DEEPGRAM_API_KEY`
    - `GOOGLE_API_KEY`
    - `VIDEOSDK_API_KEY` and `VIDEOSDK_SECRET_KEY`

## Usage

Run the agent with the following command:

```bash
python main.py
```

## What Happens Next?

The agent creates a VideoSDK playground session and a joinable URL is printed in the terminal, Open the URL in your browser and Start speaking the agent will respond in real time 🎙️

<img width="1459" height="815" alt="Screenshot 2026-01-29 at 12 03 20 PM" src="https://github.com/user-attachments/assets/0b6e20eb-7d84-404e-bdea-ad97757a8230" />


## Resources

- Read more about the Neuphonic TTS Plugin [Neuphonic TTS Plugin Documentation](https://docs.videosdk.live/ai_agents/plugins/tts/neuphonic-tts)
- Explore Pipeline (Cascade Mode) [Pipeline Documentation](https://docs.videosdk.live/ai_agents/core-components/pipeline)
- Neuphonic [Documentation link](https://docs.neuphonic.com/)

## VideoSDK Agents

Build and deploy production-ready AI voice & video agents with [VideoSDK](https://videosdk.live). This repo is your central hub for agent templates, feature examples, and everything you need to ship real-world AI-powered applications.

| Resource | Description |
|---|---|
| 🚀 [Use Case Examples](https://github.com/videosdk-live/agents/tree/main/use_case_examples) | Production-ready templates across Customer Support, Healthcare, Tech Support & more |
| ⚡ [Feature Examples](https://github.com/videosdk-live/agents/tree/main/examples) | Always up-to-date examples showcasing the latest VideoSDK Agent features |
| 📖 [AI Agents Docs](https://docs.videosdk.live/ai_agents/introduction) | Full guides, concepts & API references to get you started |

> ⭐ If this helps you, star this repo and [`videosdk-live/agents`](https://github.com/videosdk-live/agents) — it keeps us motivated to ship more!
