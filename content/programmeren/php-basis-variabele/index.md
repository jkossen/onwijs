---
title: "PHP Basis: Variabele"
date: 2020-09-27T21:04:58+02:00
tags: ["php", "programmeren", "softwaredeveloper", "mbo", "applicatieontwikkelaar", "25604", "25187"]
authors:
  - Jochem Kossen
overview: "../php-basis"
---

## Slides

### Variabelen: schematisch
![PHP Variabelen in het RAM geheugen 1](php-basis-variabele-1.png)

### Reeks blokken met naam en waarde
![PHP Variabelen in het RAM geheugen 2](php-basis-variabele-2.png)

### Apothekerskast
Een simpeler analogie voor variabelen en het RAM geheugen is wellicht de apothekerskast. Het RAM geheugen bestaat uit heel veel lades. Elke lade heeft een etiket met de **naam** van wat erin zit en de **inhoud** van de la. Wat op het etiket staat is de naam van de variabele. De inhoud is de **waarde** van de variabele. 

![RAM geheugen als apothekerskast](php-basis-variabele-3.png)

### Downloads

[[pdf](php-basis-variabele.pdf)] [[pptx](php-basis-variabele.pptx) (bronbestand)]

## Beschrijving

Met variabelen kun je gegevens in het RAM geheugen opslaan en
opvragen. Variabelen zorgen ervoor dat je het RAM geheugen kunt
gebruiken als een soort apothekerskast. Elke la in de kast krijgt een
naam en een inhoud (die noemen we "waarde").

## Voorbeeld

```php
// opslaan (in RAM)
$city = 'Maastricht';
    
// op het scherm weergeven
echo $city;
    
// nieuwe waarde toekennen
$city = "Groningen";
```

## Externe documentatie
De officiële PHP documentatie mbt variabelen vind je op:

https://www.php.net/manual/en/language.variables.basics.php
