# Modal Setup and Usage Guide

Modal is a cloud platform for running Python code at scale. This guide covers basic setup and common commands.

## Install Modal

Install the Modal client:

```bash
pip install modal
```

Authenticate with Modal:

```bash
modal token new
```

## Common Commands

### Running Code

Run a Python script on Modal:

```bash
modal run <script.py>
```

Run a specific function:

```bash
modal run <script.py>::<function_name>
```

### Managing Apps

Deploy an app:

```bash
modal deploy <script.py>
```

List deployed apps:

```bash
modal app list
```

### Monitoring

View logs:

```bash
modal logs
```

View app status:

```bash
modal app status <app_id>
```

### Development Tips

- Use `@app.function()` decorator to define Modal functions
- Use `modal.Volume` for persistent storage
- Use `modal.Secret` for environment variables
- Use `modal.Image` for custom container images
- Use `modal.schedule()` for periodic tasks
