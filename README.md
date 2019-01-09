```
NAME:
    template -- Language Templates

SYNOPSIS:
    template <language> [<options>]
    template <language> --help

Languages:
    cpp (c++), rust, ruby
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

<details>
<summary>How it works</summary>

Command `template $1 $2 $3...` will be replaced to `lang/$1 $2 $3...` and it runs.
Every `lang/$1` (`lang/cpp`, `lang/rust` ...) are scripts (i like shell script).

For convinience, `$1` can be aliases (defined in `./alias`).
For example, `template cc` will be `lang/cpp`.
</details>
