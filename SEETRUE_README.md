aws ecr get-login-password --region eu-north-1 --profile st | podman login -u AWS --password-stdin 954214240508.dkr.ecr.eu-north-1.amazonaws.com
podman build -t 954214240508.dkr.ecr.eu-north-1.amazonaws.com/labelstudio:latest .
podman push 954214240508.dkr.ecr.eu-north-1.amazonaws.com/labelstudio:latest