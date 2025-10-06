# Docker compose test for a java app testing environment

This project was made to test the capabilities of docker compose. I wanted to see how it could help me to test a java app, and help me to share it easily.

## How to start it

You only need 2 commands to start :

- In one terminal, start the docker with:

```bash
docker compose up
```

- wait for it to start, this will be the terminal where all the logs goes.
- When "Java installation complete" appear, in another terminal, use :

```bash
docker exec -it java_test_env bash
```

It will bring you inside the docker. Now, the app is in :

- /code_to_test/ for the host
- /home/app/ inside the docker
  To try the app, in the docker, go to /home/app and use the standard java command :

```bash
java -jar Untitled.jar
```
