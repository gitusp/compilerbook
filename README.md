https://www.sigbus.info/compilerbook#%E5%86%8D%E5%B8%B0%E3%82%92%E5%90%AB%E3%82%80%E7%94%9F%E6%88%90%E8%A6%8F%E5%89%87

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
