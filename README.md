# Loop-for-each-no-java

Anotações de Loop for each no java
                                                                            Loop for each

Agenda
.For each (java 5)

O for each é um for melhorado, ele é usado muito com arrays, esse for each foi adicionado no java depois d versão 5.

int[] notas = new int[10];

for (int i=0; i<notas.lenght; i++){
  System.out.println(notas[i]);
}

O array no java ele tanto pode ser um vetor como pode ser uma matriz pode ser um array multidimensional de quatro dimensões, na hora de interar array no
java nós sempre utilizamos o for, na hora de acessar aquela informação a gente passa o index o índice da posição do array onde nós queremos pegar
informação.

int[] notas = new int[10];

for (int notas : notas){
  System.out.println(nota);
}

como é esse for each que é paracada, ele é bem similar só que por exemplo você precisa saber como se você estivesse criando uma variável para receber o
valor daquela determinada posição do array então ao invés de nós termos for, int, i etc, nós temos um for each, eu vou criar uma variável para receber
aquele valor que no caso seria nota e vou esperar o array de notas e dentro desse for eu consigo acessar diretamente a variável no java ele automaticamente
vai fazer aquele incremento ele vai utilizar um contador só que é internamente nós não temos acesso.
O Random serve para usar números aleatorios.

		System.out.println("Usando o for each");
		
		for (int nota : notas) {
			System.out.println(nota);
		}
	}

}


Ex:

package com.madu.Loop.FOR.each;

import java.util.Random;

public class ForEach {

	public static void main(String[] args) {
		
		int[] notas = new int[10];
		
		Random random = new Random();
		
		for (int i=0; i<notas.length; i++) {
			
			notas[i] = random.nextInt(10);
		}
		
		for (int i=0; i<notas.length; i++) {
			int nota = notas[i];
			System.out.println(nota);
		}
		
		System.out.println("Usando o for each");
		
		for (int nota : notas) {
			System.out.println(nota);
		}
	}

}


Console:
1
0
5
1
7
7
8
3
9
4
Usando o for each
1
0
5
1
7
7
8
3
9
4

Como seria o output de uma matriz?

		//exemplo 02
		System.out.println("Exemplo com arrays multidimensionais");
		double[][] notasAlunos = new double[3][4];
		
		notasAlunos[0][0] = 10;
		notasAlunos[0][1] = 7;
		notasAlunos[0][2] = 9;
		notasAlunos[0][3] = 9.5;
		
		notasAlunos[1][0] = 9;
		notasAlunos[1][1] = 8;
		notasAlunos[1][2] = 7;
		notasAlunos[1][3] = 9;
		
		notasAlunos[2][0] = 8;
		notasAlunos[2][1] = 9;
		notasAlunos[2][2] = 10;
		notasAlunos[2][3] = 7;
		
		for (double[] notasAluno : notasAlunos) {
			for (double nota : notasAluno) {
				System.out.print(nota + " ");
			}
			System.out.println();
		}
	}

}

Console:
Exemplo com arrays multidimensionais
10.0 7.0 9.0 9.5 
9.0 8.0 7.0 9.0 
8.0 9.0 10.0 7.0 


Ex2:

package com.madu.Loop.FOR.each;

import java.util.Random;

public class ForEach {

	public static void main(String[] args) {
		
		int[] notas = new int[10];
		
		Random random = new Random();
		
		for (int i=0; i<notas.length; i++) {
			
			notas[i] = random.nextInt(10);
		}
		
		for (int i=0; i<notas.length; i++) {
			int nota = notas[i];
			System.out.println(nota);
		}
		
		System.out.println("Usando o for each");
		
		for (int nota : notas) {
			System.out.println(nota);
		}
		
		//exemplo 02
		System.out.println("Exemplo com arrays multidimensionais");
		double[][] notasAlunos = new double[3][4];
		
		notasAlunos[0][0] = 10;
		notasAlunos[0][1] = 7;
		notasAlunos[0][2] = 9;
		notasAlunos[0][3] = 9.5;
		
		notasAlunos[1][0] = 9;
		notasAlunos[1][1] = 8;
		notasAlunos[1][2] = 7;
		notasAlunos[1][3] = 9;
		
		notasAlunos[2][0] = 8;
		notasAlunos[2][1] = 9;
		notasAlunos[2][2] = 10;
		notasAlunos[2][3] = 7;
		
		for (double[] notasAluno : notasAlunos) {
			for (double nota : notasAluno) {
				System.out.print(nota + " ");
			}
			System.out.println();
		}
	}

}


Console:
0
8
1
8
4
4
1
2
7
1
Usando o for each
0
8
1
8
4
4
1
2
7
1
Exemplo com arrays multidimensionais
10.0 7.0 9.0 9.5 
9.0 8.0 7.0 9.0 
8.0 9.0 10.0 7.0 
