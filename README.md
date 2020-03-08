# hello
Go mod の versioning の方法を学ぶためのサンプルコード

## package の versioning
go.mod を生成。
```bash
$ go mod init
```
バージョニングしたいコミットにタグを打つ
```
$ git tag v1.0.0
$ git push origin --tags
```

## package を version 指定で使用する
```
$ go mod init

$ vim go.mod
module github.com/mozzzzy/hello_user

go 1.13

require github.com/mozzzzy/hello v0.0.1   # version 指定
```
