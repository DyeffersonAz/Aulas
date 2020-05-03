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

* `mkdir`
	* Esse comando serve para fazer pastas. Olha o exemplo:
		```
		$ pwd
		/home/dyefferson/Documentos/
		$ ls
		oi.txt	tchau.txt  linux.txt	cachorro.png
		$ mkdir projetos
		$ ls
		projetos/
		oi.txt	tchau.txt  linux.txt	cachorro.png
		```
* `rmdir`
	* Ele serve para remover pastas vazias. E só vazias, hein?
* `rm -r`
	* Ele serve para remover pastas que tem coisas dentro
* `man` e `--help`
	* `man`
		Ele mostra a ajuda de um documento (geralmente em inglês):
		```
		$ man ls
		<TELA CHEIA COM MANUAL>
		```
		Desculpa, mas não tem como eu mostrar aqui como vai aparecer. A única coisa que eu posso te dizer é que você vai poder rolar com o mouse e para sair digite a tecla "q".
	* `--help`
		Ele é um parâmetro que faz a mesma coisa que o man, mas tem mais chance de mostrar coisas em português 😆.
		```
		$ ls --help
		<DOCUMENTAÇÃO DO LS>
		```
		Desculpa, mas aqui é a mesma coisa do `man`, não tem como eu te dizer como vai aparecer, mas só te digo que lá tem a descrição de todos os parâmetros e argumentos que o comando pode receber. Ninguém decora aquilo lá! 😛
* `cp`
	* Esse leva dois argumentos: `cp <arquivo_para_copiar> <onde_vai_copiar>`
* `mv`
	* Ele serve para mover arquivos
	* Ele também pode renomear arquivos
	* Ele leva dois argumentos: `mv <arquivo_que_já_existe> <onde_ele_vai_passar_a_existir>`
* `locate`
	* Ele serve pra localizar um arquivo no Linux
	* O `-i` é um parâmetro pra ignorar o "case", ou seja, as maiúsculas e minúsculas.
	* Exemplo: se o arquivo que eu quero achar é `oi.txt`, e eu não sei onde ele está, eu posso usar `locate oi.txt` para achar ele, mas se eu não sei se o "o" é maiúsculo ou não eu uso assim: `locate -i Oi.txt`, assim, sendo "Oi" ou "oi" ele vai achar do mesmo jeito. Vai no terminal e pratica pra você ver a funcionalidade!
	* **Aviso:** Esse comando pode não vir instalado no seu sistema 😕. Para instalar, depende da sua distribuição. No caso em distribuições (Se você não sabe o que é isso, veja em breve num eventual *Curso de Linux*) baseadas em Debian (como o Ubuntu), se usa o comando `apt`:
		```
		$ sudo apt install locate
		```
		Este comando instala o `locate`. Vamos analisar isso depois, essa parte é um pouco mais avançada, veremos no decorrer da parte intermediária dele. Até o momento você só precisa saber que o `apt` instala programas em distribuições baseadas em Debian.😉
