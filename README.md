# docker-tar-push
push your docker tar archive image without docker

## Usage:

```shell
push your docker tar archive image without docker.

Usage:
  docker-tar-push [flags]

Flags:
  -h, --help              help for docker-tar-push
      --log-level int     log-level, 0:Fatal,1:Error,2:Warn,3:Info,4:Debug (default 3)
      --password string   registry auth password
      --registry string   registry url
      --skip-ssl-verify   skip ssl verify
      --username string   registry auth username
```

Example:

```shell
docker-tar-push alpine:latest --registry=http://localhost:5000
```

## Build

```sh
go build -o bin/docker-tar-push cmd/docker-tar-push/main.go
```

## Reference
1. https://blog.csdn.net/github_19391267/article/details/107274210
2. https://docs.docker.com/registry/spec/api/
3. https://sreekesh-s.medium.com/uploading-docker-images-using-docker-registry-api-golang-5242ccb0d3dd
4. https://github.com/distribution/distribution
