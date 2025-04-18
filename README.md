## hermes
docker build -t overstackescola/code-chat:hermes -f Dockerfile.prod .
docker push overstackescola/code-chat:hermes
kubectl apply -f k8s/app.yaml

git submodule update --remote prisma