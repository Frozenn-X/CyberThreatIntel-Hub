


<svg viewBox="0 0 800 500" xmlns="http://www.w3.org/2000/svg">
  <rect width="800" height="500" fill="#f8f9fa"/>
  <text x="400" y="30" font-family="Arial" font-size="24" text-anchor="middle" font-weight="bold">Architecture détaillée du routage en oignon (Tor)</text>
  
  <circle cx="100" cy="150" r="50" fill="#e6f7ff" stroke="#1890ff" stroke-width="2"/>
  <text x="100" y="150" font-family="Arial" font-size="16" text-anchor="middle">Utilisateur</text>
  <text x="100" y="170" font-family="Arial" font-size="12" text-anchor="middle">(Alice)</text>
  <circle cx="250" cy="150" r="50" fill="#fff2e8" stroke="#fa8c16" stroke-width="2"/>
  <text x="250" y="140" font-family="Arial" font-size="16" text-anchor="middle">Nœud</text>
  <text x="250" y="160" font-family="Arial" font-size="16" text-anchor="middle">d'entrée</text>
  <text x="250" y="180" font-family="Arial" font-size="10" text-anchor="middle">(Garde)</text>
  <circle cx="400" cy="150" r="50" fill="#f6ffed" stroke="#52c41a" stroke-width="2"/>
  <text x="400" y="140" font-family="Arial" font-size="16" text-anchor="middle">Nœud</text>
  <text x="400" y="160" font-family="Arial" font-size="16" text-anchor="middle">intermédiaire</text>
  <text x="400" y="180" font-family="Arial" font-size="10" text-anchor="middle">(Relais)</text>

  <circle cx="550" cy="150" r="50" fill="#fff1f0" stroke="#f5222d" stroke-width="2"/>
  <text x="550" y="140" font-family="Arial" font-size="16" text-anchor="middle">Nœud</text>
  <text x="550" y="160" font-family="Arial" font-size="16" text-anchor="middle">de sortie</text>
  <text x="550" y="180" font-family="Arial" font-size="10" text-anchor="middle">(Exit)</text>

  <circle cx="700" cy="150" r="50" fill="#f9f0ff" stroke="#722ed1" stroke-width="2"/>
  <text x="700" y="140" font-family="Arial" font-size="16" text-anchor="middle">Serveur</text>
  <text x="700" y="160" font-family="Arial" font-size="16" text-anchor="middle">Dark Web</text>
  <text x="700" y="180" font-family="Arial" font-size="10" text-anchor="middle">(.onion)</text>

  <line x1="150" y1="150" x2="200" y2="150" stroke="#1890ff" stroke-width="2" marker-end="url(#arrowhead)"/>
  <line x1="300" y1="150" x2="350" y2="150" stroke="#fa8c16" stroke-width="2" marker-end="url(#arrowhead)"/>
  <line x1="450" y1="150" x2="500" y2="150" stroke="#52c41a" stroke-width="2" marker-end="url(#arrowhead)"/>
  <line x1="600" y1="150" x2="650" y2="150" stroke="#f5222d" stroke-width="2" marker-end="url(#arrowhead)"/>
  
  <!-- Flèches allant vers l'utilisateur (retour) -->
  <path d="M650 170 C620 200, 580 200, 550 170" stroke="#f5222d" stroke-width="2" fill="transparent" marker-end="url(#arrowhead)"/>
  <path d="M500 170 C470 200, 430 200, 400 170" stroke="#52c41a" stroke-width="2" fill="transparent" marker-end="url(#arrowhead)"/>
  <path d="M350 170 C320 200, 280 200, 250 170" stroke="#fa8c16" stroke-width="2" fill="transparent" marker-end="url(#arrowhead)"/>
  <path d="M200 170 C170 200, 130 200, 100 170" stroke="#1890ff" stroke-width="2" fill="transparent" marker-end="url(#arrowhead)"/>
  
  <!-- Couches de chiffrement -->
  <g transform="translate(100, 280)">
    <rect width="600" height="160" fill="#f0f2f5" stroke="#bfbfbf" stroke-width="1"/>
    <text x="300" y="25" font-family="Arial" font-size="18" text-anchor="middle">Représentation des couches de chiffrement</text>
    
    <!-- Requête -->
    <rect x="20" y="50" width="120" height="80" fill="#e6f7ff" stroke="#1890ff" stroke-width="2"/>
    <text x="80" y="90" font-family="Arial" font-size="14" text-anchor="middle">Requête</text>
    
    <!-- Couche 1 -->
    <rect x="160" y="50" width="120" height="80" fill="#fff2e8" stroke="#fa8c16" stroke-width="2"/>
    <rect x="170" y="60" width="100" height="60" fill="#e6f7ff" stroke="#1890ff" stroke-width="2"/>
    <text x="220" y="90" font-family="Arial" font-size="14" text-anchor="middle">Couche 1</text>
    
    <!-- Couche 2 -->
    <rect x="300" y="50" width="120" height="80" fill="#f6ffed" stroke="#52c41a" stroke-width="2"/>
    <rect x="310" y="60" width="100" height="60" fill="#fff2e8" stroke="#fa8c16" stroke-width="2"/>
    <rect x="320" y="70" width="80" height="40" fill="#e6f7ff" stroke="#1890ff" stroke-width="2"/>
    <text x="360" y="90" font-family="Arial" font-size="14" text-anchor="middle">Couche 2</text>
    
    <!-- Couche 3 -->
    <rect x="440" y="50" width="120" height="80" fill="#fff1f0" stroke="#f5222d" stroke-width="2"/>
    <rect x="450" y="60" width="100" height="60" fill="#f6ffed" stroke="#52c41a" stroke-width="2"/>
    <rect x="460" y="70" width="80" height="40" fill="#fff2e8" stroke="#fa8c16" stroke-width="2"/>
    <rect x="470" y="75" width="60" height="30" fill="#e6f7ff" stroke="#1890ff" stroke-width="2"/>
    <text x="500" y="90" font-family="Arial" font-size="14" text-anchor="middle">Couche 3</text>
  </g>
  
  <!-- Définition des marqueurs -->
  <defs>
    <marker id="arrowhead" markerWidth="10" markerHeight="7" refX="9" refY="3.5" orient="auto">
      <polygon points="0 0, 10 3.5, 0 7" fill="#000"/>
    </marker>
  </defs>
</svg>