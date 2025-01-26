# MILNAV-projekt-amw
Nowoczesny system wyznaczania tras dla pojazdów wojskowych i żołnierzy w terenie

Produkt 1: Kod źródłowy

R1: Zagrożenie – Nieuczciwy klient wykorzysta system, aby zatankować inny podmiot bez autoryzacji.

Wymagania funkcjonalne (WF)
WF1: Kod źródłowy musi wspierać wszystkie kluczowe funkcjonalności systemu, w tym:
- Planowanie i monitorowanie tras w czasie rzeczywistym.
- Generowanie raportów i analiz danych historycznych.
- Komunikację tekstową i głosową pomiędzy użytkownikami.
WF2: Kod musi umożliwiać integrację z zewnętrznymi API do aktualizacji map i danych dynamicznych (np. warunki pogodowe).
WF3: Wbudowane moduły muszą umożliwiać rozszerzalność funkcjonalności bez konieczności gruntownej przebudowy architektury.
WF4: Kod musi obsługiwać wielojęzyczność, zapewniając dostosowanie systemu do różnych lokalizacji i użytkowników.

R2: Zagrożenie – Atakujący uzyska dostęp do serwera i zmanipuluje dane tras.

Wymagania wydajnościowe (WW)
WW1: Kod musi być zoptymalizowany pod kątem szybkości przetwarzania danych:
- Czas wyznaczenia trasy: <15 sekund.
- Czas reakcji na zmiany parametrów trasy: <5 sekund.
WW2: Kod musi umożliwiać jednoczesną obsługę co najmniej 500 aktywnych użytkowników bez wpływu na wydajność.
WW3: Moduły komunikacyjne muszą działać w czasie rzeczywistym z opóźnieniem nie większym niż 200 ms.
WW4: Kod źródłowy musi być kompatybilny z urządzeniami mobilnymi, ograniczając zużycie pamięci do maksymalnie 2 GB RAM.

R3: Zagrożenie – Przejęcie komunikacji między użytkownikami przez osoby trzecie.

Wymagania bezpieczeństwa (WB)
WB1: Kod musi obsługiwać szyfrowanie danych przesyłanych pomiędzy klientem a serwerem przy użyciu protokołów takich jak TLS 1.3.
WB2: Implementacja mechanizmów ochrony przed atakami typu SQL Injection, XSS oraz CSRF.
WB3: System musi umożliwiać szyfrowanie kodu źródłowego przed publikacją na serwerach zewnętrznych.
WB4: Każda zmiana w kodzie musi być śledzona w systemie kontroli wersji, a commitów dokonywać mogą wyłącznie uprawnieni deweloperzy.
WB5: Wprowadzenie testów penetracyjnych każdej nowej wersji kodu przed jej wdrożeniem do produkcji.
