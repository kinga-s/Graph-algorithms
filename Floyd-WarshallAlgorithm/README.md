[EN](#en) | [PL](#pl) | [DE](#de) | [FR](#fr) | [ES](#es)

<a id="en"></a>
# Floyd-Warshall algorithm

**Language:** C++20

Run the program from the command line using:

`my_program path_to_graph_file 'starting_vertex,ending_vertex' 'starting_vertex,ending_vertex'`

where:

- `path_to_graph_file` – file in CSV format,
- `'starting_vertex,ending_vertex'` – vertices for which the shortest path is searched.

The program finds the shortest paths between all vertices in a directed weighted graph using the Floyd-Warshall algorithm. Negative weights are allowed, but it is assumed that there are no negative-weight cycles. The program additionally prints information about a negative cycle (whether one exists and prints that cycle). A negative cycle exists when the value of some vertex to itself is less than 0. The program also prints the predecessor matrix (if there is no predecessor, the value is `-1`).

**Time complexity:** `O(V^3)`

The program is dominated by the Floyd-Warshall algorithm.

**Space complexity:** `O(V^2)`

The distance matrix and the predecessor matrix use the most memory.

**Test graph file:**  
`100.csv`

<a id="pl"></a>
# Algorytm Floyda-Warshalla

**Język:** C++20

Z linii poleceń wywołujemy:

`my_program path_to_graph_file 'starting_vertex,ending_vertex' 'starting_vertex,ending_vertex'`

gdzie:

- `path_to_graph_file` – plik w formacie CSV,
- `'starting_vertex,ending_vertex'` – wierzchołki, dla których poszukujemy najkrótszej ścieżki.

Program odnajduje najkrótsze ścieżki między wszystkimi wierzchołkami w skierowanym grafie ważonym dzięki algorytmowi Floyda-Warshalla. Dopuszczalne są wagi ujemne, ale zakłada się brak cyklów z ujemną wagą. Program dodatkowo wypisuje informacje o cyklu ujemnym (czy jest i wypisuje ten cykl). Cykl ujemny jest, gdy wartość jakiegoś wierzchołka do siebie samego jest mniejsza od 0. Program również wypisuje macierz poprzedników (jeśli nie ma poprzedników, to wartość `-1`).

**Złożoność czasowa:** `O(V^3)`

Program jest zdominowany przez algorytm Floyda-Warshalla.

**Złożoność pamięciowa:** `O(V^2)`

Najwięcej pamięci zajmuje macierz odległości i macierz poprzedników.

**Plik testowy z grafem:**  
`100.csv`

<a id="de"></a>
# Floyd-Warshall-Algorithmus

**Sprache:** C++20

Das Programm wird über die Kommandozeile wie folgt ausgeführt:

`my_program path_to_graph_file 'starting_vertex,ending_vertex' 'starting_vertex,ending_vertex'`

wobei:

- `path_to_graph_file` – eine Datei im CSV-Format ist,
- `'starting_vertex,ending_vertex'` – die Knoten sind, für die der kürzeste Weg gesucht wird.

Das Programm findet mithilfe des Floyd-Warshall-Algorithmus die kürzesten Wege zwischen allen Knoten in einem gerichteten gewichteten Graphen. Negative Gewichte sind zulässig, es wird jedoch davon ausgegangen, dass keine Zyklen mit negativem Gewicht vorhanden sind. Das Programm gibt zusätzlich Informationen über einen negativen Zyklus aus (ob einer vorhanden ist, und gibt diesen Zyklus aus). Ein negativer Zyklus liegt vor, wenn der Wert eines Knotens zu sich selbst kleiner als 0 ist. Das Programm gibt außerdem die Vorgängermatrix aus (wenn kein Vorgänger vorhanden ist, lautet der Wert `-1`).

**Zeitkomplexität:** `O(V^3)`

Das Programm wird vom Floyd-Warshall-Algorithmus dominiert.

**Speicherkomplexität:** `O(V^2)`

Die Distanzmatrix und die Vorgängermatrix benötigen den meisten Speicher.

**Testgraph-Datei:**  
`100.csv`

<a id="fr"></a>
# Algorithme de Floyd-Warshall

**Langage :** C++20

Le programme est exécuté depuis la ligne de commande de la manière suivante :

`my_program path_to_graph_file 'starting_vertex,ending_vertex' 'starting_vertex,ending_vertex'`

où :

- `path_to_graph_file` – fichier au format CSV,
- `'starting_vertex,ending_vertex'` – sommets pour lesquels on recherche le plus court chemin.

Le programme trouve les plus courts chemins entre tous les sommets d'un graphe orienté pondéré grâce à l'algorithme de Floyd-Warshall. Les poids négatifs sont autorisés, mais on suppose qu'il n'existe pas de cycles de poids négatif. Le programme affiche également des informations sur un cycle négatif (s'il existe et affiche ce cycle). Un cycle négatif existe lorsque la valeur d'un sommet vers lui-même est inférieure à 0. Le programme affiche également la matrice des prédécesseurs (s'il n'y a pas de prédécesseur, la valeur est `-1`).

**Complexité temporelle :** `O(V^3)`

Le programme est dominé par l'algorithme de Floyd-Warshall.

**Complexité spatiale :** `O(V^2)`

La matrice des distances et la matrice des prédécesseurs utilisent le plus de mémoire.

**Fichier du graphe de test :**  
`100.csv`

<a id="es"></a>
# Algoritmo de Floyd-Warshall

**Lenguaje:** C++20

El programa se ejecuta desde la línea de comandos de la siguiente manera:

`my_program path_to_graph_file 'starting_vertex,ending_vertex' 'starting_vertex,ending_vertex'`

donde:

- `path_to_graph_file` – archivo en formato CSV,
- `'starting_vertex,ending_vertex'` – vértices para los que se busca el camino más corto.

El programa encuentra los caminos más cortos entre todos los vértices de un grafo dirigido y ponderado mediante el algoritmo de Floyd-Warshall. Se permiten pesos negativos, pero se supone que no existen ciclos de peso negativo. El programa también muestra información sobre un ciclo negativo (si existe y muestra dicho ciclo). Existe un ciclo negativo cuando el valor de algún vértice hacia sí mismo es menor que 0. El programa también muestra la matriz de predecesores (si no hay predecesor, el valor es `-1`).

**Complejidad temporal:** `O(V^3)`

El programa está dominado por el algoritmo de Floyd-Warshall.

**Complejidad espacial:** `O(V^2)`

La matriz de distancias y la matriz de predecesores utilizan la mayor parte de la memoria.

**Archivo del grafo de prueba:**  
`100.csv`
