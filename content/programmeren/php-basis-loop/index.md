---
title: "PHP Basis: Loops"
date: 2020-09-27T21:04:58+02:00
tags: ["php", "programmeren", "softwaredeveloper", "mbo", "applicatieontwikkelaar", "25604", "25187"]
authors:
  - Jochem Kossen
overview: "../php-basis"
---

## Slides

![For loop](php-basis-loop-1.png)

### Downloads

[[pdf](php-basis-loop.pdf)] [[pptx](php-basis-loop.pptx) (bronbestand)]

## Beschrijving

Stel je voor je hebt een CSV bestand met gegevens van 42 studenten. Voor een informatiesite van school wil je van elke student bepaalde gegevens uit dit bestand weergeven.

Je zou dezelfde code 42 maal kunnen kopiëren. Want voor elke student wil je dezelfde code uitvoeren. Maar code kopiëren is iets dat programmeurs niet graag doen. Je code wordt er lang, onoverzichtelijk en gevoelig voor fouten door.

Zou het niet handig zijn als er een instructie bestond die je zou kunnen gebruiken om bepaalde code uit te voeren voor elke regel van je bestand?

Daar zijn **loops** voor bedacht. In PHP zijn drie soorten loops beschikbaar: for, foreach en while. Veel programmeertalen beschikken slechts over for en while.

Loops werken door code opnieuw uit te voeren voor elk item in iteratieve variabelen (variabelen die meerdere gegevens kunnen bevatten). In PHP is dat meestal een **[array](../php-basis-array/)**.



## foreach
### Indexed array

```php
$toolkit = ['hammer', 'screwdriver', 'drill'];

foreach ($toolkit as $item) {
    echo "<li>" . $item . "</li>";
}
```

### Associative array 

```php
$myArr = [
    'naam' => 'Epictetus',
    'leeftijd' => 24,
    'woonplaats' => 'Rome'
];

/**
 * toon elke key en waarde van $my_arr op het scherm
 */
foreach ($myArr as $key => $value) {
    echo "$key=$value\n"; // \n is een newline (volgende regel)
}
```

Wat zou er gebeuren als je een foreach met $key => $value gebruikt in combinatie met een **indexed** array? Probeer dat eens!

## for

tien maal 'Ik ga thuis oefenen met PHP' op het scherm tonen

```php
for ($i = 0; $i < 10; $i++) {
    echo "Ik ga thuis oefenen met PHP\n";
}
```

## while

zoek "Zeno" in een lijst met namen

```php
$lijst = ["Salomon", "Zeus", "Zeno", "Socrates"];
$zoek = 'Zeno';
$found = false;
$pos = 0;

while (! $found) {
    if ($lijst[$pos] === $zoek) {
        $found = true;
    }

    $pos++;
}

if ($found) {
    echo "Ja, gevonden op positie " . $pos . "!\n";
}
```

## Externe documentatie

De officiële documentatie mbt loops vind je op:

* for: https://www.php.net/manual/en/control-structures.for.php
* while: https://www.php.net/manual/en/control-structures.while.php
* foreach: https://www.php.net/manual/en/control-structures.foreach.php
