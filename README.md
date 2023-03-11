# GitHubRunner

## Build Runner

```sh
docker build --build-arg RUNNER_VERSION=2.292.0 --tag lucasschmitz/github-runner .
```

```sh
docker push lucasschmitz/github-runner:latest
```

## Run Runner

```sh
docker run --name github-runner-1 -e GH_TOKEN='myPatToken' -e GH_OWNER='orgName' -e GH_REPOSITORY='repoName' -d lucasschmitz/github-runner:latest
```