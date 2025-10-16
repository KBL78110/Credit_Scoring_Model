📘 Projet (En cours de rédaction):

Credit_Scoring_Model
Démontrer ta capacité à fiabiliser la décision d’octroi de crédit.

🔗 Notebook complet disponible ici :
https://github.com/KBL78110/Credit_Scoring_Model/blob/main/projet%20datascience%20Rafika%20Cervera%20et%20Karim%20Belgacem%20VF.html
[Télécharger le fichier HTML]


🎯 Objectif business :

Savoir identifier un client à risque est stratégique. Dans le cas contraire cela entraîne des risques financiers, tels que l’augmentation des créances non honorées, l’impact sur la rentabilité et les liquidités, ainsi que des coûts opérationnels accrus liés à la gestion des impayés et du recouvrement.

Identifier et gérer ces clients risqués est essentiel pour prendre des décisions plus éclairées et estimer avec précision la probabilité de défaut de paiement.

Ce projet illustre comment un modèle prédictif peut qualifier correctement les clients. 


🧩 Données :

Source : lien ou description rapide Taille : nombre de lignes, variables Variables clés : âge, fréquence d’achat, panier moyen, ancienneté, etc.

⚙️ Méthodologie :

- Utilisation des informations clients utiles, à notre disposition, pour alimenter notre modèle : 
    - classes d'âges, 
    - situation familiale, 
    - professions, 
    - ancienneté, 
    - domiciliation du salaire, 
    - domiciliation de l'épargne, 
    - moyenne des encours, 
    - moyenne des mouvements, 
    - autorisation de découvert,
    - autorisation de chéquier 
    - cumul des débits. 
    - Ainsi que des niveaux de scores issus d'une première étude et qu’il convient d’améliorer. 

- Analyse de ces informations pour en tirer les premiers enseignements.
- Procéder aux ajustements requis pour fiabiliser notre modèle.
- Modélisation avec divisions de nos données en 2 ensembles : de test (30%) et d’apprentissage (70%). 
- L’ensemble d’apprentissage est utilisé pour entraîner le modèle, tandis que l’ensemble de test évalue ses performances.
  
- Analyse des résultats obtenus :
   - 58% des clients sont d’âge moyen (23-50 ans). 
   - 47% d’entre eux sont mariés et 36% sont célibataires. 
   - Ils ont une faible ancienneté dans la banque. Moins d’un an pour 43%. 
   - La moitié d’entre eux sont employés. 
   - 68% ont leur salaire est domicilié à la banque. 
   - 57% ont un découvert autorisé. 
   - Seuls 11% sont interdit de chéquier.
   - 79% ne disposent pas d’épargne. 
   - En termes de train de vie la grande majorité des clients ont des encours entre 2 et 5 K€. Un tiers ont des mouvements de moins de 10 K€. Quand aux nombres de débits, c’est assez variable.
 
   - Bon client :
      - Epargnant
      - Marié
      - Ancienneté > à 4 ans
      - 40 ans et plus
      - Domiciliation du salaire
      - Cadre / Employés
      - Encours > à 2K€
      - Plus de 30 K€ de mouvements
      - Plus de 100 débits
      - Découvert autorisé

    - Mauvais client :
      - Pas d’épargne
      - Célibataire / Divorcé / Veuf
      - Ancienneté < à 4 ans
      - Moins de 40 ans
      - Salaire non domicilié
      - Employés / Autres
      - Encours < à 2K€
      - Moins de 30 K€ de mouvements
      - Moins de 100 débits
      - Interdit de découvert
      -  Interdit de chéquier

     
- Ajustements :
    - Pour la stabilité du modèle, nous avons regroupés les modalités veufs et divorcés (situation familiale).  Ayant des valeurs faibles, ces variables sont peu informatives. En les regroupant, nous réduisons        la variabilité et améliorons la stabilité des coefficients estimés.
    - Les coefficients nous aide à comprendre comment chaque variable explicative influence la probabilité, Les variables dont le coefficient est trop élevé doivent être supprimées car elles n’ont pas une             influence suffisamment significative.



📈 Résultats clés :

Précision : 88% & 85 % AUC Score 1 : 0.75 AUC Score 2 : 0.85 AUC Score 3 : 0.89 f1 score : 87%

<img width="632" height="506" alt="image" src="https://github.com/user-attachments/assets/dd9c44b7-3a3e-447c-8c2b-3939a0d1ebb1" />

<img width="683" height="271" alt="image" src="https://github.com/user-attachments/assets/f5e601e8-e377-4a24-8a90-e35c985c5a51" />

<img width="542" height="442" alt="image" src="https://github.com/user-attachments/assets/ca346811-03dd-414a-b179-557eebeb26e0" />

<img width="548" height="442" alt="image" src="https://github.com/user-attachments/assets/615d0ae1-dd8e-4c66-8a83-8d435bee8ba4" />

<img width="553" height="447" alt="image" src="https://github.com/user-attachments/assets/82a90c1b-2322-4184-a004-454c99f0d1cd" />




💡 Insights business :

Dans 89% des cas, notre modèle qualifie correctement si un client est bon ou mauvais.
Nous vous garantissons un meilleur score que ceux actuellement utilisés en production dans votre établissement.
Vous serez en mesure de mieux identifier et gérer les clients à risques. Ce qui améliorera significativement vos performances et votre bonne santé financière.
Vous pourrez également mieux cibler vos offres commerciales, votre prospection, personnaliser l’expérience client et  prendre des décisions éclairées.
Par sa stabilité et sa robustesse, ce modèle s’adaptera à l’évolution de votre base de données clients.



🧠 Pistes d’amélioration :

Tester d’autres modèles.  Mettre en place un suivi temps réel.

🧰 Stack technique :

Python, pandas, scikit-learn, matplotlib, seaborn, numpy.

👤 Auteur :

Karim — Business Analyst | Executive MBA Big Data & IA LinkedIn | Portfolio Notion (à venir)
