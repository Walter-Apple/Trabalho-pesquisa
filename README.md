# Trabalho-pesquisa

(link bem ultil)
https://profsalu.wordpress.com/wp-content/uploads/2018/08/3-unity-3d-programac3a7c3a3o01.pdf
pag 6 a 9

<h1>Mathf:</h1>

<h2>Approximately</h2>
<h3> Esta função faz uma comparação de um valor e com algum outro valor, ou resultado de algum cálculo.
E nos retorna um resultado boleano se os valores são aproximados ou não, podendo ser usado até em um if.
Por exemplo, temos o valor 7, e queremos comparar se o 7 é similar ao resultado do cálculo, 15 dividido por 2.
Neste caso, esse Mathf retornaria false, pois, 15 dividido por 2 é 7.5, então você realizaria alguma ação a partir daqui.
Mas se o valor a ser comparado fosse 7.5, ai sim teríamos um retorno de verdadeiro para essa comparação. </h3>

<h2>Max</h2>
<h3>Esta função pede dois valores para comparação, e retornara para nós o maior valor entre os comparados.
Por exemplo, se os valores forem 5 e 8, ele retornará para nós o valor 8 que é o maior entre os comparados.
E pode ser muito útil em mecânicas de Danos por combos, passando valores aleatórios e nos retornando o maior deles.</h3>

<h2>Min</h2>
<h3>Esta função funciona igualmente ao Max, porém, por sua vez nos retornará o valor mínimo da comparação.
Tanto o Max quanto o Min, podem ser muito úteis em diversas mecânicas, aliados a números Randômicos.
Pode trazer uma variabilidade ainda maior em resultados para danos, combos, ataques críticos, etc.</h3>

<h2>Abs</h2>
<h2>Esta função nos retorna um valor absoluto de um determinado cálculo, e sem dúvidas é bastante útil.
Pois, caso o valor seja negativo ele sempre retornará para nós positivo, ou seja, se for -2.4 ele retornará 2.4 positivo.
E pode ser aplicada de diversas formas, por exemplo, para saber se o player está se movendo.
Porque bastaria colocar o Input que varia de 1 e -1, nesse Mathf e ele retornaria 0 parado e 1, se movendo.</h2>

<h2>Clamp</h2>
<h3>Esta função é usada para limitar algum cálculo entre valores específicos que você determinar.
Caso você precisa que determinado resultado não saia de -4 e 4, ou 5 e 25, por exemplo, você pode usar o Clamp.
E um uso comum, seria em jogos que precise limitar a movimentação do player dentro de uma área.</h3>

<h2>Sign</h2>
<h3>Esta função nos retorna 1 caso o valor seja maior ou igual a 0, e -1 caso o valor seja menor que 0.
Podendo ser muito útil para descobrir se os valores retornados em algum cálculo, estão positivos ou negativos.</h3>

<h2>DeltaAngle</h2>
<h3>Esta função nos retorna o menor angulo existente entre 2 ângulos que você queira calcular.
Este comando pode ser usado para calcular a trajetória de bullets, ou objetos arremessáveis em seu jogo.</h3>

<h2>Floor</h2>
<h3>Esta função retorna o menor igual valor inteiro do resultado, ou seja, fazendo o arredondamento do valor.
Porém, existe um detalhe, perceba que ele arredonda para o inteiro menor mais próximo do valor.
Por exemplo, se o resultado for 37.97, ele não arredonda para 38 e sim para 37, por ser o inteiro menor do resultado.
Mas caso seja -37.97, ele arredondaria para -38, que é o inteiro menor mais próximo do valor -37.97.</h3>

<h2>Round</h2>
<h3>Já o Round faz arredondamentos mais comuns, onde valores quebrados maiores ou iguais a 5, são arredondados para cima.
Por exemplo, 3.5, 3.64, 3.76, 3.97, etc, seriam todos arredondados para o inteiro acima, 4 no caso.
E para resultados quebrados menores que 5, são todos arredondados para o inteiro menor.
Por exemplo, 3.49, 3.32, 3.27, 3.1, etc, seriam todos arredondados para o inteiro 3.</h3>

<h2>Lerp</h2>
<h3>Esta função faz uma intercalação entre 2 valores suavemente, sendo muito utilizado em movimentações de objetos.
Pois, você passa 3 parâmetros, o valor inicial, um valor final e um valor de tempo, para que seja realizado a intercalação.
E o cálculo irá aproximar suavemente o valor inicial até chegar no valor final ou muito próximo a ele.
E na movimentação ele faz o objeto acelerar suavemente, até atingir uma velocidade constante, e desacelerar no final.</h3>

(opções extras de Mathf)

<h2>Pow</h2>
<h3>Esta função faz o cálculo de um número elevado a um expoente nos retornando o resultado.
Então você passa no parâmetro dois valores, o primeiro é o número que você deseja calcular e o segundo o expoente.
Ou seja, se usarmos Mathf.Pow (2,3), teríamos o resultado de 8, pois 2X2 = 4, 4X2 = 8.</h3>

<h2>Sqrt</h2>
<h3>Esta função nos retorna a raiz quadrada de qualquer valor que precisarmos, facilitando demais nossa vida.
E até mesmo números que não possuem raiz quadrada exata, ele nos retorna o número quebrado aproximado.</h3>

<h2>PingPong</h2>
<h3>Esta função não tem esse nome atoa, pois, seu resultado é exatamente a um Ping Pong de fato.
Pois, nele passamos um parâmetro de tempo ou um valor corrente que esteja aumentando, ou diminuindo.
Por exemplo, o próprio Time.time, que é o valor de tempo de jogo, e no segundo parâmetro o valor máximo.
E este valor máximo não pode ser menor que 0, pois, ele vai partir de 0 para o valor definido.
E ao ser executado ele subirá o valor até próximo ao valor máximo e retornará para próximo de zero.
Seguindo esse loop, e quando aplicado na movimentação o objeto sofre um efeito de ir e voltar, de um ponto a outro.</h3>

<h1>Física:</h1>

https://docs.unity3d.com/Packages/com.unity.physics@0.51/manual/collision_queries.html
(Link Ultil)

<h2>Mass</h2>
<h3>A Unity trabalha com a medida de peso em quilogramas, e podemos manipular a massa através da opção Mass.
  E assim ele literalmente aumenta ou diminui seu peso, mudando totalmente a força necessária para movê-lo.</h3>

<h2>Linear Drag ou Angular e Gravity Scale</h2>
<h3>E já através do Angular e Linear Drag, podemos manipular a resistência do ar no objeto, por assim dizer.
Podendo assim cair mais rápido ou devagar ao chão, e exercendo um efeito parecido ao do Gravity Scale.
Mas nesse caso, ao manipular o Gravity Scale, estaremos literalmente ajustando a gravidade exercida no objeto.</h3>

<h2>Body Type</h2>
<h3>Esta opção, é referente ao tipo de corpo e nos permite alternar entre Dynamic, Kinematic e Static.
E por padrão já vem como Dynamic, pois, será um tipo de corpo dinâmico e suscetível a manipulação.
Mas em Kinematic, a manipulação de física ocorre através de scripts, e estes objetos só processão colisão com objetos Dynamic.
E por fim em Static, nenhuma colisão é aplicada a eles, amplamente usado em chãos e paredes.</h3>

