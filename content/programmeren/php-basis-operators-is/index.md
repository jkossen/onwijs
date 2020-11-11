---
title: "PHP Basis: operators: =, == en ==="
date: 2020-11-09T14:00:58+02:00
tags: ["php", "programmeren", "softwaredeveloper", "mbo", "applicatieontwikkelaar", "25604", "25187"]
authors:
  - Jochem Kossen
---

## Onderdeel van
Deze pagina is onderdeel van het **PHP basiskennis**
onderwijsmateriaal.

Voor een overzicht, ga naar **[PHP Basis: Overzicht](../php-basis)**.

## Beschrijving

In PHP bestaan drie `operators` voor het woordje "is": =, == en
===. Maar wanneer gebruik je nu welke?

### =: toekennen

= gebruik je om een waarde op te slaan in een variabele:

```php

$country = "Atlantis";

```

In **vergelijkingen** (if-statements e.d.) gebruik je **===** of als
het moet **==**.

### === en ==: vergelijken

Wat denk je dat bij onderstaande code op het scherm getoond wordt?

```php
$a = 1;

$b = True;

if ($a == $b) {
    echo "Same";
} else {
    echo "Different";
}
```

Kennelijk hebben 1 en True dus dezelfde **waarde**. Toch zijn ze niet
identiek. Je bent een **integer** met een **boolean** aan het
vergelijken. Appels vergelijk je toch ook niet met peren?

Eigenlijk gaat deze vergelijking alleen betrouwbaar goed als beide
kanten van de vergelijking hetzelfde datatype hebben.

**Probeer eens** 0 met "" (lege string) te vergelijken. Zijn ze
gelijk? En 0 en "0"? "" en "0"?

In de meeste gevallen wil je weten of twee variabelen **identiek**
zijn. Zowel qua waarde als qua datatype. Daar gebruik je **===** voor.

```php
$a = 1;

$b = True;

if ($a === $b) {
    echo "Same";
} else {
    echo "Different";
}
```

> Dus de regel is: **gebruik ===** tenzij je een goede reden hebt om
> **==** te gebruiken.

### Ontkenning

Soms wil je niet weten of iets gelijk is aan, maar juist of iets
**niet** gelijk is aan ...

Zowel === als == kun je ook "omdraaien" met **!**:

```php
// als userId niet 1 is
if ($userId !== 1) {
    $admin = false;
} else {
    $admin = true;
}
```

## Externe Documentatie

De officiële documentatie mbt vergelijkingsoperators (comparison
operators) vind je op:

https://www.php.net/manual/en/language.operators.comparison.php
