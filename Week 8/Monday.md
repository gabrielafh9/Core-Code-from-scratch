## Training JS #7: if..else and ternary operator!
    
Complete function saleHotdogs/SaleHotDogs/sale_hotdogs, function accepts 1 parameter:n, n is the number of hotdogs a customer will buy, different numbers have different prices (refer to the following table), return how much money will the customer spend to buy that number of hotdogs.

``` Javascript
function saleHotdogs(n){
  if (n < 5) return n * 100
  else if (n < 10) return n * 95  
  else return n * 90  
}  
```

## Training JS #8: Conditional statement--switch

Complete the function howManydays. It accepts 1 parameter month, which means the month of the year. Different months have a different number of days as shown in the table below. Return the number of days that are in month. There is no need for input validation: month will always be greater than 0 and less than or equal to 12.

``` Javascript
function howManydays(month){
  var days;
  switch (month){
  case 2:
      days = 28;
      break;
  case 4:
      days = 30;
      break;
  case 6:
      days = 30;
      break;
  case 9:
      days = 30;
      break;
  case 11:
      days = 30;
      break;
  default:
      days = 31;
  }
  return days;
}
``` 

## Basic calculator

TODO: make a basic calculator. 

``` Javascript
function calculate(num1, operation, num2) {
  switch (operation){
      case '+':
      return num1 + num2;
      break;
      case '-':
      return num1 - num2;
      break;
      case '*':
      return num1 * num2;
      break;
      case '/':
      return num2 != 0 ? num1/num2 : null;
      break;
      default:
      return null;
      break;
  }
}
```

