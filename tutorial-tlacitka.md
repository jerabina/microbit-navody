# Tlačítka

## Úvod ##

Deska @boardname@ má na sobě dvě tlačítka, označené písmeny **A** a **B**. V tomto cvičení se je naučíme používat a naprogramujeme si jednoduchý hlasovací systém.

## Obsluha tlačítek ##

Do projektu si přidejte `||input:po stisknutí tlačítka||` a všiměte si, že obsluha tlačítek je nezávislá na hlavní programové smyčce.
Můžete si vybrat, které tlačítko tento kód bude obsluhovat **A**, **B**, nebo **A+B**.

```blocks
input.onButtonPressed(Button.A, function () {
	
})
```

## Proměné a tlačítko A ##

Vytvořte proměnou `||variables:hlasovani||` a do smyčky tlačítka vložte `||variables:změň hlasovani o 1||`.

```blocks
let hlasovani = 0
input.onButtonPressed(Button.A, function () {
    hlasovani += 1
})
```

## tlačítko B ##

Do projektu si přidejte ještě jednu obsluhu tlačítka `||input:po stisknutí tlačítka||` nastavte ho na **B**.
Do jeho smyčky vložte `||variables:změň hlasovani o -1||`.

```blocks
let hlasovani = 0
input.onButtonPressed(Button.A, function () {
    hlasovani += 1
})
input.onButtonPressed(Button.B, function () {
    hlasovani += -1
})
```

## zobrazení ##
Máme hlasovací systém který nám na tlacitku **A** hlasy přičítá a na tlačítku **B** hlasy odečítá, ale nic nevidíme.
Proto si do `||basic:opakuj stále||` vložíme `||basic:zobraz číslo||` a do něj proměnou `||variables:hlasovani||`.

```blocks
let hlasovani = 0
input.onButtonPressed(Button.A, function () {
    hlasovani += 1
})
input.onButtonPressed(Button.B, function () {
    hlasovani += -1
})
basic.forever(function () {
    basic.showNumber(hlasovani)
})
```

## Simulátor ##

V Simulátoru si můžete rovnou ověřit že aplikace funguje.

## Závěr ##

Pokud máte hotovo, klikněte na `|Download|` a postupujte podle pokynů na obrazovce.
**První kdo naprogramuje** pošle svůj @boardname@ a všichni stisknou **A**, komu se lekce líbila, nebo **B** komu ne.