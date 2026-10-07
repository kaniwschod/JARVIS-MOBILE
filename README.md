# JARVIS Mobile Standalone PWA — 19.7.6.3

To jest wariant darmowy, niezależny od komputera.

## Co daje
- działa z hostingu HTTPS zamiast z `phone_server.py`,
- można dodać do ekranu początkowego iPhone'a,
- nie wygasa po 7 dniach,
- nie wymaga Apple Developer Program,
- Morning Protocol,
- pogoda z lokalizacji iPhone'a,
- My Day przechowywane lokalnie,
- głos przez Web Speech API,
- offline shell przez Service Worker.

## Czego PWA nie ma
- brak natywnego AlarmKit,
- brak bezpośredniego EventKit/Kalendarza iPhone'a,
- brak gwarantowanego działania w tle jak aplikacja natywna.

## GitHub Pages
Repozytorium zawiera workflow:
`.github/workflows/jarvis-mobile-pages.yml`

Po pushu do `main`:
1. GitHub -> Settings -> Pages.
2. W `Build and deployment` wybierz `GitHub Actions`.
3. Uruchom workflow `Deploy JARVIS Mobile PWA`.
4. Po deployu GitHub poda adres strony.
5. Otwórz go w Safari na iPhonie.
6. Udostępnij -> Dodaj do ekranu początkowego.

## Morning Protocol z alarmu
W Skrótach:
`Gdy alarm zostanie zatrzymany -> Otwórz adres URL`

URL GitHub Pages zakończ:
`?morning=1`

Przykład:
`https://twoj-login.github.io/JARVIS/?morning=1`

To otworzy JARVIS Mobile i automatycznie uruchomi odprawę.
