## Prerequisites

- [Docker Desktop]([http://](https://docs.docker.com/get-docker/))

## Testing

### Setup

```
docker run -v $(pwd):/app -w /app/test node npm install
```

### Run all tests

```
docker run -it -v $(pwd):/app -w /app/test node npm test
```

## Template

```
cat ./template/sample.in | docker run -i -v $(pwd):/app -w /app/template node node index.js
```

to run the tests:

```
docker run -it -v $(pwd):/app -w /app/test node npm test template.test.js
```

## Qualification

## Reversort

```
cat ./qualifying/reversort/sample.in | docker run -i -v $(pwd):/app -w /app/qualifying/reversort node node index.js
```

to run the tests:

```
docker run -it -v $(pwd):/app -w /app/test node npm test qualifying/reversort.test.js
```
