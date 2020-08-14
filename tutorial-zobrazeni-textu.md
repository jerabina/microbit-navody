# Zobrazení textu

## Úvod @unplugged

Cvičení vám ukaže jak naprogramovat @boardname@, aby vám zobrazoval text.

## Blok zobraz text @fullscreen

Vlož blok `||basic:zobraz text||` do smyčky `||basic:opakuj stále||`. A uprav na text který chceš zobrazit.

```blocks
basic.forever(function () {
    basic.showString("Ahoj");
})
```

## Simulátor @fullscreen

V Simulátoru si můžete rovnou ověřit že aplikace funguje.
Všimni si, že display neumí ukazovat české znaky.

## Přidání dalších bloků @fullscreen

Přidej další bloky `||basic:zobraz text||` a sleduj jak se zobrazují.

```blocks
basic.forever(function () {
    basic.showString("Ahoj");
    basic.showString("jak");
    basic.showString("se");
    basic.showString("mas");
})
```

## Závěr @fullscreen

Pokud máte hotovo, klikněte na `|Download|` a postupujte podle pokynů na obrazovce.