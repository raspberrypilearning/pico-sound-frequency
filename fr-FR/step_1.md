Tu peux créer des effets sonores intéressants et ennuyeux en jouant des sons courts à différentes fréquences.

Nous entendons différentes fréquences comme différentes notes de musique, tonalités ou hauteurs.

Cet exemple augmente progressivement la fréquence pour créer un son positif :

--- code ---
---
language: python
---
def gagner(): # fréquence croissante
    for i in range(2000, 5000, 100): 
        haut_parleur.play(i, 0.05) # courte durée

--- /code ---

Cet exemple diminue la hauteur pour créer un son de gazouillis d'oiseau :

--- code ---
---
language: python
---
def gazouiller(): # séries de gazouillis aigus
    for _ in range(2): # fréquence décroissante
        for i in range(5000, 2999, -100):
            haut_parleur.play(i, 0.02) # très courte durée
        sleep(0.2)
 --- /code ---

 Joue en jouant des notes courtes et en changeant la fréquence dans une boucle `for`. Utilise des fréquences entre `150` et `10000`. 
