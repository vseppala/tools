# Tools

## Scripts

Add both `scripts` and `scripts_private` (ignored with .gitignore) to your PATH.
```shell
echo "\nexport PATH=\"\$PATH:$(pwd)/scripts"\" >> ~/.zshrc
echo "export PATH=\"\$PATH:$(pwd)/scripts_private"\" >> ~/.zshrc
```

## Docker compose

Compose file contains multiple tools:

- n8n
  - Postgres
  - qdrant
- ollama-webui
- ollama

### Run all the tools!

```
docker compose up --profile ollama-container -d
```

If you want to run tools without ollama (need to have that running somewhere):

```
docker compose up -d
```
