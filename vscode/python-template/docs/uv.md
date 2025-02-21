# UV setup

This docs focuses on essential `uv` commands for Python project management. UV is a modern package manager for Python.

After you get uv installed, you can run `uv sync` to install the dependencies.

## Install `uv`

```bash
curl -LsSf https://astral.sh/uv/install.sh | sh
```

## Package Management

Install packages (two methods):

```bash

uv add <package>
# or
uv pip install <package>
```

## Running Code

Execute scripts/files:

```bash
uv run <script.py>
```

## Code Quality

Check and format code with Ruff:

```bash
uvx ruff check
uvx ruff format
```

## Testing

Add pytest as a development dependency:

```bash
uv add pytest --dev
```

Run tests:

```bash
uv run pytest
```

## Building and Publishing

Build your project:

```bash
uv build
```
