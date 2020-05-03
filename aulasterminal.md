# Lista de aulas de Terminal

## Aula 1

* `pwd`
	* Ele mostra o diretório atual, por exemplo:
```
$ pwd
/home/dyefferson/
```
* `cd`
	* Ele muda o diretório em que você está, por exemplo:
		```
		$ pwd
		/home/dyefferson/
		$ cd Documentos/
		$ pwd
		/home/dyefferson/Documentos/
		```
## Aula 3

* Ensinar `mkdir`
	* Fazer pastas
* Ensinar `rmdir`
	* Remover pastas vazias
* Ensinar `rm -r` (*Ensinar com docs*)
	* Remover pastas que tem coisas dentro
* Ensinar `man` e `--help`
	* O `man` mostra como se fosse um documento
	* O `--help` mostra a ajuda também, só que em português 😉
* Ensinar `cp`
	* Esse leva dois argumentos: `cp <arquivo_para_copiar> <onde_vai_copiar>`
* Ensinar `mv`
	* Ele move arquivos
	* Ele também pode renomear arquivos
	* Ele leva dois argumentos: `mv <arquivo_que_já_existe> <onde_ele_vai_passar_a_existir>`
* Ensinar `locate`
	* Usado pra localizar um arquivo no Linux
	* O `-i` é pra ignorar o "case", ou seja, as maiúsculas e minúsculas.
	* Exemplo: se o arquivo que eu quero achar é `oi.txt`, e eu não sei onde ele está, eu posso usar `locate oi.txt` para achar ele, mas e se eu não sei se o "o" é maiúsculo, eu uso assim: `locate -i Oi.txt`, assim, sendo "Oi" ou "oi" ele vai achar do mesmo jeito.
