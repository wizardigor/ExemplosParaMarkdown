##T�tulos (<h1> a <h6>)
# T�tulo n�vel 1
## T�tulo n�vel 2
### T�tulo n�vel 3
#### T�tulo n�vel 4
##### T�tulo n�vel 5
###### T�tulo n�vel 6

ou

T�tulo de n�vel 1
==================
  
T�tulo de n�vel 2
------------------

##Par�grafos e quebras de linha (<p> e <br />)
Para gerar par�grafos, basta voc� escrever o texto em uma linha.
 Alguns quebram linha quando voc� d� enter. Mas a documenta��o do Markdown diz que, para quebras de linha, voc� precisa deixar dois espa�os no final da linha:
Primeira linha do par�grafo.��
Segunda linha do par�grafo.

##�nfase (<strong> e <em>)
Para enfatizar uma palavras (<em>), usamos um * ou _:
Javascript � _cool_!

ou:	

Javascript � *cool*!

O mais utilizado para �nfase (<em>) � o underline
Para dar forte �nfase em palavras (<strong>), voc� usa dois ** ou __:
**Da2k** � a pron�ncia para **Daciuk**: DA-TWO-K!

ou

__Da2k__ � a pron�ncia para __Daciuk__: DA-TWO-K!

O mais utilizado para forte �nfase (<strong>) s�o dois asteriscos **.

##Links (<a>)
Para gerar links, voc� usa [](). Dentro dos colchetes voc� coloca o texto do link, e dentro dos par�nteses, voc� coloca a URL:
[Blog do Da2k](https://blog.da2k.com.br)

Passando um texto ap�s a URL, separando o link do texto por um espa�o em branco, esse texto ser� usado como title:
[Blog do Da2k](https://blog.da2k.com.br "Clique e acesse agora!")

Se o texto do seu link � o pr�prio link, voc� pode envolv�-lo entre < e >, que o link ser� gerado automaticamente:
<https://www.google.com.br>

E isso funciona tamb�m para e-mails:
<meu@email.com>

##Blocos de cita��o (<blockquote>)

Para criar blocos de cita��o, voc� usa o sinal de >:
> Esse � um bloco de cita��o.
> Ele pode ter v�rias linhas por par�grafo.
>
> Inclusive, dando um espa�o, voc� tem um novo par�grafo.

Listas (<ul> e <ol>)

Para listas n�o ordenadas (<ul>), voc� pode usar *, + ou -. Veja:
* Item 1
* Item 2
* Item 3
  
+ Item 1
+ Item 2
+ Item 3
  
- Item 1
- Item 2
- Item 3

E para listas ordenadas, voc� usa o n�mero, seguido de ponto:
1. Item 1
2. Item 2
3. Item 3

Alguns parsers renderizam automaticamente os pr�ximos n�meros, ap�s o 1. Voc� s� precisa usar * para os itens do 2 em diante:
1. Item 1
* Item 2
* Item 3

##Imagens (<img />)
Gera��o de imagens � bem parecido com a gera��o de links: voc� s� precisa adicionar uma ! no in�cio. E o texto que voc� coloca entre os colchetes, � usado como alt na imagem:
![Banana](http://cdn.osxdaily.com/wp-content/uploads/2013/07/dancing-banana.gif)

O title tamb�m funciona como no link:
![Banana](http://cdn.osxdaily.com/wp-content/uploads/2013/07/dancing-banana.gif "Olha a banana dan�ando!")

##Tabelas (<table>)
J� falei sobre tabelas em um post anterior. Nesse post eu falo tamb�m sobre as task lists, mas elas s�o espec�ficas do Github, n�o funcionam com qualquer parser ;)
C�digo inline e bloco (<code> e <pre>)
Voc? ainda pode adicionar trechos de c�digo via Markdown. Para adicionar c�digo a n�vel inline, voc� usa \`:
O `<blockquote>` � uma tag HTML.

E para gerar blocos de c�digo, voc� simplesmente indenta o c�digo 4 espa�os (ou 1 tab) � frente do par�grafo:
Essa � a fun��o sayHello():
    function sayHello() {
      return 'hi!';
    }

Isso � como est� na documenta��o. Mas a maior parte dos parses que eu conhe�o n�o funcionam dessa forma. Eles geram blocos de c�digo usando tr�s crases no in�cio da primeira e �ltima linha, para marcar o in�cio e o fim do bloco:
...
function sayHello(){
  return 'hi';
}
...

O Github inclusive recomenda que se use as 3 crases, pois � mais f�cil de visualizar e dar manuten��o no c�digo.
No Github, voc� ainda consegue definir qual a linguagem que est� sendo utilizada, para que seja feito code highlight no seu c�digo. S� passe a linguagem ap�s as 3 crases, dessa forma:
...
   js
function sayHello(){
  return 'hi';
}

##Backslash scapes
Para escapar caracteres que s�o parseados pelo Markdown, voc� pode usar a barra invertida \ (backslash), seguida do caractere, para imprim�-lo literalmente. O escape funciona para os caracteres listados abaixo:
\   backslash (barra invertida)
`   backtick (crase)
*   asterisk (asterisco)
_   underscore
{}  curly braces (chaves)
[]  square brackets (colchetes)
()  parentheses (par�nteses)
#   hash mark (sustenido / hash / jogo da velha)
+   plus sign (sinal de "mais" ou somar)
-   minus sign (hyphen) (sinal de menos ou h�fen)
.   dot (ponto)
!   exclamation mark (ponto de exclama��o)

Al�m de tudo isso, � importante saber tamb�m, que � poss�vel usar HTML junto com Markdown! Isso mesmo! Se voc� precisar adicionar uma classe em uma imagem para alinhar, ou colocar uma cor espec�fica em alguma palavra, voc� pode usar tags HTML normalmente.

Para saber mais sobre Markdown, recomendo a leitura da documenta��o oficial:
http://daringfireball.net/projects/markdown/

E alguns links de como o Github usa Markdown:
https://help.github.com/articles/markdown-basics/
https://help.github.com/articles/github-flavored-markdown/
https://guides.github.com/features/mastering-markdown/
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet