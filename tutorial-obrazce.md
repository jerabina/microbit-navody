# Blikající obrázek

## Úvod @unplugged

Naučte se používat LED diody a udělat blikající obrázek!

## Krok 1 @fullscreen

Umístěte blok `||basic:ukaž tvar||` do bloku `||basic:opakuj stále||` a nakreslete obrázek.

```blocks
basic.forever(function () {
    basic.showLeds(`
        . # . # .
        # # # # #
        # # # # #
        . # # # .
        . . # . .
        `)
})
```

## Krok 2 @fullscreen

Umístěte další blok `||basic:ukaž tvar||`. Můžete jej nechat prázdný, nebo cokoliv nakreslit.

```blocks
basic.forever(function () {
    basic.showLeds(`
        . # . # .
        # # # # #
        # # # # #
        . # # # .
        . . # . .
        `)
    basic.showLeds(`
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        . . . . .
        `)
})
```

## Simulátor @fullscreen

V Simulátoru si můžete rovnou ověřit že aplikace funguje.

## Závěr @fullscreen

Pokud máte hotovo, klikněte na `|Download|` a postupujte podle pokynů na obrazovce.