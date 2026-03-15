# 🤖 Jarvis

> Local LLM assistant accessible directly from your terminal, powered by llama.cpp.

## Features

- 💬 Interactive chat with local GGUF models
- 🧠 Persistent memory files for future sessions
- ⚙️ Configurable via `config.toml`
- 🔧 Slash commands: `/model`, `/memory`, `/reset`, `/save`

## Requirements

- Python 3.10+
- [llama.cpp](https://github.com/ggerganov/llama.cpp) compiled with Metal support
- A `.gguf` model file

## Installation
```bash
git clone https://github.com/David-Aflokkat/jarvis.git
cd jarvis
pip install -r requirements.txt
cp config.toml.example config.toml
# Edit config.toml to point to your model
```

## Usage
```bash
python src/main.py
```

## Project structure
```
jarvis/
├── src/           # Source code
├── memory/        # Persistent memory files (git-ignored)
├── models/        # GGUF model files (git-ignored)
├── config.toml    # Configuration
└── docs/          # Documentation
```

## License

MIT
