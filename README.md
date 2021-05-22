# kalulu-server

Tu run the app image on DockerHub, first create a folder where you want the app to save the files containing the data sent to the server in each request. Suppose this folder is `/var/received`

```bash
docker run -d --name kalulu -p 8080:3000 -v "/var/received":"/app/received" danielmmartin/kalulu-server:latest
```

The app will receive the requests in the endpoint `/log` via POST method using application/x-www-form-urlencoded Content-Type in the body.
