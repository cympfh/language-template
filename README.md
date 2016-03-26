```
NAME:
    template -- Language Templates

SYNOPSIS:
    template <language> [<options>]
    template <language> --help

Languages:
    cpp (c++), rust
```

# Usage

The following command

```bash
$ template cpp
```

outputs a Template for C++.

```bash
$ template cpp --clang
```

outputs a Template flavored for Clang.

To see options of template for C++,

```bash
$ template cpp --help
```

## 方針

1. 全部 bash
    - 単純なのは cat でも良さそうなもんだけど `--help` くらい処理したい
1. `template $1 $2 $3...` を `lang/$1 $2 $3...` に書き換えて bash で実行するだけ
    - 書き換える前にファイルが存在するかとかぐらいのラッパー

