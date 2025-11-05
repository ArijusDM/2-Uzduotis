# v1.0

Naudojimosi instrukcija: iš pradžių pasirenkama, kokio dydžio studentų failą norima generuoti (galima ir negeneruoti).
Pasirenkamas duomenų įvedimo būdas: 1) įvesti ranka, 2) generuoti kelis atsitiktinai, 3) nuskaityti iš failo.
1) Įvedamas studentų skaičius, jų vardai ir pavardės, tada yra surašomi namų darbų pažymiai (kai nusprendžiame, kad pakanka pažymių, du kartus paspaudžiam ENTER) ir galiausiai įvedamas egzamino pažimys. 2) Įvedamas studentų skaičius, jų vardai ir pavardės, o pažymiai yra sugeneruojami atsitiktinai. 3) Duomenys yra nuskaitomi iš failo, kurį prieš tai pasirinkome sugeneruoti.
Po duomenų suvedimo galima pasirinkti, kaip apskaičiuoti galutinį balą, pagal vidurkį, medianą arba abu.
Galiausiai studentai yra suskirstomi į du failus: "kietiakai.txt", kurių galutinis balas yra didesnis už 5, ir "vargsiukai.txt", kurių galutinis balas yra mažesnis už 5.

v1.0 commit 3aaaf90 – sutvarkytas 1 strategija
v1.0 commit 2f249ab – pridėta 2 strategija vector‘iui
v1.0 commit 991f50c – pridėti shrink_to_fit
v1.0 commit f41d9c5 – pridėta 2 strategija list’ui
v1.0 commit 92ef6f2 – pridėta 3 strategija vector‘iui
v1.0 commit 040a855 – sutvarkyta 2 vector’ių strategija, kad veiktų
v1.0 commit 919a733 - sutvarkyta 3 vector‘ių strategija
v1.0 commit 7d49738 - pridėta 3 strategija list‘ui
v1.0 commit afb5ef3 – pakeista 2 vector’iaus strategija iš remove_if į partition
v1.0 commit c4528d0 – sutvarkytos klaidos ir panaikintos nereikalingos eilutės

Testavimo laikai
Sistemos parametrai:
CPU: AMD Ryzen 5 9600X 6-Core
RAM: 32gb, DDR5, 6000 MHz, CL 36
SSD: 2TB, M.2, Write speed 6600 Mbytes/s, Read speed 7300 Mbytes/s

Naudojant vector:
Studentai1000.txt (5 bandymų vidurkiai) – generavimas 2ms, nuskaitymas 1.8ms, 1 strategijos rūšiavimas 0ms, 2 strategijos rūšiavimas 0ms, 3 strategijos rūšiavimas 0ms, rūšiavimas ir skirstymas kartu 1ms, išvedimas 3ms.
Studentai10000.txt (5 bandymų vidurkiai) - generavimas 20ms, nuskaitymas 19ms, 1 strategijos rūšiavimas 2ms, 2 strategijos rūšiavimas 1ms, 3 strategijos rūšiavimas 1ms, rūšiavimas ir skirstymas kartu 10ms, išvedimas 25.8ms.
Studentai100000.txt (5 bandymų vidurkiai) - generavimas 194ms, nuskaitymas 179.2ms, 1 strategijos rūšiavimas 21.2ms, 2 strategijos rūšiavimas 15.4ms, 3 strategijos rūšiavimas 12ms, rūšiavimas ir skirstymas kartu 114.2ms, išvedimas 245.6ms. 
Studentai1000000.txt (5 bandymų vidurkiai) - generavimas 1.9s, nuskaitymas 1.81s, 1 strategijos rūšiavimas 227.2ms, 2 strategijos rūšiavimas 173.6ms, 3 strategijos rūšiavimas 142.8ms, rūšiavimas ir skirstymas kartu 1.36s, išvedimas 2.47s.
Studentai10000000.txt (5 bandymų vidurkiai) - generavimas 19.21s, nuskaitymas 18.1s, 1 strategijos rūšiavimas 2.2s, 2 strategijos rūšiavimas 1.83s, 3 strategijos rūšiavimas 1.51s, rūšiavimas ir skirstymas kartu 15.75s, išvedimas 24.98s.

