# Albion DPS Overlay

Overlay DPS transparent qui se superpose à Albion Online en temps réel.

---

## ⚡ Créer l'installateur Windows (.exe) — 3 étapes

### Prérequis
- [Node.js]

- [Double clic sur ici pour le télécharger](https://nodejs.org/dist/v26.3.0/node-v26.3.0-x64.msi)


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
