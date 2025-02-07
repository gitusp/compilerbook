https://www.sigbus.info/compilerbook#make%E3%81%AB%E3%82%88%E3%82%8B%E3%83%93%E3%83%AB%E3%83%89

```sh
# Docker image for compile
docker build --platform linux/x86_64 -t compilerbook https://www.sigbus.info/compilerbook/Dockerfile

# One shot command example
docker run --platform linux/x86_64 --rm -v `pwd`:/work -w /work compilerbook cc -o dist/foo src/foo.c

# Interactive shell
docker run --platform linux/x86_64 --rm -v `pwd`:/work -w /work -it compilerbook
```

## Useful Links

- [Compiler Explorer](https://godbolt.org/z/RyNqgE)