Naudojant list:
Studentai1000.txt (5 bandymų vidurkiai) – generavimas 2ms, nuskaitymas 2ms, 1 strategijos rūšiavimas 0ms, 2 strategijos rūšiavimas 0ms, 3 strategijos rūšiavimas 0ms, rūšiavimas ir skirstymas kartu 0ms, išvedimas 3ms.
Studentai10000.txt (5 bandymų vidurkiai) - generavimas 19.8ms, nuskaitymas 17.4ms, 1 strategijos rūšiavimas 2ms, 2 strategijos rūšiavimas 0ms, 3 strategijos rūšiavimas 0.6ms, rūšiavimas ir skirstymas kartu 5ms, išvedimas 25.4ms.
Studentai100000.txt (5 bandymų vidurkiai) - generavimas 194.2ms, nuskaitymas 173.6ms, 1 strategijos rūšiavimas 20.8ms, 2 strategijos rūšiavimas 4ms, 3 strategijos rūšiavimas 13.2ms, rūšiavimas ir skirstymas kartu 64.2ms, išvedimas 253.6ms.
Studentai1000000.txt (5 bandymų vidurkiai) - generavimas 1.91s, nuskaitymas 1.77s, 1 strategijos rūšiavimas 215.8ms, 2 strategijos rūšiavimas 44.8ms, 3 strategijos rūšiavimas 171.6ms, rūšiavimas ir skirstymas kartu 963.2ms, išvedimas 2.57s.
Studentai10000000.txt (5 bandymų vidurkiai) - generavimas 19.26s, nuskaitymas 17.62s, 1 strategijos rūšiavimas 2.15s, 2 strategijos rūšiavimas 446.6ms, 3 strategijos rūšiavimas 1.73s, rūšiavimas ir skirstymas kartu 12.19ms, išvedimas 26.48s.
<img width="899" height="749" alt="image" src="https://github.com/user-attachments/assets/6a94fe60-59cb-4051-96bc-f8508a32ebd1" />

Testavimo išvados: vector konteineryje 3 strategija (stable_partition) veikia greičiausiai, tada 2 (partition) ir 1. Tuo tarpu list konteineryje 2 strategija veikia greičiausiai, tada 3 ir 1

# v0.3

v0.3 commit 5a4ed28 - sutvarkytas rūšiavimas
v0.3 commit 22f7344 – pridėtas konteineris list
v0.3 commit 0e0ce3e – padaryti du konteineriai list ir vector bei padaryta, kad būtų galima pasirinkti, su kuriuo konteineriu dirbama
v0.3 commit 4a3cfc1 – sutvarkytas skaitymo laiko matavimas
v0.3 commit a79509a – sutvarkytas skirstymo laiko matavimas
v0.3 commit c824e55 – pridėtas išvedimo laiko matavimas
v0.3 commit d7b67dc – pakeista išvedimo laiko matavimo vieta
v0.3 commit 7ed0ddf – pakeistas skaitymo laiko matavimas
v0.3 commit e3c5740 – pakeista, kad “Studentas.h” butų galima pasirinkti konteinerio tipą
v0.3 commit 3fb01e6 – pakeista, kad “Failai.h” būtų naudojamas universalus konteinerio tipas
v0.3 commit 97de75a – pakeista, kad “Failai.cpp” būtų naudojamas universalus konteinerio tipas
v0.3 commit 3f078ed – “Studentas.h” pridėta NAUDOTI_LIST, dėl patogesnio konteinerio pasirinkimo
v0.3 commit 5bba104 – pašalintas rūšiavimas pagal vardą arba pavardę
v0.3 commit 7dfbfc7 – “Studentas.h” pridėta “pragma once”
v0.3 commit 73fc354 – padaryta, kad būtų galima pasirinkti konteinerio tipą main.cpp faile bei, kai pasirenkama generuoti failą ir nuskaityti duomenis iš failo, automatiškai būtų parinktas tas sugeneruotas failas
v0.3 commit fd44dd0 – “Studentas.h” galutinai padaryta, kaip pasirinkti konteinerio tipą: užkomentuoti tą, kuris nebus naudojamas

Testavimo laikai
Sistemos parametrai:
CPU: AMD Ryzen 5 9600X 6-Core
RAM: 32gb, DDR5, 6000 MHz, CL 36
SSD: 2TB, M.2, Write speed 6600 Mbytes/s, Read speed 7300 Mbytes/s

Naudojant vector:
Studentai1000.txt (5 bandymų vidurkiai) – generavimas 2ms, nuskaitymas 2ms, rūšiavimas 0ms, išvedimas 3ms.
Studentai10000.txt (5 bandymų vidurkiai) - generavimas 20.2ms, nuskaitymas 18ms, rūšiavimas 6.4ms, išvedimas 26.2ms.
Studentai100000.txt (5 bandymų vidurkiai) - generavimas 193ms, nuskaitymas 176.2ms, rūšiavimas 80.2ms, išvedimas 250.4ms. 
Studentai1000000.txt (5 bandymų vidurkiai) - generavimas 1.92s, nuskaitymas 1.79s, rūšiavimas 976ms, išvedimas 2.49s.
Studentai10000000.txt (5 bandymų vidurkiai) - generavimas 19.21s, nuskaitymas 18.05s, rūšiavimas 11.61s, išvedimas 24.69s.

