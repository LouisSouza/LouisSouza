Algoritmo "Calculon"

Var
// Seção de Declarações das variáveis 

n1, n2, total: real
op, enter, i: inteiro

Inicio
// Seção de Comandos, procedimento, funções, operadores, etc... 

Escreval("Calculon")
escreval(" __________ ")
escreval("| ________ |")
escreval("||12345678||")
escreval("|----------|")
escreval("|[M|#|C][-]|")
escreval("|[7|8|9][+]|")
escreval("|[4|5|6][x]|")
escreval("|[1|2|3][%]|")
escreval("|[.|O|:][=]|")
escreval("*----------*")
escreval("Aperte Enter Para Calcular")
leia(enter)
limpatela

//incio da operação
escreval(" Escolha uma opção:")
escreval
escreval(" 1 - Somar")
escreval(" 2 - Subtrair")
escreval(" 3 - Multiplicar")
escreval(" 4 - Dividir")
escreval(" 5 - Potencia")
escreval(" 6 - Porcentagem")
leia(op)
limpatela

//potencia
se op = 5 entao
escreval("Digite o número base")
leia(n1)
limpatela
escreval("Digite o expoente")
leia(i)
  total <- n1^i


//porcentagem
senao
se op = 6 entao
escreval("Digite o numero para a porcentagem")
leia(n1)
limpatela
escreval("Digite a Porcentagem")
leia(n2)
limpatela
  total <- n1*n2/100
escreval("Valor menos a Porcentagem: ", n1-total)

//Soma, Subtração, Multiplicação e Divisão
senao
escreval("Digite o Primeiro Número")
leia(n1)
limpatela
escreval("Digite um outro número")
leia(n2)
limpatela

 Se op = 1 entao
    total <- n1 + n2
 Senao
    Se op = 2 entao
       total <- n1 - n2
    Senao
       Se op = 3 entao
          total <- n1 * n2
       Senao
          Se op = 4 entao
           Se n2 = 0 entao
              escreva(" Não é possivel dividir por zero")
           Senao
              total <- n1 / n2
           fimse
          fimse
        fimse
     fimse
 fimse
fimse
fimse
escreval
Se (op <> 4) ou (n2 <> 0) entao
   escreva("O resuladao da Operação é: ", total)
fimse


Fimalgoritmo
