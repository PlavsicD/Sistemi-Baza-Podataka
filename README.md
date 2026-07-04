# MongoDB projekat - Nosioci saobraćajnog osiguranja

Tema: Analiza skupa podataka o nosiocima saobraćajnog osiguranja

Autor: Dušan Plavšić IN24/2019

Opis skupa podataka

Skup podataka koji je predmet analize ovog projekta jeste "Auto Insurance churn analysis dataset", sintetički skup podataka preuzet sa Kaggle.com. Iz skupa podataka će se u ovom projektu koristiti 4 od 5 .csv fajlova (jedan od njih je fajl sa objedinjenim informacijama iz ostalih fajlova,
što bi obesmislilo projekat, te se neće koristiti za izradu). Za svaki od iskorištenih fajlova se pravi pojedinačna kolekcija istog imena, te su rezultirajuće kolekcije sledeće:

    • Customer - Opšti podaci o nosiocima - 2,3 miliona dokumenata
    • Address - Podaci o adresama nosilaca - 1,5 miliona dokumenata
    • Demographic - Demografski podaci nosilaca - 2,1 milion dokumenata
    • Termination - Skup datuma suspenzija/prekida osiguranja - 269.000 dokumenata
    

# O realizaciji

Početna shema

Početna shema baze podataka se nalazi u direktorijumu [V01](V01), gde se nalazi opis kolekcija u projektu i njihova polja.

Restruktuirana shema

Restruktuirana shema baze podataka se nalazi u direktorijumu [V02](V02).

Upiti

1. Koliko kreditno sposobnih nosilaca koji ne poseduju svoj dom i nemaju decu imaju aktivni ugovor?
2. Odrediti u kom gradu su u proseku najviša primanja i prosečnu starost nosioca u tom gradu.
3. Odrediti da li je prosecni iznos placen u toku prethodne godine veći za demografiju van braka, bez dece i bez prebivališta i njihovom vlasništvu, u braku bez dece i bez prebivališta u njihovom vlasništvu ili u braku, sa decom i sa prebivalištem u njihovom vlasništvu?
4. Koji procenat nosilaca koji su vlasnici svog prebivališta, čija je vrednost viša od 100.000, i dalje ima aktivni ugovor?
5. Da li je procenat prekinutih ugovora veći među demografijom nosilaca koja ne poseduje prebivalište ali je kreditno sposobna nego među onom koja poseduje a nije kreditno sposobna?
