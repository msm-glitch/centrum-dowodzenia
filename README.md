# Centrum dowodzenia — VII Gala Stypendialna OFF

Statyczna, samowystarczalna strona (twarze wbudowane jako dane, brak zewnętrznych zależności).
Zakładki: Zespół + kontakty · Harmonogram · Wolontariusze (z posterunkami).

## Pliki
- `index.html` — cała strona (otwórz lokalnie dwuklikiem, żeby zobaczyć).
- `package.json` — serwer statyczny dla Railway.

## Deploy na Railway (3 sposoby)

**A. Najszybciej — przeciągnij folder:**
1. Railway → New Project → Deploy from local / "Empty Service".
2. Wrzuć ten folder (lub repo z tymi plikami).
3. Railway wykryje Node, zrobi `npm install` i `npm start` → strona serwowana na przydzielonym porcie.

**B. Przez CLI:**
```
npm i -g @railway/cli
railway login
railway init
railway up
```

**C. Czysto statycznie (bez Node):**
Jeśli wolisz, ustaw w Railway „Static" / nginx i podaj `index.html` jako root — `package.json` nie jest wtedy potrzebny.

> Strona działa też offline — wystarczy otworzyć `index.html` w przeglądarce.
