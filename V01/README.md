# Početna shema baze podataka

# Kolekcije

Ovde su navedene kolekcije koje se koriste za izradu projekta. Sve kolekcije nose isto ime kao i .csv fajl iz kojeg su importovani podaci.

Kolekcija Customer

Polja:

    • INDIVIDUAL_ID - identifikaciona oznaka nosioca, ovo polje se nalazi u svakoj kolekciji osim kolekciji Address
    • ADDRESS_ID – identifikaciona oznaka adrese nosioca, ovo polje dele kolekcije Customer i Address
    • CURR_ANN_AMT – iznos osiguranja plaćen prethodne godine
    • DAYS_TENURE – koliko dugo je nosilac osiguran, izraženo u danima
    • CUST_ORIG_DATE - datum na koji je nosilac sklopio ugovor
    • AGE_IN_YEARS – uzrast nosioca
    • DATE_OF_BIRTH – datum rođenja nosioca
    • SOCIAL_SECURITY_NUMBER - matični broj nosioca

Kolekcija Address

Polja:

    • ADDRESS_ID – identifikaciona oznaka adrese nosioca, ovo polje dele kolekcije Customer i Address
    • LATITUDE – geografska širina adrese
    • LONGITUDE - geografska dužina adrese
    • STREET_ADDRESS - adresa nosioca
    • CITY - grad u kojem se adresa nalazi
    • STATE - savezna država u kojoj se adresa nalazi
    • COUNTY - opština u kojoj se adresa nalazi

Kolekcija Demographic

Polja:

    • INDIVIDUAL_ID
    • INCOME - prihod nosioca
    • HAS_CHILDREN - da li nosliac ima decu, binarna vrednost (0 - nema, 1- ima)
    • LENGTH_OF_RESIDENCE - procenjeno trajanje stanovanja nosioca u prebivalištu
    • MARITAL_STATUS - bračni status nosioca ("Single" - nije venčan, "Married" - venčan)
    • HOME_MARKET_VALUE - procenjena vrednost boravišta nosioca
    • HOME_OWNER - da li je nosilac vlasnik svog boravišta, binarna vrednost (0 - nije, 1 - jeste)
    • COLLEGE_DEGREE - da li je nosilac visoko obrazovan, binarna vrednost (0 - nije, 1 - jeste)
    • GOOD_CREDIT - kreditna sposobnost nosioca, binarna vrednost (0 - nije kreditno sposoban, 1 - jeste kreditno sposoban)

Kolekcija  Termination

Polja: 

    • INDIVIDUAL_ID
    • ACCT_SUSPD_DATE - datum suspenzije/prekida ugovora nosioca
