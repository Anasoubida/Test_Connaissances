# Test_Connaissances : Système de gestion d’emprunt dans une librairie

L'objectif est de faire des manipulations sur des dataframe en utilisant SQL et DSL sur spark. 

## Apercu sur les tables : 

On dispose des 5 tables (dataframe) suivantes : 

**book**    : représente une table de livres. Chaque ligne est un livre décrit par son identifiant, son titre et sa catégorie (roman, science-fiction, musique, etc.);


| bid|               title              |   category|
-----|----------------------------------|------------
|0001|L'existentialisme est un humanisme|Philosophie|
|0002|Huis clos. Suivi de Les Mouches   |Philosophie|
|0003|Mignonne allons voir si la rose   |Poeme      |
|0004|Les Amours                        |Poème      |

**Authors** : représente une table d'auteurs. Chaque ligne contient le nom et l'identifiant d'un auteur;

**Student** : représente une table d'étudiants. Chaque ligne est un étudiant décrit par son identifiant, son nom et son département (informatique, mécanique...);

**write**   : représente l'association entre les auteurs et les livres. Une ligne de cette table signifie que l'auteur a écrit le livre bid;

**borrow**  : représente les informations de prêt de livre. Une ligne de cette table signifie que l'étudiant a emprunté le livre bid  , à la date checkout-time et l'a retourné à la date return-time. 


