Kod agregacije 1 je sledeći:

<img width="626" height="671" alt="Agr1" src="https://github.com/user-attachments/assets/4b028424-0a8f-42d6-97be-5665503b730f" />

Primećuje se da se koriste drugačije imenovane kolekcije, sa nastavkom _sample na kraju. Razlog toga jeste što, usled velike količine podataka u kolekcijama Demographic (2,1 miliona) i Termination (269.000), agregacija postaje isuviše vremenski "skupa", to jest
za njeno izvršenje je potrebno isuviše vremena u ovom neoptimizovanom obliku nego što je razumno. Kreirane su kolekcije Demographic_sample sa 60.000 dokumenata i Termination_sample sa 10.000 dokumenata. Rezultat agregacije nad tim kolekcijama je sledeći:

<img width="424" height="69" alt="Agr1Out1" src="https://github.com/user-attachments/assets/07c3a6e4-8e0b-4977-9c75-334e80cda882" />

Vremenska kompleksnost može da se uoči iz toga što je za kolekciju Termination_sample sa 10.000 dokumenata potrebno vremena koliko je prikazano na sledećoj slici sa rezultatom explain komande u agregaciji:

<img width="914" height="460" alt="Agr1Explain1" src="https://github.com/user-attachments/assets/71039493-e1e4-4986-9735-76176861037b" />

Dok je za kolekciju Termination_sample sa 11.000 dokumenata rezultat sledeći:

<img width="831" height="67" alt="Agr1Out2" src="https://github.com/user-attachments/assets/37acc0a4-579c-494b-af57-fcdf4aa01819" />

A za njega je potrebno vremena koliko je prikazano na sledećoj slici:

<img width="1129" height="457" alt="Agr1Explain2" src="https://github.com/user-attachments/assets/fdca96f3-ec52-4689-b72a-d483e27707e5" />

Iz navedenog se vidi da je, sa blagim porastom veličine podataka u drugoj kolekciji, potrebno vreme naglo skočilo. U jednom izvršavanju koje nije zabeleženo na slici je bilo potrebno čak 85 sekundi i 450 milisekundi, što je najgori slučaj koji je izmeren.
Iz tog razloga, za sve neoptimizovane agregacije (bez indeksa i izmenjene šeme), će se koristiti podskupovi kolekcija sa nastavkom _sample.
