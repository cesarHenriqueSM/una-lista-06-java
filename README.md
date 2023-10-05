# César Henrique Soares Marques - RA 622120352

## UNA - Lista VI - 2023/2

### 1. Explique o que é um vetor, uma matriz e um cubo em estrutura de dados. Escreva em Java exemplos de um vetor e de uma matriz.

#### Em estrutura de dados, os conceitos de vetor, matriz e cubo são usados para organizar e armazenar dados de forma multidimensional. Aqui está uma explicação de cada um deles:

Vetor (Array):

Um vetor, também conhecido como array, é uma estrutura de dados que armazena elementos em uma única dimensão. Cada elemento do vetor é acessado por um índice único que começa em 0 e vai até o tamanho do vetor menos um.
Os vetores são usados para armazenar uma coleção de elementos do mesmo tipo de dados, como inteiros, números reais, strings, etc.
Exemplo em pseudocódigo: vetor[0] = 10; vetor[1] = 20; vetor[2] = 30;

Matriz (Array Bidimensional):

Uma matriz é uma estrutura de dados que armazena elementos em duas dimensões, ou seja, em linhas e colunas. Cada elemento da matriz é identificado por dois índices, um para a linha e outro para a coluna.
As matrizes são usadas para representar dados tabulares ou estruturados, como uma planilha de Excel.
Exemplo em pseudocódigo: matriz[1][2] = 42; matriz[0][0] = 5;

Cubo (Array Tridimensional):

Um cubo é uma extensão do conceito de matriz para três dimensões. Ele armazena elementos em uma estrutura tridimensional, composta por linhas, colunas e profundidade.
Cada elemento do cubo é identificado por três índices: um para a linha, um para a coluna e outro para a profundidade.
Os cubos são usados em situações em que os dados têm uma natureza tridimensional, como em imagens volumétricas ou séries temporais 3D.
Exemplo em pseudocódigo: cubo[2][3][1] = 100; cubo[0][1][2] = 42;

Abaixo, estão exemplos do funcionamento de um vetor e uma matriz em Java:

Vetor:
'''
package lista5;
import java.util.Scanner;

public class exercicio1 {
	
	public static void main(String[] args) {
		
		Scanner read = new Scanner(System.in);
		
			int vet[] = new int [5];
			
			for (int i = 0; i < vet.length; i++) {
				System.out.printf("Informe o %d° número: ", i+1);
					vet[i] = read.nextInt();
			}
			
			System.out.print("Impressão: ");
			
			for (int i = 0; i < vet.length; i++) {
				System.out.print(vet[i] + "\n");
			}
		
	}

}
'''

Matriz:
'''
package lista5;
import java.util.Scanner;

public class exemplo {
	
	public static void main(String[] args) {
		
		Scanner read = new Scanner(System.in);
		
			int matriz_bingo[] [] = new int [4] [4];
			
			for (int linha = 0; linha < matriz_bingo.length; linha++) {
				for (int coluna = 0; coluna < matriz_bingo.length; coluna++) {
					System.out.printf("Informe o número da %dª linha; %dª coluna: ", linha+1, coluna+1);
						matriz_bingo[linha][coluna] = read.nextInt();
				}
			}
			
			System.out.println("Matriz:");
			for (int linha = 0; linha < matriz_bingo.length; linha++) {
				System.out.print("\n");
				for (int coluna = 0; coluna < matriz_bingo.length; coluna++) {
					System.out.print(matriz_bingo[linha] [coluna] + " ");
				}
			}

	}
}
'''
