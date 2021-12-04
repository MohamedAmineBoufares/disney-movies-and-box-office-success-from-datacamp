
## 1. Le Dataset

Tout d'abord, nous examinerons les données Disney compilées par [Kelly Garrett](https://data.world/kgarrett/disney-character-success-00-16).

Les données contiennent **579 films** Disney avec six caractéristiques : 

* Movie title.
* Release date.
* Genre.
* MPAA rating.
* Total gross.
* Inflation-adjusted gross.

## 2. Top ten movies at the box office

Commençons par explorer les données.

Nous vérifierons quels sont les **10 films Disney** qui ont **le plus gagné au box-office**.

## 3. Movie genre trend

Parmi les 10 meilleurs films ci-dessus, il semble que certains genres soient plus populaires que d'autres. Nous allons donc vérifier quels genres gagnent en popularité.

**Nous allons faire une intrigue à partir de ces moyens de groupes pour mieux voir comment les revenus du box-office ont changé au fil du temps.**

## 4. Data transformation

L'intrigue de la ligne soutient notre conviction que certains genres gagnent en popularité plus rapidement que d'autres. Pour les films Disney, **les genres Action et Aventure connaissent la croissance la plus rapide**. 

Ensuite, nous construirons un modèle de régression linéaire pour comprendre la relation entre le genre et le brut du box-office.

Étant donné que la régression linéaire nécessite des variables numériques et que la variable de genre est une variable catégorielle, nous utiliserons une technique appelée encodage à chaud pour convertir les variables catégorielles en variables numériques. Cette technique transforme chaque valeur de catégorie en une nouvelle colonne et attribue un 1 ou un 0 à la colonne.

## 5. The genre effect

Maintenant que nous avons des variables muettes, nous pouvons construire un modèle de régression linéaire pour **prédire le adjusted gross** à l'aide de ces variables muettes.