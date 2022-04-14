GIT - system kontroli wersji. Pozwala na zarządzanie historią kodu źródłowego, umożliwia szybki powrót do dowolnego wcześniej zapisanego stanu projektu.
Branching - tworzenie i edycja kopii istniejącego kodu, by równolegle go modyfikować dla wprowadzenia zmian lub naprawienia bugów, bez ingerencji w główny kod.

Klonowanie i zmiany w repozytorium:
1. Aby sklonować repozytorium potrzebujemy najpierw adresu repozytorium, np: "https://github.com/frastrusiek/second-repo.git".
Należy otworzyć okno poleceń GIT Bash, wejść do folderu, w którym chcemy utworzyć sklonowane repozytorium, prz pomocy
polecenia "cd [adres folderu na komputerze]" następnie użyć polecenia "git clone [skopiowany wcześniej adres repozytorium]".
2. Aby zapisać jakiekolwiek zmiany do naszego repozytorium musimy przejść dwuetapowy proces. 
Najpierw za pomocą polecenia "git add [nazwy plików]" dodajemy pliki, które finalnie chcemy zapisać. 
Do samego zapisania plików w repozytorium służy polecenie commit, składa się ono z dwóch elementów: surowej treści polecenia
oraz dodanego przez nas komentarza, który opisuje, co w danym commicie dodaliśmy, np. "updated README.md file".
Polecenie wygląda następująco: " git commit -m "updated REAMDE.md file" ", zapisuje ono pliki dodane do "kolejki zapisywania"
przy pomocy wcześniejszego polecenia add.
3. Gdy zmiany zostały zapisane do naszego lokalnego repozytorium na komputerze, możemy zapisać te zmiany w repozytorium zdalnym.
Robimy to przy pomocy dwóch poleceń: remote add origin oraz push. Pierwsze informuje, gdzie nasze zmiany mają zostać zapisane,
używamy go w następujący sposób: "git remote add origin [skopiowany wcześniej adres repozytorium]", w miejsce adresu
wstawiamy nasz adres repozytorium, dokładnie ten sam, którgo używaliśmy w poleceniu clone (w naszym przypadku było to 
https://github.com/frastrusiek/second-repo.git). Gdy poinformowaliśmy GIT-a gdzie chcemy zapisać nasze pliki, pora na push.
Polecenie push działa w następujący sposób: wpisujemy "git push -u origin master" (master to nazwa brancha któego chcemy 
wpushować do zdalengo repozytorium, możemy tam wpisać nazwę dowolnego brancha) i zatwierdzamy, pojawi nam się okienko,
w które należy wpisać nasz wcześniej nadany Nick oraz hasło, po wprowadzeniu danych powinien pojawić się komunikat
opowiedzeniu się procesu, w ten sposób zapisaliśmy zmiany w naszym lokalnym repozytorium do naszego zdalnego repozytorium,
teraz możemy znaleźć nasze pliki na przykład na GITHubie na naszym koncie, pod powyższym skopiowanym adresem.
