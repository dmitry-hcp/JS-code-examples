This kata is about multiplying a given number by eight if it is an even number and by nine otherwise.  
  
**Solution:**
```
function simpleMultiplication(number){
    if(number % 2) {
      return number * 9
    } else {
      return number * 8
    }  
}
```