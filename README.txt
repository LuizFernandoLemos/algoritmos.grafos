Algoritmos a serem implementados:

	-Algoritmo de Kruskal; OK
	-Algoritmo de Dijkstra; OK
	-Busca em Largura;	
	-Busca em Profundidade; OK
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
		1 String nome;
		1 String cor;
		1 int distancia; (que � a soma dos pesos de um grafo ponderado em um determinado caminho)
		1 ArrayList de Arestas incidentes;
		1 ArrayList de Vertices vizinhos;
		1 Vertice pai; (vertice anterior a ele em um determinado caminho)
		1 boolean visitado; (booleano para determinar se o vertice ja foi visitado em determinado caminho)
	
	2� Aresta: Compostas por:
		1 int peso;
		2 Vertices; (origem, destino)
		1 boolean visitado; (boolean usado para controle de fluxo nas buscas de ciclo, de aresta de menor Peso ou para montar arvores para determinados caminhos)

	3� Grafo: Composta por:
		1 ArrayList de Arestas
		1 ArrayList de Vertices

___________Main___________

-Para se inserir um Grafo as ENTRADAS que devem ser dadas a partir do console sao:

	1� Peso (int);
	2� Origem (String) - Nome do primeiro vertice;
	3� Destino (String) - Nome do segundo vertice;

___Algoritmo de Kruskal___

-Busca uma arvore formada de menores custos em um grafo ponderado.
-Recebe Grafo dado pelo usuario tratando prioritariamente das arestas como principal objeto de fluxo.

-Os m�todos de tal algoritmo est�o na classe Grafo e s�o:
	1� "menorPeso" (retorna o menor peso ainda n�o verificado da �rvore dada);
	2� "temCiclo" (retorna se inserindo determinada aresta a arvore ter� um ciclo ou n�o);
	
___Algoritmo de Dijkstra___

-Busca um caminho de menor custo em um grafo ponderado entre 2 vertices do mesmo.
-Recebe Grafo dado pelo usuario tratando prioritariamente dos vertices como principal objeto de fluxo.
-A ENTRADA que deve ser dada ao se chamar tal Algoritmo a partir do console e:

	1� Origem (String) - Nome do primeiro vertice do caminho;
	2� Destino (String) - Nome do segundo vertice;

-O metodo de tal algoritmo esta na classe Grafo, sendo:
	1� "encontrarMenorCaminhoDijkstra"
	
___Busca em Profundidade___

-Busca um vertice em um determinado Grafo.
-Recebe Grafo dado pelo usuario tratando prioritariamente dos vertices como principal objeto de fluxo e sinalizando arestas passadas para que se monte a arvore da Busca em Profundidade.
-A ENTRADA que 
-A ENTRADA que deve ser dada ao se chamar tal Algoritmo a partir do console e:

	1� Origem (String) - Nome do vertice raiz do grafo;
	2� Destino (String) - Nome do vertice buscado;

-Os metodos de tal algoritmo estao na classe Grafo, sendo:
	1� "buscaEmProfundidade" (metodo que chama a busca recursiva em profundidade e retorna a arvore da busca em profundidade)
	2� "buscaRecursiva" (metodo recursivo que retorna um booleano como resposta da busca pelo vertice e seta como true os vertices e arestas que estarao na arvore de Busca em Profundidade)







