Zapoctovy Program UNIX
Dan Raffl, IOI, 2. rocnik 
LS 2019 
Uvod do Unixu

Popis:

Zapoctovy program se sklada z:
	- movesongs ... hlavni skript
	- demo ... ukazka jak movesongs.sh pracuje
	- pomocne skripty na mazani a tvoreni dat
		- createTestData, removeTestData, clearMusic

Movesongs - help:

	Skript movesongs presune vsechny zvukove soubory (.wav, .ogg, .mp3 ) ze slozky
	o jine:

	Defaultne skript pracuje v aktualnim adresari, ve kterem je slozka
	Downloads a z te se presunou vsechny zvukove soubory do slozky Music,
	ktera je ve stejne slozce jako tento skript. Zvukove souory musi byt ve
	formatu: 'Album:Autor-NazevPisnicky.ZvukovyFormat'. Skript takto
	strukturovana data roztridi do hierchie:

	CilovaSlozka/Autor/Album/NazevPisnicky.ZvukovyFormat.  

	Optiony: (v libovolnem poradi) 
	
	-a      Zmeni hierchii na CilovaSlozka/Autor/NazevPisnicky.ZvukovyFormat (nebere v potaz album} 

	-s	Zmeni slozku z defaultniho Downloads na lib. slozku odkud chceme brat soubory: -s DirName 

	-f      Zmeni slozku z defaultniho Music na lib. slozku, kam vysledek chceme ukladat: -f DirName -m
		Selektivne vybiram pouze format .mp3(*)

	-w      Selektivne vybiram pouze format .wav(*)

	-o      Selektivne vybiram pouze format .ogg(*)

	--help  napoveda pozn. (*) selektivne mohu vybirat POUZE JEDEN format
		./movesongs -m -o ........ invalidni vstup 
		./movesongs -m ........... validni vstup


Demo:

Pred spustenim dema je potreba inicializovat v aktualnim adresari adresar Music a Downloads, tedy provest prikazy:
mkdir Music
mkdir Downloads
