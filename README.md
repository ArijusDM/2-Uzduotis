v.pradinė commit f4b0c38 - Pradinio kodo sukūrimas, kodas paimtas iš paskaitos darbo ir truputį bandymas patobulinti, kad įvedimas neveiktų "bug'ovai" .
v.pradinė commit f675ff5 - Pridedamas galutinio balo medianos apskaičiavimas.
v.pradinė commit 540a23b - Padaroma, kad galima pasirinkti lentelės atsakymus: matyti tik galutinio balo vidurkį, tik medianą arba vidurkį ir medianą. 
v.pradinė commit c4dcba7 - Pridedamas variantas, kad galima įrašyti namų darbų pažymius nežinant, kiek yra namų darbų. T.y. pažymių rašai, kiek nori, ir kai nusprendi, kad užtenka, įrašai 0, kad nutraukti pažymių įrašymą. Taip pat bandoma toliau tvarkyti įvedimus, kad jie neveiktų "bug'ovai".
v.pradinė commit 469dab3 - Pridedama funkcija, kad namų darbų ir egzamino rezultatai būtų generuojami atsitiktinai.
v.pradinė commit 5ab2768 - Pridedamas variantas, kad duomenis galima būtų nuskaityti iš failo.

# v0.1

v0.1 commit da6eaa1 - Bandymas sutvarkyti įvedimo būdo veikimą, kad neveiktų "bug'ovai" bei patvarkomas lentelės formatas, kad labiau būtų sulygiuota
v0.1 commit fe9da83 - Patobulinimas įvedimo būdo veikimas.
v0.1 commit 1efdb59 - Padaroma, kad programa būtų sustabdoma, jeigu nepavyksta nuskaityti failo.
v0.1 commit ee0994c - Pilnai sutvarkomas įvedimo būdo ir studentų grupėje skaičiau įvedimo veikimas.
v0.1 commit 8a543cc - Sutvarkomas namų darbų pažymių įvedimo sutvarkymas.
v0.1 commit 1db89c7 - Galutinio balo skaičiavimo pasirinkimo įvedimo sutvarkymas.
v0.1 commit ba2acba - Pridedamas studentų išvedimas (output'as) pagal vardus.

# v0.2

v0.2 commit f9a7740 - klaidų ištaisymas ir natūralaus palyginimo patobulinimas
v0.2 commit 3d2c3ba - pridėtas didelių failų generavimas
v0.2 commit bb754ec - sutvarkomas didelių failų generavimas
v0.2 commit 1c36c4d - pridėtas išskistymas į du failus, pagal vidurkio/medianos pažymį
v0.2 commit e8ee862 - atliktas kodo reorganizavimas, sukurti antraštiniai failai
v0.2 commit 83d05da - pridėtos programos veikimo greičio analizės
v0.2 commit 7b95de1 - patobulintas laiko skaičiavimas ir pridėtas pasirinkimas kokio dydžio failą sukurti bei, kokio failo duomenis skaityti ir rūšiuoti.

Failų laikai:
1000 irašų failas: generavimas - 2ms nuskaitymas 2ms, rusiavimas ir isvedimas 5ms.
10000 irašų failas: generavimas - 23ms nuskaitymas 20ms, rusiavimas ir isvedimas 58ms.
100000 irašų failas: generavimas - 211ms nuskaitymas 186ms, rusiavimas ir isvedimas 625ms.
1000000 irašų failas: generavimas - 2.02s nuskaitymas 1.73s, rusiavimas ir isvedimas 7.08s.
10000000 irašų failas: generavimas - 20.37s nuskaitymas 17.52s, rusiavimas ir isvedimas 84.81s.

# v0.3
Testavimo laikai
Sistemos parametrai:
CPU: AMD Ryzen 5 9600X 6-Core
RAM: 32gb, DDR5, 6000 MHz, CL 36
SSD: 2TB, M.2, Write speed 6600 Mbytes/s, Read speed 7300 Mbytes/s

Naudojant vector:
Studentai1000.txt – generavimas 2ms, nuskaitymas 2ms, rūšiavimas 0ms, išvedimas 3ms.
Studentai10000.txt - generavimas 21ms, nuskaitymas 19ms, rūšiavimas 8ms, išvedimas 27ms.
Studentai100000.txt - generavimas 194ms, nuskaitymas 175ms, rūšiavimas 98ms, išvedimas 248ms.
Studentai1000000.txt - generavimas 1.93s, nuskaitymas 1.76s, rūšiavimas 1.18s, išvedimas 2.46s.
Studentai10000000.txt - generavimas 19.27s, nuskaitymas 17.71s, rūšiavimas 14.05s, išvedimas 24.41s.

Naudojant list:
Studentai1000.txt – generavimas 2ms, nuskaitymas 2ms, rūšiavimas 0ms, išvedimas 3ms.
Studentai10000.txt - generavimas 22ms, nuskaitymas 19ms, rūšiavimas 4ms, išvedimas 28ms.
Studentai100000.txt - generavimas 202ms, nuskaitymas 178ms, rūšiavimas 43ms, išvedimas 265ms.
Studentai1000000.txt - generavimas 1.93s, nuskaitymas 1.81s, rūšiavimas 675ms, išvedimas 2.62s.
Studentai10000000.txt - generavimas 19.19s, nuskaitymas 17.64s, rūšiavimas 9.96s, išvedimas 25.71s.


