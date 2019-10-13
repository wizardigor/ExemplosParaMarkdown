##Tìtulos (<h1> a <h6>)
# Título nível 1
## Título nível 2
### Título nível 3
#### Título nível 4
##### Título nível 5
###### Título nível 6

ou

Título de nível 1
==================
  
Título de nível 2
------------------

##Parágrafos e quebras de linha (<p> e <br />)
Para gerar parágrafos, basta você escrever o texto em uma linha.
 Alguns quebram linha quando você dá enter. Mas a documentação do Markdown diz que, para quebras de linha, você precisa deixar dois espaços no final da linha:
Primeira linha do parágrafo.··
Segunda linha do parágrafo.

##Ênfase (<strong> e <em>)
Para enfatizar uma palavras (<em>), usamos um * ou _:
Javascript é _cool_!

ou:	

Javascript é *cool*!

O mais utilizado para ênfase (<em>) é o underline
Para dar forte ênfase em palavras (<strong>), você usa dois ** ou __:
**Da2k** é a pronúncia para **Daciuk**: DA-TWO-K!

ou

__Da2k__ é a pronúncia para __Daciuk__: DA-TWO-K!

O mais utilizado para forte ênfase (<strong>) são dois asteriscos **.

##Links (<a>)
Para gerar links, você usa [](). Dentro dos colchetes você coloca o texto do link, e dentro dos parênteses, você coloca a URL:
[Blog do Da2k](https://blog.da2k.com.br)

Passando um texto após a URL, separando o link do texto por um espaço em branco, esse texto será usado como title:
[Blog do Da2k](https://blog.da2k.com.br "Clique e acesse agora!")

Se o texto do seu link é o próprio link, você pode envolvê-lo entre < e >, que o link será gerado automaticamente:
<https://www.google.com.br>

E isso funciona também para e-mails:
<meu@email.com>

##Blocos de citação (<blockquote>)

Para criar blocos de citação, você usa o sinal de >:
> Esse é um bloco de citação.
> Ele pode ter várias linhas por parágrafo.
>
> Inclusive, dando um espaço, você tem um novo parágrafo.

Listas (<ul> e <ol>)

Para listas não ordenadas (<ul>), você pode usar *, + ou -. Veja:
* Item 1
* Item 2
* Item 3
  
+ Item 1
+ Item 2
+ Item 3
  
- Item 1
- Item 2
- Item 3

E para listas ordenadas, você usa o número, seguido de ponto:
1. Item 1
2. Item 2
3. Item 3

Alguns parsers renderizam automaticamente os próximos números, após o 1. Você só precisa usar * para os itens do 2 em diante:
1. Item 1
* Item 2
* Item 3

##Imagens (<img />)
Geração de imagens é bem parecido com a geração de links: você só precisa adicionar uma ! no início. E o texto que você coloca entre os colchetes, é usado como alt na imagem:
![Banana](http://cdn.osxdaily.com/wp-content/uploads/2013/07/dancing-banana.gif)

O title também funciona como no link:
![Banana](http://cdn.osxdaily.com/wp-content/uploads/2013/07/dancing-banana.gif "Olha a banana dançando!")

##Tabelas (<table>)
Já falei sobre tabelas em um post anterior. Nesse post eu falo também sobre as task lists, mas elas são específicas do Github, não funcionam com qualquer parser ;)
Código inline e bloco (<code> e <pre>)
Voc? ainda pode adicionar trechos de código via Markdown. Para adicionar código a nível inline, você usa \`:
O `<blockquote>` é uma tag HTML.

E para gerar blocos de código, você simplesmente indenta o código 4 espaços (ou 1 tab) à frente do paràgrafo:
Essa é a função sayHello():
    function sayHello() {
      return 'hi!';
    }

Isso é como está na documentação. Mas a maior parte dos parses que eu conheço não funcionam dessa forma. Eles geram blocos de código usando três crases no início da primeira e última linha, para marcar o início e o fim do bloco:
...
function sayHello(){
  return 'hi';
}
...

O Github inclusive recomenda que se use as 3 crases, pois é mais fácil de visualizar e dar manutenção no código.
No Github, você ainda consegue definir qual a linguagem que está sendo utilizada, para que seja feito code highlight no seu código. Só passe a linguagem após as 3 crases, dessa forma:
...
   js
function sayHello(){
  return 'hi';
}

##Backslash scapes
Para escapar caracteres que são parseados pelo Markdown, você pode usar a barra invertida \ (backslash), seguida do caractere, para imprimí-lo literalmente. O escape funciona para os caracteres listados abaixo:
\   backslash (barra invertida)
`   backtick (crase)
*   asterisk (asterisco)
_   underscore
{}  curly braces (chaves)
[]  square brackets (colchetes)
()  parentheses (parênteses)
#   hash mark (sustenido / hash / jogo da velha)
+   plus sign (sinal de "mais" ou somar)
-   minus sign (hyphen) (sinal de menos ou hífen)
.   dot (ponto)
!   exclamation mark (ponto de exclamação)

Além de tudo isso, é importante saber também, que é possível usar HTML junto com Markdown! Isso mesmo! Se você precisar adicionar uma classe em uma imagem para alinhar, ou colocar uma cor específica em alguma palavra, você pode usar tags HTML normalmente.

Para saber mais sobre Markdown, recomendo a leitura da documentação oficial:
http://daringfireball.net/projects/markdown/

E alguns links de como o Github usa Markdown:
https://help.github.com/articles/markdown-basics/
https://help.github.com/articles/github-flavored-markdown/
https://guides.github.com/features/mastering-markdown/
https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet