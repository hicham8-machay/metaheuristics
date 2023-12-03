# Genetic Algorithm for TSP

Le script résout le problème du voyageur de commerce (TSP) en utilisant un algorithme génétique pour trouver le chemin le plus court visitant toutes les villes une seule fois et retournant à la ville de départ.

## Fonctions principales

### `getCity(file_path)`
- **Entrée :** Chemin du fichier des coordonnées des villes.
- **Sortie :** Liste des villes avec leur numéro, coordonnées x et y.

### `euclideanDistance(city1, city2)`
- **Entrée :** Deux villes avec leurs coordonnées.
- **Sortie :** Distance euclidienne entre les deux villes.

### `calcDistance(cities)`
- **Entrée :** Liste des villes.
- **Sortie :** Distance totale du chemin pour visiter toutes les villes une seule fois et retourner à la ville de départ.

### `orderCrossover(parent1, parent2, point1, point2)`
- **Entrée :** Deux parents (chromosomes), et deux points de crossover.
- **Sortie :** Enfant généré en utilisant la technique de crossover par ordre.

### `cycleCrossover(parent1, parent2)`
- **Entrée :** Deux parents (chromosomes).
- **Sortie :** Enfant généré en utilisant la technique de crossover par cycle.

### `inversionMutation(chromosome)`
- **Entrée :** Chromosome à muter.
- **Sortie :** Chromosome muté en utilisant la mutation par inversion.

### `swapMutation(chromosome)`
- **Entrée :** Chromosome à muter.
- **Sortie :** Chromosome muté en utilisant la mutation par échange.

### `selectPopulation(cities, size)`
- **Entrée :** Liste des villes et la taille de la population.
- **Sortie :** Population initiale générée avec des chromosomes aléatoires, ainsi que le chromosome le plus adapté (fittest).

### `geneticAlgorithm(population, lenCities, TOURNAMENT_SELECTION_SIZE, MUTATION_RATE, CROSSOVER_RATE, max_generations)`
- **Entrée :** Population initiale, taille des villes, taille de la sélection par tournoi, taux de mutation, taux de crossover, nombre maximal de générations.
- **Sortie :** Meilleur chromosome trouvé, le nombre de générations, et le temps écoulé.

### `drawMap(cities, answer)`
- **Entrée :** Liste des villes et la meilleure solution trouvée.
- **Sortie :** Affiche la carte avec les villes et le meilleur chemin trouvé.

### `main()`
- **Fonction principale du script :**
    - Définit les paramètres.
    - Récupère les données des villes.
    - Génère la première population.
    - Applique l'algorithme génétique.
    - Affiche les résultats.

## Exécution principale
- La fonction `main()` est exécutée si le script est exécuté directement.

## Paramètres modifiables
- `POPULATION_SIZE`: Taille de la population.
- `TOURNAMENT_SELECTION_SIZE`: Taille de la sélection par tournoi.
- `MUTATION_RATE`: Taux de mutation.
- `CROSSOVER_RATE`: Taux de crossover.
- `MAX_GENERATIONS`: Nombre maximal de générations.

## Affichage des résultats
- Affiche le nombre de générations, la distance avant et après l'entraînement, et le temps écoulé.

## Visualisation
- Utilise la bibliothèque Matplotlib pour afficher la carte avec les villes et le meilleur chemin trouvé.

## Limitations
- Limite le temps d'exécution à 180 secondes (3 minutes).
- Utilise différentes techniques de crossover et de mutation avec des probabilités définies.

 ## Auteurs :

IDAHMED MINA

M'RHAR KAOUTAR

ESSAMIH HIBA
