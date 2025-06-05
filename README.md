https://www.sigbus.info/compilerbook#%E9%96%A2%E6%95%B0%E3%81%A8%E3%83%AD%E3%83%BC%E3%82%AB%E3%83%AB%E5%A4%89%E6%95%B0

```sh
# Docker image for compile
docker build --platform linux/x86_64 -t compilerbook https://www.sigbus.info/compilerbook/Dockerfile

# One shot command example
docker run --platform linux/x86_64 --rm -v `pwd`:/work -w /work compilerbook cc -o dist/foo src/foo.c

# Interactive shell
docker run --platform linux/x86_64 --rm -v `pwd`:/work -w /work -it compilerbook

# Testing
docker run --platform linux/x86_64 --rm -v `pwd`:/work -w /work compilerbook make test
```

## Useful Links

- [Compiler Explorer](https://godbolt.org/z/RyNqgE)
