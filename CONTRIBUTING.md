## How to run docker locally

```
docker build -t IMAGE_NAME .
docker run -dp 5005:5000 -w /app -v "$(pwd):/app" IMAGE_NAME sh -c "flask run --host 0.0.0.0"
```