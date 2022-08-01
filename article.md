---
title: |
  ![](./img/Logo.png){width=2in}  
  "Rapport de stage."
subtitle: "Overview"
date: \today{}
lang: fr-FR
urlcolor: blue
geometry: "left=2.5cm,right=2.5cm,top=3cm,bottom=3cm"
documentclass: article

---
# Rapport de stage: 
## Gestion automatisée des points de branchemnt optique (PBO)
effectué par ***Alioune MBODJI***


**Tuteur de stage** : Patrick NSUKAMI
**Superviseur académique** : Robert THIAW


**Établissement**: Dakar Institut of Technology DIT
**Entreprise d’accueil**: FREE

### REMERCIEMENTS

En premier lieu, je tiens à remercier M. Patrick , mon professeur en python. En tant que maître de stage, il m’a beaucoup appris et assisté par rapport à la réalisation de ce projet.
Je saisi cette occasion pour adresser mes profonds remerciements aux responsables et au personnel de l‘école.
Un grand merci à ma mère, ma famille et mes camarades de classe pour leurs conseils ainsi que leur soutien.


#### SOMMAIRE
	
* 1. L’environnement de travail	
* 2. Le secteur :	
* 3. Présentation :	
* 4. Le cadre du stage :	
* 5. Description de la structure sociale	
* 6. Fonctionnement	
* 7. Les travaux effectués et les apports du stage	
* 8. Les travaux effectués	
* 9. Les outils mis à ma disposition	
* 10. Les Missions du poste occupé	
* 11. Les tâches périphériques	
* 12. Les apports du stage	
* 13. Conclusion	
* 14. Bibliographie	

 
#### INTRODUCTION

Amorce et présentation du stage
Du 31Juillet 2022 au 04 Août 2022 (1 mois), j’ai effectué un stage au sein de l’école DIT (située à la cité Keur Guorgui). Au cours de ce stage, j’ai pu m’intéresser aux tâches qui sont directement liées à mon travail notamment le déploiement de la fibre optique. 

**Les missions :** 
Mon stage consiste principalement à mettre en place un système de gestion automatisé des points de branchement optique dans le cadre du déploiement de la fibre optique de FREE. 
Plus largement, ce stage a été l’opportunité pour moi d’appréhender et de mettre en pratique les connaissances (python, SGBD, devOPS) que j’ai eu à capitaliser au cours de ma première année d’étude en BIG DATA au Dakar Institut of Technology DIT.
Au-delà d’enrichir mes connaissances en développement notamment en python, ce stage m’a permis de comprendre l’impact que pourrait avoir ma formation appliquée à mon métier.

**Problématique et objectifs du rapport :**

Ce rapport de stage se développe ainsi au prisme de la problématique de comment gérer de manière automatique le déploiement des boîtiers de fibre optique et de faire un récapitulatif de ceux-ci à la fin de chaque semaine en envoyant un courriel à mon N+1. 
L’élaboration de ce rapport a pour principale source les données de recette hebdomadaire de ces boîtiers.

**Annonce du plan :**
En vue de rendre compte de manière fidèle et analytique de la période passée au sein de DIT, il apparaît logique de présenter à titre préalable l’environnement de travail, à savoir le secteur des télécommunications, puis d’envisager le cadre du stage Enfin, il sera précisé les différentes missions et tâches que j’ai pu effectuer. 



I / L’environnement de travail
A – Le secteur : Les télécommunications
1. **Présentation :**
Free au Sénégal est un opérateur global de Téléphonie mobile au Sénégal. Il compte aujourd’hui plus de 4 millions de clients qui utilisent tous les jours ses services mobiles, internet et financiers. 
En avril 2018, Tigo Sénégal devenu free est cédé à Saga Africa Holdings Limited, un consortium Sénégalo-Franco-Malgache.

Axian, groupe malgache appartenant à la famille Hiridjee, est présent à Madagascar et dans l’océan Indien à travers 4 secteurs d’activités : les télécoms, les services financiers, l’immobilier et l’énergie. Dans le domaine des télécoms, l’entreprise Telma se positionne comme le premier opérateur malgache grâce à ses offres mobiles et son réseau fibre optique le plus rapide d’Afrique. 


II / Le cadre du stage :
1. **Description de la structure sociale :**
L’école DIT regroupe un effectif de 12 employés, qui sont divisés départements, tous sous la direction du directeur général.
-         Directeur général
-         Directeur des études 
-         Responsable 
-         
-         
2. **Fonctionnement :**
Au sein de cette société, il est aisé de percevoir l’interaction constante entre les différents départements décrits plus haut.
Compte tenu du fait que mon stage a été exclusivement réalisé dans le cadre de mon travail professionnel, je vais plus m’atteler aux aspects techniques (mise en place du projet ainsi qu’aux travaux effectués)



III / Les travaux effectués et les apports du stage
A – Les travaux effectués 
Au cours de ce stage, j’ai eu l’opportunité de découvrir la multitude de solutions que pourrait m’offrir l’IA appliqué aux télécommunications. Pour une meilleure compréhension des tâches que j’ai pu effectuer, il apparaît approprié de traiter en premier lieu des outils qui étaient mis à ma disposition, puis de traiter de manière détaillée les tâches que j’ai pu effectuer.

