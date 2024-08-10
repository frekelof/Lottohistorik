# Lottohistorik
Lottohistorik på Discord: https://discord.gg/JjQv7hxWSX

Projektet Lottohistorik innehåller resultathistorik av de rätta raderna för Svenska Spels Lotto 1, Lotto 2 & Joker, Eurojackpot, samt Vikinglotto. Möjlighet finns att rätta egna rader mot historiska resultat.

För att ladda ned Lottohistorik-filer, klicka på "senaste release" till höger, och välj "Source Code.zip".

* Databasen för Lotto innehåller historisk data från spelstart 1980-09-06 till senaste release. Resultat mellan 1980-09-06 och 1999-10-02 är separerade som "legacy" och används inte i några beräkningar. Se "Spelinformation.pdf" för mer information.

* Databasen för Joker innehåller historisk data från spelstart 1984-09-15 till senaste release.

* Databasen för Eurojackpot innehåller historisk data från spelstart 2012-03-23 till senaste release.

* Databasen för Vikinglotto innehåller historisk data från spelstart 1993-03-17 till senaste release. Resultat mellan 1993-03-17 och 2017-05-17 är separerade som "legacy" och används inte i några beräkningar. Se "Spelinformation.pdf" för mer information.

* Alla vinstsummor är i SEK.

* All rådata finns tillgänglig i SQLite-format i filen lottohistorik_raw.db. DB Browser for SQLite rekommenderas för att öppna databasen.

* Se fliken "Wiki" och "Discussions" för mer information.

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

För att rätta dina spel, öppna filen lottohistorik.odb. LibreOffice Base krävs för att köra filen och macro security ska vara satt till medium. Se Användarmanual.pdf för mer information.

1. Det finns tabeller, "Mina Rader - XXXX" för Lotto, Joker, Eurojackpot och Vikinglotto. Radera befintliga "Dummies" och lägg in dina spelade rader.
2. För att rätta dina spel, öppna Forms och kör "XXXX - Rätta Spel".
3. Om du spelar med systemspel måste det konverteras till rader. I Forms > Scripts > "Lottosystem -> Lottorader"" finns ett Pythonscript som utför detta (gäller endast lotto).

För att lägga in nya resultat:
1. Öppna Form "XXXX - Nya Resultat".
2. Fyll formuläret med de rätta raderna.
3. Tryck på knappen "Lägg till rad"

- - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - - -

Nummerfrekvenser

Filen Lottohistorik.ods innehåller nummerfrekenser för nedan spel. Talen som är "upplysta" med bakgrundsfärg är den rätta raden för respektive dragning. Observera att filen är väldigt stor och tar lång tid att ladda in. LibreOffice Calc eller MS Excel krävs för att köra filen. Beroende på personlig uppsättning kan vissa kolumner/celler presentera ### istället för ett tal, anpassa då kolumnbredden så all information visas.

* Nummerfrekvensen för Lotto är kumulativ. Den är uppdelad för Lotto 1 och Lotto 2. På grund av tekniska begränsningar presenteras data endast från 2020-01-01, men resultaten är baserade på alla dragningar från 1999-10-06 till och med dragningsdatum. Sorteringen är från vanligast förekommande tal (Hot) till minst vanligast tal (Cold).

* Nummerfrekvensen för Eurojackpot är kumulativ. Den är baserad på alla dragningar från Spelstart 2012-03-23 till och med dragningsdatum. Sorteringen är från vanligast förekommande tal (Hot) till minst vanligast tal (Cold). Vid ändring av antal Euronummer har nummerfrekvensen för Euronummer nollställts.

* Nummerfrekvensen för Vikinglotto är kumulativ. Den är baserad på alla dragningar från 2017-05-24 till och med dragningsdatum. Sorteringen är från vanligast förekommande tal (Hot) till minst vanligast tal (Cold). Vid ändring av antal Vikingnummer har nummerfrekvensen för Vikingnummer nollställts.
