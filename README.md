# Wen CLI

An AI-powered command-line assistant that helps you execute shell commands and multi-step tasks.

## Features

- AI-powered command generation
- Multi-step task execution
- Command safety analysis
- Cross-platform color support
- Conversation history with context

## Installation

### From Source

1. Clone this repository:
```bash
git clone <your-repo-url>
cd wen-cli
```

2. Install the package in development mode:
```bash
pip3 install -e .
```

### Global Installation

To install globally so you can run `wen` from anywhere:

#### Linux & macOS

```bash
pip3 install -e . --user
```

**Verify PATH Setup**: After installation, verify that `~/.local/bin` is in your PATH:

```bash
echo $PATH | grep -q "\.local/bin" && echo "PATH OK" || echo "Add ~/.local/bin to PATH"
```

If the command shows "Add ~/.local/bin to PATH", you'll need to add it to your shell configuration file (`.bashrc`, `.zshrc`, etc.):
```bash
export PATH="$HOME/.local/bin:$PATH"
```

#### Windows

```cmd
pip install -e . --user
```

**Verify PATH Setup**: After installation, verify that the Python Scripts directory is in your PATH:

```cmd
echo %PATH% | findstr "Scripts" && echo PATH OK || echo Add Python Scripts to PATH
```

If the command shows "Add Python Scripts to PATH", you'll need to add the Scripts directory to your system PATH. The typical location is:
```
%APPDATA%\Python\Python3x\Scripts
```
Where `3x` is your Python version (e.g., `Python39`, `Python310`, etc.).

## Setup

1. Create a `.env` file in the project root:
```
OPENAI_API_KEY=your_openai_api_key_here
```

2. Make sure you have an OpenAI API key and add it to your `.env` file.

## Usage

After installation, you can run the CLI from anywhere:

```bash
wen
```

The CLI will start and you can interact with it using natural language to execute commands.

## Examples

- "find my documents folder"
- "setup a new python project"
- "open visual studio code"
- "list all python files in current directory"

## Note

The `wen` command provides an AI-powered CLI assistant. It doesn't conflict with any system commands.

## Requirements

- Python 3.7+
- OpenAI API key
- Internet connection for AI responses

## License

MIT License 