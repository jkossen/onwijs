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

![RAM geheugen als apothekerskast](php-basis-variabele-3.png)

### Downloads

[[pdf](php-basis-variabele.pdf)] [[pptx](php-basis-variabele.pptx) (bronbestand)]

## Beschrijving
Met behulp van variabelen kun je gegevens in het RAM geheugen opslaan en opvragen. Je kunt variabelen en het RAM geheugen vergelijken met het gebruik van een apothekerskast. Elke lade heeft een label met de **naam** van wat erin zit. In de la zelf zit de **inhoud**. Variabelen hebben ook een naam en een inhoud. Bij variabelen noem je die inhoud de **waarde**. 

## Voorbeeld

### Voorbeeld 1
```php
// sla 'Maastricht' op in de variabele $city
$city = 'Maastricht';
    
// op het scherm weergeven
echo $city;
    
// nieuwe waarde toekennen
$city = "Groningen";
```

### Voorbeeld 2
```php
$aantalStudenten = 28;

// bereken iets vanuit de ene variabele en sla de uitkomst op
// in de andere
$aantalGroepen = $aantalStudenten / 4;

echo $aantalGroepen
```

## Externe documentatie
De officiële PHP documentatie mbt variabelen vind je op:

https://www.php.net/manual/en/language.variables.basics.php
 