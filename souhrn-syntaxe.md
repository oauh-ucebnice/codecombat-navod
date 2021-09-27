# Souhrn syntaxe z CodeCombatu

## Posílání zprávy objektu 

Syntaxe:
```
nazevObjektu.nazevZpravy();  // volám metodu "nazevZpravy"
nazevObjektu.nazevZpravy(parametry);
```

Příklady:
```java
hero.moveRight();    // volání metody bez parametru
hero.say("Hello");   // volání metody s parametrem
hero.attack(enemy);  // enemy je v tomto případě „proměnná“ (viz dále)
hero.moveRight(3);
```

> Terminologie:
> - práce s objekty: „_posíláme zprávu_ nějakému objektu“
> - programování: „_voláme metodu_ nějakého objektu“

## Vytvoření _proměnné_ (anglicky _variable_):

_Proměnné_ jsou pojmenovaná místa v&nbsp;operační paměti, do kterých můžeme ukládat informace.

Příklady:
```java
var enemy;                       //vytvořil jsem proměnnou s názvem "enemy"
enemy = hero.findNearestEnemy(); // do proměnné jsme uložili hodnotu
hero.attack(enemy);              // dosadím jako parametr hodnotu proměnné.
```

```java
var enemy = hero.findNearestEnemy();
```

Označení `hero` je také jen název proměnné. Vyzkoušejte:
```java
var franta = hero;
franta.moveRight();
```

Do proměnné můžeme uložit obsah jiné proměnné (obsah se zkopíruje):
```java
var enemy = hero.findNearestEnemy();
var karel = enemy;
hero.attack(karel);
hero.attack(enemy);
```
