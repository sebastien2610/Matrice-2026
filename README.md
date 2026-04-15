# Matrice-2026
Matrice 2026 Mobicore
<!DOCTYPE html>
<html lang="fr">
<head>
    <meta charset="UTF-8">
    <title>Pilotage Matrice Salariale | Vue Direction</title>
    <style>
        :root {
            --primary: #1a2a6c;
            --accent: #b21f1f;
            --bg: #f0f2f5;
        }
        body { font-family: 'Inter', sans-serif; background: var(--bg); margin: 0; display: flex; flex-direction: column; height: 100vh; }
        header { background: var(--primary); color: white; padding: 1rem 2rem; box-shadow: 0 2px 10px rgba(0,0,0,0.2); display: flex; justify-content: space-between; align-items: center; }
        .grid-container { display: grid; grid-template-columns: repeat(2, 1fr); gap: 20px; padding: 20px; flex-grow: 1; }
        .card { background: white; border-radius: 12px; overflow: hidden; box-shadow: 0 4px 6px rgba(0,0,0,0.05); border: 1px solid #e1e4e8; position: relative; }
        .card-header { padding: 10px 15px; background: #fafbfc; border-bottom: 1px solid #e1e4e8; font-weight: bold; color: var(--primary); }
        iframe { width: 100%; height: calc(100% - 40px); border: none; }
        .status-tag { background: #2ecc71; color: white; padding: 4px 10px; border-radius: 20px; font-size: 0.8rem; }
    </style>
</head>
<body>

<header>
    <div>
        <h2 style="margin:0;">Dashboard Matrice Salariale</h2>
        <small>Mise à jour en temps réel via Excel Engine</small>
    </div>
    <div class="status-tag">Connecté au flux Excel</div>
</header>

<div class="grid-container">
    <div class="card">
        <div class="card-header">Analyse par Département (TCD)</div>
        <iframe src="LIEN_EMBED_EXCEL_TCD"></iframe>
    </div>

    <div class="card">
        <div class="card-header">Répartition Salariale Mensuelle</div>
        <iframe src="LIEN_EMBED_EXCEL_GRAPHIQUE"></iframe>
    </div>

    <div class="card" style="grid-column: span 2;">
        <div class="card-header">Vue détaillée des effectifs</div>
        <iframe src="LIEN_EMBED_EXCEL_TABLEAU"></iframe>
    </div>
</div>

</body>
</html>
