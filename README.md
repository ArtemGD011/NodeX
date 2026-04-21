# NodeX

NodeX is an advanced Python-based terminal with a customizable interface, built-in commands, plugin support, file management tools, scripting features, and mini-games. It provides a powerful and flexible alternative to a traditional shell.

## Features

* Customizable interface with ANSI colors and themes
* Minecraft-style color codes (`&a`, `&c`, etc.)
* Built-in commands for files, system, and utilities
* Plugin system for extending functionality
* Variables and aliases support
* Pipes and output redirection (`|`, `>`, `>>`)
* Built-in text editor (`nano`)
* Command history and autocomplete
* Mini-games (Snake, Minesweeper, 2048, Tetris, Pong)
* Multilingual support (including Russian aliases)

## Installation

```
git clone https://github.com/ArtemGD011/nodex.git
cd nodex
python test.py
```

## Usage

```
help
echo &aHello World
calc 2 + 2 * 5
mkdir test
cd test
write file.txt Hello
cat file.txt
snake
```

## Plugins

Create a Python file in the `plugins` folder:

```
from nodex import command

@command("hello", "Say hello")
def hello(console, args):
    console.print_line("Hello from plugin!")
```

## Configuration

All configuration files are stored in:

```
~/.nodex/
```

* config.json
* history.json
* aliases.json
* variables.json

## License

MIT License

## Author

Veez_615
