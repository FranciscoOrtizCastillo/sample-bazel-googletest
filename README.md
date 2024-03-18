# Ejemplo Bazel con GoogleTest

## Referencias

[Bazel as an alternative to CMake](https://medium.com/@Vertexwahn/bazel-as-an-alternative-to-cmake-fb7c86d95b48)

[Creating Bazel C++ project with Google Test & Google Benchmark](https://blog.slys.dev/creating-bazel-cpp-project-with-google-test-and-google-benchmark/)

[Casos de uso comunes de compilación de C++ ](https://bazel.build/tutorials/cpp-use-cases?hl=es-419)

[GoogleTest User’s Guide](https://google.github.io/googletest/)

[Bazel Central Registry](https://registry.bazel.build/)

## Pasos

```bash
bazel build //main:HelloWorld     
#bazel build main:HelloWorld  

bazel run //main:HelloWorld     

# Ejectuar test individual por nombre
#bazel run test:test
bazel test --cxxopt=-std=c++14 --test_output=all //test:test

# Ejecutar todos los test
bazel test --cxxopt=-std=c++14 --test_output=all //test:all

bazel run -c opt benchmark:benchmark

```

