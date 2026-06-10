# Albion DPS Overlay

Overlay DPS transparent qui se superpose à Albion Online en temps réel.

---

## ⚡ Créer l'installateur Windows (.exe) — 3 étapes

### Prérequis
- [Node.js](https://nodejs.org) (LTS) — télécharge et installe si pas déjà fait

### Étapes

**1. Ouvre un terminal dans ce dossier**
   - Clic droit sur le dossier → "Ouvrir dans le terminal"
   - ou CMD : `cd C:\chemin\vers\albion-dps-overlay`

**2. Installe les dépendances**
```
npm install
```

**3. Lance la compilation**
```
npm run dist
```

⏳ Patiente 2-3 minutes (télécharge Electron ~100 Mo la première fois)

**Résultat** : le fichier `dist\Albion DPS Overlay Setup 1.0.0.exe` apparaît.
Double-clique dessus → installation classique Windows → raccourci sur le bureau.

---

## Utilisation

Deux fenêtres s'ouvrent au démarrage :

| Fenêtre | Rôle |
|---|---|
| **Contrôles** | Ajouter joueurs, saisir dégâts, importer logs |
| **Overlay** | Fenêtre transparente par-dessus Albion |

### Raccourcis globaux (fonctionnent même quand Albion est en avant-plan)

| Raccourci | Action |
|---|---|
| `Ctrl+Shift+Space` | Start / Pause le timer |
| `Ctrl+Shift+R` | Reset la session |
| `Ctrl+Shift+D` | Toggle clic-travers overlay |

### Conseil
Lance Albion en **mode fenêtré sans bordures** (paramètres graphiques du jeu) pour que l'overlay s'affiche par-dessus.

---

## Structure du projet
```
albion-dps-overlay/
├── src/
│   ├── main.js         ← Processus principal Electron
│   ├── overlay.html    ← Fenêtre overlay transparente
│   └── control.html    ← Panneau de contrôle
├── assets/
│   └── icon.ico        ← Icône de l'app
├── package.json
└── README.md
```
