# Social Living Europe — landing „Analiza działek”

Statyczny landing page reklamujący bezpłatną wstępną analizę gruntów pod
budownictwo społeczne i komunalne (dofinansowane).

## Zawartość

- `index.html` — kompletna, samodzielna strona (style inline, bez zależności build).
- `logo-sle.png`, `szkic-budynku-mieta.png` — grafiki marki.
- `Wizualna część aplikacji działek (5).zip` — oryginalny handoff (wytyczne + referencja + zrzuty).

## Uruchomienie

Otwórz `index.html` w przeglądarce albo serwuj katalog statycznie:

```bash
python3 -m http.server 8000
# http://localhost:8000
```

Fonty (IBM Plex Sans/Mono, Playfair Display) ładowane z Google Fonts.

## Zgodność z wytycznymi

Strona odwzorowuje 1:1 referencję `SLE-landing-wytyczne.md` /
`Landing Analiza Dzialek.dc.html` z handoffu: jeden dominujący styl CTA
(powtórzony w hero, po sekcjach, w CTA końcowym i stopce), formularz „wpisz
działkę” widoczny od razu (także na mobile), gwiazdki przy mocnych
twierdzeniach linkujące do widocznych zastrzeżeń, identyczne wizualnie kafle
liczbowe PL/EU z mikro-źródłami, wyróżniony blok „wkład własny”, sekcja „Rola
gminy”, pełne zastrzeżenia prawne w stopce oraz sticky CTA na mobile.

Framework `support.js` z referencji zastąpiono statycznym HTML; interakcje
(accordion FAQ i sekcja „Źródła”) obsługuje lekki vanilla JS na końcu pliku.

Odnośniki CTA prowadzą do formularza w hero (`#formularz`) — po podpięciu
właściwej aplikacji wystarczy podmienić `href` przycisków „Sprawdź działkę za
darmo” na docelowy URL.
