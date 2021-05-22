# kalulu-server

Tu run the image on DockerHub, you can do

```bash
docker run -d --name kalulu -p 8080:3000 -v "$PWD/received":"/app/received" danielmmartin/kalulu-server:latest
```

Then open a browser and visit `http://localhost:8080/`
