> ~~# project-7~~
> ~~## Objectives~~
> ~~- Managing every stage of my own project.~~
> ~~- Creating my own system from scratch.~~
> ~~- Creating application using my system.~~
> ~~- Bilingual documentation and application.~~
# projekt-7
## Cele
- Tworzenie własnego systemu od zera.
  - Stworzyć system zarządzania zasobami.
- Zarządzanie własnym projektem od początku do końca.
  - Stworzyć portfolio.
- Tworzenie aplikacji używając własnego w/w systemu.

~~- Dokumentacja i aplikacja dwujęzyczna.~~

### Aplikacja - luźny projekt.
- Logowanie do systemu.
  > Użytkownicy systemu mają dostęp do aplikacji, ale nie mogą tworzyć swoich kont.
  - Tworzenie nowych użytkowników wyłącznie za pośrednictwem konta administratora / właściciela / mnie.
    > Zarządzanie istniejącymi użytkownikami - j.w.
  - Tworzenie struktury organizacyjnej.
    > Tworzenie hierarchii kont użytkowników, w celu, m.in zarządzania dostępem do zasobów, np. użytkownik może jedynie widzieć zasoby konta użytkownika nadrzędnego (materiały dydaktyczne, zasoby projektów itp.).
- Korzystanie z systemu - czyli jakie funkcje będzie miała aplikacja.
  > Jak system będzie wykonywał swoje operacje - próba stworzenia programu zorientowanego obiektowo, wykorzystanie wzorców projektowych i własnej analizy. 
  - Aplikacja prowadzi rejestr - historię wszystkich czynności wykonywanych w systemie.
    > Obiekty odpowiedzialne za logowanie wydarzeń w rejestrze - instancje klas, których metody: łączą się z bazą danych, umieszczają odpowiednie rekordy w tabeli rejestr, zamykają połączenie.
    > Rejestr jest na bieżąco aktualizowany. Nie mam jeszcze spójnej koncepcji, jedynie wstępną implementację.
    > Wpisy rejestru jako źródło statystyk konta użytkownika.
  - Aplikacja umożliwia komunikację między użytkownikami.
    > Konto użytkownika posiada prywatny obiekt zawierający historię konwersacji, umożliwiający ponadto komunikację z użytkownikami w systemie. Historia konwersacji jest prywatna - jawna tylko między użytkownikami odbiorcy i nadawcy, zapisywana przez obiekt klasy pokrewnej klasie prowadzącej rejestr (albo odwrotnie, albo dziedzicząca, tego jeszcze nie wiem). Wiadomości same w sobie będą obiektami, tworzonymi wewnątrz obiektu zawierającego historię konwersacji, istniejącymi wyłącznie w zakresie tego obiektu.
  - Aplikacja umożliwia zarządzanie dokumentacją, archiwizację plików i pomaga w tworzeniu spójnych zasobów.
    > To jest moja urojona koncepcja, snucie fantazji o możliwościach tego systemu. Problem polega na tym, że mam naprawdę ogromną liczbę plików, różnych. I od jakiegoś czasu moim celem jest znalezienie jak najlepszej metody na ogarnięcie tego bałaganu. Nie wiem jeszcze w jaki sposób, ale będę próbował do momentu aż znajdę ten jeden właściwy. No i oczywiście zrealizuję go w ramach tego projektu. A przynajmniej mam taką nadzieję.
  - Aplikacja umożliwi pracę z kalendarzem.
    > Kalendarz systemu będzie napisany niemalże od zera. Chodzi przede wszystkim o to, by wszystko było spójne wewnątrz systemu, wynikało z jasno wykonanych wyliczeń i nie było wykonane nieudolnie (tak jak ma to miejsce w implementacjach z którymi miałem do czynienia, przy okazji pracy z systemami HR w korporacji, o Excelu nie wspominając bo to jakiś żart). Mam w głowie pewną koncepcję, której szczegóły zostawię dla siebie, bo jednak spędziłem nad tym zdecydowanie zbyt dużo godzin.
  - Aplikacja umożliwi budowę grafików.
    > Tutaj możliwości jest o wiele więcej niż się na pierwszy rzut oka wydaje. Oto moja koncepcja: grafik będzie składał się z zadań, natomiast te będą obiektami kalendarza, klasy dziedziczącej (prawdopodobnie).
  - Aplikacja umożliwi planowanie czasu pracy.
    > Planowanie zadań, ich realizacja i coś, co nazywam "reality check", czyli porównywanie planu i realizacji, wyciąganie odpowiednich wniosków z pomocą algorytmów i wprowadzanie odpowiednich poprawek na podstawie obliczeń.
 
### System - stan obecny.
- Kilka implementacji - luźno i niedbale w kilku różnych nieudokumentowanych projektach.
  - Logowanie do strony - projekt stoły, strona 9, projekt SAJ, biblioteka.
    - SQL - Tworzenie tabel, dodawanie rekordów.
    - PHP - Tworzenie połączenia z bazą danych. Tworzenie zapytań SQL jako kodu PHP wykonywanego przez obiekt połączenia z bazą - mysqli. Obsługa formularza.
    - HTML - Tworzenie formularza logowania. Tworzenie wyglądu i struktury strony.
    - CSS - Wygląd elementów.
  - Dodawanie rekordów do bazy danych z pól formularza na stronie internetowej.
  - Wyświetlanie zawartości z bazy danych na stronie internetowej.
