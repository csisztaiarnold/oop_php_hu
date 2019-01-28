# Bevezető

Kezdő programozók első tapasztalati a PHP-n belül általában procedurális programozási minta formájában történnek meg. A procedurális megközelítésnek megvannak a saját előnyei, főképp olyankor, ha csupán egy specifikus problémára kell fókuszálnunk, de minél bonyolultabbá válik egy projektünk és érezhetően egyre gyorsabban haladunk a spagetti kód felé, annál jobban felmerül annak az igénye, hogy a kódunkat objektumorientált architektúra alapján építsük fel.

## Mit jelent az objektumorientáltság?

Az objektumelvű programozás egy fejlesztési eljárás, melyben a szoftverarchitektúrát olyan független, különálló, modularizált elemekre választjuk szét, amelyek szükség esetén képesek kölcsönhatásba lépni egymással. Ezek az elemek az __osztályok__ (class) és az osztályokon belüli _egy bizonyos hatáskörbe_ tartozó __metódusok__ (method).

A jól átgondolt objektumorientált szemlélet eredménye az áttekinthetőbb, könnyen bővíthető és fenntartható kódbázis lesz.

## Az objetkumorientáltság fő jellemzői

__Egységbezárás vagy betokozás (Encapsulation)__

Abban az esetben beszélhetünk egységbezárásról, amennyiben egy objektum tulajdonságait és annak viselkedését leíró eljárásokat (metódusok) hordozó osztályt elzárunk a külvilágtól. Az objektum használójának nem kell tudnia, hogy az miként működik, csupán hogy miként épül fel.

__Öröklés (Inheritance)__

Egy szülő objektum (ős- vagy szülőosztály - ancestor class) átadhatja egy gyermek objektumnak (leszármazott, származtatott vagy gyermekosztály - descendant class) a saját tulajdonságait. A leszármazott objektum létrehozhat új tulajdonságokat, vagy felülírhatja és újradefiniálhatja az ősosztály tulajdonságait. 

__Többrétűség (Polymorphism)__
