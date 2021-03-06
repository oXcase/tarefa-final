# tarefa-final
<b> Exercício final do Curso de Orientação a Objetos com Java, oferecido pelo Instituto Tecnológico da Aeronáutica em parceria com o Coursera. </b>


<b>Enunciado: </b> </br>

Jogo das Palavras Embaralhadas<br>
O objetivo desse exercício é criar um jogo onde partes de sua execução possam ser trocadas.<br>

O jogo é simples: é apresentado ao jogador uma palavra com as letras embaralhadas e o jogador deve
tentar adivinhar a palavra correta. O jogo será jogado no próprio console e a lista de palavras utilizadas
pode ser fixa (pelo menos 20).<br>

<b>PASSOS</b> <br>
A classe Scanner pode ser utilizada para ler a entrada do usuário no console.
Ela deve ser criada da seguinte forma: Scanner in = new Scanner(System.in); e
em seguida métodos como nextLine() ou nextInt() podem ser utilizados para
recuperar o que foi digitado pelo usuário.
<br>
O jogo deve possuir os seguintes componentes com as seguintes responsabilidades:<br>

• Principal: representa a classe com o método main(). É essa classe que é responsável por ler
a entrada do usuário e por imprimir as informações no console. Nenhuma outra classe pode
imprimir ou ler do console.<br>

• BancoDePalavras: classe que possui um método que retorna uma palavra retirada
aleatóriamente de uma lista de palavras lida a partir de um arquivo.<br>

• Embaralhador: interface que representa classes reponsáveis por receber uma palavra e
retornar ela embaralhada. Pelo menos duas implementações deverão ser feitas. <br>

• FabricaEmbaralhadores: possui um método que retorna um embaralhador
aleatóriamente.<br>

• MecanicaDoJogo: interface que representa o andamento e a lógica do jogo. É responsável
por ditar o andamento do jogo. Ela que vai dizer se o jogo acabou ou não, se o usuário acertou a
palavra ou não, se o usuário pode tentar acertar a palavra novamente e qual foi a pontuação final
do jogador. Pelo menos duas implementações dessa interface devem ser criadas.<br>

• FabricaMecanicaDoJogo: retorna a MecanicaDoJogo que deve ser utilizada.<br>

A classe Principal deve recuperar a instância de MecanicaDoJogo de FabricaMecanicaDoJogo e não
pode conter nenhuma referência direta a uma das implementações, apenas a interface. Da mesma
forma, as implementações de MecanicaDoJogo devem recuperar os embaralhadores de
FabricaEmbaralhadores e também não pode conter nenhuma referência direta a implementações de
Embaralhador, apenas a interface. <br>

As implementações de embaralhador devem conter algoritmos para o embaralhamento de palavras.
Exemplo: inverter string, permutar randomicamente, trocar letras impares por pares e etc...<br>

As implementações de MecanicaDoJogo devem retratar o andamento do jogo. Exemplos de questões
que podem mudar: quando o jogo termina (após um número fixo de palavras, após um número de
erros); quantas tentativas podem ser feitas por palavra; como são computados os pontos; qual
embaralhador será utilizado e em que momento; e etc... O importante é que independente do
funcionamento, a classe Principal deverá interagir com ele da mesma forma. <br>

<b>DICA</b> <br>

É você quem irá definir as interfaces! Então se houver alguma informação que
precise saber daquela a respeito da implementação, inclua um método que
retorna aquela informação. Exemplo: um embaralhador pode gerar uma mistura
mais difícil que outros, então se caso essa informação seja relevante (para
pontuação, por exemplo) crie um método na interface Embaralhador que
retorne sua dificuldade.
<br>

Deverá ser entregue:<br>

• O código criado para o jogo<br>
• O diagrama de classes com todas as classes criadas<br>
• Testes de unidade para as classes de embaralhamento<br>
• O link para um video disponibilizado de forma aberta com a gravação de uma partida do seu jogo <br>
<br>
Link do vídeo: https://www.youtube.com/watch?v=gmZGiddY_Lw

<b> IDE Eclipse </b>

