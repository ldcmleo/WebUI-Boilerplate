# WebUI-Boilerplate
A simple Docker project with Docker Compose to set up a WebUI and Ollama Service environment.
## Requiriments/Requisitos
- Docker Engine or Docker Desktop installed
- Docker compose plugin

## Usage
Clone this repository in a specific folder
```bash
git clone git@github.com:ldcmleo/WebUI-Boilerplate.git
```

This will create a folder called WebUI-Boilerplate. Navigate into this folder and start the services:

```bash
cd WebUI-Boilerplate
docker compose up -d
```

## Creating a Model for Ollama
This service uses Ollama to create models, providing an environment similar to ChatGPT. To create a new model with your Ollama service, follow these steps:

### Using the Ollama container
To access the Ollama container, run the following command:

```bash
docker exec -it ollama bash
```

Once inside the container, create the new model using an Ollama command, for example:
```bash
ollama run llama3.2
```

You can find available models for Ollama here: 
![Ollama Website](https://ollama.com/library)