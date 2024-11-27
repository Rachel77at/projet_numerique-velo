# **Simulation de la chute libre de Felix Baumgartner 🚀**

## **Description du projet**
Ce projet consiste à **simuler et analyser la chute libre de Felix Baumgartner**, un événement emblématique qui a marqué l'histoire en 2012 lorsqu'il a franchi le mur du son.  
L'objectif est de combiner **mécanique physique** et **modélisation numérique** pour reproduire les données expérimentales et explorer les dynamiques de la chute.

Le projet se divise en trois parties :
1. **Analyse des données expérimentales** : Extraction de la vitesse maximale et comparaison avec la vitesse du son.
2. **Modélisation théorique** : Simulation de la chute libre à partir des forces physiques (poids, traînée).
3. **Simulation numérique** : Application de la méthode d'Euler-Cromer pour analyser la vitesse, l'altitude et l'accélération au cours du saut.

---

## **Caractéristiques principales**
- **Langage utilisé** : Python (bibliothèques `numpy`, `matplotlib`).
- **Méthodologie** :
  - Analyse des forces physiques : **gravité** et **traînée**.
  - Utilisation des modèles atmosphériques (variations de la densité de l'air, vitesse du son).
  - Méthode d'Euler-Cromer pour la résolution des équations différentielles.

---

## **Parties du projet**
### **1. Analyse des données expérimentales**
- Tracé des courbes de vitesse de Baumgartner et de la vitesse du son en fonction de l'altitude.
- Identification de la **vitesse maximale mesurée** (377 m/s) et des altitudes où Baumgartner est supersonique.
- Calcul des vitesses moyennes sur différentes phases de la chute.

### **2. Modélisation théorique**
- Forces modélisées :
  - **Poids** : dépendant de l'altitude via la loi de gravitation universelle.
  - **Force de traînée** : dépendant de la densité de l'air et de la vitesse.
- Deux approches pour la densité de l'air :
  - Constante (modèle simplifié).
  - Variable avec l'altitude (modèle atmosphérique basé sur la loi des gaz parfaits).
- Calcul de la **vitesse maximale théorique** dans chaque cas, avec comparaison aux données expérimentales.

### **3. Simulation numérique**
- Mise en œuvre de la méthode d'Euler-Cromer pour simuler :
  - L’accélération, la vitesse et l’altitude de Baumgartner.
  - L’évolution temporelle de la chute jusqu’à l’ouverture du parachute.
- Analyse et comparaison des courbes simulées avec les données expérimentales :
  - Vitesse maximale simulée.
  - Histogramme des erreurs relatives.

---

## **Prérequis**
Pour exécuter ce projet, vous devez disposer de :
- **Python 3.9+**
- Bibliothèques Python : `numpy`, `matplotlib`

---

## **Exécution**
### **Installation**
Clonez le dépôt sur votre machine locale :
```bash
git clone https://github.com/nom-utilisateur/chute-libre-baumgartner.git
cd chute-libre-baumgartner
