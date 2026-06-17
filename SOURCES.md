# Sources des données — Projet "L'IA et la productivité économique"

## 1. Adoption de l'IA par les entreprises (par pays et taille d'entreprise)
- **Source officielle** : Eurostat, enquête ICT usage and e-commerce in enterprises (ICT ENT)
- **Code dataset Eurostat** : isoc_eb_ai
- **Fichier source exact** : 2025_Enterprises_using_AI_tables_and_graphs.xlsx — fichier Excel officiel
  publié par Eurostat en annexe de l'article Statistics Explained, téléchargé directement par
  l'utilisateur depuis ec.europa.eu/eurostat/statistics-explained
- **Document complémentaire** : "The use of artificial intelligence (AI) technologies in the European Union — Key results, 2026 edition"
- **Éditeur** : Office des publications de l'Union européenne, Luxembourg, 2026
- **ISBN** : 978-92-68-37450-4 | DOI: 10.2785/9221093
- **Feuilles utilisées** :
  - Figure 2 — adoption IA précise par pays, 2024 ET 2025 (% d'entreprises), permettant de calculer
    la croissance en points de pourcentage
  - Table 1 (rapport PDF) — détail par taille d'entreprise (petite/moyenne/grande), 2025
- **Année de référence** : 2024 et 2025
- **Champ d'application** : entreprises de 10+ employés et travailleurs indépendants
- **Taille d'échantillon** : 157 000 entreprises enquêtées dans l'UE en 2025
- **Date d'accès** : 17 juin 2026
- **Note** : break in time series pour les Pays-Bas en 2025 (signalé par Eurostat, donnée gardée
  mais à mentionner en cas d'analyse spécifique de ce pays)

## 2. Productivité du travail (PIB par heure travaillée)
- **Source officielle** : International Labour Organization (ILOSTAT), modeled estimates and projections
- **Méthodologie** : Organisation internationale du travail, dollars internationaux 2021
- **Page source** : Wikipedia "List of countries by labour productivity" (compilation citant ILOSTAT)
- **URL ILOSTAT** : https://ilostat.org/topics/labour-productivity/
- **Année de référence** : 2025
- **Date d'accès** : 17 juin 2026

## 3. PIB réel par habitant
- **Source officielle** : Eurostat (online data code: sdg_08_10)
- **Page source** : Wikipedia "List of European countries by Real GDP per capita" (compilation citant Eurostat)
- **URL Eurostat** : https://ec.europa.eu/eurostat/databrowser/view/sdg_08_10/default/table
- **Année de référence** : 2023 (dernière année disponible au moment de la compilation Wikipedia)
- **Unité** : euros par habitant
- **Date d'accès** : 17 juin 2026

## Limites méthodologiques importantes (à mentionner dans l'analyse)

1. **Décalage temporel** : l'adoption de l'IA est mesurée en 2025, la productivité du travail en 2025
   (mais sur une méthodologie ILO différente d'Eurostat), et le PIB par habitant en 2023. Ce
   décalage signifie qu'on ne capture pas un effet causal immédiat — c'est une limite à
   mentionner explicitement dans toute conclusion.

2. **Corrélation ≠ causalité** : un pays peut avoir une forte adoption de l'IA ET une forte
   productivité simplement parce qu'il est riche et technologiquement avancé pour d'autres
   raisons (infrastructure, éducation, institutions). D'où l'intérêt d'inclure le PIB par
   habitant comme variable de contrôle dans la régression multiple.

3. **Échantillon européen uniquement** : les données Eurostat ne couvrent que l'UE + quelques
   pays associés (Norvège, Albanie, Bosnie, Monténégro, Serbie, Turquie). Les résultats ne sont
   pas généralisables à l'OCDE entière ou au monde sans réserve.

4. **Causalité inverse possible** : les pays plus productifs ont peut-être plus de ressources
   à investir dans l'IA, plutôt que l'inverse (l'IA cause la productivité).

5. **Mesure de l'adoption** : Eurostat mesure l'usage d'au moins une technologie IA listée
   (text mining, machine learning, etc.) — une définition large qui inclut des usages très
   basiques au même titre que des usages avancés.
