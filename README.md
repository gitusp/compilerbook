https://www.sigbus.info/compilerbook#%E9%96%A2%E6%95%B0%E5%91%BC%E3%81%B3%E5%87%BA%E3%81%97%E3%82%92%E5%90%AB%E3%82%80%E4%BE%8B

```sh
# Docker image for compile
docker build -t compilerbook https://www.sigbus.info/compilerbook/Dockerfile

# One shot command example
docker run --rm -v .:/work -w /work compilerbook make test
```
