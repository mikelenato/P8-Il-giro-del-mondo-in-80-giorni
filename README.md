# P8-Il-giro-del-mondo-in-80-giorni
Prova finale del Corso di Programmazione Python - Master in Data Science for Economics, Business and Finance

Il Main è eseguibile su Linux; per l'esecuzione su Windows è necessario installare Basemap con i comandi specifici per Windows.

Il flusso di lavoro è il seguente:
1. Calcolo grafo: si esegue grafo.ipynb che prende come input il dataset iniziale worldcities.xlsx e restituisce in output il dataset input.csv (o in alternativa input.xlsx) con la lista di ciascuna città come npdo source del grafo direzionato e le 3 città target a cui ciascun nodo è collegato;
2. Calcolo dello shortest path con dijkstra da zero: si esegue dijkstra.ipynb che prende il file input.xlsx in input e restituisce la lista dei nodi che costituiscono lo shortest path;
3. Calcolo dello shortest path con dijkstra del package networkx e mappa dei due shortest path: si esegue Main.ipynb che prende il file input.xlsx in input e restituisce la lista dei nodi dello shortest path con dijkstra di networkx (e anche lo sp con dikstra di networkx per grafi non weighted) e il display su mappa con il package basemap.
