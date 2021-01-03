# P8-Il-giro-del-mondo-in-80-giorni
Prova finale del Corso di Programmazione Python - Master in Data Science for Economics, Business and Finance

Il Main è eseguibile su Linux; per l'esecuzione su Windows è necessario installare Basemap con i comandi specifici per Windows.

Il flusso di lavoro è il seguente:

1. Calcolo grafo: si esegue grafo.ipynb.
	a. Input: il dataset iniziale worldcities.xlsx 
	b. Output: input.csv (o in alternativa input.xlsx) che contiene la lista di ciascuna città come nodo source del grafo direzionato e le 3 città target a cui ciascun nodo è   collegato;
  
2. Calcolo dello shortest path con dijkstra da zero: si esegue dijkstra.ipynb.
	a. Input: file input.xlsx 
	b. Output: file shortest_path_dijkstra.xlsx con la lista dei nodi che costituiscono lo shortest path;
  
3. Calcolo dello shortest path con dijkstra del package networkx e mappa dei due shortest path: si esegue Main.ipynb.

Input:
	1. input.xlsx
	2. shortest_path_dijkstra.xlsx 
 
Output: 
	1. la lista dei nodi dello shortest path con dijkstra di networkx (e anche lo sp con dikstra di networkx per grafi non weighted) 
	2. la lista dei nodi dello shortest path con dijkstra da zero
	3. i giorni impiegati 
	4. display su mappa dei 3 path con il package basemap.