1. **Les outils mis à ma disposition :**
Au cours de ce stage, j’ai pu bénéficier d’une bonne documentation sur la mise en place d’une base de données SQLite, ainsi que sur la façon de réaliser une application web avec Flask sur python3. Les liens ci-dessous : 
https://nskm.xyz/documents/sql-introduction.pdf
https://python.developpez.com/tutoriel/intro-flask-python3/#LVI
 De plus des données que m’ont fourni FREE dans le cadre du déploiement du réseau optique. 

2. **Les Missions du poste occupé :**
***Présentation :***
Comme il a été précisé en introduction, ma mission principale est de superviser le déploiement du réseau optique de l’opérateur FREE de bout en bout. Ainsi dans cette optique, j’ai pu constater qu’il était nécessaire d’automatiser certaines tâches fastidieuses. Notamment la phase de recette qui se déroule à la fin de chaque semaine. Cette phase a pour principalement objectif de recenser tous les boitiers qui ont été déployés au niveau des différentes zones de déploiement.  
En relevant les éléments suivants : le numéro du boitier, le nom de la plaque, le central sur lequel le boîtier est raccordé, la mesure prise sur une fibre du boitier, le port concerné, la nature de l’infrastructure (type PBO), le statut (rejeté ou non) et la partie commentaire.  

Au cours de ce stage, différentes sortes de tâches m’ont été confiées :
-         Définir un format d’input bien défini.
-         Stocker les données au niveau de la base de données.
-         Envoyer un courriel récapitulatif sur l’état d’avancement des travaux (Nombre de PBO (point de branchement optique) raccordés et ceux rejetés au cours de la recette. 

3. **Les tâches périphériques :** 
Au cours de mon stage, j’ai pu effectuer deux tâches qui se situent à la périphérie. Dès lors qu’elles m’ont permis d’apprendre différents aspects, il paraît approprié de s’y attarder. Il s’agit : 
-         L’élaboration des différentes étapes du formatage de mon input (code python).
-         La rédaction du rapport de stage.

B – Les apports du stage
***Les compétences : *** 
Au cours de ce stage, j’ai beaucoup appris. Les apports que j’ai tiré de cette expérience professionnelle et académique peuvent être regroupés autour de trois idées principales : les compétences acquises, les difficultés rencontrés et solutions apportées ainsi que la vie en société.
Compétences acquises
Ce stage m’a permis de consolider mes connaissances apprises au cours de cette première année d’étude en informatique spécialisation BIG DATA plus précisément en python et à la tenue d’une base de données. Aussi en termes de savoir-faire, j’ai pu apporter une plus-value à mon métier notamment avec un gain de temps considérable et très grande efficience. 

***Difficultés rencontrées et solutions apportées :***  
Les difficultés rencontrées sont principalement liées à l’élaboration du plan de travail, c’est-à-dire comment définir l’enchaînement des étapes à la suite des autres, la réalisation de l’interface web avec python et le délai de réalisation du rapport compte tenu de mon calendrier professionnel.

Comme solution, j’ai pu bénéficier du support de mon professeur, qui m’a orienté sur mes recherches ainsi qu’à la compréhension de mes supérieurs hiérarchiques.

***La vie en société :*** 
Mon stage chez DIT a été très instructif. Au cours de cette période j’ai ainsi pu observer le fonctionnement d’une société en l’occurrence l’école]. Par ailleurs, les relations humaines entre les différents employés, indépendamment de l’activité exercée par chacun d’eux, m’a appris sur le comportement à avoir en toute circonstance.



#### Conclusion 

**Résumé global :** 

Pour conclure, j’ai effectué mon stage de ma première année en BIG DATA au sein de l’école (DIT) en apportant plus-value à mon métier de superviseur déploiement fibre optique chez FREE. Lors de ce stage d’un (1) mois, j’ai pu mettre en pratique mes connaissances théoriques acquises durant ma formation au Dakar Institut of Technology (DIT), tout en étant confronté aux difficultés réelles du monde du travail.

**Apport et bilan :**

Ce stage a été très enrichissant pour moi, car il m’a permis d’entreprendre, m’a imprégné sur les métiers du BIG DATA et de l’IA et leurs impacts. Il m’a permis de participer concrètement à la résolution d’un problématique majeur dans le cadre de mon travail. Ce stage m’a aussi permis d’échelonner les paliers professionnellement avec un curriculum vitae beaucoup plus enrichissant.

**Réponse à la problématique :**

Cette expérience m’a permis de répondre aux questionnements que j’avais en ce qui concerne les moyens utilisés par les entreprises pour s’adapter à l’évolution des TIC notamment avec l’avènement de l’IA. Ainsi cela a contribué fortement à résoudre la gestion de l’infrastructure optique avec une très grande efficacité. 

**Perspective :**

A la fin de mon stage, l’objectif serait la mise en place de l’interface web (avec Flask) et de rajouter des fonctionnalités à savoir la partie exploitation de la fibre optique : gestion des abonnés en plus de la partie déploiement.

#### Bibliographie

1.	https://nskm.xyz/documents/sql-introduction.pdf
2.	https://python.developpez.com/tutoriel/intro-flask-python3/#LVI
3.	Fichier de recette des points de branchement optique.
4.	Cours Python 
 






