# 02. Słownik pojęć dziedziny

**System:** System zarządzania zleceniami napraw z modułem inteligentnych rekomendacji serwisowych (AI) dla niezależnego warsztatu samochodowego.

> Słownik opracowano na podstawie dokumentu `01_wizja_i_zakres.md` przekazanego przez zespół oraz uwag prowadzącego. Przykłady mają charakter ilustracyjny. Nazwy statusów i zasady przejść między nimi są propozycją do potwierdzenia podczas wywiadu z klientem.

<!--
Zasady:
- Jedno pojęcie, jedna nazwa. Synonimy wpisujemy w osobnej kolumnie i NIE używamy ich w dokumentacji.
- Definicja w języku klienta, bez żargonu technicznego.
- Nazwa angielska posłuży w cz. 2 jako nazwa klasy/tabeli.
- Kolejność alfabetyczna.
-->

| Pojęcie | Nazwa ang. (dla kodu) | Definicja | Synonimy (niezalecane) | Przykład | Powiązane pojęcia |
|---|---|---|---|---|---|
| Akceptacja kosztorysu | EstimateApproval | Potwierdzenie przez Klienta zgody na wykonanie prac objętych przedstawionym Kosztorysem. | zatwierdzenie wyceny, zgoda na naprawę | Klient akceptuje kosztorys o wartości 640 zł. | Klient, Kosztorys, Zlecenie naprawy |
| Asystent AI | AIAdvisor | Funkcja wspierająca Mechanika przez przedstawianie możliwych przyczyn Usterki na podstawie opisu Objawów. Nie zastępuje decyzji Mechanika. | konsultant AI, chatbot diagnostyczny | Asystent AI wskazuje możliwe przyczyny trudności z uruchomieniem silnika. | Mechanik, Objaw usterki, Rekomendacja serwisowa, Usterka |
| Część zamienna | SparePart | Element przeznaczony do wymiany lub montażu w Pojeździe podczas Naprawy. | część, podzespół | Filtr oleju wymieniony podczas naprawy. | Naprawa, Pojazd, Zużyta część |
| Diagnoza | Diagnosis | Ustalenie przez Mechanika prawdopodobnej lub potwierdzonej przyczyny Usterki na podstawie objawów i sprawdzenia Pojazdu. | diagnostyka, rozpoznanie problemu | Mechanik ustala, że przyczyną braku rozruchu jest niesprawny akumulator. | Mechanik, Objaw usterki, Usterka, Rekomendacja serwisowa |
| Historia napraw | RepairHistory | Zestaw informacji o wcześniejszych Zleceniach naprawy dotyczących danego Pojazdu. | karta napraw, archiwum serwisowe | W historii pojazdu widnieje wymiana hamulców w maju. | Pojazd, Zlecenie naprawy |
| Kierownik warsztatu | WorkshopManager | Osoba odpowiedzialna za przyjmowanie Zleceń naprawy, przygotowanie Kosztorysów i organizację prac w warsztacie. | doradca serwisowy, recepcjonista | Kierownik przypisuje nowe zlecenie mechanikowi. | Kosztorys, Mechanik, Zlecenie naprawy |
| Klient | Customer | Osoba lub podmiot zlecający warsztatowi wykonanie prac przy Pojeździe i podejmujący decyzję o akceptacji Kosztorysu. | zleceniodawca, kierowca, właściciel auta | Klient indywidualny zleca naprawę hamulców; klient flotowy zleca naprawę samochodu firmowego. | Akceptacja kosztorysu, Pojazd, Zlecenie naprawy |
| Kosztorys | Estimate | Zestawienie planowanych prac, Części zamiennych oraz przewidywanych kosztów Naprawy, przedstawiane Klientowi do akceptacji. | wycena, kalkulacja naprawy | Kosztorys obejmuje wymianę tarcz i klocków za 640 zł. | Akceptacja kosztorysu, Część zamienna, Naprawa, Status kosztorysu |
| Mechanik | Mechanic | Pracownik warsztatu wykonujący Diagnozę i Naprawę Pojazdu oraz zapisujący wykonane prace i Zużyte części. | serwisant, technik | Mechanik zapisuje wymianę filtra oleju w zleceniu. | Diagnoza, Naprawa, Zlecenie naprawy |
| Naprawa | Repair | Prace wykonywane przy Pojeździe w celu usunięcia Usterki lub przywrócenia jego prawidłowego działania. | usługa serwisowa, czynność naprawcza | Wymiana uszkodzonego alternatora. | Część zamienna, Mechanik, Usterka, Zlecenie naprawy |
| Objaw usterki | FaultSymptom | Zauważalna przez Klienta albo Mechanika oznaka nieprawidłowego działania Pojazdu, która pomaga w Diagnozie. | symptom, zgłoszony problem | Samochód nie uruchamia się przy niskiej temperaturze. | Asystent AI, Diagnoza, Usterka |
| Odrzucenie kosztorysu | EstimateRejection | Decyzja Klienta o niewyrażeniu zgody na przedstawiony Kosztorys. Dalsze postępowanie ze Zleceniem naprawy wymaga ustalenia zasad warsztatu. | odmowa wyceny, brak zgody | Klient odrzuca kosztorys wymiany sprzęgła. | Klient, Kosztorys, Status kosztorysu, Zlecenie naprawy |
| Pojazd | Vehicle | Samochód przyjęty do warsztatu w ramach Zlecenia naprawy, identyfikowany danymi umożliwiającymi odróżnienie go od innych pojazdów. | auto, samochód klienta | Samochód osobowy o podanym numerze rejestracyjnym. | Historia napraw, Klient, Zlecenie naprawy |
| Powiadomienie | Notification | Wiadomość skierowana do Klienta w związku z Kosztorysem albo zmianą Statusu zlecenia. Może być przekazana e-mailem lub SMS-em. | alert, komunikat | SMS z informacją, że pojazd jest gotowy do odbioru. | Klient, Kosztorys, Status zlecenia |
| Przypisanie zlecenia | RepairAssignment | Wskazanie Mechanika odpowiedzialnego za wykonanie prac w ramach konkretnego Zlecenia naprawy. | przydzielenie zadania, delegowanie naprawy | Kierownik przypisuje wymianę rozrządu mechanikowi. | Kierownik warsztatu, Mechanik, Zlecenie naprawy |
| Rekomendacja serwisowa | ServiceRecommendation | Propozycja możliwej przyczyny Usterki lub kierunku dalszej Diagnozy przekazana Mechanikowi przez Asystenta AI. Wymaga oceny przez Mechanika. | podpowiedź AI, sugestia naprawy | Rekomendacja sprawdzenia akumulatora i połączeń elektrycznych. | Asystent AI, Diagnoza, Mechanik, Objaw usterki |
| Status kosztorysu | EstimateStatus | Określenie etapu decyzji o Kosztorysie, pozwalające rozróżnić dokument przygotowywany, oczekujący na odpowiedź Klienta, zaakceptowany i odrzucony. | stan wyceny | OCZEKUJE_NA_AKCEPTACJE. | Akceptacja kosztorysu, Kosztorys, Odrzucenie kosztorysu |
| Status zlecenia | RepairOrderStatus | Określenie aktualnego etapu obsługi Zlecenia naprawy, od przyjęcia Pojazdu do zakończenia obsługi. | stan naprawy, etap realizacji | W_TRAKCIE. | Powiadomienie, Zlecenie naprawy |
| Usterka | Fault | Nieprawidłowość w działaniu Pojazdu, która jest przedmiotem Diagnozy i może wymagać Naprawy. | awaria, defekt | Niesprawny alternator powodujący brak ładowania akumulatora. | Diagnoza, Naprawa, Objaw usterki |
| Wykonana praca | CompletedWork | Czynność naprawcza lub diagnostyczna faktycznie wykonana przez Mechanika i odnotowana przy Zleceniu naprawy. | robocizna, wykonana czynność | Wymiana klocków hamulcowych. | Mechanik, Naprawa, Zlecenie naprawy |
| Zlecenie naprawy | RepairOrder | Zapis uzgodnionego z Klientem zakresu obsługi Pojazdu, łączący informacje o zgłoszonej Usterce, Kosztorysie, Mechaniku, przebiegu prac i Statusie zlecenia. | zgłoszenie serwisowe, karta zlecenia | Zlecenie wymiany hamulców w samochodzie klienta. | Klient, Kosztorys, Mechanik, Pojazd, Status zlecenia |
| Zużyta część | UsedPart | Część zamienna rzeczywiście wykorzystana przy realizacji Zlecenia naprawy i zapisana w wykazie wykonanych prac. | rozchodowana część, zamontowany element | Dwa klocki hamulcowe odnotowane przy zleceniu. | Część zamienna, Naprawa, Zlecenie naprawy |

