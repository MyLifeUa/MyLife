
## How to speed up pipelines

Only 2000 minutes/month for pipelines on Gitlab shared runners.

**Solution:** Our own runner

*Or:* Speed up the process

### 3 points

1. [Cache Dependencies](https://docs.gitlab.com/ee/ci/caching/)
2. [Cache Docker Containers](https://docs.gitlab.com/ee/ci/docker/using_docker_build.html#using-docker-caching) (between jobs on the same pipeline)
3. [Docker-Slim](https://github.com/docker-slim/docker-slim) (smaller docker images)
