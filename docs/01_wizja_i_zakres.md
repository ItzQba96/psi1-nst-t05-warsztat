# 01. Wizja i Zakres Systemu

## 1.1 Problem biznesowy
| Element | Opis |
|---|---|
| **Problem** | Zbyt długi czas oczekiwania na diagnozę pojazdu, przedłużające się akceptacje wycen oraz konflikty o ostateczny koszt naprawy. |
| **Kogo dotyczy** | Kierownika warsztatu, mechaników, klientów warsztatu. |
| **Skutki** | Blokowanie stanowisk naprawczych (podnośników), przestoje w pracy mechaników, niezadowolenie klientów zaskoczonych ceną. |
| **Rozwiązanie** | Wdrożenie systemu zarządzania zleceniami z asystentem AI wspierającym diagnozę usterek oraz z systemem elektronicznych kosztorysów dla klientów. |

## 1.2 Cele biznesowe SMART
* **CEL-01:** Skrócenie średniego czasu od wystawienia kosztorysu do jego akceptacji przez klienta z obecnych 4 godzin do maksymalnie 30 minut, w ciągu 3 miesięcy od wdrożenia systemu.
* **CEL-02:** Skrócenie czasu diagnozowania usterek przez mechaników o średnio 20% dzięki wsparciu konsultanta AI, mierzone po miesiącu od uruchomienia platformy.

## 1.3 Interesariusze
| Interesariusz | Wpływ | Zainteresowanie | Opis / Rola w projekcie |
|---|---|---|---|
| Właściciel (Klient) | Wysoki | Wysokie | Płaci za system, oczekuje zwrotu z inwestycji i usprawnienia procesów w warsztacie. |
| Kierownik Warsztatu | Wysoki | Wysokie | Główny użytkownik biurowy, zarządza zleceniami, przydziela pracę mechanikom. |
| Mechanik | Średni | Wysokie | Użytkownik warsztatowy, oczekuje uproszczenia pracy i czytelnego interfejsu przy stanowisku. |
| Klient Warsztatu | Niski | Wysokie | Nie używa bezpośrednio systemu, ale otrzymuje linki do kosztorysów. Chce szybko poznać cenę. |
| Dostawca API AI | Średni | Niskie | Podmiot zewnętrzny zapewniający silnik wnioskujący dla konsultanta diagnostycznego. |
| Urząd Skarbowy | Wysoki | Niskie | Wymaga zgodności fakturowania z prawem (moduł księgowy świadomie wyrzucony poza MVP). |

## 1.4 Aktorzy bezpośredni
1. **Kierownik Warsztatu** – kompetencje cyfrowe: średnie. Korzysta z systemu na komputerze w biurze. Tworzy zlecenia i przypisuje pojazdy.
2. **Mechanik** – kompetencje cyfrowe: podstawowe. Korzysta z systemu na tablecie/telefonie przy podnośniku. Opisuje objawy i tworzy listę części do wymiany.
3. **Klient Warsztatu** – kompetencje cyfrowe: zróżnicowane. Otwiera link z SMS/e-mail w przeglądarce mobilnej, aby zaakceptować lub odrzucić kosztorys.

## 1.5 Zakres MVP (Co robimy)
* Zarządzanie flotą i klientami (rejestracja pojazdu, przypisanie do klienta).
* Tworzenie zlecenia naprawy i przypisanie go do konkretnego mechanika.
* Generowanie interaktywnego kosztorysu (części + robocizna).
* Zewnętrzny, unikalny link dla klienta z przyciskami "Akceptuj" / "Odrzuć".
* Konsultant AI: wpisywanie objawów usterki i otrzymywanie listy prawdopodobnych przyczyn.

### Poza zakresem (Czego NIE robimy w MVP)
* Pełny system księgowy (wystawianie faktur VAT, integracja z KSeF).
* Obsługa bramek płatności online (Przelewy24, PayU, Blik) za naprawy.
* Zaawansowany moduł magazynowy z automatycznym zamawianiem części.

## 1.6 Systemy zewnętrzne
* **Bramka powiadomień (SMS/e-mail):** Do wysyłania klientom linków z wyceną do akceptacji.
* **API modułu AI (np. OpenAI / dedykowany model):** Do analizy wprowadzonych przez mechanika objawów.
* **API hurtowni motoryzacyjnej (np. Inter Cars / Auto Partner):** Do pobierania aktualnych cen części zamiennych do kosztorysu.

## 1.7 Założenia biznesowe i ograniczenia
* Warsztat dysponuje stabilnym łączem Wi-Fi pokrywającym hale naprawcze (konieczne do działania tabletów).
* Klienci warsztatu posiadają smartfony z dostępem do internetu, co umożliwia im kliknięcie w link do wyceny.
* Ze względu na warunki warsztatowe, interfejs dla mechanika musi obsługiwać responsywność (RWD), posiadać duże elementy klikalne i obsługiwać tryb ciemny.

## 1.8 Analiza istniejących rozwiązań
| Rozwiązanie | Plusy | Minusy | Wnioski dla naszego systemu |
|---|---|---|---|
| **Tradycyjny zeszyt + telefon** | Niezawodność, brak konieczności szkoleń. | Brak spójnej historii napraw, notoryczne zapominanie o pozycjach na rachunku, blokowanie pracy przez czekanie na decyzję klienta. | Konieczność wyeliminowania papieru przy jednoczesnym zachowaniu intuicyjności. Proces akceptacji musi być asynchroniczny (link). |
| **Gotowe systemy klasy "Asystent Warsztatu"** | Rozbudowane zarządzanie magazynem i zintegrowane fakturowanie. | Przeładowanie funkcjami, wysoki próg wejścia dla mechaników, brak asystentów AI do diagnozy. | Nasz system MVP skupi się na innowacji (moduł AI) oraz prostocie kosztorysowania, odrzucając skomplikowane i nieużywane w małych warsztatach moduły magazynowe. |