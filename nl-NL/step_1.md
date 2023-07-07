You can make interesting, and annoying, sound effects by playing short sounds at different frequencies.

We hear different frequencies as different musical notes, tones or pitches.

This example gradually increases in frequency to create a positive sound:

--- code ---
---
language: python
---
def win(): # rising frequency for i in range(2000, 5000, 100): speaker.play(i, 0.05) # short duration

--- /code ---

This example decreases the pitch to create a bird chirping sound:

--- code ---
---
language: python
---
def chirp(): # series of high-pitched chirps for _ in range(2): # decreasing frequency for i in range(5000, 2999, -100): speaker.play(i, 0.02) # very short duration sleep(0.2) --- /code ---

 Play around with playing short notes and changing the frequency in a `for` loop. Use frequences between `150` and `10000`. 
