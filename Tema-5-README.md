# Tema 5 Vizualizarea datelor

## Pentru început, descarcă fișierul cu statisticile campaniilor publicitare de pe Facebook pe calculatorul tău: [facebook_ads_data.csv](https://github.com/user-attachments/files/16750900/facebook_ads_data.csv)

##Într-un notebook nou, încarcă acest fișier într-un DataFrame Pandas și realizează următoarele vizualizări:

1. Grupează datele după zile și creează două grafice pentru datele grupate:

- Un grafic cu suma totală a cheltuielilor publicitare în anul 2021;
- Un grafic cu ROMI-ul zilnic în anul 2021.
> [!TIP]
> Poți compara și filtra datele chiar și fără a converti valorile câmpurilor. De exemplu, încearcă să compari valoarea "ad_date" cu textul '2022-01-01'.

> [!NOTE]
> Sarcină bonus
> Aplică metoda rolling() pentru a afișa o medie mobilă a cheltuielilor și a ROMI-ului.

2. Grupează datele după numele campaniei și creează două grafice:

- Un grafic cu suma totală a cheltuielilor publicitare pentru fiecare campanie;
- Un grafic cu ROMI-ul total pentru fiecare campanie.
  
3. Utilizând un box plot, determină distribuția ROMI-ului zilnic în fiecare campanie (după numele campaniei).

4. Creează o histogramă cu distribuția valorilor ROMI din tabelul facebook_ads_data.csv.

5. Creează un heat map a corelației între toți indicatorii numerici din tabelul facebook_ads_data.csv. Care indicatori au cea mai mare și cea mai mică corelație? Cu ce corelează “total_value”?

6. Creează un grafic cu puncte cu regresie liniară (poți folosi funcția lmplot()), pe baza datelor din “total_spend” și “total_value” pentru a vizualiza relația dintre aceste variabile.


