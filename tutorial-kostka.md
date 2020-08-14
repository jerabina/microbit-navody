# Házecí kostka

## Úvod @unplugged

Cvičení vám ukaže jak naprogramovat @boardname@, jako házecí kostku.

## Krok 1 @fullscreen

Potřebujeme 3 kusy kódu: jeden pro detekci hodů (zatřesení), druhý pro výběr náhodného čísla a třetí pro zobrazení čísla.
Vložte do editoru blok  `||input: při zatřesení||` ten vám spustí kód při zatřesení @boardname@.

```blocks
input.onGesture(Gesture.Shake, function () {
})
```

## Krok 2 @fullscreen

Vemte blok `||basic: zobraz číslo||` a vložte jej do bloku `||input: při zatřesení||` tím se vám po zatřesení zobrazí číslo.

```blocks
input.onGesture(Gesture.Shake, function () {
    basic.showNumber(0);
})
```

## Krok 3 @fullscreen

Vložte blok `||Math: náhodné číslo od 0 do 10||` do bloku `||basic:zobraz číslo||` pro výběr náhodného čísla.

```blocks
input.onGesture(Gesture.Shake, function () {
    basic.showNumber(randint(0, 10));
})
```

## Sever @fullscreen

Typická kostka ukazuje hodnoty od 1 do 6. Takže v `||Math: náhodné číslo od 0 do 10||` nezapomeňte zvolit správné minimální a maximální hodnoty!

```blocks
input.onGesture(Gesture.Shake, function () {
    basic.showNumber(randint(1, 6));
})
```

## Sever @fullscreen

Pomocí simulátoru vyzkoušejte svůj kód. Ukazuje to číslo, které jste očekávali?

## Závěr @fullscreen

Pokud máte hotovo, klikněte na `|Download|` a postupujte podle pokynů na obrazovce.