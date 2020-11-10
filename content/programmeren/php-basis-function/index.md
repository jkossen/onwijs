---
title: "PHP Basis: Function"
date: 2020-09-27T21:04:58+02:00
tags: ["php", "programmeren", "softwaredeveloper", "mbo", "applicatieontwikkelaar", "25604", "25187"]
authors:
  - Jochem Kossen
---

## Onderdeel van
Deze pagina is onderdeel van het **PHP basiskennis**
onderwijsmateriaal.

Voor een overzicht, ga naar **[PHP Basis: Overzicht](../php-basis)**.

## Beschrijving

Met een functie kun je een blok code schrijven dat je meermaals kunt
aanroepen. Vaak hebben functies `input`, doen ze iets met die input,
en geven ze het resultaat terug als de `output`.

### Een voorbeeld

**LET OP** De code gaat ervan uit dat je je functies in een Class
schrijft. Doe je dat niet, laat dan het woord `public` weg.

```php
public function sayHello()
{
    echo "Hello!";
}
```

## Parameters

Bovenstaand voorbeeld laat wat zien op het scherm, maar gebruikt nog
geen `input`. Input kun je aan functies meegeven met `parameters` (ook
wel "argumenten"). Deze geef je als variabelen mee tussen de haakjes
achter de functienaam:

```php
public function sayHello($name)
{
    echo "Hello " . $name;
}
```

Meerdere parameters meegeven is mogelijk door ze te scheiden door een
komma.

## Return

Een belangrijke call binnen functies is `return`. Met `return` kun je
de `output` van je functie terugsturen naar de code die de functie
aanroept.

**LET OP**: `return` stopt de functie en stuurt het resultaat
terug. Code binnen een functie die na `return` staat wordt niet
uitgevoerd.

## De ene functie kan de andere uitvoeren

Een functie kan ook een andere functie uitvoeren. Kijk maar eens naar
onderstaande code. Kijk maar eens naar de functie `doHeadline()`:

```php
public function say($text)
{
    echo $text;
}

public function getHeadline($text)
{
    return "<h1>" . $text . "</h1>";
}

public function doHeadline()
{
    $this->say($this->getHeadline('Salvador Dali had a mustache'));
}
```

## Externe Documentatie

De officiële documentatie van PHP kun je vinden op:

https://www.php.net/manual/en/functions.user-defined.php

