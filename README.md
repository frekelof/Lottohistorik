# Lottohistorik
Lottohistorik på Discord: https://discord.gg/JjQv7hxWSX

För att ladda ned, klicka på filerna och välj sedan "Download raw file".

Filen lottohistorik.odb innehåller resultathistorik av de rätta raderna för Svenska Spels Lotto 1, Lotto 2 & Joker, Eurojackpot, samt Vikinglotto. LibreOffice Base krävs för att köra filen och macro security ska vara satt till medium.

För att rätta dina spel:
1. Det finns tabeller, "Mina Rader - XXXX" för Lotto, Joker, Eurojackpot och Vikinglotto. Radera befintliga "Dummies" och lägg in dina spelade rader.
2. För att rätta dina spel, öppna Forms och kör "XXXX - Rätta Spel".
3. För att kontrollera dina rader mot äldre lottodragningar (innan år 2000) måste queries "Lotto Legacy - 4R, 5R, 6R, 7R" köras.
4. Om du spelar med systemspel måste det konverteras till rader. I Forms > Scripts > "Lottosystem -> Lottorader"" finns ett Pythonscript som utför detta (gäller endast lotto). 

För att lägga in nya resultat:
1. Öppna Form "XXXX - Nya Resultat".
2. Fyll formuläret med de rätta raderna.
3. Tryck på knappen "Lägg till rad"

* Databasen för Lotto innehåller historisk data för alla resultat sedan starten 1980-09-06 till 2024-07-20. Lottoresultat innan 2000-01-05 är separerade som ”legacy” och är begränsade till 7 huvudnummer (inga tilläggsnummer). Vissa datum kan avvika från verkligt dragningsdatum i detta dataset.

* Databasen för Joker innehåller historisk data mellan 2012-07-18 och 2024-07-20.

* Databasen för Eurojackpot innehåller historisk data från spelstart 2012-03-23 till 2024-07-19. 

* Databasen för Vikinglotto innehåller historisk data från senaste spelregeländring 2017-05-24 till 2024-07-17. Äldre resultat mellan 1993-03-17 och 2017-05-17 är arkiverade som ”legacy” då resultaten bygger på föråldrade spelregler.

* Alla vinstsummor är i SEK.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

Nummerfrekvenser

Filen Lottohistorik.ods innehåller nummerfrekenser för nedan spel. Talen som är "upplysta" med bakgrundsfärg är den rätta raden för respektive dragning. Observera att filen är väldigt stor och tar lång tid att ladda in. LibreOffice Calc eller MS Excel krävs för att köra filen.

* Nummerfrekvensen för Eurojackpot är kumulativ. Den är baserad på alla dragningar från Spelstart 2012-03-23 till och med dragningsdatum. Sorteringen är från vanligast förekommande tal (Hot) till minst vanligast tal (Cold). Vid ändring av antal Euronummer har nummerfrekvensen för Euronummer nollställts.

* Nummerfrekvensen för Lotto är kumulativ. Den är uppdelad för Lotto 1 och Lotto 2. På grund av tekniska begränsningar presenteras data endast från 2020-01-01, men resultaten är baserade på alla dragningar från 2000-01-05 till och med dragningsdatum.. Sorteringen är från vanligast förekommande tal (Hot) till minst vanligast tal (Cold).

* Nummerfrekvensen för Vikinglotto är kumulativ. Den är baserad på alla dragningar från 2017-05-24 till och med dragningsdatum. Sorteringen är från vanligast förekommande tal (Hot) till minst vanligast tal (Cold). Vid ändring av antal Vikingnummer har nummerfrekvensen för Vikingnummer nollställts.
