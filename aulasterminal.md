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

## Aula 2

* `ls`
	* Ele mostra a lista de coisas que existem onde você está, por exemplo:
		```
		$ pwd
		/home/dyefferson/Documentos/
		$ ls
		oi.txt         tchau.txt       cachorro.png
		```
* Parâmetros e Argumentos
	Eles são diferentes, aqui vai a definição de cada um. Por elas você já vai entendendo a diferença.
	* Argumento
		É aquilo que você dá de informação ao comando. Olha o exemplo:
		```
		$ <COMANDO> <ARGUMENTO>
		```
		Mas assim não dá pra entender, né? Olha lá com um comando de verdade:
		```
		$ pwd
		/home/dyefferson/
		$ cd Documentos/
		```
		Neste caso, `cd` é o comando e `Documentos/` é o argumento. Um comando pode ter vários argumentos, esses a gente vai ver ao decorrer do curso. 😅
	* Parâmetro
		São aqueles *argumentos* que dão as configurações do comando. Eles são muitas vezes definidos com um sinal de menos (`-`). Ficou confuso? Olha aqui:
		```
		$ pwd
		/home/dyefferson/Documentos/
		$ ls -a
		.	..	oi.txt	tchau.txt	cachorro.png
		```
		Viu? O `ls` é um comando em que a gente deu um parâmetro `-a`, que serve pra configurar o `ls` pra te mostrar os arquivos escondidos. Para saber mais sobre isso, fique no aguardo para um *Curso de Linux*.

* `touch`
	* Esse comando serve pra criar um arquivo, olha aí:
		```
		$ pwd
		/home/dyefferson/Documentos/
		$ ls
		oi.txt	tchau.txt	cachorro.png
		$ touch linux.txt
		$ ls
		oi.txt	tchau.txt  linux.txt	cachorro.png
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
