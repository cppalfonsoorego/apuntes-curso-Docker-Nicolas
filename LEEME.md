## Tunel para publicar server local (IMPREIONANTE!!!)

cloudflared tunnel --url http://172.24.210.34:5173/

<!-- Instrucciones para crear el repo en local -->
## Instrucciones para crear el repo en local

echo "# apuntes-curso-Docker-Nicolas" >> README.md
git init
git add README.md
git commit -m "first commit"
git branch -M main
git remote add origin git@github.com:cppalfonsoorego/apuntes-curso-Docker-Nicolas.git
git push -u origin main

<!-- --> Ejemplos de FIND
```
$ find
```

```
$ find ./test -name "*.php"
```
```
$ find ./test -iname "*.Php"
```

```
$ find ./test -maxdepth 2 -name "*.php"
./test/subdir/how.php
./test/cool.php
```

```
$ find ./test -maxdepth 1 -name *.php
./test/cool.php
```

```
$ find ./test -not -name "*.php"
$ find ./test ! -name "*.php"
```

```
$ find ./test -name 'abc*' ! -name '*.php'
$ find -name '*.php' -o -name '*.txt'
```

```
$ find ./test -name abc*
./test/abc.txt
./test/abc

Only files

$ find ./test -type f -name "abc*"
./test/abc.txt

Only directories

$ find ./test -type d -name "abc*"
./test/abc
```

```
$ find ./test ./dir2 -type f -name "abc*"
./test/abc.txt
./dir2/abcdefg.txt
```

```
$ find ~ -type f -name ".*"
```

```
$ find . -type f -perm 0664
./abc.txt
./subdir/how.php
./abc.php
./cool.php
```

```
$ find . -type f ! -perm 0777
./abc.txt
./subdir/how.php
./abc.php
./cool.php
```

