# VideoSDK Neuphonic TTS Demo

This example demonstrates how to build a conversational AI Voice Agent using VideoSDK with **Neuphonic TTS** in Cascading Pipeline.

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
    - `VIDEOSDK_AUTH_TOKEN`

## Usage

Run the agent with the following command:

```bash
python main.py
```

The script will initialize a playground session and provide a URL. Join the room from your browser.

## Documentation

- [Neuphonic TTS Plugin Documentation](https://docs.videosdk.live/ai_agents/plugins/tts/neuphonic-tts)
- [Cascading Pipeline Documentation](https://docs.videosdk.live/ai_agents/core-components/cascading-pipeline)
