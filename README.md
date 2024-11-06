# WebUI-Boilerplate
A simple docker project with docker compose to create a WebUI + Ollama Service.

## Requiriments/Requisitos
- Docker Engine or Docker Desktop installed
- Docker compose plugin

## Usage
Clone this repository in a specific folder
```bash
git clone git@github.com:ldcmleo/WebUI-Boilerplate.git
```

this create a new folder called _WebUI-Boilerplate_, go to this folder and run:

```bash
cd WebUI-Boilerplate
docker compose up -d
```

## Create a model for Ollama
This service use Ollama to create models and use it like chatgpt to create a similar environment.
To create a new model in your Ollama service u need to:

### Using the Ollama container
To enter to the Ollama's container you need to do:

```bash
docker exec -it ollama bash
```

Once you get into the container just create the new model with ollama instruction
```bash
ollama run llama3.2
```

Found available models for ollama here:
![Ollama Website](https://ollama.com/library)