## Wartości wyliczeniowe

### Status zlecenia naprawy

| Wartość | Znaczenie |
|---|---|
| PRZYJETE | Pojazd i zgłoszona Usterka zostały zarejestrowane w warsztacie. |
| WYCENA | Kierownik warsztatu przygotowuje Kosztorys planowanych prac. |
| OCZEKUJE_NA_AKCEPTACJE | Kosztorys przekazano Klientowi i warsztat oczekuje na jego decyzję. |
| W_TRAKCIE | Prace przy Pojeździe są realizowane. |
| GOTOWE_DO_ODBIORU | Prace zakończono, a Pojazd może zostać odebrany. |
| WYDANE | Pojazd został przekazany Klientowi po obsłudze zlecenia. |
| ANULOWANE | Zlecenie zakończono bez wykonania planowanej naprawy. Przyczyny i zasady anulowania wymagają potwierdzenia. |

### Status kosztorysu

| Wartość | Znaczenie |
|---|---|
| ROBOCZY | Kosztorys jest przygotowywany i nie został jeszcze przekazany Klientowi. |
| OCZEKUJE_NA_AKCEPTACJE | Kosztorys przekazano Klientowi, ale nie podjął on jeszcze decyzji. |
| ZAAKCEPTOWANY | Klient wyraził zgodę na przedstawiony Kosztorys. |
| ODRZUCONY | Klient nie wyraził zgody na przedstawiony Kosztorys. |

