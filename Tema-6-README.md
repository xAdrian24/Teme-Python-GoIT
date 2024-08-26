# Tema 6  Curățarea datelor cu Pandas
## Sarcini:
Trebuie să lucrezi cu două fișiere:

[applications.csv](https://github.com/user-attachments/files/16750922/applications.csv) <br>
[industries.csv](https://github.com/user-attachments/files/16750924/industries.csv)

1. Încarcă tabelul din fișierul applications.csv într-un DataFrame Pandas pe laptop și curăță datele:
- Elimină duplicatele din coloana applicant_id;
- În câmpul ```External Rating ```, completează valorile lipsă cu zero
- În câmpul ``` Education level ```, completează valorile lipsă cu textul "Average".
2. Adaugă datele din fișierul industries.csv în acest DataFrame, respectiv, evaluările industriilor.
3. Calculează evaluarea cererii conform următoarelor condiții:
- Evaluarea trebuie să fie un număr între 0 și 100;
- Evaluarea este suma scorurilor pentru cele 6 criterii;
- Evaluarea este zero dacă nu există valoarea ```Amount``` sau dacă ```External Rating``` este zero.
  
### Din ce constă evaluarea:

- Dacă vârsta aplicantului este între 35 și 55 de ani, se adaugă 20 de puncte la evaluare.
- Dacă aplicația a fost depusă în weekend, se adaugă 20 de puncte la evaluare.
- Dacă aplicantul este căsătorit, se adaugă 20 de puncte la evaluare.
- Dacă aplicantul este localizat în Kyiv sau în regiune, se adaugă 10 puncte la evaluare.
- Valoarea ```Score``` din tabelul industries.csv este de asemenea adăugată la cerere (și variază între 0 și 20 de puncte).
- Dacă ```External Rating``` este mai mare sau egal cu 7, se adaugă 20 de puncte la evaluare.
- Dacă ```External Rating``` este mai mic sau egal cu 2, se scad 20 de puncte din evaluare.
  
> [!TIP] 
> Poți înmulți array-uri booleane cu numere întregi și obține array-uri de numere întregi. De exemplu, pe tabelul tău "df", rulează următoarea comandă și vei obține un tablou de numere întregi în care fiecare element are valoarea 0 sau 20. (df['Age'] >= 35) * 20 Și apoi poți aduna aceste array-uri împreună și să salvezi rezultatul ca o coloană nouă în DataFrame.

4. În tabelul rezultat, lasă doar cererile cu o evaluare mai mare decât zero, aceste cereri vor fi considerate acceptate.
5. Grupează datele din tabelul rezultat în funcție de săptămâna depunerii cererii și afișează evaluarea medie a cererilor acceptate în fiecare săptămână pe grafic.
