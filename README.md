## perseu
docker build -t overstackescola/code-chat:latest -f Dockerfile.prod .
docker push overstackescola/code-chat:latest
kubectl apply -f k8s/app.yaml

git submodule update --remote prisma