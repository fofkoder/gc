# gc
Workshop

Link: https://bit.ly/2NdaVoO


Hvad er Python
- Hurtigt programmeringssprog.
- Kan bruges på alle typer computere
- Open Source

Basis
Tal - Python som regnemaskine
Åben din Python editor(enten IDLE eller Spyder).
+, -, /, *, %, **
Indtast: 6 + 8
Indtast: 6 * 3
Indtast: 4 / 3
Indtast: 8 % 6
Indtast: 5 ** 3

Strings 
Indhold af tegn.
Inddeles med et quatation mark: “ eller ‘
Indtast: “Dette er en string”
Indtast: “6 + 8”
Indtast: “7 æbler, 5 appelsiner og 3 poser slik”
Indtast: “%&&# gkjgrYK !356#%/()?”
Indtast: “Hej” + “Python”
Indtast: “Hej” + “ “ + “Python”
Indtast: “Hej” * 5
Indtast: print(“Hej Python”)

Variabler
Indtast: x = “Dette er en string”
Indtast: print(x)
indtast: y = “Hej ”+ “Python”
indtast: print(y)
indtast: print(y + “. ” + x)
Indtast: z = 5
indtast: z + 10
indtast: a = z + 10
Indtast: a
Indtast: a + z
Indtast: a + a

Input
Indtast: input(“Hvad er dit navn?”)
navn = input(“Hvad er dit navn?”)
print(navn)
print(“Hej “ + navn)

Kommentarer
# Dette er en kommentar
# Vores program læser ikke kommentarer

Vores første program
# Dette program siger hej + dit navn og alder
print("Hej ukendte!")
navn = input("Hvad hedder du?")
print("Tak " + navn)
print("Hvor gammel er du? " + navn)
alder = input()
print("Du er " + alder + " " + "år," + navn)


Loops
Loops
Et loop afgør hvor længe et program skal kører.
- for loop = sat til et bestemt antal gange et program skal kører
- while loop = stopper programmet, når brugeren fx skriver “quit” og er derfor bestemt ud fra brugerens kommandoer.

 for loops
# Looper 10 gange
for i in range(10):
    print(i)

Starter fra 1 og slutter inden 11    
for i in range(1, 11):
    print(i)


# Starter fra 0, slutter inden 101 og springer 5 tal over    
for i in range(0, 101, 5):
    print(i)
    
Turtle grafik
from turtle import *

for i in range(500): #For loop loops i from 500 times, counting from 0 - 499
	forward(i) 
	left(90) 
	hideturtle() 
    speed(0)
    
for i in range(50, 400):
    forward(i)
    left(90)
    hideturtle()
    speed(0)
    
for i in range(70, 500, 10):
    forward(i)
    left(90)
    hideturtle()
    speed(0)
    



# Ændring af vinkel
    
for i in range(500):
	forward(i) 
	left(91) 
	hideturtle() 
    	speed(0)   

for i in range(200):
	circle(200)
	left(53)
	hideturtle()
    	speed(0)

Random
Random kan fx danne vilkårlige tal

Indtast:
import random
random.randint(1, 200)
random.randint(1, 200)
random.randint(1, 200)








Gæt tallet
# Gæt et nummer
import random

antal_gaet = 0

nummeret = random.randint(1,20)

for gaet in range(10):
    print("Gæt et tal: ")
    mit_gaet = input()
    mit_gaet = int(gaet) # konverterer string til int.
    
    if mit_gaet != nummeret:
        print("Forkert")
        
        
    if mit_gaet == nummeret:
        break
    
if mit_gaet == nummeret:
    gaet = str(gaet + 1)
    print("Godt klaeret! " + "Du gættede nummeret på " + gaet + " forsøg!")
    
if mit_gaet != nummeret:
    nummeret = str(nummeret)
    print("Det rigtige nummer var " + nummeret)


# while loop
# Stopper ved instruktion

tal = 1        
while tal <= 20:
    print(tal)
    tal +=1 # tallet adderes med 1 for hvert nyt loop
print(tal)



by_var = "Hvilken by har du besøgt?"
by_var += "Tryk Q for at afslutte programmet. "

while True:
    by = input(by_var)

    if by == "q":
        break
    else:
        print("Jeg har været i " + by + ".")



Lister
- En liste indeholder data
- starter fra 0
Indtast: 
min_liste = [1, 4, 6, 8, 10, 20]
print(min_liste)
print(min_liste[0])
print(min_liste[1])
print(min_liste[2])
print(min_liste[-1])
print(min_liste[20])


# Yatzee
import random

keep_going = True
while keep_going:
    dice = [0, 0, 0, 0, 0]
    for i in range(5):
        dice[i] = random.randint(1,6)
    print("You rolled:", dice)
    dice.sort()
    if dice[0] == [4]:
        print("Yatze")
    elif (dice[0] == [3]) or (dice[1] == dice[4]):
        print("Four of a kind")
    elif (dice[0] == [2]) or (dice[1] == dice[3]) or (dice[2] == dice[4]):
        print("Three of a kind")
    keep_going = (input("Hit enter to keep going, any key to exit: ") == "")      
