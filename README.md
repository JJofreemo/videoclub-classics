# VideoClub Clàssics (exemple per Azure Static Web Apps)

Petit lloc web estàtic en català que simula un videoclub amb 6 pel·lícules clàssiques.

## Estructura
```
/videoclub
  ├── index.html
  ├── styles.css
  ├── app.js
  ├── /img
  │    └── *.png (pòsters generats)
  └── /pellicules
       └── *.html (fitxes de cada pel·lícula)
```

## Com pujar-ho a GitHub
1. Crea un repositori nou a GitHub (p.ex. `videoclub-classics`).
2. Puja el contingut de la carpeta `videoclub/` a la branca `main` del teu repositori.

## Desplegar a Azure Static Web Apps (SWA)
1. Al portal d'Azure, crea **Static Web App** (pla *Free* és suficient).
2. Connecta la teva subscripció de GitHub i selecciona el repositori i la branca.
3. Configuració de *Build presets*: **No framework** (o *Custom*). Directori d'app: `/`.
4. Azure crearà automàticament un workflow de GitHub Actions i publicarà el lloc.

## Desenvolupament local
Obre `index.html` amb un navegador o usa una extensió de *Live Server* a VS Code.
