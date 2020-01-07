This repo reproduces a typescript issue where the compiler creates a 'http' directory instead of the 'Http' directory, missing the first letter's case.

This happens(in my case) only for the `Http` directory when using `sqlite3` on Windows 10

##### Reproducing
```sh
$ npm install
$ tsc
```

##### Now observe that the `dist/http` is not `dist/Http` with uppercase `H` as the original directory.