Naudojant list:
Studentai1000.txt (5 bandymų vidurkiai) – generavimas 2ms, nuskaitymas 1.6ms, rūšiavimas 0ms, išvedimas 3ms.
Studentai10000.txt (5 bandymų vidurkiai) - generavimas 20ms, nuskaitymas 17.8ms, rūšiavimas 3.4ms, išvedimas 27.4ms.
Studentai100000.txt (5 bandymų vidurkiai) - generavimas 194.8ms, nuskaitymas 172.6ms, rūšiavimas 44.4ms, išvedimas 260.6ms.
Studentai1000000.txt (5 bandymų vidurkiai) - generavimas 1.92s, nuskaitymas 1.78s, rūšiavimas 685.4ms, išvedimas 2.6s.
Studentai10000000.txt (5 bandymų vidurkiai) - generavimas 19.25s, nuskaitymas 17.28s, rūšiavimas 9.96s, išvedimas 25.69s.
<img width="914" height="753" alt="image" src="https://github.com/user-attachments/assets/981909fd-08b5-4e8e-9f78-37185299a79b" />

Testavimo išvados: Generavimas tiek vector, tiek list pakankamai panašus. Nuskaitymas ir rūšiavimas greitesnis naudojant list. Išvedimas greitesnis naudojant vector.

# v0.2

v0.2 commit f9a7740 - klaidų ištaisymas ir natūralaus palyginimo patobulinimas
v0.2 commit 3d2c3ba - pridėtas didelių failų generavimas
v0.2 commit bb754ec - sutvarkomas didelių failų generavimas
v0.2 commit 1c36c4d - pridėtas išskistymas į du failus, pagal vidurkio/medianos pažymį
v0.2 commit e8ee862 - atliktas kodo reorganizavimas, sukurti antraštiniai failai
v0.2 commit 83d05da - pridėtos programos veikimo greičio analizės
v0.2 commit 7b95de1 - patobulintas laiko skaičiavimas ir pridėtas pasirinkimas kokio dydžio failą sukurti bei, kokio failo duomenis skaityti ir rūšiuoti.

Failų laikai:
1000 irašų failas: generavimas - 2ms nuskaitymas 2ms, rūšiavimas ir išvedimas 5ms.
10000 irašų failas: generavimas - 23ms nuskaitymas 20ms, rūšiavimas ir išvedimas 58ms.
100000 irašų failas: generavimas - 211ms nuskaitymas 186ms, rūšiavimas ir išvedimas 625ms.
1000000 irašų failas: generavimas - 2.02s nuskaitymas 1.73s, rūšiavimas ir išvedimas 7.08s.
10000000 irašų failas: generavimas - 20.37s nuskaitymas 17.52s, rūšiavimas ir išvedimas 84.81s.

# v0.1

v0.1 commit da6eaa1 - Bandymas sutvarkyti įvedimo būdo veikimą, kad neveiktų "bug'ovai" bei patvarkomas lentelės formatas, kad labiau būtų sulygiuota
v0.1 commit fe9da83 - Patobulinimas įvedimo būdo veikimas.
v0.1 commit 1efdb59 - Padaroma, kad programa būtų sustabdoma, jeigu nepavyksta nuskaityti failo.
v0.1 commit ee0994c - Pilnai sutvarkomas įvedimo būdo ir studentų grupėje skaičiau įvedimo veikimas.
v0.1 commit 8a543cc - Sutvarkomas namų darbų pažymių įvedimo sutvarkymas.
v0.1 commit 1db89c7 - Galutinio balo skaičiavimo pasirinkimo įvedimo sutvarkymas.
v0.1 commit ba2acba - Pridedamas studentų išvedimas (output'as) pagal vardus.

# v.pradinė

v.pradinė commit f4b0c38 - Pradinio kodo sukūrimas, kodas paimtas iš paskaitos darbo ir truputį bandymas patobulinti, kad įvedimas neveiktų "bug'ovai" .
v.pradinė commit f675ff5 - Pridedamas galutinio balo medianos apskaičiavimas.
v.pradinė commit 540a23b - Padaroma, kad galima pasirinkti lentelės atsakymus: matyti tik galutinio balo vidurkį, tik medianą arba vidurkį ir medianą. 
v.pradinė commit c4dcba7 - Pridedamas variantas, kad galima įrašyti namų darbų pažymius nežinant, kiek yra namų darbų. T.y. pažymių rašai, kiek nori, ir kai nusprendi, kad užtenka, įrašai 0, kad nutraukti pažymių įrašymą. Taip pat bandoma toliau tvarkyti įvedimus, kad jie neveiktų "bug'ovai".
v.pradinė commit 469dab3 - Pridedama funkcija, kad namų darbų ir egzamino rezultatai būtų generuojami atsitiktinai.
v.pradinė commit 5ab2768 - Pridedamas variantas, kad duomenis galima būtų nuskaityti iš failo.
