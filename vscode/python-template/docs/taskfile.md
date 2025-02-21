# Taskfile Setup and Usage Guide

## Installation

Install Task:

```bash
# For macOS (using Homebrew)
brew install go-task/tap/go-task

# For Linux (using snap)
sudo snap install task --classic

# For Windows (using scoop)
scoop install task
```

## Common Commands

### Basic Usage

- List all available tasks:

  ```bash
  task --list
  ```

- Run a specific task:

  ```bash
  task <task-name>
  ```

- Run a task with arguments:

  ```bash
  task <task-name> -- <arguments>
  ```

### Advanced Usage

- Watch for file changes and run task:

  ```bash
  task --watch <task-name>
  ```

- Run multiple tasks sequentially:

  ```bash
  task <task1> <task2>
  ```

- Force task execution (ignore up-to-date status):

  ```bash
  task --force <task-name>
  ```

- Show task details and dependencies:

  ```bash
  task --summary <task-name>
  ```

### Development Tips

- Use `silent: true` to suppress command output
- Use `dir:` to specify working directory for a task
- Use `sources:` and `generates:` for file-based task dependencies
- Use `env:` for environment variables
- Use `preconditions:` to add execution conditions
