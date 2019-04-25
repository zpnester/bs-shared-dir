Problem occurs when using both

* sources dir with `../shared/src`
* `"in-source": false`

No such problem with `"in-source": true`

Same results for BuckleScript 4 and 5

## Linux/macOS

`1` fails to (clean) compile
```
I/O error: /app/web/lib/js/../shared/src/shared.bs.js: No such file or directory
```

`2` compiles OK

`2` differs only by one empty .re file

## Windows

Both examples work OK on Windows

## Example
```
cd 1/web
npm i
npm run build
```

## Docker example
```
cd 1
docker build -t test1 .
docker run --rm test1
```

