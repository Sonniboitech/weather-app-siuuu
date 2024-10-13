Väderapplikation
Denna applikation är en enkel väderapplikation där användare kan söka efter väderinformation för en specifik stad. Applikationen visar temperatur, väderbeskrivning, vindhastighet och luftfuktighet med ett stilrent användargränssnitt och en bakgrund med sol och moln.

Funktioner
Sök efter väder baserat på stadens namn.
Visa väderdata inklusive temperatur, väderbeskrivning, vindhastighet och luftfuktighet.
Responsivt och användarvänligt gränssnitt.
Bakgrund med sol och moln som ger en fin visuell upplevelse.
Förutsättningar
För att kunna köra denna applikation lokalt behöver du:

En webbläsare – Applikationen körs i alla moderna webbläsare (Chrome, Firefox, Edge, Safari etc.).
PHP – Applikationen kräver en PHP-server för att köra backend-koden.
Installera XAMPP eller MAMP om du inte redan har PHP på ditt system.
OpenWeatherMap API-nyckel – Du behöver registrera dig och få en API-nyckel från OpenWeatherMap.
Internetuppkoppling – Applikationen gör externa API-anrop för att hämta väderdata.
Installation
Klona eller ladda ner projektet:

bash
Kopiera kod
git clone https://github.com/ditt-anvandarnamn/vaderapplikation.git
Placera projektet i din lokala servermapp:

Om du använder XAMPP, placera projektet i htdocs-mappen (vanligtvis under C:\xampp\htdocs\).
Om du använder MAMP, placera projektet i htdocs-mappen (vanligtvis under /Applications/MAMP/htdocs/).
Skapa en .env-fil (om du använder API-nyckelhantering): Om du vill hantera din API-nyckel säkrare, kan du skapa en .env-fil för att lagra din nyckel. För tillfället anger du dock API-nyckeln direkt i PHP-koden.

Redigera index.php för att ange din OpenWeatherMap API-nyckel: Öppna filen index.php och ändra följande rad:

php
Kopiera kod
$apiKey = 'DIN_OPENWEATHERMAP_API_NYCKEL';
Hur man startar applikationen
Starta din lokala server (XAMPP eller MAMP):

Starta Apache-servern från kontrollpanelen.
Öppna webbläsaren och navigera till följande adress:

arduino
Kopiera kod
http://localhost/vaderapplikation/
Ange en stad i sökfältet och tryck på "Sök". Applikationen hämtar och visar väderinformationen.

Struktur
Projektet har följande struktur:

bash
Kopiera kod
├── index.php        # Huvudfilen som hanterar väderdata och frontend
├── script.js        # JavaScript för att hantera API-anrop och dynamiskt visa väderinfo
├── style.css        # CSS-filen för att styla sidan, bakgrunden och väderinformationen
└── README.md        # Instruktionsfilen (du läser just nu)
Beroenden
PHP – Backend-delen är skriven i PHP och kräver en PHP-server för att köra.
OpenWeatherMap API – Används för att hämta väderdata baserat på stadens namn.
Felsökning
Om väderinformationen inte visas:
Kontrollera att du har angett en giltig OpenWeatherMap API-nyckel.
Kontrollera att du har internetanslutning för att kunna anropa API
.
Kontrollera att din PHP-server körs korrekt.
Öppna webbläsarens utvecklingskonsol (F12) för att se om det finns några felmeddelanden i JavaScript.
