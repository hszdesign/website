# HSZ Design — strona

Strona studio druku 3D HSZ Design. Statyczny HTML hostowany na GitHub Pages, custom domena: [hszdesign.pl](https://hszdesign.pl).

## Struktura

- `index.html` — landing page (one-pager)
- `admin/` — panel admina (login Google, edycja realizacji/tekstów/briefów)
- `assets/` — logo i statyczne zasoby
- `CNAME` — custom domena dla GitHub Pages

## Backend

Formularz briefu i admin panel komunikują się z Google Apps Script Web App. Kod backendu i instrukcja deploya: [../google-apps-script/](../google-apps-script/) (poza repo strony — wdrażany ręcznie z konta Google HSZ).

## Lokalne uruchomienie

```bash
python3 -m http.server 4321 --directory .
# → http://localhost:4321
```

## Deploy

Każdy push do `main` automatycznie publikowany przez GitHub Pages na hszdesign.pl.
