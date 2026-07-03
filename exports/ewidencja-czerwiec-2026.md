# Ewidencja czasu pracy — czerwiec 2026

**Repozytorium:** `centrum-dowodzenia`
**Zakres miesiąca:** 1–30 czerwca 2026
**Podstawa:** historia git (`git log`, `git log --numstat`)
**Data wygenerowania:** 2026-07-03

> Uwaga metodologiczna: ewidencja bazuje wyłącznie na danych z gita. Znaczniki czasu to momenty commitów — faktyczna praca (projektowanie, kodowanie, testy w przeglądarce) rozpoczyna się przed pierwszym commitem, dlatego zakres godzin commitów traktowany jest jako **dolne oszacowanie** rzeczywistego czasu pracy.
>
> Uwaga o autorstwie: 16 z 17 commitów zapisano jako autor `noreply@anthropic.com` (praca prowadzona w sesji Claude Code), 1 commit jako `msm@off.org.pl` (wgranie plików startowych). Ponieważ całość reprezentuje jedną sesję roboczą użytkownika, ewidencja obejmuje wszystkie commity dnia, a nie tylko filtrowane po adresie `msm@off.org.pl` (który sam w sobie dałby tylko 1 wpis).

---

## Ewidencja dzienna

| Data | Zakres godzin (pierwszy–ostatni commit) | Opis pracy | Szac. godziny |
|------|------------------------------------------|------------|---------------|
| 2026-06-22 (pon.) | 19:36–21:37 (~2h01m span commitów) | Zbudowanie i dopracowanie aplikacji „Centrum Dowodzenia" — jednostronicowego panelu (`index.html`) do koordynacji Gali. Utworzono szkielet projektu (strona ~303 linii, `README.md`, `package.json`), następnie zaktualizowano dane osobowe zespołu (usunięcie Roksany Dziury, przypisanie laureatów/finalistów do Wojtka i Nataszy, ujednolicenie stylu koordynatorki Alicji Janek, dodanie numeru telefonu Nikoli Sochy). Główny rezultat dnia to gruntowny redesign interfejsu Gali przeprowadzony w kilku iteracjach: najpierw wariant „dark glass Bento" z ambient glow i typografią szeryf+sans, potem zmiana na motyw jasny w stylu Efektoś (białe karty, jasne tło), a na końcu dopasowanie 1:1 do designu Efektoś z tokenami brandowymi OFF. Dzień zamknięto poprawkami jakościowymi: naprawą ucinania nazwiska koordynatora na kartach posterunków oraz zamianą emotek na spójny zestaw ikon (lucide SVG + kropki). Skala: 9 commitów właściwych (+8 merge), 3 pliki, ~700 dodanych / ~299 usuniętych linii. | ~3,5 h |

---

## Szczegóły dnia 2026-06-22

**Commity (chronologicznie):**

| Godzina | Opis commita | Zmiany |
|---------|--------------|--------|
| 19:36 | Usuń Roksanę Dziurę z Centrum Dowodzenia; laureaci/finaliści na Wojtka i Nataszę | `index.html` +7 / −15 |
| 20:44 | Ujednolić styl koordynatorki Alicji Janek z resztą koordynatorów | `index.html` +2 / −2 |
| 20:48 | Dodaj numer telefonu Nikoli Sochy | `index.html` +1 / −1 |
| 21:02 | Redesign UI Gali: dark glass Bento, ambient glow, szeryf+sans (2026) | `index.html` +147 / −78 |
| 21:09 | Zmiana motywu Gali na jasny (styl Efektoś): białe karty, jasne tło | `index.html` +76 / −84 |
| 21:17 | Dopasowanie 1:1 do designu Efektoś (tokeny OFF brand) | `index.html` +105 / −107 |
| 21:17 | Add files via upload (pliki startowe projektu) | `README.md` +28, `index.html` +303, `package.json` +12 |
| 21:21 | Napraw ucinanie nazwiska koordynatora na kartach posterunków | `index.html` +3 / −3 |
| 21:36 | Zamień emotki na spójny zestaw ikon (lucide SVG + kropki) | `index.html` +16 / −9 |

*(Ponadto 8 commitów typu merge integrujących powyższe zmiany do gałęzi głównej.)*

**Zmienione pliki (agregacja dnia):**

| Plik | Dodane | Usunięte |
|------|--------|----------|
| `index.html` | 660 | 299 |
| `README.md` | 28 | 0 |
| `package.json` | 12 | 0 |
| **Razem** | **700** | **299** |

---

## Podsumowanie

- **Dni z aktywnością:** 1 (22 czerwca 2026)
- **Łączna liczba commitów:** 17 (9 właściwych + 8 merge)
- **Zmienione pliki:** 3 (`index.html`, `README.md`, `package.json`)
- **Bilans linii:** +700 / −299
- **Łączny szacowany czas pracy w miesiącu:** **~3,5 h**

**Kamienie milowe:**

1. **Inicjalizacja projektu** — utworzenie struktury aplikacji „Centrum Dowodzenia" (panel Gali) z plikami `index.html`, `README.md`, `package.json`.
2. **Aktualizacja danych zespołu** — uporządkowanie listy koordynatorów, laureatów i finalistów oraz danych kontaktowych.
3. **Redesign interfejsu Gali** — trzy iteracje designu: dark glass Bento → jasny motyw Efektoś → dopasowanie 1:1 do designu Efektoś z tokenami brandowymi OFF.
4. **Poprawki jakościowe (polish)** — naprawa ucinania nazwisk koordynatorów na kartach posterunków oraz ujednolicenie ikonografii (lucide SVG zamiast emotek).

---

### Metodyka szacowania godzin

Zakres commitów w dniu 22.06 wynosi ~2 godziny (19:36–21:37). Do tego doliczono pracę poprzedzającą pierwszy commit oraz nieujętą w metadanych git: zbudowanie strony startowej (~303 linie), projektowanie i iteracyjne dopasowanie trzech pełnych wariantów UI oraz weryfikację wyglądu w przeglądarce między iteracjami. Z uwagi na charakter pracy (intensywne, wielokrotne przeprojektowania interfejsu) rzeczywisty czas oszacowano na **~3,5 h** — wartość traktowana jako ostrożne, dolne oszacowanie.
