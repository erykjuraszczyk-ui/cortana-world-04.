# Cortana World 04.0 — prototyp 3D

Gotowa, statyczna strona HTML/CSS/JavaScript. Nie wymaga Node.js ani własnego serwera. Scena 3D korzysta z Three.js ładowanego z CDN, więc przeglądarka potrzebuje internetu.

## Funkcje prototypu

- responsywny holograficzny interfejs dla telefonu i komputera;
- proceduralna scena 3D, pierścienie i cząsteczki;
- obracanie sceny, pauza animacji i przełączanie poświaty;
- demonstracyjny czat po polsku;
- synteza mowy i rozpoznawanie mowy, jeśli przeglądarka je obsługuje;
- brak kluczy API i brak połączenia z prawdziwym modelem AI.

## Darmowy hosting: GitHub Pages

Repozytorium musi być publiczne, aby korzystać z GitHub Pages w bezpłatnym planie GitHub Free.

1. Zaloguj się na https://github.com/new
2. Utwórz **publiczne** repozytorium o nazwie `cortana-world-04`. Nie zaznaczaj opcji tworzenia README, jeśli wgrywasz pliki z tego pakietu.
3. Rozpakuj ZIP i wgraj całą zawartość katalogu `cortana-world-free` do głównego katalogu repozytorium. Włącz również ukryty katalog `.github` — zawiera automatyczne wdrożenie.
4. Otwórz repozytorium → **Settings → Pages** i w polu **Build and deployment → Source** wybierz **GitHub Actions**.
5. Otwórz zakładkę **Actions**. Workflow „Deploy Cortana World to GitHub Pages” uruchomi się po wypchnięciu plików. Poczekaj na zielony status.
6. Adres strony będzie zwykle wyglądał tak: `https://TWOJ_LOGIN.github.io/cortana-world-04/`.

Po pierwszym skonfigurowaniu Pages każda zmiana wypchnięta do gałęzi `main` będzie publikowana automatycznie.

## Alternatywa: Cloudflare Pages

https://pages.cloudflare.com/ — można połączyć z repozytorium GitHub i wdrażać automatycznie pod adresem `*.pages.dev`.

## Następny etap: prawdziwe AI

Czat w tej paczce jest demonstracyjny. Do integracji modelu AI potrzebny jest backend (np. FastAPI) i klucz API przechowywany wyłącznie jako sekret po stronie serwera. Nie umieszczaj klucza w `index.html` ani w repozytorium.

## Informacja prawna

To nieoficjalny prototyp koncepcyjny, niezwiązany z Microsoftem. Nazwa i elementy identyfikacji Cortany mogą podlegać ochronie znaków towarowych i praw autorskich.
