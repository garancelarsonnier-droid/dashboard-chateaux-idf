# Tableau de bord — Châteaux et demeures en Île-de-France (TP2 SIG & CIM)

## Contenu du dossier
- `index.html` — la page du tableau de bord (titres, indicateurs, carte Leaflet, graphique, tableau, interprétation).
- `data/` — dossier où s'ouvrent les exports ArcGIS Pro.

## Ce qu'il faut mettre dans `data/`
Exporté depuis ArcGIS Pro avec **Outils de Conversion → JSON → Entités vers JSON** (système de coordonnées de sortie **WGS 84, EPSG:4326**) :

1. `Chateaux_demeures_IDF.geojson` — la couche des châteaux et demeures (obligatoire : c'est elle qui alimente la carte, les indicateurs, le graphique et le tableau).
2. `communes_RP2017.geojson` — facultatif, si vous souhaitez ajouter un fond communal.

⚠️ Si l'export « Entités vers JSON » d'ArcGIS produit du format Esri JSON, il est lu aussi, mais gardez le nom exact du fichier ci-dessus (ou modifiez la ligne `FICHIERS` en haut du `<script>` dans `index.html`).

## Lancer le tableau de bord
Double-cliquer sur `index.html` suffit si le navigateur autorise le chargement local de fichiers.
Sinon (recommandé), dans le dossier, lancer :

```
python -m http.server 8000
```

puis ouvrir http://localhost:8000

## Fichiers inutiles au rendu
Aucune installation, aucun compte : tout est embarqué (Leaflet et Chart.js chargés depuis des CDN).
