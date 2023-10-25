# Dockerfileをローカルで実行する方法

# CONTRIBUTING

## How to run the dockerfile lockally

### ビルド
```
docker build -t flask-gunicorn-api .
```


### コンテナ起動
```
Linux
docker run -dp 5000:5000 -w /app -v "$(pwd)/app" flask-gunicorn-api sh -c "flask run --host 0.0.0.0"
```

```
Windows comand prompot
docker run -dp 5000:5000 -w /app -v "%cd%:/app" flask-gunicorn-api sh -c "flask run --host 0.0.0.0"
```