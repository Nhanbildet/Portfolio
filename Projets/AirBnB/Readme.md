* Analyse du marché Airbnb avec Microsoft Fabric

Ce projet analyse le marché de la location courte durée sur **Airbnb** afin d’identifier les opportunités d’investissement les plus rentables.

L’objectif est de déterminer quelles combinaisons de **localisation, type de logement, capacité et prix** permettent d’atteindre un revenu cible de **3 000 € par mois (36 000 € par an)**.

L’analyse se concentre sur trois marchés :

* Bordeaux
* Lyon
* Pays Basque

Le dataset contient environ **26 000 annonces Airbnb**.

## Architecture des données

Un pipeline de données end-to-end a été mis en place dans **Microsoft Fabric selon une architecture **Medallion (Bronze, Silver, Gold).

Flux de données :

Airbnb Dataset
→ Fabric Lakehouse (Bronze – stockage des données brutes)
→ PySpark / SQL (Silver – transformation des données)
→ Dataflows Gen2 (préparation et nettoyage)
→ Modèle en **Star Schema** (Gold – modèle analytique)
→ **Power BI** (visualisation et analyse)
