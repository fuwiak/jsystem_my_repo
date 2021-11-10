# jsystem_my_repo

Zrodlo danych 




## Plan na piatek

https://paper.dropbox.com/doc/Plan-na-piatek--BV6GT1EMaCMKZ6pU9abH229ZAg-BqbYnti3BhVeoajTa2BGI






#praca domowa link

https://paper.dropbox.com/doc/praca-domowa--BV3PdApRQ9~KjooclOBVK_8PAg-NCrQbXBZwxsS2qcFGY2jX

LINKI:
https://colab.research.google.com/drive/1Hft8V1vN3QtSg4oSKG7iYkgRxVVA1MKq#scrollTo=1Y1TxclQC1m-





Ujęte tematy:
- czytanie różnych formatów danych(csv, excel, json).
- operacje arytmetyczne na kolumnach, statystyki opisowe kolumns.
- filtrowanie danych.
- merge, join itd
- Numpy, Scipy
- wykresy i wizualizacje.
- praca z szeregami czasowymi
- praca z tekstem
- testy statystyczne
- Machine Learning(regresja liniowa, klasyfikacja, redukcja wymiarów, klasteryzacja)


## Pandas
- Turorial pandas https://pandas.pydata.org/docs/user_guide/merging.html

- dane do uzycia dla joina https://github.com/realpython/materials/tree/master/introduction-combining-data-pandas-merge-join-and-concat

Krótkie porównanie merge, join i concat.
Metody merge i join DataFrame (a nie Series) oraz funkcja concat zapewniają bardzo podobną funkcjonalność do łączenia wielu obiektów pandas razem. Ponieważ są one tak podobne i mogą się powielać w pewnych sytuacjach, może to być bardzo mylące, kiedy i jak używać ich poprawnie. Aby pomóc wyjaśnić różnice, spójrz na porównanie:

**concat**
- funkcja bezposrednio z pandass(nie DataFrame)
- Łączy dwa lub więcej obiektów typu pandas w pionie lub poziomie.
- dopasowanie obiektow wg indeksow.
- rzuca wyjątkiem, jeśli w łączonych obiektach mamy tą samą wartośc indeksu.
- domyślne używa outer join


**join**
- Metoda DataFrame
- Łączy horyzontalnie dwa lub więcej obiektów pandas
- Wyrównuje kolumnę(y) lub indeks wywołującej DataFrame z indeksem innych obiektów (a nie kolumn)
- Obsługuje zduplikowane wartości na łączonych kolumnach/indeksach poprzez wykonanie iloczynu kartezjańskiego
- Domyślnie left join z opcjami dla inner, outer i right

**merge**
- Metoda DataFrame
- Łączy dokładnie dwie DataFrame w poziomie
- Wyrównuje kolumnę(y)/indeks wywołującej DataFrame z kolumną(ami)/indeksem drugiej DataFrame
- Obsługuje zduplikowane wartości na łączących się kolumnach/indeksach poprzez wykonanie iloczynu kartezjańskiego
- Domyślnie inner join, z opcją na left, outer i right

# zadane pytania
- Kazdy przypadek braku danych w kolumnach i dataframe https://datatofish.com/check-nan-pandas-dataframe/
- kilka separatow podczas wczytywnia pliku
```{python}
pd.read_csv(filename,sep="\s+|;|:")
```
- formatowanie warunkowe w pandas(funkcja style) https://www.datasciencelearner.com/styling-pandas-dataframe-like-a-master/
