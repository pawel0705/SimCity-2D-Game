# SimCity-Project
 Prosta (i niedokończona ;) ) gra bazowana na starej grze SimCity-budowanie i zarządzanie miastem. Gra pisana z użyciem języka C++ oraz multimedialnej biblioteki graficznej SMFL.

# Opis gry

Gra polega na budowaniu i zarządzaniu miastem. Aplikacja posiada graficzny interfejs użytkownika. Celem gracza jest zbudowanie jak największego miasta, zasiedlenie jak największej ilosci ludzi oraz zgromadzenie jak największej ilości pieniędzy.

# Użyte biblioteki

Pisząc aplikację graficzną użyto w tym celu dość prostej i popularnej obiektowej biblioteki graficznej SFML (Simple and Fast Multimedia Library) w wersji 2.5.1. Biblioteka ta jest wieloplatformową biblioteką programistyczną, która ułatwia pisanie programów i gier multimedialnych. Jej popularność wywodzi się stąd, że jest napisana w języku C++ i możebyć wykorzystywana w języku C++, C, platformie .NET, D, Pythonie, Javie i kilku innych mniej znanych językach. Niestety nie ma wsparcia dla podstawowych struktur wejścia-wyjścia takich jak przycisk, text-box itp., które trzeba samemu zaimplementować.

# Algorytmy użyte w grze

Algorytm A* (A-star), jest heurystycznym algorytmem służącym do znajdowania najkrótszej ścieżki w grafie. „Agwiazdka” to algorytm zupełny i optymalny, co znaczy, że zawsze zostanie znalezione najlepsze rozwiązanie o ile istnieje. Algorytm A* działa najlepiej, jeżeli przestrzeń przeszukiwań jest przestrzenią drzewiastą. Algorytm ten został wykorzystany dla samochodów występujących w grze oraz linii wysokiego napięcia. Pojazdy poruszają się po drogach, po najkrótszej znalezionej ścieżce (po specjalnych kafelkach symbolizujących ulicę) pomiędzy budynkami. Przez linie wysokiego napięcia „płynie prąd” od elektrowni do budynków.

Szum Perlina (Perlin noise) nazwany na cześć swojego twórcy Ken’a Perlin’a, który użył go do tworzenia tekstur proceduralnych, dla efektów generowanych komputerowo pod film „Tron”. Natomiast w grze algorytm ten jest wykorzystany do generowania mapy i ukształtowania jej terenu. Szum Perlina można porównywać do generatora liczb pseudolosowych, ale wygląda bardziej naturalnie, gdyż wytwarza naturalne ich sortowane sekwencje. Używając tego sposobu można wyznaczyć pewne poziomy zakresu generowania wykresu, by od danego poziomu przykładowo tworzył się las drzew, a od innego poziomu jeziora tak jak zostało wykorzystane w tej aplikacji.

# Launcher i menu główne

Program, jako że jest aplikacją okienkową, uruchamia się poprzez zainicjowanie działania pliku o rozszerzeniu .exe, lub po prostu skompilowaniu kodu źródłowego.
Po uruchomieniu gry przed użytkownikiem pojawi się launcher aplikacji. Można w nim wybrać jedną z dziesięciu (zaczynając od największej i schodząc w dół) obsługiwanych rozdzielczości monitora oraz przyciskiem „apply” zatwierdzić swój wybór.

Po wyborze rozdzielczości użytkownikowi pokaże się proste menu wyboru dalszego działania. Ten stan obsługuje wejście w nową grę, załadowanie gry, przejście do ustawień, wyjście z gry.

# New Game

Po wybraniu opcji „New Game” (nowa gra). Gracz stanie przed wyborem nazwania swojego miasta (liczba znaków jest ograniczona), wpisaniu seed’u (ciąg cyfr, który zostanie podany do algorytmu generowania szumu Perlina (by stworzyć unikalne ukształtowanie drzew,
wody i kamieni na mapie), oraz wybraniu rozmiaru mapy spośród kilku dostępnych. Po zatwierdzeniu ustawień użytkownik zostanie przeniesiony do stanu rozgrywki.

# Load Game

W stanie ładowania gry, użytkownik może wczytać zapisany stan gry. Do wyboru jest lista przechowująca maksymalnie 10 stanów gry. Zapis można wczytać lub usunąć. Możliwy jest również powrót do głównego menu.

# Options

W stanie opcji, użytkownik może zmienić rozdzielczość gry, wyłączyć muzykę lub zmienić jej głośność oraz ustawić czy gra ma być pokazywana na całym ekranie czy w okienku.

# Stan rozgrywki

Po wejściu do rozgrywki użytkownikowi pokaże się mapa, HUD oraz gazeta powitalna. 

# Opis interfejsu

**File:**

Save – zapisuje mapę i miasto

Load – przechodzi do stanu ładowania gry

Pause – pauzuje rozgrywkę i przechodzi do stanu ustawień (po powrocie gra jest wznawiana)

Menu – powraca do głównego menu

Exit – Wychodzi z gry

**Speed:**

Slow – tempo rozgrywki jest wolne

Normal – tempo rozgrywki jest normalne

Fast – tempo rozgrywki jest szybkie

Uber – tempo rozgrywki jest bardzo szybkie

**View:**

Short – zasięg rysowania mapy jest krótki

Medium – zasięg rysowania mapy jest normalny

Long – zasięg rysowania mapy jest daleki

**Natural:**

Cyclone – na mapie pojawia się tornado

Epidemic – w losowych budynkach pojawia się epidemia

Fire – losowy budynek zostaje podpalony

Meteorite – (niezaimplementowana opcja, zostawiona przyszłościowo)

**Probe:**

Info – pokazuje się tabela z informacjami o mieście

**Daily:**

Newest – pokazuje się najnowsza gazeta

**Opis przycisków budowania obiektów (od lewej do prawej, z góry na dół):**

-budowanie stref mieszkalnych

-budowanie stref fabryki

-budowanie stref komercyjnych

-stawienie elektrowni lub linii wysokiego napięcia (do wyboru)

-stawianie drogi

-kanalizacje (niezaimplementowane)

-burzenie terenu (nie działa na wodę)

-budowanie szpitala

-zmiana podatków

-budowanie straży pożarnej

-budowanie komisariatu policji

-stawienie drzewa lub drzewa z trawą (do wyboru)

-stawienie pomnika

# Screeny z gry

![Image](/images/city1.jpg)

![Image](/images/city2.jpg)

![Image](/images/city3.jpg)

![Image](/images/city4.jpg)

![Image](/images/city5.jpg)

![Image](/images/city6.jpg)

![Image](/images/city7.jpg)
