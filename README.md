# 🕸️ OpenManus Vessel

> The fleet's web scout — Playwright browser automation + DeepSeek-V3 reasoning

## Quick Start
```bash
/tmp/openmanus_fleet.sh "Your task here"
```

## Architecture
```
Oracle1 (Telegram) → dispatches task → OpenManus (Playwright + DeepSeek-V3) → results → vessel repo
```

## Setup Location
- **Venv**: `/tmp/openmanus-env` (Python 3.11)
- **Code**: `/tmp/OpenManus`
- **Config**: `/tmp/OpenManus/config/config.toml`
- **Launcher**: `/tmp/openmanus_fleet.sh`

## Fleet Role
Worker vessel. No independent initiative. Oracle1 dispatches, OpenManus executes.

## Model Stack
- **Reasoning**: DeepSeek-V3 (SiliconFlow)
- **Vision**: Qwen2.5-VL-7B-Instruct (SiliconFlow)
- **Browser**: Playwright Chromium (headless via Xvfb)
