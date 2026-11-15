# Alcara

Polski prototyp menu gry 2D, z warszawską panoramą, tramwajem i ekranami logowania oraz rejestracji.

## Podgląd

Otwórz `index.html`, aby zobaczyć menu i formularze. Do logowania uruchom stronę przez HTTP, np. poleceniem `python -m http.server 8000`, i odwiedź `http://localhost:8000/`.

## Supabase Auth

1. W projekcie Supabase włącz logowanie e-mailem. W `config.js` wpisz adres projektu i jego publiczny klucz publishable zaczynający się od `sb_publishable_`.
2. W Authentication → URL Configuration ustaw Site URL i dodaj adres strony do Redirect URLs. Dla lokalnego testu dodaj `http://localhost:8000/`.
3. Zarejestruj testowe konto. Jeśli potwierdzanie e-maila jest włączone, użyj linku z wiadomości, a następnie sprawdź logowanie i wylogowanie.

Do konfiguracji przeglądarkowej używaj wyłącznie klucza publishable. Hasła obsługuje Supabase Auth. Prototyp nie wymaga własnych tabel.

## GitHub Pages

Umieść pliki w katalogu głównym repozytorium. W Settings → Pages wybierz publikację z gałęzi `main` i katalogu `/ (root)`. Dodaj pełny adres strony Pages do Redirect URLs w Supabase.
