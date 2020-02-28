# aws-tools
docker-compose of the best tools

Install docker-compose
https://docs.docker.com/compose/install/

For ubuntu:
```
sudo curl -L "https://github.com/docker/compose/releases/download/1.25.3/docker-compose-$(uname -s)-$(uname -m)" -o /usr/local/bin/docker-compose
```
Next, edit the .env file. Typically you can set the AWS_CONF_DIR to ~/.aws depending on your OS.

```
AWS_CONF_DIR=~/.aws # (or $HOME/.aws, or /user/username/.aws)
```

```
docker-compose up
```
