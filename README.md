# jjudkins notes

## Mac/Win git carriage-return issues

Windows machine, set it to true – this converts LF endings into CRLF when you check out code:

> $ git config --global core.autocrlf true

On mac, tell Git to convert CRLF to LF on commit but not the other way around by setting core.autocrlf to input:

> $ git config --global core.autocrlf input

Windows-only project, set the config value to false:

> $ git config --global core.autocrlf false

Src: https://stackoverflow.com/questions/5834014/lf-will-be-replaced-by-crlf-in-git-what-is-that-and-is-it-important
