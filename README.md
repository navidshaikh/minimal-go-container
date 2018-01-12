Minimal golang container
------------------------


To create a static binary, run
```
CGO_ENABLED=0 GOOS=linux go build -a -installsuffix cgo -o main .
```

Build container image
```
docker run --rm -t go-helloworld -f Dockerfile.scratch .
```
