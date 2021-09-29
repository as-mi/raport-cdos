# Raport CDOS

Acest repository conține un script care poate genera automat grafice (bar charts, pie charts, etc.) pe baza răspunsurilor primite la chestionarul CDOS, realizat de [Asociația Studenților la Matematică și Informatică](https://www.asmi.ro/).

## Configurarea mediului de dezvoltare

Pentru a rula script-ul trebuie să aveți [Python](https://www.python.org/) și [Jupyter](https://jupyter.org/). Pe Windows, ambele se pot instala facil prin pachetul [Anaconda](https://www.anaconda.com/products/individual).

Celelalte pachete necesare se pot instala folosind [pip](https://pip.pypa.io/en/stable/user_guide/) cu fișierul de [`requirements.txt`](requirements.txt):

```sh
python -m pip install -r requirements.txt
```

De asemenea, trebuie să descărcați și să instalați font-ul [IBM Plex Sans](https://fonts.google.com/specimen/IBM+Plex+Sans?query=plex), care este folosit pentru textul din grafice.

Dacă script-ul nu găsește font-ul nou instalat, încercați [să resetați cache-ul de font-uri al `matplotlib`](https://stackoverflow.com/a/26106170/5723188).

## Generarea graficelor

Notebook-ul cu codul poate fi deschis folosind comanda:

```sh
jupyter notebook Grafice.ipynb
```

Executând fiecare celulă din notebook puteți genera automat toate graficele din raport.

## Datele de intrare

Script-ul se așteaptă să găsească în acest director fișierul Excel `Răspunsuri Licență.xlsx`, cu răspunsurile exportate din formularul pentru licență.

## Datele de ieșire

Graficele generate sunt salvate în directorul `output` și în alte subdirectoare ale acestuia.
