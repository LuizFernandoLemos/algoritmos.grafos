Algoritmos a serem implementados:

	-Algoritmo de Kruskal; OK
	-Algoritmo de Dijkstra;
	-Busca em Largura;
	-Busca em Profundidade;
	-Ordena��o topologica;
	-Fecho transitivo;
	-Algoritmo de Warshall;

Produto: Implementa��o e relat�rio.

Data de entrega: 11/02/2014

__________________________________________________________
Relat�rio

O projeto foi feito em java e a intera��o � em console, consta de 3 pacotes:

	1 com os algoritmos pedidos;
	1 com as estruturas necess�rias;
	1 com a classe de entrada e sa�da de dados para Java;

As estruturas encontradas no projeto s�o:

	1� Vertice: Composto por:
		1 nome;
		1 ArrayList de Arestas incidentes;
	
	2� Aresta: Compostas por:
		1 peso;
		2 vertices;
		2 vari�veis verificadoras;

	3� Grafo: Composta por uma ArrayList de Arestas.


___Algoritmo de Kruskal___

Recebe �rvores dadas pelo usu�rio da forma:

	1� Peso (int);
	2� Origem (String) - Nome do primeiro vertice;
	3� Destino (String) - Nome do segundo vertice;

Os m�todos que tal algoritmo mais utiliza da classe Grafo s�o:
	1� "menorPeso" (retorna o menor peso ainda n�o verificado da �rvore dada);
	2� "temCiclo" (retorna se inserindo determinada aresta a arvore ter� um ciclo ou n�o);
	
___Algoritmo de Dijkstra___

