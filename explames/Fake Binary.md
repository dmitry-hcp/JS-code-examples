Given a string of digits, you should replace any digit below 5 with '0' and any digit 5 and above with '1'. Return the resulting string.

**Note:** input will never be an empty string  
  
**Solution:**
```
function fakeBin(x){
  x = Array.from(x);
    for (let i = 0; i < x.length; i++) {
        if (x[i] < 5) {
            x[i] = 0; 
        } else if (x[i] >= 5) {
            x[i] = 1;
        }        
    }
    let str = x.join('');
    return str;
}
``` 