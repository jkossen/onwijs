---
title: "PHP Basis: if statement"
date: 2020-11-09T14:00:58+02:00
tags: ["php", "programmeren", "softwaredeveloper", "mbo", "applicatieontwikkelaar", "25604", "25187"]
authors:
  - Jochem Kossen
overview: "../php-basis"
---

## Slides

![if-statement](php-basis-if-1.png)

Net zoals je in een autorit keuzes kunt maken welke richting je op
wilt gaan (is je eindbestemming Londen? Ga dan links. Is je
eindbestemming Parijs? Ga dan rechts) kun je in je computerprogramma
verschillende stukken code aanspreken op basis van keuzes.

Dit kunnen bijvoorbeeld keuzes op basis van gebruikersinvoer zijn ("**Als** de gebruiker het geluid aanzet piept het programma als je een toets indrukt").

Een ander voorbeeld is op basis van de situatie (**als** het na 18:00 is zegt het programma "goedenavond").

Een beslisboom is een ander voorbeeld waarvoor je een if-statement kunt gebruiken:

![if-statement](php-basis-if-2.png)

### Downloads

[[pdf](php-basis-if.pdf)] [[pptx](php-basis-if.pptx) (bronbestand)]

## Beschrijving

Je ziet dat in de tekst bij de slides dat **als** vetgedrukt is. Dit soort keuzes in je programma maak je namelijk meestal met behulp van de engelse vertaling van als: `if`.

Nog een paar voorbeelden: Bij een game kan het zijn dat je pas naar
een volgend level mag **als** je het vereiste puntenaantal bereikt
hebt. Een rij-examen mag je pas aanvragen **als** je 17 jaar oud bent.

### Voorbeeldcode

Met een if statement kun je ook meerdere situaties van elkaar onderscheiden. Is de gebruiker ouder dan 12? Doe dan actie 1. Is de gebruiker ouder dan 16? Doe dan actie 2. Is de gebruiker ouder dan 18? Doe dan actie 3. Enzovoort.

In code ziet dat er in PHP als volgt uit:

```php
$age = 13;

if ($age >= 18) {
    echo "U heeft toegang tot de volledige site";
} elseif ($age >= 16) {
    echo "Je hebt toegang tot een gedeelte van de site";
} elseif ($age >= 12) {
    echo "Je hebt toegang als er een ouder/verzorger aanwezig is";
} else {
    echo "Sorry, deze site is voor iedereen van 12 jaar en ouder";
}
```
## Externe Documentatie

De officiële documentatie mbt if-statements vind je op:

https://php.net/if

