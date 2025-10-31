# Analyse et Modélisation des Sentiments des Tweets sur les Produits Apple et Google

## Description du projet
Ce projet vise à analyser les sentiments exprimés sur **Twitter** à propos des produits **Apple** et **Google**, en utilisant des techniques de **traitement automatique du langage naturel (NLP)** et de **machine learning**.  
L’objectif est de fournir des insights exploitables pour comprendre la perception du public et orienter les stratégies de **marketing**, de **développement produit** et de **gestion de marque**.

---

## Objectifs

- Analyser les tweets concernant Apple et Google afin de déterminer la polarité (positive, négative, neutre).  
- Identifier les tendances, les mots-clés dominants et la répartition des émotions.  
- Développer et comparer plusieurs modèles de classification pour la prédiction du sentiment.  
- Fournir des recommandations basées sur les résultats analytiques.

---

##  Méthodologie

1. **Collecte et exploration des données**
   - Nettoyage des tweets (suppression des stopwords, ponctuation, hashtags, etc.)
   - Gestion des valeurs manquantes et transformation des entités textuelles.  

2. **Analyse exploratoire (EDA)**
   - Distribution des sentiments  
   - Nuages de mots (word clouds)  
   - Analyse des hashtags et de la longueur des tweets.  

3. **Modélisation**
   - Modèles testés :
     - Régression Logistique  
     - SVM (Support Vector Machine)  
     - Random Forest  
     - Multinomial Naive Bayes  
   - Évaluation à l’aide de métriques : Accuracy, Precision, Recall, F1-score.  

4. **Interprétation et visualisation des résultats**

---

##  Résultats clés

Type d’analyse, Modèle, Précision obtenue, Observations 

 Binaire,  Random Forest  **87.48 %**  Bon équilibre précision/rappel pour sentiments positifs et négatifs. 
 Multiclasse  Multinomial Naive Bayes  **85.88 %**  Performances équilibrées sur plusieurs catégories. 

Les analyses montrent une prédominance des tweets **neutres (~5200)**, suivis des **positifs (~3000)**, puis des **négatifs (~600)**.  
Les termes les plus fréquents sont liés à **SXSW**, **Apple**, **Google**, et leurs produits phares (*iPad*, *Android*, *iPhone*).

---

##  Enseignements

- Les tweets relatifs à **Apple** sont globalement plus nombreux et souvent plus positifs.  
- Les émotions négatives sont minoritaires mais concentrées autour de mots-clés spécifiques (ex. *hate*, *bad*, *terrible*).  
- Les modèles montrent un **déséquilibre de classes**, avec une surreprésentation du sentiment neutre.

---

##  Technologies utilisées

- **Python 3.x**
- **Bibliothèques principales :**
  - pandas, numpy  
  - matplotlib, seaborn, wordcloud  
  - scikit-learn  
  - nltk, re (pour le prétraitement du texte)

