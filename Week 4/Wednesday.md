## Distance to zero

Make a program that asks for 5 values ​​and also allows us to know which one is furthest from zero, once obtained it returns that number (the numbers can be negative), showing only the integer part of the number.

### Solution:

[![Distancetozerow4.png](https://i.postimg.cc/sfJJTpTQ/Distancetozerow4.png)](https://postimg.cc/rzKWmtXM)

## Toss Coin

From the data we receive first a name and a value, then another name and another value, using the built-in function aleatorio() 
we simulate the flip of a coin, We must return the name of the winner in capital letters and the value I win, to avoid cheating, 
if a player puts a value of zero or negative, the opponent automatically wins, in case both cheat, "game canceled" is returned.

### Solution:

``` Javascript
Algoritmo tossCoin
	Imprimir "Enter the name of the first player"
	Leer firstPlayer
	Imprimir "Enter the amount to play"
	Definir firstAmount Como Real
	Leer firstAmount 
	Imprimir "Enter the name of the second player"
	Leer secondPlayer
	Imprimir "Enter the amount to play"
	Definir secondAmount Como Real
	leer secondAmount
	
	flip = Aleatorio(1, 2)
	
	Imprimir "Flipping coins!"
	Para count = 1 Hasta 10 Hacer
		Imprimir "..."
	FinPara
	
	Si firstAmount  <= 0 | secondAmount  <= 0 Entonces
		Si firstAmount   <= 0 & secondAmount  <= 0 Entonces
			Imprimir "Game canceled because both are cheating!"
		SiNo
			Si firstAmount  <= 0 Entonces
				Imprimir  firstplayer "is cheating"
				Imprimir "Player" Mayusculas(secondPlayer) "wins, amount won: " firstAmount
			SiNo 
				Imprimir secondPlayer "is cheating"
				Imprimir "Player" Mayusculas(firstplayer) "wins, amount won: " secondAmount
			FinSi
		FinSi
	SiNo
		Si flip = 1 Entonces
			Imprimir "Player" Mayusculas(firstplayer) "wins, amount won: " firstAmount
		SiNo
			Imprimir "Player" Mayusculas(secondPlayer) "wins, amount won: " secondAmount
		FinSi
	FinSi	
FinAlgoritmo
```
