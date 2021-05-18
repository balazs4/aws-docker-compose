# aws-ecs :heart: docker-compose :whale:

> the true lift-and-shit approach

## setup

```bash
#https://github.com/docker/compose-cli
curl -L https://raw.githubusercontent.com/docker/compose-cli/main/scripts/install/install_linux.sh | sh

# https://docs.docker.com/cloud/ecs-integration/
docker context create ecs aws-from-env

# export AWS_ACCESS_KEY_ID=xxxxxxxxxxxxxxxxxx
# export AWS_SECRECT_ACCESS_KEY=xxxxxxxxxxxxxxxxxx
```


```bash
# switch context
docker context use aws-from-env

# inspect docker-compose
cat docker-compose.yaml

# inspect cloudformation
docker compose convert

# deploy docker-compose as cloudformation stack in AWS :heat: :heart_eyes:
docker compose up

# get the domain
docker compose ps

# check content
curl <domain>

# show cloudwatch logs :exploding_head:
docker compose logs

# remove AWS resources :money_with_wings:
docker compose down
```
