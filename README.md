# tstl-monorepo

This repository showcases a bug with TypeScriptToLua. It can't resolve code specified with the "paths" option in the "tsconfig.json" file.

Steps to reproduce:

```sh
git clone git@github.com:Zamiell/tstl-monorepo.git
cd tstl-monorepo
yarn
cd packages/tstl-program
cat src/main.ts # Observe what this simple "hello world" style program is doing.
npx tstl # Notice that TypeScript can compile the program just fine.
npx tstl # Notice that TypeScriptToLua fails to compile the program.
```
