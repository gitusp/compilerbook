https://www.sigbus.info/compilerbook#%E8%91%97%E8%80%85%E3%81%AB%E3%81%A4%E3%81%84%E3%81%A6

```sh
# Docker image for compile
docker build -t compilerbook https://www.sigbus.info/compilerbook/Dockerfile

# One shot command example
docker run --rm -v .:/work -w /work compilerbook make test
```
