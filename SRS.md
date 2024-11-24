![](zasoby/logo.svg)

# Misja projektu

Naszym celem jest stworzenie otwartej i wspierającej społeczności, która będzie dzielić się wiedzą i doświadczeniami ze świata IT. Wartości takie jak szacunek, współpraca i innowacyjność są dla nas kluczowe, a nasze forum ma na celu zaspokajanie potrzeb naszych użytkowników, oferując im bezpieczną i przyjazną przestrzeń do dyskusji.

# Krótki opis

Celem naszego projektu jest stworzenie forum internetowego, skupiającego się wokół tematu informatyki. Użytkownicy będą mogli prowadzić dyskusje, odpowiadać na pytania, głosować w ankietach i wiele więcej. Posty będą grupowane według tagów, co ułatwi wyszukiwanie. Aplikacja będzie w pełni internetowa. Każdy będzie mógł stworzyć swoje konto, wystarczy połączenie z Internetem.

# Cele biznesowe
* **Reklama marki** - na stronie będzie znajdowało się logo przedsiębiorstwa. Im popularniejsze forum, tym więcej użytkowników zapamięta to logo, co przełoży się na zwiększoną rozpoznawalność marki. Po dwóch latach, liczba zapytań do wyszukiwarki Google odnośnie przedsiębiorstwa powinna wzrosnąć o minimum 300% (można to mierzyć za pomocą Google Trends).
* **Zachęcenie do zatrudnienia się** - wysoka rozpoznawalność marki powinna przełożyć się na zwiększenie liczby otrzymywanych CV od potencjalnych przyszłych pracowników o minimum 50%.
* **Podniesienie kompetencji** - na forum będą działać grupy badawcze i koła naukowe. Przełoży się to na zwiększenie kompetencji specjalistów, co pozwoli oszczędzić 15% kosztów wydawanych do tej pory na szkolenia (wewnątrz firmy).

# Cele klienta
* **Usprawnienie komunikacji** - użytkownicy będą mogli w bardzo prosty sposób wymieniać informacje ze sobą, uzyskiwać cenne wskazówki i porady. Pozwoli to zachęcić użytkowników do studiowania informatyki o minimum 5%.
* **Ułatwienie dostępu do informacji** - dzięki zaawansowanemu silnikowi do wyszukiwania postów na podstawie tagów, użytkownicy oszczędzą średnio 6 minut dziennie podczas korzystania z naszego forum, w porównaniu do Reddita.

# Wymagania funkcjonalne

## Tworzenie nowych kont
### User story
Jako użytkownik z dostępem do Internetu, chcę mieć możliwość utworzenia konta na forum. Zależy mi, aby dane które podam, takie jak np. hasła były bezpiecznie przetwarzane.
### Warunki początkowe
* Użytkownik nie ma konta na naszym forum (tzn. w bazie danych nie ma konta o podanym adresie e-mail).
* Wprowadzone hasło składa się z minimum 8 znaków i co najmniej jednej cyfry.
* Użytkownik zapoznał się z regulaminem RODO i regulaminem forum.
### Warunki końcowe
* System tworzy konto na podstawie wprowadzonych danych. Przetwarzanie informacji powinno być bezpieczne.
* System wysyła wiadomość na wskazany adres mailowy z powitaniem.
* Następuje automatyczne zalogowanie na forum.

## Logowanie
### User story
Jako użytkownik posiadający konto na IT-forum.net, chcę mieć możliwość logowania się.
### Warunki początkowe
* W systemie istnieje konto o wskazanym adresie e-mail.
* Użytkownik nie został zbanowany.
* Użytkownik podał poprawne hasło.
### Warunki końcowe
* Zalogowanie użytkownika do systemu.
* Automatyczne przekierowanie na stronę główną IT-forum.net.

## Dodawanie postów
### User story
Jako zalogowany użytkownik, chcę mieć możliwość dodawania postów na forum. Oczekuję, że po wprowadzeniu wiadomości, post będzie publiczny.
### Warunki początkowe
* Użytkownik jest zalogowany.
* Użytkownik nie przekroczył dziennego limitu utworzonych postów (zabezpieczenie przed spamem).
* Użytkownik wpisał minimum 20 znaków treści posta, wybrał odpowiednie tagi i zatwierdził publikację.
* Post jest zgodny z regulaminem.
### Warunki końcowe
* Post zostaje zapisany do bazy danych.
* Na stronie internetowej, post pojawia się nie później niż minutę po jego dodaniu.

