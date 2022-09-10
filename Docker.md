# Docker environment

Build image 

```
docker build -t torchdiffeq -f Dockerfile .
```

Run tests

```
docker run --rm -it --env="DISPLAY" -v $PWD:/app torchdiffeq python tests/run_all.py
```