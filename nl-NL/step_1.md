Je kunt interessante en irritante geluidseffecten maken door korte geluiden op verschillende frequenties af te spelen.

We horen verschillende frequenties als verschillende muzieknoten, tonen of toonhoogtes.

Dit voorbeeld neemt geleidelijk toe in frequentie om een positief geluid te creëren:

--- code ---
---
language: python
---
def win(): # rising frequency for i in range(2000, 5000, 100): speaker.play(i, 0.05) # short duration

--- /code ---

In dit voorbeeld wordt de toonhoogte verlaagd om een vogelgeluid te creëren:

--- code ---
---
language: python
---
def chirp(): # series of high-pitched chirps for _ in range(2): # decreasing frequency for i in range(5000, 2999, -100): speaker.play(i, 0.02) # very short duration sleep(0.2) --- /code ---

 Experimenteer met het afspelen van korte noten en het veranderen van de frequentie in een `for` lus. Je kunt waarden gebruiken tussen `150` en `10000`. 
