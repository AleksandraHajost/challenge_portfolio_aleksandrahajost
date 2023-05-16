# TASK 1

## Subtask 1

_7 punktów_

## Subtask 3

___Cześć! Nazywam się Ola___ :blush: _i postanowiłam wziąć udział w wyzwaniu z __DareIT__, żeby wkroczyć do świata MATRIXA i ulepszyć go (testami) do poziomu 2.0 gdzie sam Morfeusz nie rozróżni świata realnego od wygenerowanego :nerd_face:.
Chcę, żeby testowanie było moim początkiem kariery w IT. Moim celem jest znalezienie pracy po tym kursie, co przekłada się na oczekiwania związane z tym projektem. Liczę, że nabędę przede wszystkim umiejętności, ale także kontaktów i rozeznania w branży oraz zainteresuje waszych partnerów biznesowych jako ich przyszły pracownik._

_Mój profil na __[LinkedIn](https://www.linkedin.com/in/aleksandra-hajost/)__ jest jeszcze do dopracowania pod kątem przyszłego testera, do tej pory pracowałam nad nim dla swojej marketingowej ścieżki kariery._

## Subtask 4
Strona https://scouts-test.futbolkolektyw.pl/pl dotyczy piłki nożnej, służy do zarządzania graczami, meczami i do tworzenia raportów. 

Strona umożliwia dodawania nowych zawodników, meczy, raportów do nich oraz przeglądanie już istniejących. Dodania meczy i raportów jest bardzo nieintuicyjne, trzeba doszukiwac sie tej funkcjonalności. Funkcjonalnośc "Rozpocznij mecz" w sekcji "Mecze" również jest niejasna w obsłudze, również myląca jest kolejnośc "Akcji" - najpierw "Dodaj raport" a dopiero później "Rozpocznij mecz" - informacje z drugiej sekcji, zawierają się w raporcie więc ikona powinna być jako pierwsza. Do sensu istnienia tej funkcjonalności trzeba dopisać więcej informacji, nie jest to intuicyjne narzędzie.

Interfejs aplikacji wygląda jak szkic. Po wejściu nie wiemy od razu czego dotyczy strona - równie dobrze mogłaby dotyczyć czegokolwiek innego od piłki nożnej. Strona nie zachęca do pozostania na niej, należąłoby dodać oprócz grafik, także grafiki ułatwiające lokalizowanie funkcjonalności (żeby nie trzeba było wszystkiego czytać i się doszukiwać) - np. dodaj gracza - automatycznie kojarzy się z plusem, ewentualnie ikonografika piłkarza. 

Aplikacja jest słabo intuicyjna, powinny zostać dodane w panelu po lewej stronie na niebiesko dostępne dla użytkownika podstrony np. Mecze, Raporty meczów, - ich szukanie jest uciążliwe. Użytkownik po wejściu na strone musi doszukiwać się funkcjonalności, które umożliwia strona, przez co możemy stracić jego zainteresowanie. 

PS. Podczas testowania nie zapomnij z korzystania z poznanych dzisiaj DEVTOOLSÓW 

Znalezione błędy:

1. W panelu "gracze" dodać funkcjonalność o braku duplikacji zawodnika np. kilka razy David Beckham.
2. W panelu "gracze" po kliknięciu "Print" drukuje się tylko Imię i Nazwisko zawodników bez pozostałych informacji z tabeli.
3. W panelu "Edycja gracza" w sekcji "Imie" uniemożliwić wpisywanie znaków np. "*&^%*$", jedynie tekst.
4. W panelu "Edycja gracza" w sekcji "Nazwisko" uniemożliwić wpisywanie znaków np. "&*^%&*^#", jedynie tekst.
5. W panelu "Edycja gracza" w sekcji "Wiek" uniemożliwić wpisywanie liczby równej lub mniejszej od 0 - dodatkowo o ile jest ustalony minimalny wiek zapisu uczestnika do strony np. 6 lat nie powinno być możliwości rejestracji uczestników poniżej tego wieku (przeciez roczne dzieci nie grają w piłkę nożną). Dodatkowo można dodać górną racjonalną granicę wiekową np. 130 lat.
6. W panelu "Edycja gracza" w sekcji "E-mail" uniemożliwić wpisywanie innych treści poza emailem.
8. W panelu "Edycja gracza" w sekcji "90 minut" brak informacji o informacjach do wprowadzenia.
7. W panelu "Edycja gracza" w sekcji "Telefon" uniemożliwić wpisywanie innych treści cyframi (proponuję dodac funklcjonalność z wyborem numerów kierunkowych i ograniczeniami co do długości numerów dla danego państwa - 9 cyfr mają numery polski, a np. 11 cyfr mają numery amerykańskie).
9. W panelu "Edycja gracza" w sekcji "Waga" uniemożliwić wpisywanie liczby mniejszej lub równej 0.
10. W panelu "Edycja gracza" w sekcji "Wzrost" uniemożliwić wpisywanie liczby mniejszej lub równej 0.
11. W panelu "Edycja gracza" w sekcji "Wzrost" ustalić maksytmalną możliwą wartość np. 300.
12. W panelu "Edycja gracza" w sekcji "Data urodzenia" uniemożliwić wpisywanie daty późniejszej niż dzień zapisu (dziś).
13. W panelu "Edycja gracza" w sekcji "Poziom rozgrywek" dodać listę rozwijaną z ustalonymi w piłce nożnej poziomami rozgrywki lub uniemożliwić wpisywanie wartości niepoprawnych np. "4444ProfessionalProfessionalProfessionalProfessionalProfessionalProfessionalProfessionalProfessional".
14. W panelu "Edycja gracza" w sekcji "Główna pozycja" oraz "Pozycja alternatywna" uniemożliwić wpisywanie znaków i liczb tylko ustalony w piłce nożnej pozycje np. Bramkarz, Obrońcy, Pomocnicy, Napastnicy.
15. W panelu "Edycja gracza" w sekcji "Pozycja alternatywna" uniemożliwić wpisywanie tej samej frazy co w "Główna pozycja" lub wyświetlić komunikat.
16. W panelu "Edycja gracza" w sekcji "Osiągnięcia" znajdują się nieuporządkowane informacje np. tylko cyfry bez tekstu - czy taka ma być funkcjonalność czy .
17. W panelu "Edycja gracza" w sekcji "Łączy nas piłka" brak informacji o informacjach do wprowadzenia.
18. Po kliknięciu "Polski" w panelu "gracze" brak tłumaczenia "1-10 of 3096" na "1-10 z 3096".
19. Po kliknięciu "Polski" w panelu "gracze" brak tłumaczenia ikon w prawym górnym rogu "Download CSV "Print", "View columns", "Filter Table" oraz na niebieskim obszarze na górze strony wyszukiwania "Search...".
20. Po kliknięciu na "Strona główna" "DEV TEAM CONTACT" przekierowanie na stronę https://app.slack.com/workspace-signin?redir=%2Fgantry%2Fauth%3Fapp%3Dclient%26lc%3D1682004939%26return_to%3D%252Fclient%252FT3X4CAKNU%252FC3XTEGXB6%26teams%3DTASA2Q716 zamiast na stronę z informacjami kontaktowymi.
21. W panelu "Dodaj gracza" w sekcji "Wiek" można wpisać tekst "e" - zablokowac wpisywanie tekstu.
22. W panelu "Dodaj gracza" w sekcji "Wzrost" można wpisać tekst "e" - zablokowac wpisywanie tekstu.
23. W panelu "Dodaj gracza" w sekcji "Link do YouTube" uniemożliwić wpisywanie innych treści niż adres URL.
24. W panelu "Dodaj gracza" w sekcji "Dodaj język" dodac listę rozwijaną z językami.
25. W panelu "Dodaj gracza" w sekcji "Dodaj język" unimożliwić wpisywanie cyfr, znaków specjalnych.
26. W panelu "Dodawanie meczu" w sekcji "Data" uniemożliwić wpisywanie daty późniejszej niż dzień zapisu (dziś).
27. W panelu "Dodawanie meczu" w sekcji "Kolor koszulki" uniemożliwić wpisywanie cyfr, znaków szczególnych jedynie tekst, ewentualnie dodać listę rozwijaną z ustalonymi wartościami.
28. W panelu "Dodawanie meczu" w sekcji "Czas gry" można wpisać tekst "e" - zablokowac wpisywanie tekstu.
29. W panelu "Dodawanie meczu" w sekcji "Czas gry" dodać informację o jednostce pomiaru "minuty/godziny".
30. W panelu "Dodawanie meczu" w sekcji "Czas gry" uniemożliwić wpisywanie liczby mniejszej lub równej 0.
31. W panelu "Dodawanie meczu" w sekcji "Czas gry" ustawić maksymalną możliwą do wpisania wartość np. 200 min.
32. W panelu "Dodawanie meczu" w sekcji "Numer" sprecyzować co powinno się tam znaleźć "numer czego? buta? autobusu? konta bankowego? zawodnika?".
33. W panelu "Dodawanie meczu" w sekcji "Numer" można wpisać tekst "e" - zablokowac wpisywanie tekstu.
34. W panelu "Dodawanie meczu" w sekcji "Numer" uniemożliwić wpisywanie liczby mniejszej lub równej 0.
35. W panelu "Dodawanie meczu" w sekcji "Web match" uniemożliwić wpisywanie treśli innych niż Adres URL.
36. W panelu "Dodawanie meczu" w sekcji "General" sprecyzować co powinno się tam znaleźć.
37. W panelu "gracze" lepiej wyglądałoby domyślne formatowanie danych bez względu na sposób ich wprowadzenia (np. ustalone od górnie Imie, Nazwisko, Pozycja, Klub z dużej litery reszta małe.
38. Page has no manifest <link> URL
39. Does not register a service worker that controls page and start_url
40. Is not configured for a custom splash screenFailures: No manifest was fetched.
41. Does not set a theme color for the address bar.Failures: No manifest was fetched.
42. Manifest doesn't have a maskable iconNo manifest was fetched
43. Document does not have a meta description
44. Fonts with font-display: optional are preloaded
45. [accesskey] values are unique
46. button, link, and menuitem elements have accessible names
47. ARIA input fields have accessible names
48. ARIA meter elements have accessible names
49. ARIA progressbar elements have accessible names
50. [role]s have all required [aria-*] attributes
51. Elements with an ARIA [role] that require children to contain a specific [role] have all required children.
52. [role]s are contained by their required parent element
53. [role] values are valid
54. ARIA toggle fields have accessible names
55. ARIA tooltip elements have accessible names
56. ARIA treeitem elements have accessible names
57. The page contains a heading, skip link, or landmark region
58. Definition list items are wrapped in dl elements
59. [id] attributes on active, focusable elements are unique
60. ARIA IDs are unique
61. No form fields have multiple labels
62. frame or iframe elements have a title
63. Image elements have [alt] attributes
64. input type="image" elements have [alt] text
65. Form elements have associated labels
66. Lists contain only li elements and script supporting elements (script and template).
67. List items li are contained within ul, ol or menu parent elements
68. The document does not use meta http-equiv="refresh"
69. object elements have alternate text
70. Cells in a <table> element that use the [headers] attribute refer to table cells within the same table.
71. th elements and elements with role="columnheader"/"rowheader" have data cells they describe.
72. [lang] attributes have a valid value
73. video elements contain a <track> element with [kind="captions"]
74. Heading elements are not in a sequentially-descending order - "Ostatnio stworzony gracz" na "Strona główna"
75. Poprawić Performance strony First Contentful Paint 3.9s, Speed Index 6.6s, Largest Contentful Paint 4.0s
# TASK 2

## Subtask 3 Po co piszemy test case’y?

_Test casy piszemy żeby zweryfikować zakres testów aplikacji. Sprawdzić, czy aplikacja działa zarówno tak jak firma chce żeby działała oraz przedewszystkim żeby działała tak jak klinet chce oraz tak jak potrzebuje na miarę swojej sytuacji. Przypadki testowe piszemy także po to aby aplikacja wraz z rozwojem i nowymi wersjami nadal była funkcjonalna i aby było jak najmniej nieprzyjemnych wrażeń użytkownika w zetknięciu się z naszym projektem. Test casy są pisane również w celu testowania aplikacji przez więcej niż 1 i tą samą osobę na przestrzeni czasu bez zbędnego wprowadzenia w projekt._

  # TASK 3

## Subtask 2 & 3
__[Subtask 2 GoogleDrive](https://docs.google.com/spreadsheets/d/1vevT8rdbsilyGd9dm00crWbtseSPT6DUAycOVXLRG3I/edit?usp=sharing)__

__[Subtask 3 GoogleDrive](https://docs.google.com/spreadsheets/d/1fxyQlES0bNrmUB55BCzWNbdy_YNCCjdS9J7DgjFUI3I/edit?usp=sharing)__
  
# TASK 4
## Subtask 3 - Do czego służy ta aplikacja?
1. Do czego służy ta aplikacja? Jaki jest cel tej aplikacji?
2. Kto ma być użytkownikiem końcowym aplikacji?
3. Czy według Ciebie aplikacja jest user friendly? (Przyjazna dla użytkownika- np. wchodzisz do aplikacji i szybko łapiesz do czego służą przyciski. Poczytaj na ten temat w internecie- co to znaczy, że aplikacja jest przyjazna dla użytkownika)
4. Jak byś usprawnił aplikację? Co byś w niej poprawił. Czy masz jakiś pomysł na dodatkową funkcjonalność? (Żeby nie było: nie jest to aplikacja przy której pracuję, takie pytania pojawiają się na rozmowach rekrutacyjnych dlatego dobrze jest to przećwiczyć :D )
5. Jakie dostrzegasz różnice pomiędzy testowaniem aplikacji internetowej, a natywnej?
