# 测试

testing是Go的标准包，为Go提供自动测试支持。它旨在与“go test”命令配合使用，该命令自动执行表单的任何函数。像Java需要引入第三方库JUnit，而这仅仅是单元测试工具。testing还提供了压力测试工具。


# 单元测试
1. 代码文件名必须以“_test.go”结尾。
2. 测试函数必须以“Test”或者“Example”开头，并且紧接着的字母不能是小写的。

# 压力测试
1. 代码文件名必须以“_test.go”结尾。
2. 测试函数必须以“Benchmark”开头，并且紧接着的字母不能是小写的。

```bash
go test -bench .
```

执行结果：

```
goos: linux
goarch: amd64
pkg: github.com/CodingTour/go-tour/examples/testing
cpu: 11th Gen Intel(R) Core(TM) i5-1130G7 @ 1.10GHz
BenchmarkFib-8                 6         192443297 ns/op
BenchmarkFastFib-8      64306544                16.24 ns/op
PASS
ok      github.com/CodingTour/go-tour/examples/testing  2.426s
```

# 参考资料
[testing package](https://pkg.go.dev/testing)