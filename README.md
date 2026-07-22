# Asociația Buni Prieteni — site

Site static (HTML/CSS/JS, fără build step) pentru Asociația Buni Prieteni —
împotriva cancerului, conectați prin speranță (Oradea).

## Structură

```
index.html         Acasă
despre.html         Despre noi
programe.html       Programe
implica-te.html      Implică-te / Donează
contact.html         Contact
404.html            Pagină de eroare (GitHub Pages)
assets/css/style.css  Stiluri (culori/token-uri în :root)
assets/js/main.js    Meniu mobil
assets/img/          Logo + ilustrații SVG
```

## Rulare locală

Nu e nevoie de build. Deschide `index.html` direct în browser, sau pornește
un server simplu din folder:

```
python -m http.server 8000
```

apoi accesează `http://localhost:8000`.

## De completat înainte de lansarea publică

Conținutul este un prim draft, cu texte realiste dar generice. Caută
`de completat` / `de confirmat` (marcate vizual cu o etichetă portocalie) în
paginile HTML pentru:

- **Contact** (`contact.html`): telefon, email oficial, adresă exactă.
- **Implică-te** (`implica-te.html`): IBAN, bancă, CIF/CUI, date pentru
  Formularul 230.
- **Despre noi** (`despre.html`): povestea reală a asociației, echipă.
- **Programe** (`programe.html`): confirmarea programelor active — lista
  actuală e orientativă, bazată pe tonul altor asociații similare.
- **Branding**: `assets/img/logo.svg` și paleta de culori din
  `assets/css/style.css` (`--color-primary`, `--color-accent`) sunt
  placeholder — se pot înlocui cu logo-ul și culorile reale ale asociației.

## Publicare cu GitHub Pages

Repo-ul e configurat să publice din branch-ul `main`, folder rădăcină.
După push, activează Pages din Settings → Pages → Source: `main` / `/(root)`.
