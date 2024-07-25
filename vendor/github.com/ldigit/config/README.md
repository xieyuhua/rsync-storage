# config
一个方便使用的Go语言YAML配置读取库，封装自yaml.v3

[![Go](https://github.com/ldigit/config/actions/workflows/build.yml/badge.svg?branch=master)](https://github.com/ldigit/config/actions/workflows/build.yml)
[![GitHub release (latest by date)](https://img.shields.io/github/v/release/ldigit/config)](https://github.com/ldigit/config/releases)
[![GitHub go.mod Go version](https://img.shields.io/github/go-mod/go-version/ldigit/config)](https://github.com/ldigit/config/blob/master/go.mod)
[![MIT License](http://img.shields.io/badge/license-MIT-blue.svg)](http://copyfree.org)
[![Go Report](https://goreportcard.com/badge/github.com/ldigit/config)](https://goreportcard.com/report/github.com/ldigit/config)
[![Codacy Badge](https://app.codacy.com/project/badge/Grade/43ca0a1bf7894ecb9389f0a1406b9fc5)](https://www.codacy.com/gh/ldigit/config/dashboard?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=ldigit/config&amp;utm_campaign=Badge_Grade)
[![Codacy Badge](https://app.codacy.com/project/badge/Coverage/43ca0a1bf7894ecb9389f0a1406b9fc5)](https://www.codacy.com/gh/ldigit/config/dashboard?utm_source=github.com&utm_medium=referral&utm_content=ldigit/config&utm_campaign=Badge_Coverage)

## Installation

```shell
go get -u github.com/ldigit/config
```

## Quick Start

```go

// Suppose your config file path is config_test.yaml
const ConfigFilePath = "config_test.yaml"

cfg, err := config.Load(ConfigFilePath)
if err != nil {
    log.Fatalln(err)
}

// Suppose there are demo_string entries of type string in your config file
fmt.Println(cfg.GetString("demo_string", "it is default value"))


```

## License
Released under the [MIT License](LICENSE).
