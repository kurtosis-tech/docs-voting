# docs-voting
a simple backend server to track upvotes/downvotes for features in documentation

### Instructions to Run

1. Start a Redis instance locally (ideally using kurtosis - `kurtosis run github.com/kurtosis-tech/redis-package`) :)
2. Build a docker image `docker build . -t <>`
3. Run container
```
docker run --network=host -e REDIS_HOST=redis://localhost:<port your redis instance is running on> tedim52/docs-voting-app:latest 
```