https://www.sigbus.info/compilerbook#%E5%86%8D%E5%B8%B0%E4%B8%8B%E9%99%8D%E6%A7%8B%E6%96%87%E8%A7%A3%E6%9E%90

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
