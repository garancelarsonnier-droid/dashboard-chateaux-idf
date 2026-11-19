# Tableau de bord — Châteaux et demeures en Île-de-France

TP2 SIG & CIM (ESTP) — Partie 3 : tableau de bord HTML valorisant les résultats du projet ArcGIS Pro.

## Contenu
- `index.html` — le tableau de bord : descriptions, 4 indicateurs clés, carte interactive Leaflet,
  graphique des catégories (Chart.js), population par département, carte ArcGIS Pro (Q3.1), interprétation.
- `data/Chateaux_demeu_FeaturesToJSO.geojson` — 76 châteaux et demeures (Institut Paris Region), WGS 84.
- `data/communes_RP2017_Project.geojson` — 1 287 communes + données INSEE 2017, WGS 84.
- `data/departement_IDF.geojson` — 8 départements avec population sommée (fusion ArcGIS Pro), WGS 84.
- `data/Q3.1.png` — impression d'écran de la mise en page ArcGIS Pro (Q3.1).

## Ouvrir le tableau de bord
Double-cliquer sur `index.html` fonctionne dans la plupart des navigateurs.
Sinon, depuis ce dossier :

```
python -m http.server 8000
```

puis ouvrir http://localhost:8000

## Fichiers de rendu
Ne transmettre que l'index ne suffit pas : le dossier complet `index.html` + `data/` est requis,
en conservant les chemins relatifs utilisés dans le code (`data/…`).
