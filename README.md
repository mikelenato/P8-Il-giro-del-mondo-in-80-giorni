# P8-Il-giro-del-mondo-in-80-giorni
Prova finale del Corso di Programmazione Python - Master in Data Science for Economics, Business and Finance

Il Main è eseguibile su Linux; per l'esecuzione su Windows è necessario installare Basemap con i comandi specifici per Windows.

Il flusso di lavoro è il seguente:

1. Calcolo grafo: si esegue grafo.ipynb; 
	a. input: il dataset iniziale worldcities.xlsx 
	b. output: input.csv (o in alternativa input.xlsx) che contiene la lista di ciascuna città come nodo source del grafo direzionato e le 3 città target a cui ciascun nodo è   collegato;
  
2. Calcolo dello shortest path con dijkstra da zero: si esegue dijkstra.ipynb 
	a. input: file input.xlsx 
	b. output: file shortest_path_dijkstra.xlsx con la lista dei nodi che costituiscono lo shortest path;
  
3. Calcolo dello shortest path con dijkstra del package networkx e mappa dei due shortest path: si esegue Main.ipynb:
a. input:
	a1. input.xlsx
	a2. shortest_path_dijkstra.xlsx 
 
b. output: 
	b1. la lista dei nodi dello shortest path con dijkstra di networkx (e anche lo sp con dikstra di networkx per grafi non weighted) 
	b2. la lista dei nodi dello shortest path con dijkstra da zero
	b3. i giorni impiegati 
	b4. display su mappa dei 3 path con il package basemap.