## Dodawanie odpowiedzi do postów
### User story
Jako zalogowany użytkownik, chcę mieć możliwość dodawania odpowiedzi do postów, aby uczestniczyć w dyskusji i dzielić się swoimi opiniami.
### Warunki początkowe
* Użytkownik jest zalogowany.
* Użytkownik nie przekroczył dziennego limitu utworzonych odpowiedzi (zabezpieczenie przed spamem).
* Istnieje post na który można odpowiedzieć.
* Użytkownik uzupełnił treść odpowiedzi i zatwierdził publikację.
### Warunki końcowe
* Nowa odpowiedź zostaje dodana do postu i wyświetlona w sekcji odpowiedzi.
* Odpowiedź jest dostępna dla innych użytkowników do przeglądania nie później niż minutę po dodaniu.


## Przeglądanie postów
### User story
Jako użytkownik, chcę mieć możliwość przeglądania postów opublikowanych na forum.
### Warunki początkowe
* Forum posiada przynajmniej jeden opublikowany post.
* Użytkownik wybiera interesujący go post z dostępnej listy.
### Warunki końcowe
* Następuje przekierowanie użytkownika na stronę postu.
* Wyświetlana jest treść postu, odpowiedzi do niego (jeżeli istnieją) oraz metadane postu takie jak autor, data publikacji czy tagi.


## Wyszukiwanie postów
### User story
Jako użytkownik, chcę mieć możliwość wyszukiwania postów na forum. Zależy mi na tym, aby wyszukiwarka dawała mi opcję do wyszukiwania postów według różnych kryteriów.
### Warunki początkowe
* Forum posiada przynajmniej jeden opublikowany post.
* Użytkownik może wybrać różne kryteria wyszukiwania (np.: wyszukiwanie po tagach, wyszukiwanie po treści posta), domyślnie wyszukiwanie po tytule posta.
* Użytkownik wypełnia pole wyszukiwania.
### Warunki końcowe
* System wyświetla listę wyników odpowiadających zastosowanym kryteriom wyszukiwania.
* Wyniki domyślnie są posortowane według daty.
* Użytkownik ma możliwość przeglądania wybranego postu z listy wyników.

# Atrybuty jakościowe

## Przystępność (accesibility)
Przystępność oznacza tworzenie oprogramowania w taki sposób, aby było ono zdatne do użytku przez jak największą grupę ludzi, w szczególności przez osoby z niepełnosprawnościami.

Ponieważ celem naszego projektu jest zbudowanie platformy do dzielenia się wiedzą i rozwijania swojej pasji z dziedziny informatyki, a więc dziedziny, która jest możliwa do wykonywania bez większych problemów również przez osoby z niepełnosprawnościami, chcemy oferować szereg opcji, które zapewnią że nasza strona będzie przystępna i wygodna do korzystania przez jak największą ilość ludzi.

## Bezpieczeństwo (security)
Bezpieczeństwo to zdolność systemu do zmniejszenia ryzyka złośliwych lub przypadkowych działań poza zaprojektowanymi funkcjonalnościami oprogramowania oraz zapobiegania ujawnieniu lub utracie informacji.

Chcemy, aby dane naszych użytkowników, takie jak hasła i loginy były zabezpieczone przed możliwością wykradnięcia ich. Dodatkowo usprawnienie zabezpieczeń zmniejszy szanse powodzenia ataków, które mogłyby spowolnić lub zatrzymać działalność naszego systemu.

## Skalowalność (scalability)
Skalowalność jest atrybutem, który zakłada, że wraz ze wzrostem aktywności oraz ilości użytkowników naszej aplikacji, nasze oprogramowanie nadal będzie zdolne do sprawnego działania.

Jako iż nasz projekt za zadanie ma oferować platformę do komunikacji między wieloma użytkownikami, których ilość z biegiem czasu będzie wzrastała, powinniśmy zagwarantować możliwość rozbudowy naszego systemu w taki sposób, aby był w stanie przyjąć narastające obciążenia.

## Łatwość w zarządzaniu (manageability)
Łatwość w zarządzaniu określa jak łatwo jest administratorowi zarządzać aplikacją, zazwyczaj poprzez wyodrębnienie przez system wystarczających i użytecznych narzędzi i danych.

Jako forum będziemy musieli moderować treści publikowane przez naszych użytkowników, dlatego musimy zapewnić, aby system zapewniał nam szereg wystarczających informacji i narzędzi, które pozwolą nam stworzyć funkcjonalności zdolne do efektywnego zarządzania użytkownikami.

# Ograniczenia w projekcie
## Technologiczne
* Zabezpieczenie danych użytkowników
* Zaplecze technologiczne do ewentualnej rozbudowy, w celu zapewnienia skalowalności
* Projekt wymaga integracji z bazą danych do przechowywania danych użytkowników, jak i wpisów na forum

## Organizacyjne
* Posiadania stałego zespołu zajmującego się moderacją forum.
* Niewielki zespół deweloperski
* Wymagania funkcjonalne nie adresują wszystkich celów projektowych (np. reklama marki)

## Środowiskowe
* Problemy z przestrzeganiem regulacji dotyczących moderacji treści czy praw autorskich
* Brak kontroli nad zachowaniem użytkowników, potrzeba moderacji treści