###logo 
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


### Ulubione 3 polecenia z linuxa z zajęc 5.10.2019:
```sh
pwd
ls
mkdir
cat
cd
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




#### Polecnia z linuxa: 
1. Tworzenie katalogów:
```bash
mkdir <nazwa katalogu>
```
2. listowanie katalogu:
```bash
ls 
```
3. instalowanie aplikacji
```shell
sudo apt get <nazwa aplikacji>
```
4. przechodzenie po katalogach:
+ ```bash cd <nazwa katalogu> ``` - przejscie do wybranego katalogu 
+ ```bash cd ... ``` - przejscie do katalogu powyzej 
+ ```bash cd - ``` - przejscie do poprzednieg katalogu 

Jak sprawdzić wersję:
```$ git --version```

##UPDATED 06.10