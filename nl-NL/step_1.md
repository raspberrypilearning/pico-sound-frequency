Je kunt interessante en irritante geluidseffecten maken door korte geluiden op verschillende frequenties af te spelen.

We horen verschillende frequenties als verschillende muzieknoten, tonen of toonhoogtes.

Dit voorbeeld neemt geleidelijk toe in frequentie om een positief geluid te creëren:

--- code ---
---
language: python
---
def winst(): # stijgende frequentie
    for i in range(2000, 5000, 100): 
        luidspreker.play(i, 0.05) # korte duur

--- /code ---

In dit voorbeeld wordt de toonhoogte verlaagd om een vogelgeluid te creëren:

--- code ---
---
language: python
---
def tjilpen(): # reeks hoge pieptonen
    for _ in range(2): # afnemende frequentie
        for i in range(5000, 2999, -100):
            luidspreker.play(i, 0.02) # zeer korte duur
        sleep(0.2)
--- /code ---

 Experimenteer met het afspelen van korte noten en het veranderen van de frequentie in een `for` lus. Je kunt waarden gebruiken tussen `150` en `10000`. 
