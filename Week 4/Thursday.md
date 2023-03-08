## Total price

Create a function called TotalPrice that takes 2 parameters, price and VAT, and returns the price including VAT. if the price exceeds 3000 a 10 percent discount is made on the total price.

### Solution:

``` Javascript
Funcion money <- totalPrice (price, iva)
	Definir money Como Real
	ValueTotalPrice = price + ((price * iva) / 100)
	
	Si price > 3000 Entonces
		money = ValueTotalPrice - (ValueTotalPrice * 0.10)
		Imprimir "El descuento de" ValueTotalPrice "es" money
	SiNo
		money = ValueTotalPrice
	FinSi
FinFuncion

Algoritmo functionTotalPrice
	 Imprimir totalPrice(5000, 21)
FinAlgoritmo
```


## Reverse direction and size

Create a function called ReverseDirectionAndSize that takes some text as a parameter and reverses it, eg: "Hello" -> "olleH" and also reverses the letters if they are uppercase to lowercase and if they are lowercase to uppercase, it should do something. like this:

```
"HelLO" --> "olLEh"

"Leonardo" --> "ODRANOEl"

"Text" --> "TXEt"
```

[![Captura-de-pantalla-20221226-172615.png](https://i.postimg.cc/xCX36Hwm/Captura-de-pantalla-20221226-172615.png)](https://postimg.cc/TLXbwyY2)

