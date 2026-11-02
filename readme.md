# @defaultuser233/koishi-plugin-glot

[![npm](https://img.shields.io/npm/v/@defaultuser233/koishi-plugin-glot?style=flat-square)](https://www.npmjs.com/package/@defaultuser233/koishi-plugin-glot)

在 Koishi 中使用 [glot.io](https://glot.io) 执行代码。

> 这是 [koishijs/koishi-plugin-glot](https://github.com/koishijs/koishi-plugin-glot) 的维护分支。
> glot.io 已停用旧的 `/api/run/:language/latest` 接口，本分支改用新前端调用的
> `/api/mux` 接口，并按语言内置了容器镜像、编译命令和运行命令。

## 配置项

### apiToken

- 类型: `string`

已弃用。新版 glot.io 接口无需令牌，保留此项仅为兼容旧配置。

### defaultLanguage

- 类型: `string`
- 默认值: `'javascript'`

默认的执行语言。

## 指令: glot

支持的语言:

assembly, ats, bash, c, clisp, clojure, cobol, coffeescript, cpp, crystal, csharp, d,
dart, elixir, elm, erlang, fsharp, go, groovy, guile, hare, haskell, idris, java,
javascript, julia, kotlin, lua, mercury, nim, nix, ocaml, pascal, perl, php, python,
raku, ruby, rust, sac, scala, swift, typescript, zig

- 基本语法: `glot <code>`
- 选项列表:
  - -l, --language \<language> 语言
  - -s, --stdin \<stdin> 标准输入
