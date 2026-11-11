# 02. Słownik pojęć dziedziny

**System:** System zarządzania zleceniami napraw z modułem inteligentnych rekomendacji serwisowych (AI) dla niezależnego warsztatu samochodowego.

Słownik określa nazwy używane w całej dokumentacji projektu. Synonimy służą jedynie do rozpoznawania innych określeń; w wymaganiach, diagramach i makietach należy używać nazw z pierwszej kolumny. Definicje oraz statusy wymagają potwierdzenia podczas wywiadu z klientem.

## Pojęcia dziedzinowe

| Pojęcie | Nazwa ang. (dla kodu) | Definicja | Synonimy (niezalecane) | Przykład | Powiązane pojęcia |
|---|---|---|---|---|---|
| Akceptacja kosztorysu | EstimateApproval | Decyzja Klienta wyrażająca zgodę na wykonanie prac i poniesienie kosztów wskazanych w Kosztorysie. | zatwierdzenie wyceny, zgoda na naprawę | Klient akceptuje kosztorys na 640 zł. | Klient, Kosztorys, Zlecenie naprawy |
| Asystent AI | AIAdvisor | Narzędzie przedstawiające Mechanikowi możliwe przyczyny Usterki na podstawie opisu Objawu usterki. Podpowiedź nie zastępuje Diagnozy Mechanika. | konsultant AI, chatbot diagnostyczny | Asystent AI sugeruje sprawdzenie akumulatora. | Diagnoza, Mechanik, Objaw usterki, Rekomendacja serwisowa |
| Część zamienna | SparePart | Element, który może zostać użyty do naprawy Pojazdu. W systemie może występować w Kosztorysie lub w zapisie Zużytej części. | część, podzespół | Filtr oleju. | Kosztorys, Pojazd, Zużyta część |
| Diagnoza | Diagnosis | Ustalenie przez Mechanika przyczyny Usterki na podstawie objawów i sprawdzenia Pojazdu. | diagnostyka, rozpoznanie usterki | Mechanik ustala, że przyczyną braku rozruchu jest akumulator. | Mechanik, Objaw usterki, Usterka |
| Historia napraw | RepairHistory | Zestaw informacji o wcześniejszych Zleceniach naprawy danego Pojazdu. | archiwum napraw, karta napraw | Lista poprzednich wymian hamulców w samochodzie. | Pojazd, Zlecenie naprawy |
| Kierownik warsztatu | WorkshopManager | Pracownik organizujący obsługę Zleceń naprawy, przygotowanie Kosztorysów i przydzielanie pracy Mechanikom. | recepcjonista, doradca serwisowy | Kierownik przydziela zlecenie mechanikowi. | Kosztorys, Mechanik, Przypisanie zlecenia |
| Klient | Customer | Osoba lub firma zlecająca obsługę Pojazdu i uprawniona do podjęcia decyzji o Kosztorysie. | zleceniodawca, właściciel auta | Klient indywidualny lub firma posiadająca flotę. | Akceptacja kosztorysu, Pojazd, Zlecenie naprawy |
| Kosztorys | Estimate | Zestawienie planowanych prac, Części zamiennych i przewidywanych kosztów Naprawy przedstawiane Klientowi do decyzji. | wycena, oferta naprawy | Wymiana klocków i tarcz hamulcowych za 640 zł. | Klient, Pozycja kosztorysu, Status kosztorysu |
| Mechanik | Mechanic | Pracownik wykonujący Diagnozę i Naprawę oraz zapisujący Wykonane prace i Zużyte części. | serwisant, technik | Mechanik wymienia rozrusznik. | Diagnoza, Naprawa, Zlecenie naprawy |
| Naprawa | Repair | Prace prowadzone przy Pojeździe w celu usunięcia Usterki lub przywrócenia prawidłowego działania. | usługa naprawcza | Wymiana uszkodzonego alternatora. | Mechanik, Usterka, Zlecenie naprawy |
| Objaw usterki | FaultSymptom | Zauważalna przez Klienta lub Mechanika oznaka nieprawidłowego działania Pojazdu. | symptom, zgłoszony problem | Stuki w zawieszeniu podczas jazdy. | Asystent AI, Diagnoza, Usterka |
| Odrzucenie kosztorysu | EstimateRejection | Decyzja Klienta oznaczająca brak zgody na przedstawiony Kosztorys. Nie oznacza automatycznie anulowania całego Zlecenia naprawy. | odmowa wyceny, brak zgody | Klient nie zgadza się na wymianę sprzęgła za wskazaną kwotę. | Klient, Kosztorys, Status kosztorysu |
| Pojazd | Vehicle | Samochód, którego dotyczy Zlecenie naprawy. Jego dane pozwalają odróżnić go od innych samochodów obsługiwanych przez warsztat. | auto, karta pojazdu | Samochód o numerze rejestracyjnym WA 12345. | Historia napraw, Klient, Zlecenie naprawy |
| Powiadomienie | Notification | Wiadomość do Klienta dotycząca Kosztorysu lub postępu Zlecenia naprawy. | komunikat, alert | E-mail z informacją o gotowości auta do odbioru. | Klient, Kosztorys, Status zlecenia |
| Pozycja kosztorysu | EstimateItem | Pojedyncza pozycja Kosztorysu określająca planowaną pracę albo Część zamienną wraz z przewidywanym kosztem. | element wyceny, pozycja wyceny | Wymiana filtra oleju: robocizna 80 zł. | Część zamienna, Kosztorys, Robocizna |
| Przypisanie zlecenia | RepairAssignment | Wskazanie Mechanika odpowiedzialnego za prace w ramach Zlecenia naprawy. | przydzielenie zadania | Kierownik przydziela mechanikowi naprawę hamulców. | Kierownik warsztatu, Mechanik, Zlecenie naprawy |
| Rekomendacja serwisowa | ServiceRecommendation | Propozycja możliwej przyczyny Usterki lub dalszego sprawdzenia Pojazdu przedstawiona przez Asystenta AI. Ostatecznej oceny dokonuje Mechanik. | podpowiedź AI, sugestia diagnostyczna | Sprawdzenie napięcia akumulatora. | Asystent AI, Diagnoza, Mechanik |
| Robocizna | LaborCost | Przewidywany koszt pracy Mechanika potrzebnej do wykonania czynności przy Pojeździe, wykazywany w Kosztorysie. | koszt pracy, RBG | Robocizna przy wymianie klocków: 120 zł. | Kosztorys, Pozycja kosztorysu |
| Status kosztorysu | EstimateStatus | Informacja, czy Kosztorys jest przygotowywany, oczekuje na decyzję Klienta, został zaakceptowany czy odrzucony. | stan wyceny | ZAAKCEPTOWANY. | Kosztorys, Akceptacja kosztorysu, Odrzucenie kosztorysu |
| Status zlecenia | RepairOrderStatus | Informacja o aktualnym etapie obsługi Zlecenia naprawy. | stan naprawy, etap zlecenia | W_TRAKCIE. | Zlecenie naprawy, Powiadomienie |
| Usterka | Fault | Nieprawidłowość w działaniu Pojazdu, która wymaga Diagnozy i może wymagać Naprawy. | awaria, defekt | Uszkodzony alternator. | Diagnoza, Naprawa, Objaw usterki |
| Wykonana praca | CompletedWork | Czynność diagnostyczna lub naprawcza faktycznie wykonana przez Mechanika i odnotowana w Zleceniu naprawy. | wykonana usługa, wykonana czynność | Wymiana tarcz hamulcowych. | Mechanik, Naprawa, Zlecenie naprawy |
| Zlecenie naprawy | RepairOrder | Zapis obsługi danego Pojazdu obejmujący zgłoszony problem, Kosztorys, przypisane prace i aktualny Status zlecenia. | karta zlecenia, zgłoszenie naprawy | Zlecenie usunięcia usterki hamulców. | Klient, Kosztorys, Mechanik, Pojazd |
| Zużyta część | UsedPart | Część zamienna rzeczywiście wykorzystana podczas Naprawy i zapisana przy Zleceniu naprawy. Nie oznacza prowadzenia pełnego magazynu części. | zamontowana część | Filtr oleju wykorzystany podczas przeglądu. | Część zamienna, Naprawa, Zlecenie naprawy |

