# TABULEIRO-DAMA-MATRIZ-CHAR-COD-JAVA


Escreva um programa que monte o estado inicial de um tabuleiro de damas em uma matriz de char, como mostrado abaixo:

B

 

B

 

B

 

B

 

 

B

 

B

 

B

 

B

B

 

B

 

B

 

B

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

 

P

 

P

 

P

 

P

P

 

P

 

P

 

P

 

 

P

 

P

 

P

 

P

Complete o programa Java abaixo, arrastando e soltando os trechos de código nos espaços em branco, de forma que o problema acima seja corretamente implementado.
public class TabuleiroDamas {
	public static void main(String[] args) {
		[char[][] tabuleiro = new char[8][8];]
		
		for(int lin = 0; lin < tabuleiro.length; lin++) {
			for(int col = 0; col < tabuleiro[lin].length; col++) {
				if(col % 2 == lin % 2 && lin < 3) 
					[tabuleiro[lin][col] = 'B';]
				else if(col % 2 == lin % 2 && lin > 4)
					[tabuleiro[lin][col] = 'P';]
				else
					[tabuleiro[lin][col] = ' ';]
			}
		}
		
		for(int lin = 0; lin < tabuleiro.length; lin++) {
			[for(int col = 0; col < tabuleiro[lin].length; col++)] {
				[System.out.printf("%c ", tabuleiro[lin][col]);]
			}
			[System.out.println();]
		}
	}
}
