# Go 泛型约束

# 一、为什么有这个？
- Go原生的`golang.org/x/exp/constraints`已经被被官方标记为不推荐，随时可能会移除
- Go原生的包名太长不好记忆，我本人几乎是每次都得去复制粘贴，这个包把包名缩短为了`gtypes`，更短更容易记忆 
- 提供比原生更多一些的类型，目前增加了个Number类型，表示数字的集合，这样当你同时需要Integer和Float的时候就不需要自己组合了 

# 二、安装

```bash
go get -u github.com/golang-infrastructure/go-gtypes
```

# 三、Example

```go
func f[T gtypes.Ordered](t T)
```