## Wartości wyliczeniowe

Poniższe statusy są **propozycją do potwierdzenia z klientem**. Wymagania i diagramy powinny używać dokładnie tych samych nazw po ich uzgodnieniu.

### Status zlecenia naprawy

| Wartość | Znaczenie |
|---|---|
| PRZYJETE | Pojazd i zgłoszony problem zostały zarejestrowane. |
| W_DIAGNOZIE | Mechanik sprawdza przyczynę zgłoszonego problemu. |
| WYCENA | Kierownik przygotowuje Kosztorys. |
| OCZEKUJE_NA_AKCEPTACJE | Kosztorys został przekazany Klientowi. |
| W_TRAKCIE | Trwają zaakceptowane prace naprawcze. |
| GOTOWE_DO_ODBIORU | Naprawa została zakończona i Pojazd może zostać odebrany. |
| WYDANE | Pojazd został wydany Klientowi. |
| ANULOWANE | Obsługę Zlecenia naprawy zakończono bez realizacji zaplanowanej Naprawy. |

### Status kosztorysu

| Wartość | Znaczenie |
|---|---|
| ROBOCZY | Kosztorys jest przygotowywany. |
| OCZEKUJE_NA_AKCEPTACJE | Kosztorys wysłano Klientowi i czeka na decyzję. |
| ZAAKCEPTOWANY | Klient zaakceptował Kosztorys. |
| ODRZUCONY | Klient odrzucił Kosztorys. |

## Do potwierdzenia z klientem

1. Czy Klient może być firmą flotową i kto wtedy akceptuje Kosztorys?
2. Co ma się stać ze Zleceniem naprawy po odrzuceniu Kosztorysu? Czy możliwa jest nowa wycena?
3. Czy potrzebne są wszystkie proponowane Statusy zlecenia, w tym `W_DIAGNOZIE` i `WYCENA`?
4. Jakie dane Pojazdu są konieczne (np. numer rejestracyjny, VIN, marka i model)?
5. Czy Powiadomienia mają być wysyłane e-mailem, SMS-em czy oboma sposobami?
6. Jakie dane wolno wysyłać do zewnętrznego Asystenta AI i kto odpowiada za weryfikację rekomendacji?
7. Czy kierownik zarządza stanowiskami naprawczymi? Na razie nie ma takiej funkcji w potwierdzonym MVP.
8. Czy Robocizna jest liczona według roboczogodzin, stawki za usługę czy w inny sposób?

**Granice MVP:** Słownik nie zakłada pełnej gospodarki magazynowej, automatycznych zamówień u hurtowni, płatności online ani fakturowania. „Zużyta część” oznacza wyłącznie odnotowanie części wykorzystanej w naprawie. Integracja z katalogiem hurtowni i zarządzanie stanowiskami mogą zostać rozważone później, jeżeli klient potwierdzi taką potrzebę.
