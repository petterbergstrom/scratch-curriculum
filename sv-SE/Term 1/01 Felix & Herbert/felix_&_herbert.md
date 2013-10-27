Level 1

#Felix & Herbert

__Introduktion:__
Vi skall leka tafatt med med __katten Felix__ och __Musen Herbert__. Du styr Herbert med musen och du skall försöka låta bli att fångas av Felix. Desto längre du lyckas hålla dig undan desto fler poäng får du men fångas du då blir du av med poäng, så akta dig för katten!

##STEG 1: Felix följer muspekaren

1. Starta ett nytt projekt
2. Ändra bakgrundsbild för spelet. För att göra det så klickar på scenen bredvid spriten och växla till "Bakgrunder" fliken. Importera bilden som ligger i indors/hall. Ta bort den tomma bakgrundsbilden som låg där sedan innan.
3. Ändra namnet på spriten till Felix.
4. Försäkra dig om att Felix endast pekar vänster-höger genom att klicka på knappen som ser ut så här:
5. Skapa det här scriptet:

```scratch

	När FLAG klickas på

	för alltid

		peka mot muskarkör

		gå 10 steg

		nästa klädsel

		spela trumman 52 för 0.3 taktslag

	(slut på för alltid)
```
		
###Testa dig projekt
__Klicka på den gröna flaggan.__
Följer Felix muspekaren? Ser det ut som han går när han rör sig? Har han rätt fart?

Spara ditt projekt

##STEG 2: Felix Jagar Herbert

__NU är det dags för Felix att jaga musen Herbert i stället för att jaga muspekaren.__

1. Skapa en annan sprite genom att klicka på knappen "Ny sprite från fil" välj sedan animals/mouse1.
2. Ändra namnet på spriten till Herbert.
3. Ändra kostymen och gör den mindre än Felix.
Testa med sex klick på krymp knappen:
4. Make sure Herbert only points left-right. 
Set till att Herbert endast kår vänster-höger.
5. Ge Herbert det här scriptet:


```scratch
	
	När FLAG klickas på
	för allid
		gå till musmarkör
		peka mot Felix
	(slut på för alltid)
```

###Testa ditt projekt
__Klicka på den gröna flaggan.__

Rör sig Herbert med muspekaren? Följer Felix efter Herbert?

Spara ditt projekt.

##STEG 3: Felix säger till när han fångat Herbert.

__Vi vill att Felix skall veta när han fångat Herbert och säga till oss.__

1. Change Felix’s script to be this:
1. ÄNdra Felix script till detta:

```scratch
	
	När FLAG Klickas på
	För alltid
		peka mot musmakör
		gå 10 steg
		nästa klädsel
		spela trumman 52 för 0.3 taktslag
		om rör Herbert?
			säg Fick dig! i 1 sekuder
		(end om)
	(slut på för alltid)
```

###Testa ditt projekt
__Klicka på den gröna flaggan.__

Säger Felix till när han fångar Herbert?

Spara ditt projekt.

##STEG 4: Herbert blir ett spöke när han blir fångad.

__Istället för att Felix skall säga något vill vi att Herbert skall bli ett spöke när han blir fångad.__

1. Ändra Felix script så det sänder ett meddelande när han fångar Herbert.

```scratch

	När FLAG Klickas på
	för alltid
		peka mot musmakör
		gå 10 steg
		nästa klädsel
		spela trumman 52 för 0.3 taktslag
		om rör Herbert?
			sända fångad
			spela trumman 58 för 0.2 taktslag
			vänta 1 sekunder
		(end om)
	(slut på för alltid)
	
```
2. Importera en ny klädsel till Herbert från fantasy/ghost2-a
3. Ändra klädseln så att den blir mindre
Sex klick på krympknappen bör räcka.
4. Ändra namnen på Herbers klädslar så musen heter ‘levande’ och spöket heter ‘död’.
5. Skapa ett nytt script som gör att Herbert blir ett spöke när han fångas.

```scratch
	
	när jag tar emot fångad
	ändra till klädsel död
	vänta 0.5 sekunder
	ändra till klädsel levande

```
	
###Testa ditt projekt.
__Klicka på den gröna flaggan.__

Blir Herbert ett spöka när han fångas?
Spelar Felix rätt ljud när han skall?
Står Felix still tillräckligt länge för att Herbert skall hinna i väg?

Spara ditt projekt

##STEG 5: Räkna poäng

__För att få reda på hur bra vi är på att hålla Herbert levande så får vi lägga till poängräkning. Vi börjar med noll poäng och ökar med 1 varje sekund. Om Felix får tag på Herbert minskar vi poängen med ett hundra.__ 

1. Skapa en variabel för alla spritar och kallar den för poäng. FÖr att göra detta: Klicka på variabler i menyn, skapa en variabel och döp den till ‘poäng’
2. På scenen, skapa två script

```scratch
	
	när FLAG klickas på
	sätt poäng till 0
	för alltid
		ändra poäng med 1
		vänta 1 sekunder
	(slut för alltid)
	
	när jag tar emot fångad
	ändra poäng med -100
```
	
###Testa ditt projekt
__Klicka på den gröna flaggan.__

Går poängen upp med ett poäng varje sekund?
Går poänget ner med ett hundra när Herbert fångas?
Vad händer när Herbert fångas innan poänget när ett hundra? Sätts poänget till noll när du startar ett nytt spel?

Spara ditt projekt.

__Bra gjort! Nu är du färdig och kan njuta av ditt alldeles egna spel!__
Glöm inte att dela med dig av ditt spel med dina kompisar och din familj. Det gör du genom att klicka på __Dela ut detta projekt__ i menyn.

