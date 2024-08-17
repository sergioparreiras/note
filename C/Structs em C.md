
Em C, as Structs são como classes que contem apenas atributos, os métodos ainda sao feitos separados.

Exemplo:

	struct ficha_aluno{
		int id;	
		float nota;
		char nome[40];
	};
	
armazendo na "Classe de atributos" (que no caso é uma struct) ficha_aluno:

//Declarando a varrável aluno
strutct ficha_aluno aluno;

//armazena o nome do aluno
fgets(aluno.nome, 40, stdin);
