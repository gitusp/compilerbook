https://www.sigbus.info/compilerbook#%E3%82%B9%E3%83%86%E3%83%83%E3%83%977-%E6%AF%94%E8%BC%83%E6%BC%94%E7%AE%97%E5%AD%90

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
