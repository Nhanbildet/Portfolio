📊 Analyse du risque de crédit – Microsoft Fabric
📌 Ce projet a pour objectif d’analyser le risque de défaut afin d’identifier les profils clients à risque et d’améliorer la prise de décision dans l’octroi de crédit.
Le dataset contient 33 000 prêts provenant du Royaume-Uni, du Canada et des États-Unis, avec des montants allant jusqu’à 35 000 USD.

🎯 Problématique métier: Dans un contexte bancaire, la maîtrise du risque de défaut est essentielle pour garantir la rentabilité et la stabilité du portefeuille.Les principales questions :

    - Le pays influence-t-il le risque de défaut ?
    
    - Quels types de prêts sont les plus risqués ?
    
    - Quels profils clients présentent un risque élevé ?

⚙️ Technologies utilisées: Microsoft Fabric, Lakehouse, Data Warehouse, Dataflows Gen2, SQL, Python, Power BI

🏗️ Architecture de données

Le projet suit une architecture de type Medallion :

    - Bronze (Ingestion): Collecte et stockage des données brutes dans le Lakehouse
    
    - Silver (Transformation): Nettoyage et transformation des données avec Dataflows Gen2
    
    - Gold (Serving): Modélisation dans le Data Warehouse (schéma en étoile)
    
    - Visualisation: Dashboard interactif dans Power BI

📊 Principaux insights

    - Le pays n’est pas un facteur déterminant du risque
    
    - Les prêts Conso dettes et Médical sont les plus risqués
    
    - Les clients avec des grades D à G présentent un risque élevé
    
 Le risque augmente lorsque :
    
    - Taux d’intérêt > 11%
    
    - Montant du prêt < 8K
    
    - Ratio dette/revenu > 33%
    
    - Revenu < 55K
    
👉 Le risque est encore plus élevé lorsque ces facteurs sont combinés

📈 Dashboard: Le dashboard Power BI permet :

    - Une vue globale des KPI (taux de défaut, volume de prêts, taux moyen)
    
    - Une segmentation du risque par type de prêt et classe de crédit
    
    - Une analyse des facteurs (revenu, ratio d’endettement)
    
    - Une interaction via des filtres (pays, type de prêt, classe)

👩‍💻 Auteur

Nhan Bildet
Data Analyst
