<h1>Projekt:</h1> 
<h2>Brevlådeövervakning med objektigenkänning</h2>
Mitt  projekt blir att utveckla ett brevlådeövervakningssystem som kan detektera när post har levererats av PostNord. 
Det kommer bli en utökning av ett tidigare arduinoprojekt där jag idag har en sändare på min brevlåda som känner av när 
min brevlåda öppnas och meddelar mig när jag får post. Idag skickas en signal till en mottagare i mitt hus när locket 
till brevlådan öppnas. 
Mottagaren är uppkopplad tiill mitt nätverk och postar till en databas via ett API. När en förändring sker i databasen
skickas en notis till min telefon. Min algoritm känner av om jag fått post eller om det bara är reklam beroende på om
det är en dag då postnord levererar post (varannan dag) samt vilket klockslag händelsen sker. Detta är dock inte 100%
säkert just nu och tanken är att utöka sändarenheten med en videokamera som kan känna igen en bil från postnord. <br><br>

Tanken är att använda mig utav YOLO då det verkar vara både bra och snabbt för att känna igen specifika objekt 
och även enkel att implemetera och förstå. Datasetet tänkte jag skapa själv med bilder på postnordbilar.