## Kwestie do potwierdzenia podczas wywiadu z klientem

1. Czy **Klient** obejmuje także firmę zarządzającą flotą, a jeśli tak, kto jest uprawniony do akceptacji Kosztorysu?
2. Czy warsztat dopuszcza częściową akceptację Kosztorysu oraz jego zmianę po rozpoczęciu prac?
3. Jakie są dokładne Statusy zlecenia i dozwolone przejścia między nimi, szczególnie po odrzuceniu Kosztorysu?
4. Jakie dane identyfikujące **Pojazd** będą zapisywane (np. numer rejestracyjny, VIN)?
5. Czy **Powiadomienie** ma być wysyłane SMS-em, e-mailem czy oboma kanałami?
6. Jakie informacje wolno przekazać zewnętrznemu dostawcy Asystenta AI i czy Mechanik ma obowiązek potwierdzić Rekomendację serwisową przed wykonaniem prac?
7. Czy **Kierownik warsztatu** wykonuje także zadania recepcjonisty i czy istnieją inni pracownicy przyjmujący zlecenia?

> **Uwaga dotycząca zakresu:** Słownik obejmuje pojęcia potrzebne do funkcji MVP. Integracja z hurtownią, system magazynowy, płatności online, fakturowanie i kalendarz wizyt pozostają poza MVP zgodnie z `01_wizja_i_zakres.md`. Nie oznacza to, że zewnętrzny dostawca AI lub bramka SMS zostały już wybrane.
