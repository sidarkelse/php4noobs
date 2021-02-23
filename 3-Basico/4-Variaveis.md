# 3.4 - Variáveis

Pra começar, todos sabemos que para guardar informação as linguagens de programação utilizam variáveis certo? na maioria das linguagens você precisa especificar o tipo de variável antes de declara-lá, PHP é diferente.

No PHP existe a "tipagem dinâmica", onde você pode criar a variável sem precisar declarar seu tipo(float, string, int) e também você pode alterar o tipo de variável enquanto o programa roda, não importando o tipo anterior.
Antes de alguns exemplos, vamos determinar algumas regras para nomeação de variáveis.

- Toda variável no PHP é declarada por \$ e em seguida o nome da variável;
- O jeito correto e válido para declarar o nome de uma variável no PHP é iniciar por sublinhado também chamado de underscore ou letra, após isso, seguido de qualquer número de letras, números ou sublinhados;
- As variáveis no PHP são case-sensitive, então, $He4rt não é o mesmo que $he4rt;
- O $this é uma variável que não pode ser atribuida, você irá entender o que significa $this nos próximos módulos do curso;
- Você pode juntar duas variveis, strings ou qualquer tipo com a concatenação, que é usado o sinal ( . ) entre os elementos (exemplo abaixo).

Lembrando que para atribuirmos um valor a uma variável passamos o sinal de ( = ) e o seu valor.

```php
<?php
//Mostrando o case sensitive
$He4rt = 'Eu ';
$he4rt = 'amo ';
$he4rT = 'a He4rt ';
$HE4RT = 'Developers';
echo $He4rt . $he4rt . $he4rT . $HE4RT;
?>
```

<p align="center"><i>Arquivo encontrado em: exemplos/variaveis1.php</i></p>

```console
danielhe4rt@he4rt:~/dev/he4rt/php4noobs/3-Basico/exemplos$ php variaveis1.php
Eu amo a He4rt Developers
```

## Observações

- Como vocês podem ver, o PHP por possuir [case-sensitive](https://pt.wikipedia.org/wiki/Case-sensitive), as variáveis $He4rt,$he4rt,$he4rT e $HE4RT não são a mesma coisa;
- É preciso sempre utilizar ponto e virgula no final de cada declaração ( ; ), se porventura você esquecer, irá dar erro;
- Lembrando que é sempre bom se antenar as boas práticas, use variáveis que condizem com o código escrito, não utilize nomes como $a, $b, \$c e se torne um programador alfabético.

Como eu expliquei antes, variáveis podem mudar o valor no tempo de execução, ou seja, durante a execução do código, vamos para mais um exemplo!

```php
<?php
$idade = '18 Anos';
echo "Me chamo João e tenho " .$idade . "\n";
$idade = '19 Anos';
echo "Porém fiz aniversário e agora tenho " .$idade;
?>
```

<p align="center"><i>Arquivo encontrado em: exemplos/variaveis1.php</i></p>

```console
danielhe4rt@he4rt:~/dev/he4rt/php4noobs/3-Basico/exemplos$ php variaveis2.php
Me chamo João e tenho 18 Anos
Porém fiz aniversário e agora tenho 19 Anos
```
 <p align="center"><i>Outros tipos de váriaveis usadas </i></p>
   
   ```php
    <?php 

   #Tipos de variáveis
    //As váriaveis em php podem ter diferentes tipos de valores 
    //E a mesma váriavel pode  ter diferente tipos de valores.
    #Exemplo:
     $variavel =100;
     $variavel ="cem";

     #Também existem variáveis de tipo implícito,Que é importante saber:
    $inteiros =100; #int
    $float = 10.5; #float(com  casas decimais)
    $bool = true; #verdadeiro ou falso
    $string = "Olá mundo!"; #String(Cadeia de caracteres )
    $array = [1,2,3]; #Array - coleção de valores 
    $pessoa = new Pessoa(); #objeto com propriedade e métodos
    $nulo = null; #Váriavel com valor nulo
    ?>
    ```

