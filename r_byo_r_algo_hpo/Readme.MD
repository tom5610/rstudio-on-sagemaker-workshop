
### build

Use the commands to build the image. 

```shell
aws ecr get-login-password --region us-east-1 | docker login --username AWS --password-stdin 482851446821.dkr.ecr.us-east-1.amazonaws.com

docker build -t rmars:latest .

docker tag rmars:latest 482851446821.dkr.ecr.us-east-1.amazonaws.com/rmars:latest

docker push 482851446821.dkr.ecr.us-east-1.amazonaws.com/rmars:latest
```