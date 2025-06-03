# Chatbot TF-IDF – Analyse de discours présidentiels

Ce projet est un chatbot qui utilise les techniques de **TF-IDF** et de **similarité cosinus** pour générer des réponses à partir d'un corpus de discours de présidents français.  
Il est conçu entièrement en Python, sans librairie externe autre que `math` et `os`, et le code est organisé en plusieurs fichiers qui ont chacun un rôle précis.

## Fonctionnalités
- Prétraitement de discours : nettoyage des caractères spéciaux
- Calcul des matrices TF, IDF et TF-IDF
- Similarité cosinus entre questions et documents
- Génération automatique de réponses les plus pertinentes
- Affichage optionnel de la matrice TF-IDF
- Ajout facile de nouveaux discours au corpus

## Structure
- `main.py` : lance l'interface utilisateur textuelle
- `traitement_fichiers.py` : nettoyage et gestion des fichiers texte
- `calcul_tf_idf.py` : calculs TF, IDF, et TF-IDF
- `fonctionnalites.py` : fonctions pour explorer certains aspects du corpus
- `generation_reponse.py` : détection et génération de réponses
- `speeches/` : discours d'origine
- `cleaned/` : discours nettoyés automatiquement

## Lancer le programme
Assurez-vous d'avoir Python 3 installé.

```bash
python main.py
```

Le programme s'utilise en ligne de commande, avec affichage console.

## Ajouter de nouveaux discours

Ajoutez un fichier au format :
```
Nomination_[NomDuPrésident][Numéro].txt
```
dans le dossier `speeches/` (ex: `Nomination_Macron2.txt`). Le fichier sera automatiquement traité au prochain lancement.

---

*Projet réalisé en décembre 2023, mis en ligne ici en juin 2025.*
