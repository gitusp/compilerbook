https://www.sigbus.info/compilerbook#%E5%88%86%E5%89%B2%E3%82%B3%E3%83%B3%E3%83%91%E3%82%A4%E3%83%AB%E3%81%A8%E3%83%AA%E3%83%B3%E3%82%AF

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
