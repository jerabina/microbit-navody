# Kompas

Cvičení vám ukaže jak naprogramovat microbit, aby vám ukazoval, kterým směrem jsou světové strany.

## Čtení proměné z čidla kompasu ##

Ve smyčce `||basic:opakuj stále||`, ulož vstupní proměnou `||input:nasměrování kompasu (°)||` do proměné `||variables:stupne||`.

```blocks
let stupne = 0
basic.forever(function () {
    stupne = input.compassHeading()
})
```

## Sever ##

`||logic:Když||` jsou `||variables:stupne||` `||logic:menší než||` `45`, tak je směr kompasu na **sever**.
Pomocí funkce `||basic:zobraz text||` ukážeme na display @boardname@ znak `S`.

```blocks
let stupne = 0
basic.forever(function () {
    stupne = input.compassHeading()
    if (stupne < 45) {
        basic.showString("S")
    }
})
```

## Východ ##

`||logic:Jinak když||` jsou `||variables:stupne||` `||logic:menší než||` `135`, tak je směr kompasu na **východ**.
Pomocí funkce `||basic:zobraz text||` ukážeme na display @boardname@ znak `V`.

```blocks
let stupne = 0
basic.forever(function () {
    stupne = input.compassHeading()
    if (stupne < 45) {
        basic.showString("S")
    } else if (stupne < 135) {
        basic.showString("V")
    }
})
```

## Simulátor ##

Přejděte do simulátoru a otáčejte @boardname@ logem, tím budete simulovat změny kompasu.",

## Jih ##

`||logic:Jinak když||` jsou `||variables:stupne||` `||logic:menší než||` `225`, tak je směr kompasu na **jih**.
Pomocí funkce `||basic:zobraz text||` ukážeme na display @boardname@ znak `J`.

```blocks
let stupne = 0
basic.forever(function () {
    stupne = input.compassHeading()
    if (stupne < 45) {
        basic.showString("S")
    } else if (stupne < 135) {
        basic.showString("V")
    } else if (stupne < 225) {
        basic.showString("J")
    }
})
```

## Západ ##

`||logic:Jinak když||` jsou `||variables:stupne||` `||logic:menší než||` `315`, tak je směr kompasu na **západ**.
Pomocí funkce `||basic:zobraz text||` ukážeme na display @boardname@ znak `Z`.

```blocks
let stupne = 0
basic.forever(function () {
    stupne = input.compassHeading()
    if (stupne < 45) {
        basic.showString("S")
    } else if (stupne < 135) {
        basic.showString("V")
    } else if (stupne < 225) {
        basic.showString("J")
    } else if (stupne < 315) {
        basic.showString("Z")
    }
})
```

## Znovu sever ##

`||logic:Jinak||` je hodnota 315 až 360, tak budeme také ukazovat na  **sever**.
Na display @boardname@ opět zobrazíme znak `S`.

```blocks
let stupne = 0
basic.forever(function () {
    stupne = input.compassHeading()
    if (stupne < 45) {
        basic.showString("S")
    } else if (stupne < 135) {
        basic.showString("V")
    } else if (stupne < 225) {
        basic.showString("J")
    } else if (stupne < 315) {
        basic.showString("Z")
    } else {
        basic.showString("S")
    }
})
```

## Závěr ##

Pokud máte hotovo, klikněte na `|Download|` a postupojte podle pokynů na obrazovce.
Kompas potřebuje kalibraci, jak na to je k vidění v tomto videu: https://youtu.be/IL5grHtz_MU