# Docker Configuration

Build the Docker image
```bash
docker build -t python-whatsapp-bot .
```

To pass the .env file, remove the quotes (") and the comments after the varibles.

Run the Docker container, mapping port 8000 inside the container to port 8000 on your host
```bash
docker run --rm --env-file .env --name zap -p 8000:8000 python-whatsapp-bot
```

