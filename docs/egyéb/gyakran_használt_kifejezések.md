# Gyakran használt kifejezések

## Coupling (csatoltság)

A csatoltság az objektumok közötti függőség mértéke.

__Tight coupling (mereven vagy szorosan csatolt függőség)__

Szoros függőségről akkor beszélünk, amikor bizonyos osztályok nagymértékben függnek egymástól. Szoros függőség olyankor jön létre, amennyiben egy osztálynak túl sok a felelőssége, vagy egy konkrét hatáskör szétoszlik több osztályra. A szoros függőséget laza csatolással lehet feloldani.

Mivel a fejlesztés szoros függőség esetében gyorsabb lehet, leginkább prototípusok és kísérletek létrehozásához használható.

__Loose coupling (lazán csatolt függőség)__

A lazán csatolt osztályoknak az a nagy előnye, hogy egymástól függetlenül tudjuk őket használni és tesztelni. Laza csatolásokhoz általában interfészeket (interface) használunk. Az osztályok az interfészeken át kommunikálhatnak egymással, és ez a kommunikáció lefolytatható minden olyan osztály között amely implementálja az interfészt.

Leegyszerűsítve: egy szorosan csatolt függőséget úgy lehet elképzelni, mint a testünk és a börünk közti kapcsolatot. A bőrt értelemszerűen nehéz lenne lecserélni, ahhoz újra kellene tervezni a testünket. A lazán csatolt függőség a testünk és a ruhánk közti kapcsolathoz hasonlítható: bármikor lecserélhetünk egy-egy ruhadarabot. Emellet az ingünket kölcsönadhatjuk a barátainknak, mivel az ing nem tudja (és nem is érdekli), hogy kinek a testére kerül.
 

## SOLID tervezési elv

...