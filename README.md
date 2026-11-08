# Adresskoll för Bulletinen

Ett program som kontrollerar om de som får Bulletinen fortfarande bor kvar på adressen
i medlemsregistret. Det jämför varje adress med hitta.se och visar vilka som troligen
har flyttat. Du godkänner varje ändring själv, och programmet sparar resultatet som en
**ny fil** – originalfilen ändras aldrig.

## Ladda ner programmet

Programmet behöver inte installeras – det är en enda fil som du laddar ner och
dubbelklickar på. Du behöver bara göra det här en gång (och igen om det kommer en ny
version).

### Mac

1. Gå till **<https://github.com/patrik-eriksson1/adresskoll/releases/latest>**
   Du behöver inget konto eller lösenord.
2. Längst ner på sidan, under rubriken **Assets**, klickar du på den fil som passar din Mac:
   - **Adresskoll-Mac-Apple-chip.zip** – för de flesta Mac-datorer från 2021 och senare.
   - **Adresskoll-Mac-Intel.zip** – för äldre Mac-datorer.

   *Osäker?* Klicka på äpplet  uppe i vänstra hörnet → **Om den här datorn**. Står det
   **Chip: Apple M…** ska du ta Apple-chip. Står det **Processor: … Intel** ska du ta Intel.
3. Öppna mappen **Hämtade filer** (i Finder). Dubbelklicka på zip-filen om den inte
   redan är uppackad – då dyker **Adresskoll** upp.
4. Dra **Adresskoll** till mappen **Program** i Finders sidofält. Nu finns den bland dina
   andra program.
5. **Första gången** du startar den säger Mac att programmet inte kan öppnas eftersom
   det kommer från en okänd utvecklare. Det är normalt för små program som inte säljs
   i App Store. Gör så här:
   1. Dubbelklicka på **Adresskoll**. Tryck **Klar** (eller **OK**) när varningen kommer.
   2. Öppna **Systeminställningar** → **Integritet och säkerhet**.
   3. Scrolla ner. Där står det att Adresskoll blockerades – tryck **Öppna ändå** och
      skriv ditt datorlösenord.
   4. Tryck **Öppna** i rutan som kommer.

   Efter det startar programmet direkt när du dubbelklickar.
6. Om Mac frågar om Adresskoll får komma åt mappen **Dokument**, svara **Tillåt**.
   Det är där programmet sparar den nya medlemsfilen.

### Windows

1. Gå till **<https://github.com/patrik-eriksson1/adresskoll/releases/latest>**
   Du behöver inget konto eller lösenord.
2. Längst ner på sidan, under rubriken **Assets**, klickar du på
   **Adresskoll-Windows.zip**.
3. Öppna mappen **Hämtade filer** (Utforskaren → Hämtade filer). Högerklicka på
   **Adresskoll-Windows.zip** → **Extrahera alla…** → **Extrahera**.
4. I mappen som öppnas finns **Adresskoll.exe**. Vill du ha den på skrivbordet:
   högerklicka på den → **Visa fler alternativ** → **Skicka till** → **Skrivbord (skapa genväg)**.
5. **Första gången** du dubbelklickar kan Windows visa en blå ruta, ”Windows skyddade
   datorn”. Det är normalt för små program. Klicka på **Mer information** och sedan
   **Kör ändå**.

### Ny version?

Om programmet visar ett meddelande om en ny version, eller om något har slutat
fungera: ladda ner på samma sätt och ersätt den gamla filen. Det du har sparat
(påbörjade kontroller) finns kvar.

## Så här gör du (en gång om året, innan Bulletinen skickas)

**Starta programmet** genom att dubbelklicka på **Adresskoll**. Programmet öppnas i din
webbläsare (Safari, Chrome, Edge eller liknande). Sedan följer du stegen på skärmen:

1. **Öppna medlemsfilen** – välj `Alla.xlsx` och skriv filens lösenord.
2. **Kontrollera adresserna** – tryck **Starta kontrollen**. Det tar ungefär en
   halvtimme. Programmet visar hela tiden vad det gör just nu.
   - Du kan trycka **Pausa** när du vill och **Fortsätt** när du vill fortsätta.
   - Allt sparas automatiskt. Du kan stänga programmet och fortsätta en annan dag –
     starta programmet och öppna samma fil med samma lösenord, så fortsätter det där
     du slutade.
   - **Börja om från början** tar bort allt och kontrollerar alla på nytt.
3. **Gå igenom resultatet** – börja med fliken **Att granska**. För varje person
   trycker du **Ja, byt till den nya adressen** eller **Nej, behåll den gamla**.
   - *Troligen flyttat* – samma namn och ålder på en annan adress.
   - *Oklart* – flera möjliga personer. Klicka på rätt person i listan.
   - *Hittades inte* – sök själv med knapparna hitta.se, Ratsit, Merinfo eller Eniro,
     skriv in den nya adressen och tryck **Ja, byt till den nya adressen**.
   - Du kan rätta i adressfälten innan du godkänner.
4. **Spara ny medlemsfil** – knappen längst ner. Två filer sparas i mappen
   **Dokument → Bulletin-adresskoll**:
   - `Alla_uppdaterad_<datum>.xlsx` – medlemsfilen med de godkända ändringarna
     (samma lösenord som originalet)
   - `Adressändringar_<datum>.xlsx` – vad som ändrades, från vad till vad.

   Tryck **Visa filerna** för att öppna mappen. Titta igenom den nya filen och använd
   den sedan i stället för den gamla. Behåll gärna den gamla som säkerhetskopia.

Tryck **Avsluta** uppe till höger när du är klar. (Glömmer du det stänger programmet
sig självt efter en kvart utan aktivitet. Det du gjort är sparat.)

## Bra att veta

- Programmet läser bladet med kolumnerna **Namn, Gata, Adress, Ej Bulletin** (och gärna
  **Födelsedatum** och **Medl.nr.**). Kolumnerna får flyttas, men rubrikerna måste heta
  så. Den som har *något* skrivet i Ej Bulletin kontrolleras inte.
- Födelsedatum används för att skilja personer med samma namn åt (hitta.se visar ålder).
  Inga personnummer används eller sparas.
- Pågående arbete sparas krypterat med medlemsfilens lösenord, i programmets egen mapp
  på datorn. Ingen annan än den som har lösenordet kan läsa det.
- Personer under 18 år söks inte upp. De visas under fliken *Utland och under 18*.
- Personer med skyddad adress syns oftast inte på hitta.se.
- Om hitta.se ber programmet vänta, väntar det själv och försöker igen. Svarar hitta.se
  inte alls pausar programmet – vänta en stund och tryck **Fortsätt**.

## Om något inte fungerar

Programmet testar själv att hitta.se fungerar innan varje kontroll och säger tydligt
till om något är fel – det ger aldrig felaktiga svar. Kontakta den som underhåller
programmet (just nu Patrik Eriksson) och beskriv vad som står på skärmen.

Den här sidan innehåller bara nedladdningen och instruktionerna. Själva koden ligger
i ett privat förråd som underhållaren har tillgång till.
