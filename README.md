# Explicação e Código

Código criado em sala de aula na aprendizagem industrial do Senai, em portugol. Com o propósito de mostrar um menu ao usuário e permitir que o próprio escolha vários produtos, mostrando o valor total da compra deste usuário e o que foi adicionado.

~~~~
programa{
	inteiro opcao
	real total
 
	funcao menu(){
		escreva("Menu do restaurante: \n")
		escreva("Digite 1 para refrigerantes (5 reais)\n")
		escreva("Digite 2 para hamburguer (20 reais)\n")
		escreva("Digite 3 para pizza (30 reais)\n")
		escreva("Digite 4 para batata frita (15 reais)\n")
		escreva("Digite 0 para sair \n")
		}
	
	funcao inicio()
	{
		
		total = 0

		enquanto(verdadeiro)
		{
			menu()
			leia(opcao)
			se(opcao == 0)
			{
				escreva("pedido encerrado\n")
				pare
				}
				
			escolha(opcao){
				caso 1: escreva("Refrigerante adicionado\n")
				total += 5
				pare
				caso 2: escreva("hamburguer adicionado\n")
				total += 20
				pare
				caso 3: escreva("pizza adicionada\n")
				total += 30
				pare
				caso 4: escreva("batata frita adicionada\n")
				total += 15
				pare
				}
			}
			escreva ("O total da sua conta é " + total)
	}
}
~~~~
