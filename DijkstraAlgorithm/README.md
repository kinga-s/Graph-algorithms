[EN](#en) | [PL](#pl) | [DE](#de) | [FR](#fr) | [ES](#es)

<a id="en"></a>
# Dijkstra's algorithm

**Language:** C++20

A program that searches for single-source shortest paths for directed, weighted graphs with non-negative weights.

From the command line, run:

`my_program path_to_graph_file starting_vertex ed_v_1 end_v_2`

where:

- `path_to_graph_file` is a file in CSV format,
- `starting_vertex` is the starting vertex for which Dijkstra's algorithm is run,
- `ed_v_1 end_v_2` are the distances from `starting_vertex`.

The program returns the distances and its execution time given in ms.

In the solution, the graph was implemented as a matrix. I chose this implementation because it is readable and easy, but because of this, the execution time is longer than it would be for an adjacency list. The program uses Dijkstra's algorithm to calculate the shortest path between the starting vertex and the remaining vertices. As a queue, I added a second dimension for the adjacency list. For each vertex, it stores the values 0 - if it has not been visited yet (white), 1 - if it is in the queue (gray), and 2 if it has already been removed from the queue (black). This is not the most efficient solution, but certainly one of the more pleasant, clearer, and simpler ones to implement.

**Note!** Implementing the graph as an adjacency list and then using heap sort will noticeably speed up the program.
My goal is to show different ways of solving and implementing graph algorithms, and in this particular program my goal was to show that a program implemented this way works slowly and that this is intentional. In the other selected programs, both the graph implementation as an adjacency list and heap sort were used.

**Time complexity:** `O(V^2)`

Creating the adjacency matrix takes the most time. Dijkstra's algorithm also takes `O(V^2)` here.

**Space complexity:** `O(V^2)`

Creating the adjacency matrix takes the most memory.

**Test graph file:**
`1000.csv`

<a id="pl"></a>
# Algorytm Dijkstry

**Język:** C++20

Program wyszukujący najkrótsze ścieżki z jednym źródłem dla grafów skierowanych, ważonych z nieujemnymi wagami.

Z linii poleceń wywołujemy:

`my_program path_to_graph_file starting_vertex end_v_1 end_v_2`

gdzie:

- `path_to_graph_file` plik w formacie CSV,
- `starting_vertex` wierzchołek startowy, dla którego uruchamiamy algorytm Dijkstry,
- `end_v_1 end_v_2` odległości od `starting_vertex`.

Program zwraca odległości oraz czas swojego wykonania podany w ms.

W rozwiązaniu został zaimplementowany graf w postaci macierzy. Wybrałam tę implementację, ponieważ jest czytelna i łatwa, lecz przez to czas wykonania jest większy niż byłby dla listy sąsiedztwa. Program wykorzystuje algorytm Dijkstry, by obliczyć najkrótszą ścieżkę pomiędzy wierzchołkiem startowym, a pozostałymi. Jako kolejkę dodałam tu drugi wymiar dla listy sąsiedztwa. Przechowuje ona dla każdego wierzchołka wartości 0 - jeśli nie został jeszcze odwiedzony (`white`), 1 - jeśli znajduje się w kolejce (`gray`) i 2 jeśli już został usunięty z kolejki (`black`). Nie jest to najwydajniejsze rozwiązanie, ale z pewnością jedno z przyjemniejszych, bardziej przejrzystych i prostszych do zaimplementowania.

**Uwaga!** Zaimplementowanie grafu jako listy sąsiedztwa, a następnie wykorzystanie sortowania przez kopcowanie zauważalnie przyspieszy pracę programu.
Moim celem jest pokazanie różnych sposobów rozwiązań i implementacji algorytmów grafowych, w tym konkretnym programie moim celem było pokazanie, że program tak zaimplementowany działa wolno i jest to zabieg celowy. W pozostałych wybranych programach została użyta zarówno implementacja grafu jako listy sąsiedztwa jak i sortowanie przez kopcowanie.

**Złożoność czasowa:** `O(V^2)`

Najwięcej czasu zajmuje utworzenie macierzy sąsiedztwa. Algorytm Dijkstry też zajmuje tu `O(V^2)`.

**Złożoność pamięciowa:** `O(V^2)`

Najwięcej pamięci zajmuje stworzenie macierzy sąsiedztwa.

**Plik z grafem testowym:**
`1000.csv`

<a id="de"></a>
# Dijkstra-Algorithmus

**Sprache:** C++20

Ein Programm zur Suche nach kürzesten Wegen von einer einzelnen Quelle für gerichtete, gewichtete Graphen mit nichtnegativen Gewichten.

Über die Kommandozeile wird das Programm wie folgt aufgerufen:

`my_program path_to_graph_file starting_vertex ed_v_1 end_v_2`

wobei:

- `path_to_graph_file` eine Datei im CSV-Format ist,
- `starting_vertex` der Startknoten ist, für den der Dijkstra-Algorithmus ausgeführt wird,
- `ed_v_1 end_v_2` die Entfernungen von `starting_vertex` sind.

Das Programm gibt die Entfernungen sowie seine Ausführungszeit in ms zurück.

In der Lösung wurde der Graph in Form einer Matrix implementiert. Ich habe diese Implementierung gewählt, weil sie übersichtlich und einfach ist, allerdings ist dadurch die Ausführungszeit größer als bei einer Adjazenzliste. Das Programm verwendet den Dijkstra-Algorithmus, um den kürzesten Weg zwischen dem Startknoten und den übrigen Knoten zu berechnen. Als Warteschlange habe ich hier eine zweite Dimension für die Adjazenzliste hinzugefügt. Sie speichert für jeden Knoten die Werte 0 - wenn er noch nicht besucht wurde (white), 1 - wenn er sich in der Warteschlange befindet (gray), und 2, wenn er bereits aus der Warteschlange entfernt wurde (black). Dies ist nicht die effizienteste Lösung, aber sicherlich eine der angenehmeren, übersichtlicheren und einfacher zu implementierenden.

**Hinweis!** Die Implementierung des Graphen als Adjazenzliste und die anschließende Verwendung von Heapsort würden die Arbeit des Programms merklich beschleunigen.
Mein Ziel ist es, verschiedene Arten der Lösung und Implementierung von Graphenalgorithmen zu zeigen, und in diesem konkreten Programm war mein Ziel zu zeigen, dass ein so implementiertes Programm langsam arbeitet und dass dies beabsichtigt ist. In den übrigen ausgewählten Programmen wurden sowohl die Implementierung des Graphen als Adjazenzliste als auch Heapsort verwendet.

**Zeitkomplexität:** `O(V^2)`

Das Erstellen der Adjazenzmatrix nimmt die meiste Zeit in Anspruch. Der Dijkstra-Algorithmus benötigt hier ebenfalls `O(V^2)`.

**Speicherkomplexität:** `O(V^2)`

Das Erstellen der Adjazenzmatrix benötigt den meisten Speicher.

**Testgraph-Datei:**
`1000.csv`

<a id="fr"></a>
# Algorithme de Dijkstra

**Langage :** C++20

Programme recherchant les plus courts chemins à partir d'une source unique pour des graphes orientés et pondérés avec des poids non négatifs.

Depuis la ligne de commande, on exécute :

`my_program path_to_graph_file starting_vertex ed_v_1 end_v_2`

où :

- `path_to_graph_file` est un fichier au format CSV,
- `starting_vertex` est le sommet de départ pour lequel on exécute l'algorithme de Dijkstra,
- `ed_v_1 end_v_2` sont les distances depuis `starting_vertex`.

Le programme renvoie les distances ainsi que son temps d'exécution indiqué en ms.

Dans cette solution, le graphe a été implémenté sous forme de matrice. J'ai choisi cette implémentation parce qu'elle est lisible et simple, mais cela rend le temps d'exécution plus long qu'avec une liste d'adjacence. Le programme utilise l'algorithme de Dijkstra afin de calculer le plus court chemin entre le sommet de départ et les autres sommets. Comme file, j'ai ajouté ici une deuxième dimension pour la liste d'adjacence. Elle stocke pour chaque sommet les valeurs 0 - s'il n'a pas encore été visité (white), 1 - s'il se trouve dans la file (gray), et 2 s'il a déjà été retiré de la file (black). Ce n'est pas la solution la plus efficace, mais certainement l'une des plus agréables, des plus claires et des plus simples à implémenter.

**Attention !** Implémenter le graphe sous forme de liste d'adjacence, puis utiliser le tri par tas, accélérera sensiblement le fonctionnement du programme.
Mon objectif est de montrer différentes méthodes de résolution et d'implémentation des algorithmes de graphes, et dans ce programme particulier, mon objectif était de montrer qu'un programme implémenté de cette manière fonctionne lentement et que cela est intentionnel. Dans les autres programmes sélectionnés, l'implémentation du graphe sous forme de liste d'adjacence ainsi que le tri par tas ont été utilisés.

**Complexité temporelle :** `O(V^2)`

La création de la matrice d'adjacence prend le plus de temps. L'algorithme de Dijkstra prend également `O(V^2)` ici.

**Complexité spatiale :** `O(V^2)`

La création de la matrice d'adjacence utilise le plus de mémoire.

**Fichier du graphe de test :**
`1000.csv`

<a id="es"></a>
# Algoritmo de Dijkstra

**Lenguaje:** C++20

Programa que busca los caminos más cortos desde una única fuente para grafos dirigidos y ponderados con pesos no negativos.

Desde la línea de comandos se ejecuta:

`my_program path_to_graph_file starting_vertex ed_v_1 end_v_2`

donde:

- `path_to_graph_file` es un archivo en formato CSV,
- `starting_vertex` es el vértice inicial para el que se ejecuta el algoritmo de Dijkstra,
- `ed_v_1 end_v_2` son las distancias desde `starting_vertex`.

El programa devuelve las distancias y su tiempo de ejecución indicado en ms.

En la solución se implementó el grafo en forma de matriz. Elegí esta implementación porque es clara y sencilla, pero debido a ello el tiempo de ejecución es mayor que el que tendría con una lista de adyacencia. El programa utiliza el algoritmo de Dijkstra para calcular el camino más corto entre el vértice inicial y los demás vértices. Como cola, añadí aquí una segunda dimensión para la lista de adyacencia. Esta almacena para cada vértice los valores 0 - si todavía no ha sido visitado (white), 1 - si se encuentra en la cola (gray), y 2 si ya ha sido eliminado de la cola (black). No es la solución más eficiente, pero sin duda es una de las más agradables, claras y sencillas de implementar.

**¡Atención!** Implementar el grafo como una lista de adyacencia y después utilizar ordenamiento por montículo acelerará notablemente el funcionamiento del programa.
Mi objetivo es mostrar distintas formas de resolver e implementar algoritmos de grafos, y en este programa concreto mi objetivo era mostrar que un programa implementado de esta manera funciona lentamente y que esto es intencionado. En los demás programas seleccionados se utilizó tanto la implementación del grafo como lista de adyacencia como el ordenamiento por montículo.

**Complejidad temporal:** `O(V^2)`

La creación de la matriz de adyacencia es lo que más tiempo requiere. El algoritmo de Dijkstra también requiere aquí `O(V^2)`.

**Complejidad espacial:** `O(V^2)`

La creación de la matriz de adyacencia es lo que más memoria utiliza.

**Archivo del grafo de prueba:**
`1000.csv`
