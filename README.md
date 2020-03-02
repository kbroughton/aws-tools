# aws-tools
docker-compose of the best tools

Install docker-compose
https://docs.docker.com/compose/install/

For ubuntu:
```
sudo curl -L "https://github.com/docker/compose/releases/download/1.25.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
Next, edit the .env file. Docker-compose doesn't seem to expand `~` or $HOME, so you need a full path.

```
AWS_CONF_DIR=<your-path-to>/.aws # (or $HOME/.aws, or /user/username/.aws)
```

```
docker-compose up
```

The above will bring up all containers. To just run a single container, specify the name of the service in the compose file.
```
docker-compose up -d cloudmapper
```

