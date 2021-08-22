# Raport CDOS

Acest repository conține un script care poate genera automat grafice (bar charts, pie charts, etc.) pe baza răspunsurilor primite la chestionarul CDOS, realizat de [Asociația Studenților la Matematică și Informatică](https://www.asmi.ro/).

## Configurarea mediului de dezvoltare

Pentru a rula script-ul trebuie să aveți [Python](https://www.python.org/) și [Jupyter](https://jupyter.org/). Pe Windows, ambele se pot instala facil prin pachetul [Anaconda](https://www.anaconda.com/products/individual).

Celelalte pachete necesare se pot instala folosind [pip](https://pip.pypa.io/en/stable/user_guide/) cu fișierul de [`requirements.txt`](requirements.txt):

```sh
python -m pip install -r requirements.txt
```

```sh
jupyter notebook Grafice.ipynb
```

## Datele de intrare

Script-ul se așteaptă să găsească fișierele Excel cu răspunsurile exportate în acest director.

## Datele de ieșire

Graficele generate sunt salvate în directorul `output` și în alte subdirectoare ale acestuia.
