# 00. Zarządzanie Projektem

## Komunikacja i sposób pracy
* **Główny kanał komunikacji:** Serwer Discord (kanał tekstowy i głosowy).
* **Częstotliwość spotkań:** Raz w tygodniu (niedziela wieczór) spotkanie statusowe całego zespołu na Discordzie.
* **Zarządzanie zadaniami:** GitHub Projects (tablica Kanban z kolumnami Todo, In Progress, Done).
* **Repozytorium:** GitHub (włączona ochrona gałęzi `main`, wymagane 1 zatwierdzenie PR przed scaleniem).

## Harmonogram (Kamienie Milowe)
* **M1 (Zajęcia 2):** Zarządzanie, wizja i zakres, słownik, przygotowanie pytań do wywiadu, ochrona gałęzi.
* **M2 (Zajęcia 3):** Wymagania (WF, WNF, US), Reguły Biznesowe, diagram kontekstu C4.
* **M3 (Zajęcia 4):** Procesy biznesowe (BPMN), przypadki użycia (UML), model danych (ERD), architektura, bezpieczeństwo.
* **M4 (Zajęcia 5):** Makiety UX/UI (Figma), audyt całego repozytorium, oddanie ostatecznej dokumentacji.

## Rejestr ryzyk
| ID | Nazwa ryzyka | Prawd. (1-5) | Wpływ (1-5) | PxW | Reakcja |
|---|---|---|---|---|---|
| R1 | Brak zaangażowania członka zespołu | 2 | 5 | 10 | PM przejmuje zadania krytyczne, eskalacja problemu do prowadzącego. |
| R2 | Niezrozumienie specyfiki pracy mechaników | 3 | 4 | 12 | Dokładny wywiad z klientem, opieranie się na słowniku pojęć dziedzinowych. |
| R3 | Błędy w scalaniu kodu (konflikty w Git) | 4 | 3 | 12 | Ścisłe przypisywanie zadań, praca na osobnych gałęziach (branchach), weryfikacja przez QA. |
| R4 | Zbyt duży zakres przyjęty do MVP | 3 | 4 | 12 | Priorytetyzacja MoSCoW, asertywne odrzucenie funkcjonalności pobocznych na rzecz głównych. |
| R5 | Niedostępność zewnętrznego API dla modułu AI | 2 | 4 | 8 | Zaprojektowanie mocka (zaślepki) symulującego odpowiedzi AI na etapie tworzenia makiet i architektury. |

## Dziennik decyzji
* **Wybór platformy repozytorium:** Wybrano GitHuba ze względu na wbudowane mechanizmy Pull Requestów, intuicyjną tablicę Issues oraz darmową ochronę gałęzi dla repozytoriów publicznych.
* **Wybór narzędzia do makiet:** Wybrano Figmę ze względu na możliwości współdzielenia projektu i łatwego udostępniania linku w dokumentacji.