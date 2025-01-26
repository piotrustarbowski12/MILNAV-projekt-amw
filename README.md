# MILNAV-projekt-amw
Nowoczesny system wyznaczania tras dla pojazdów wojskowych i żołnierzy w terenie

Produkt 1: Kod źródłowy
Wprowadzenie

Kod źródłowy systemu MILNAV jest kluczowym elementem projektu, zapewniającym działanie wszystkich modułów, w tym planowania tras, analizy danych oraz komunikacji. Jego rozwój, jakość oraz zabezpieczenie są priorytetowe dla realizacji celów projektu. Kod musi być napisany w sposób skalowalny, bezpieczny i zgodny z najlepszymi praktykami inżynierii oprogramowania.

Charakterystyka produktu

Charakter: Systemowy komponent bazowy umożliwiający działanie aplikacji MILNAV.
Cel: Realizacja funkcji planowania, monitorowania i analiz tras oraz komunikacji użytkowników w czasie rzeczywistym.
Funkcje: Obsługa algorytmów tras, przetwarzanie danych, interfejsy API.
Wygląd: Kod źródłowy zapisany i przechowywany w repozytorium Git.

Użytkownicy:
- Zespół deweloperski
- Testerzy oprogramowania
- Administratorzy systemu

Źródła informacji o funkcjonowaniu:
- Specyfikacja wymagań systemowych
- Dokumentacja techniczna MILNAV
- Raporty z testów i audytów bezpieczeństwa

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

---

Produkt 2 - Dokumentacja techniczna
Wprowadzenie
Dokumentacja techniczna projektu MILNAV zapewnia szczegółowe informacje dotyczące architektury systemu, sposobu działania modułów oraz wymagań funkcjonalnych i niefunkcjonalnych. Jest kluczowym narzędziem dla zespołów deweloperskich, testerów oraz administratorów.

Charakterystyka produktu:

Charakter: Zbiór informacji opisujących szczegóły techniczne systemu.
Cel: Ułatwienie zrozumienia działania systemu oraz jego rozwoju i utrzymania.
Funkcje: Dokumentowanie architektury, API, procesów instalacji i konfiguracji.
Wygląd: Pliki tekstowe i graficzne w formatach online (HTML) oraz PDF.

Użytkownicy:
- Programiści
- Testerzy
- Administratorzy systemu
- Menedżerowie projektu

Źródła informacji o funkcjonowaniu
- Specyfikacja techniczna MILNAV
- Raporty z testów i wdrożeń
- Opinie użytkowników końcowych

---
Prodkukt 3 - Fizyczne komponenty systemu
Wprowadzenie
Fizyczne komponenty systemu MILNAV obejmują urządzenia mobilne, stacje robocze oraz serwery odpowiedzialne za przetwarzanie danych i komunikację w czasie rzeczywistym. Ich niezawodność i wydajność są kluczowe dla zapewnienia ciągłości działania systemu w trudnych warunkach.

Charakterystyka produktu:
Charakter: Elementy sprzętowe wspierające funkcjonowanie systemu MILNAV.
Cel: Zapewnienie infrastruktury dla przetwarzania danych, komunikacji i obsługi użytkowników.
Funkcje: Przechowywanie danych, przetwarzanie w czasie rzeczywistym, komunikacja sieciowa.
Wygląd: Urządzenia mobilne, serwery w obudowach rackowych, stacje robocze z monitorami dotykowymi.

Użytkownicy:
- Żołnierze w terenie
- Operatorzy systemu w centrach dowodzenia
- Administratorzy infrastruktury IT

Źródła informacji o funkcjonowaniu:
- Dokumentacja techniczna MILNAV
- Raporty producentów sprzętu
- Instrukcje użytkowania

R4: Zagrożenie – Dokumentacja zostanie wykorzystana przez osoby niepowołane do ataku na system.

Wymagania funkcjonalne (WF)
WF1: Dokumentacja musi obejmować szczegółowy opis wszystkich modułów systemu, w tym:
Planowania tras.
- Analizy i raportowania.
- Komunikacji tekstowej i głosowej.
WF2: Musi zawierać przykłady użycia API, w tym zapytania i odpowiedzi w formacie JSON.
WF3: Dokumentacja powinna zawierać przewodnik instalacji systemu, konfiguracji serwerów oraz klientów.
WF4: Powinna być dostępna w wersji online oraz w formacie PDF.
WF5: Każda aktualizacja systemu musi być odzwierciedlona w dokumentacji w czasie nie dłuższym niż 24 godziny.
R5: Zagrożenie – Niedostępność dokumentacji podczas awarii serwera.

Wymagania wydajnościowe (WW)
WW1: Dokumentacja online musi być dostępna 24/7 z czasem ładowania poniżej 2 sekund na łączach o przepustowości 10 Mbps.
WW2: Wersja PDF nie może przekraczać rozmiaru 50 MB, zachowując pełną czytelność i grafikę.
WW3: Wyszukiwanie w dokumentacji online musi zwracać wyniki w czasie poniżej 1 sekundy.
R6: Zagrożenie – Nieautoryzowany dostęp do dokumentacji zawierającej wrażliwe dane.

Wymagania bezpieczeństwa (WB)
WB1: Dostęp do dokumentacji online musi być chroniony przez system autoryzacji z wykorzystaniem 2FA.
WB2: Dokumentacja zawierająca szczegółowe dane techniczne powinna być dostępna wyłącznie dla uprawnionych użytkowników.
WB3: Kopie zapasowe dokumentacji muszą być przechowywane w co najmniej dwóch lokalizacjach.
WB4: Dokumentacja PDF musi być zabezpieczona hasłem przed nieautoryzowanym otwarciem i edycją.

---

