# LLM CLI Usage Guide

This is all excerpted from the documentation [here](https://llm.datasette.io/en/stable/index.html)

## Installation

```bash
uv tool install llm
```

## Setup with Keys

```bash
llm keys set openai
```
Copy the api key into the terminal when prompted.

## Use Programmatically

```bash
llm 'what is the capital of france?'
```

## Use Interactively

```bash
llm chat -m chatgpt
```

## Check Downloaded Models

```bash
llm models
```

## Check Available Plugins

```bash
llm plugins
```

## Plugin Management

### Install Plugin

```bash
llm install llm-ollama
```

> This plugin provides access to all the models from [https://ollama.com/](https://ollama.com/)

### Uninstall Plugin

```bash
llm uninstall llm-ollama
```

## Logs

### Log Storage

- Logs are stored in an SQLite database

### Check Log Path

```bash
llm logs path
```

### Log Status

```bash
llm logs status
```

### Turn Logging Off

```bash
llm logs off
llm logs status
```

### Turn Logging On

```bash
llm logs on
```

### Show a Truncated JSON Log

```bash
llm logs -n 1 -t --json
```

### Show a Human-Readable Log

```bash
llm logs -n 1 --short
```

### Query Logs

```bash
llm logs -q "france"
```
