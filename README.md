# Project initialization:
    uv init livekit-voice-agent --bare
    cd livekit-voice-agent


# Install packages
uv add \
  "livekit-agents[silero,turn-detector]~=1.3" \
  "livekit-plugins-noise-cancellation~=0.2" \
  "python-dotenv"


# Download model files:
    uv run agent.py download-files


# Speak to your agent via console (Python Only):
    uv run agent.py console