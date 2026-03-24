# pySpark-valst-numeriu-analize
Sintetinių 7,7mln valstybinių numerių analizė naudojant pySpark: duomenų valymas, klasifikavimas su regex, ir top statistika naudojant window funkciją

# Valstybinių numerių analizė su PySpark (7,7 mln. įrašų)
Šiuo projektu norėjau parodyti gebėjimą apdoroti didelius duomenų kiekius naudojant pySpark.

## Technologijos
* PySpark: Duomenų apdorojimas ir Window funkcijos.
* Python (Pandas/Requests): Duomenų surinkimas iš GitHub API.
* Regex: Sudėtingas numerių klasifikavimas pagal Regitros taisykles.
* Google Colab: Vykdymo aplinka.

## Pagrindiniai žingsniai
1. **Duomenų surinkimas**: Siunčiami 3 CSV failai (viso ~7,7 mln. eilučių).
2. **Valymas**: Pašalinta virš 860,000 dublikatų naudojant `dropDuplicates`.
3. **Klasifikacija**: Su `rlike` ir Regex numeriai suskirstyti į kategorijas (EV, diplomatiniai, bendro naudojimo ir kt.).
4. **Analizė**: Naudojant `Window` funkcijas, rastos 5 dažniausiai pasitaikančios pradžios raidės kiekvienoje kategorijoje.

## Rezultatai
Analizė parodė, kad bendro naudojimo numerių grupėje dažniausiai pasitaikančios raidės yra Z, V ir M. 
