[EN](#en) | [PL](#pl) | [DE](#de) | [FR](#fr) | [ES](#es)

<a id="en"></a>
# Topological sorting of a graph

**Language:** C++20

A program implementing the DFS algorithm in order to topologically sort a given graph.

Run the program from the command line using:

`my_program path_to_graph_file`

where:

- `path_to_graph_file` – file in CSV format.

The program returns the order produced by topological sorting.

**Proposed test data set:** a graph consisting of 20 vertices. To apply topological sorting, the graph cannot contain cycles. The test data set does not contain any.

In the solution, I implemented the DFS algorithm, which searches the vertices in depth. In the `Vertex` structure, each vertex stores information about its previous parent, entry time, and exit time, so the same vertex will not be visited twice. At the beginning, a reversed adjacency list of the graph is created. It is needed to check whether a given vertex has a parent or has already become a parent itself, as well as an array indicating which vertices in the input graph no longer have any parent.

**Time complexity:** `O(V+E)`

**Space complexity:** `O(V+E)`

<a id="pl"></a>
# Sortowanie topologiczne grafu

**Język:** C++20

Program implementujący algorytm DFS w celu posortowania topologicznego zadanego grafu.

Z linii poleceń wywołujemy:

`my_program path_to_graph_file`

gdzie:

- `path_to_graph_file` – plik w formacie CSV.

Program zwraca porządek zwrócony przez sortowanie topologiczne.

**Proponowany zestaw danych testowych:** graf składający się z 20 wierzchołków. Aby zastosować sortowanie topologiczne, graf nie może posiadać cykli. Zestaw danych testowych ich nie posiada.

W rozwiązaniu zaimplementowałam algorytm DFS, który przeszukuje w głąb wierzchołki. W strukturze `Vertex` każdy wierzchołek ma zapisywaną informację o jego poprzednim rodzicu, czasie wejścia i wyjścia, przez co ten sam wierzchołek nie zostanie odwiedzony dwukrotnie. Na początku zostaje utworzona odwrócona lista sąsiedztwa grafu, która będzie nam potrzebna, by sprawdzać, czy nasz wierzchołek ma rodzica, czy już sam został rodzicem, a także tablica mówiąca, które wierzchołki w naszym grafie na wejściu już nie mają żadnego rodzica.

**Złożoność czasowa:** `O(V+E)`

**Złożoność pamięciowa:** `O(V+E)`

<a id="de"></a>
# Topologische Sortierung eines Graphen

**Sprache:** C++20

Ein Programm, das den DFS-Algorithmus implementiert, um einen gegebenen Graphen topologisch zu sortieren.

Das Programm wird über die Kommandozeile wie folgt ausgeführt:

`my_program path_to_graph_file`

wobei:

- `path_to_graph_file` – eine Datei im CSV-Format ist.

Das Programm gibt die durch die topologische Sortierung erhaltene Reihenfolge zurück.

**Vorgeschlagener Testdatensatz:** ein Graph mit 20 Knoten. Damit eine topologische Sortierung angewendet werden kann, darf der Graph keine Zyklen enthalten. Der Testdatensatz enthält keine.

In der Lösung habe ich den DFS-Algorithmus implementiert, der die Knoten in die Tiefe durchsucht. In der Struktur `Vertex` speichert jeder Knoten Informationen über seinen vorherigen Elternknoten sowie über die Eintritts- und Austrittszeit, wodurch derselbe Knoten nicht zweimal besucht wird. Zu Beginn wird eine umgekehrte Adjazenzliste des Graphen erstellt. Sie wird benötigt, um zu prüfen, ob ein Knoten einen Elternknoten hat oder bereits selbst zu einem Elternknoten geworden ist, sowie eine Tabelle, die angibt, welche Knoten im Eingabegraphen keinen Elternknoten mehr haben.

**Zeitkomplexität:** `O(V+E)`

**Speicherkomplexität:** `O(V+E)`

<a id="fr"></a>
# Tri topologique d'un graphe

**Langage :** C++20

Programme implémentant l'algorithme DFS afin d'effectuer le tri topologique d'un graphe donné.

Le programme est exécuté depuis la ligne de commande de la manière suivante :

`my_program path_to_graph_file`

où :

- `path_to_graph_file` – fichier au format CSV.

Le programme renvoie l'ordre obtenu par le tri topologique.

**Jeu de données de test proposé :** un graphe composé de 20 sommets. Pour appliquer un tri topologique, le graphe ne doit pas contenir de cycles. Le jeu de données de test n'en contient pas.

Dans la solution, j'ai implémenté l'algorithme DFS, qui parcourt les sommets en profondeur. Dans la structure `Vertex`, chaque sommet enregistre des informations sur son parent précédent ainsi que sur son temps d'entrée et de sortie, ce qui empêche qu'un même sommet soit visité deux fois. Au début, une liste d'adjacence inversée du graphe est créée. Elle est nécessaire pour vérifier si un sommet possède un parent ou s'il est déjà devenu lui-même un parent, ainsi qu'un tableau indiquant quels sommets du graphe d'entrée n'ont déjà plus aucun parent.

**Complexité temporelle :** `O(V+E)`

**Complexité spatiale :** `O(V+E)`

<a id="es"></a>
# Ordenamiento topológico de un grafo

**Lenguaje:** C++20

Programa que implementa el algoritmo DFS con el fin de ordenar topológicamente un grafo dado.

El programa se ejecuta desde la línea de comandos de la siguiente manera:

`my_program path_to_graph_file`

donde:

- `path_to_graph_file` – archivo en formato CSV.

El programa devuelve el orden obtenido mediante el ordenamiento topológico.

**Conjunto de datos de prueba propuesto:** un grafo compuesto por 20 vértices. Para aplicar el ordenamiento topológico, el grafo no puede contener ciclos. El conjunto de datos de prueba no contiene ninguno.

En la solución implementé el algoritmo DFS, que recorre los vértices en profundidad. En la estructura `Vertex`, cada vértice almacena información sobre su padre anterior, así como sobre su tiempo de entrada y salida, por lo que el mismo vértice no será visitado dos veces. Al principio se crea una lista de adyacencia invertida del grafo. Se necesita para comprobar si un vértice tiene un padre o si ya se ha convertido él mismo en padre, así como una tabla que indica qué vértices del grafo de entrada ya no tienen ningún padre.

**Complejidad temporal:** `O(V+E)`

**Complejidad espacial:** `O(V+E)`
