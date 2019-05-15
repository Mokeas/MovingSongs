Movesongs

Skript pracuje v adresari, ve kterem je slozka
Downloads a z te se presunou vsechny zvukove soubory do slozky Music,
ktera je ve stejne slozce jako tento skript. Zvukove souory musi byt ve
formatu: 'Album:Autor-NazevPisnicky.ZvukovyFormat'. Skript takto
strukturovana data roztridi do hierchie:
CilovaSlozka/Autor/Album/NazevPisnicky.ZvukovyFormat.
Pro vice optionu pouzijte -help.

Example:

Downloads:
"54 Dole Hlavou:Horkyze Slize-Silny Refren.mp3" 
"Corrida: Kabat-Kostlivci.ogg"
"adfafaffaf.dfs"
"tosemnepatri.csv"
"Hybrid Theory:Linkin Park-In The End.mp3"
"Hybrid Theory:Linkin Park-Forgotten.mp3"
"Meteora: Linkin Park-Breaking The Habit.mp3"

./movesongs -m 			(-m = selektive vybiram .mp3)

Music:
Horkyze Slize
	54 Dole Hlavou
		Silny Refren.mp3
		
Linkin Park
	Meteora
		Breaking The Habit.mp3
	Hybrid Theory
		In The End.mp3
		Forgotten.mp3
