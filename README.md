# iOS-project
Application for iOS made as an project for college 

## Razvoj i stvaranje promjena

Repozitorij će imati "master" (glavna) granu i "development" (razvojnu) granu.

  - Glavna grana koristi se za "produkciju" i sadrži najnoviju verziju koda koja je objavljena "javnosti".

  - Razvojna grana koristi se za razvoj i testiranje u QA okruženju. Na kraju koda svaku kontrolnu točku, sve promjene na razvojnoj grani trebaju biti testirane i spojene na glavnu granu.

Prilikom pokretanja nove značajke, trebata granu stvoriti od glavne ili od razvojne grane. Kada završiš svoj kod, predložite svoje izmjene na razvojnu granu (zadano ponašanje), a ne na glavnu granu. Sve izmjene na razvojnoj grani bit će spojene na glavnu nakon "QA (Quality Assurance) testiranja".

Prilikom stvaranja nove grane, dodijeliti joj isti naziv kao i ID Exellice za zadatak, na primjer "TAG-1234". TAG koristimo kao placeholder.

Naslov commit poruke treba odgovarati nazivu ID zadatka iz exellice, na primjer "TAG-1 Inicijalizacija repozitorija".

## Korištenje GIT-a

Osnovne naredbe (ili koristi GitHub Desktop):

    - git clone - ako nemaš lokalnu kopiju repozitorija sa ovom naredbom klonirate repozitorij (Kad uđeš na repozitorij na GitHub, klik na zeleni gump <> Code i kopiraj link)
    - git status 
        - informacija o grani na kojoj se trenutno nalaziš, promjene na datotekama
        - koristite uvijek, provjerite na kojoj se grani nalaziš, ne raditi na main ili develop grani
    - git checkout - prelazak na drugu granu
        - npr. prelazak na postojecu granu - git checkout grana
        - stvaranje nove grane i prelazak na nju - git checkout -b grana
    - git add ime-datoteke ili git add . (dodaju se sve promjene, najbolje tako)
        - dodati izmjene za commit
    - git commit -m "commit message"
        - commitati promjene sa odgovarajucom porukom prema uputama (koristiti ID taska)
    - git pull
        - povuci najnovije promjene s udaljenog repozitorija
    - git push
        - poslati nove izmjene na udaljeni repozitorij
        - sa ovim salješ sve izmjene, mozeš koristiti git push origin ime-grane-za-poslati

Zaključak uputa za korištenje:
    - ne koristiti grane main i develop, koristiti nove grane za feature koje radiš
  - nakon završetka rada na npr. TAG-23 pushaj nove izmjene i napravi PR (Pull Request)
