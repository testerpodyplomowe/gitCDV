![alt text](https://cdv.pl/wp-content/uploads/2018/02/logo.svg "Logo CDV")

### Python webdriver command

```Python
from selenium import webdriver
from selenium.webdriver.common.keys import Keys

driver = webdriver.Firefox()
driver.get("http://www.python.org")
assert "Python" in driver.title
elem = driver.find_element_by_name("q")
elem.clear()
elem.send_keys("pycon")
elem.send_keys(Keys.RETURN)
assert "No results found." not in driver.page_source
driver.close()
```



# Konfiguracja środowiska 

### Instalacja GITA dla UBUNTU LINUX
```sh
sudo apt install git
```

### Polecenia Git'a:
```git
git status
git add .
git log --oneline
git commit -a -m "zmiany"
```

### Ulubione 6 polecenia z linuxa z zajęc 5.10.2019:
```sh
pwd
ls
ls --all
mkdir
cat
cd
```

### Ulubione 5 poleceń z linuxa z zajęc 5.10.2019 AGNIESZKI:
```sudo apt install [installing stuff]
touch [creating a file]
clear [cleaning the console]
rmdir [remove directory]
```

### Fragmenty kodu w Pythonie z 5.10.2019:
```python
s = "Python syntax highlighting"
print s
```



Przykład tabeli:

| Fun                  | With                 | Tables          |
| :------------------- | -------------------: |:---------------:|
| left-aligned column  | right-aligned column | centered column |
| $100                 | $100                 | $100            |
| $10                  | $10                  | $10             |
| $1                   | $1                   | $1              |


### Linux
*Aby wyjść z interpretatora, wcisamy **CTRL** lub uruchamiamy funkcje **quit()**


Polecenia związane z użytkownikami, grupami, loginami i zamykaniem systemu
```newgrp (dodajemy nową grupę)
passwd (zmieniamy hasła)
logout (wylogowanie się)
who (sprawdzamy kto jest aktualnie zalogowany)
users (j/w)
whoami (sprawdzamy kim jesteśmy)
mesg (zezwolenie na przyjmowania komunikatów)
write (wysłanie wiadomości do danego użytkownika)
wall (j/w tylko do wszystkich użytkowników)
rwall (j/w tylko do wszystkich w sieci)
ruser (wyświetla użytkowników pracujących w systemie)
talk (możliwość interaktywnej rozmowy)
su (zmieniamy się w innego użytkownika)
chmod (zmieniamy parametry pliku)
chgrp (zmieniamy jaka grupa jest właścicielem pliku) 
```


### Python z 5.10.2019:
```python
s = "Python is not a snake"
print s
```

```python
s = "Java is not an island"
print s
```

```python
s = "Ruby is not a jewel"
print s
```

```Python

def fib_iter1(n):  # definicja funkcji
    """
        Funkcja drukuje kolejne wyrazy ciągu Fibonacciego
        aż do wyrazu n-tego, który zwraca.
        Wersja iteracyjna z pętlą while.
    """
    pwyrazy = (0, 1)  # dwa pierwsze wyrazy ciągu zapisane w tupli
    a, b = pwyrazy  # przypisanie wielokrotne, rozpakowanie tupli
    print(a, end=" ")
    while n > 1:
        print (b, end=" ")
        a, b = b, a + b  # przypisanie wielokrotne
        n -= 1


def fib_iter2(n):
    """
        Funkcja drukuje kolejne wyrazy ciągu Fibonacciego
        aż do wyrazu n-tego, który zwraca.
        Wersja iteracyjna z pętlą for.
    """
    a, b = 0, 1
    print("wyraz", 1, a)
    print("wyraz", 2, b)
    for i in range(1, n - 1):
        # wynik = a + b
        a, b = b, a + b
        print("wyraz", i + 2, b)

    print()  # wiersz odstępu
    return b


def fib_rek(n):
    """
        Funkcja zwraca n-ty wyraz ciągu Fibonacciego.
        Wersja rekurencyjna.
    """
    if n < 1:
        return 0
    if n < 2:
        return 1
    return fib_rek(n - 1) + fib_rek(n - 2)


def main(args):
    n = int(input("Podaj nr wyrazu: "))
    fib_iter1(n)
    print()
    print("=" * 40)
    fib_iter2(n)
    print("=" * 40)
    print(fib_rek(n - 1))
    return 0


if __name__ == '__main__':
    import sys
    sys.exit(main(sys.argv))
``` 



[Click to get GIT an GITHUB CHEATSHEET](https://github.github.com/training-kit/downloads/github-git-cheat-sheet.pdf)

Jak sprawdzić wersję:
```$ git --version```

[Link do maszyny wirtualnej dla studentów tester CDV](https://drive.google.com/drive/folders/1N-e3ZdpwvghxOLhC9_4ED9KxRK2YNL9e)


##UPDATED 06.10
