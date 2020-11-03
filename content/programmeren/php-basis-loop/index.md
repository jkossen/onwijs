---
title: "PHP Basis: Loops"
date: 2020-09-27T21:04:58+02:00
tags: ["php", "programmeren", "softwaredeveloper", "mbo", "applicatieontwikkelaar"]
authors:
  - Jochem Kossen
---
[PHP Basis: index](../php-basis)

### Inleiding

Met loops kun je herhalende acties uitvoeren. Je kunt bijvoorbeeld voor elk item in een lijst (bijvoorbeeld een array) met studenten hun voornaam op het scherm tonen.

In PHP zijn drie soorten loops beschikbaar: for, foreach en while.

foreach: door een array heen lopen

Let op: veel programmeertalen hebben geen foreach, en beschikken slechts over for en while.

### Array met waarden:

```php
$gereedschapskoffer = ['hamer', 'schroevendraaier', 'boormachine'];

foreach ($gereedschapskoffer as $item) {
    echo "<li>" . $item . "</li>";
}
```

### Array met keys en waarden:

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

In PHP Basis: Arrays kun je lezen dat arrays met waarden eigenlijk ook een key hebben. Wat zou er gebeuren als je een foreach met $key => $value gebruikt in combinatie met een array met "alleen" maar waarden? Probeer het eens!


### for

tien maal 'Ik ga thuis oefenen met PHP' op het scherm tonen

```php
for ($i = 0; $i < 10; $i++) {
    echo "Ik ga thuis oefenen met PHP\n";
}
```

### while

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