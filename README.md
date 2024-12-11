<h1>Projekt:</h1> 
<h2>Brevlådeövervakning med objektigenkänning</h2>
Detta är en uppdatering av ett tidigare projekt för att uppmärksamma när jag får post i min brevlåda.

Som projekt har jag valt att utveckla ett brevlådeövervakningssystem som kan detektera när post har levererats av PostNord.
Det är en utökning av ett tidigare arduinoprojekt där jag tidigare har haft en sändare på min brevlåda som känner av när
min brevlåda öppnas och meddelar mig när jag får post. Innan har en signal skickats till en mottagare i mitt hus när locket
till brevlådan öppnas. Mottagaren är uppkopplad till mitt nätverk och postar till en databas via ett API.
När en förändring sker i databasen skickas en notis till min telefon. Min algoritm känner av om jag fått post eller om
det bara är reklam beroende på om det är en dag då postnord levererar post (varannan dag) samt vilket klockslag händelsen sker.
Detta var dock inte 100% säkert och tanken är att utöka sändarenheten med en videokamera som kan känna igen en bil från postnord.

Jag har provat olika lösningar så som Tensorflow och olika versioner utav Yolo men har inte fått det att fungera.
Till slut valde jag att använda mig utav YOLO v11 då det verkade vara både bra och snabbt för att känna igen specifika objekt och även enkelt att implemetera
och förstå. Datasetet har jag skapat själv med bilder på postnordbilar samt vanliga bilar. För att märka upp mina bilder med vad som
är postnord-bilar och vanliga bilar har jag använt mig utav Label-studio.

Med detta tillvägagångssätt kan jag helt utesluta arduino-delen i projektet och istället använda en kamera som är riktad mot min brevlåda
vilket sparar in på 9v batterier vid sändaren samt skapar en mer vädertålig lösning.

I videon explanation.mp4 visar och förklarar jag lite hur projektet fungerar.
