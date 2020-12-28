---
title: "PHP Basis: Datatype"
date: 2020-09-27T21:04:58+02:00
tags: ["php", "programmeren", "softwaredeveloper", "mbo", "applicatieontwikkelaar", "25604", "25187"]
authors:
  - Jochem Kossen
overview: "../php-basis"
---

## Beschrijving

```php
// Wat denk jij dat onderstaande code op het scherm toont? 35? of 8?
echo "3" + 5;

// En deze code?
$number = 01;
echo $number;

// Deze dan?
$number = "01";
echo $number;
```

In het eerste geval proberen we 5 op te tellen bij de String "3". PHP
gebruikt de `+` operator alleen om getallen op te tellen. Doordat we
deze operator gebruiken zet PHP de String "3" automatisch om naar een
integer, want kennelijk willen we getallen optellen. De uitkomst is
dus 8.

Als er een geheel getal zonder quotes staat, zoals 01 of 1 of 100 of
0002, dan ziet PHP dat als een **integer**. Voor een integer is 01
hetzelfde als 1.

Zo heeft elke variabele een datatype. Wat je met de waarde van een
variabele kunt doen wordt bepaald door het datatype van de
variabele. Elke variabele heeft een datatype. Met een "Boolean" kun je
bijvoorbeeld aangeven of iets waar of onwaar is.

Wil je weten wat het datatype van je variabele is? Kijk eens naar de
functie `gettype`.

## Meest gebruikte datatypes

|Datatype	|Gebruikt voor	|Voorbeeld|
|-----------|---------------|---------|
|String     | Tekst         | "Jochem" (vergeet de quotes niet)|
|Integer    | Geheel getal  | 4       |
|Float      | Getal met decimalen | 4.234 |
|Boolean    | Waar/onwaar   | true of false |
|Array      | Lijst met meerdere waarden |	['zaandam', 'maastricht', 'leeuwarden'] |

## Externe Documentatie

De officiële documentatie mbt datatypes vind je op:

https://secure.php.net/manual/en/language.types.php
