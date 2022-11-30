Simple, remove the spaces from the string, then return the resultant string.  
  
**Solution:**
```
function noSpace(x){
  x = Array.from(x);
    for (let i = 0; i < x.length; i++) {
        if (x[i] === ' ') {
            x[i] = '';
        }
    }
    let str = x.join(''); 
    return str;
}
```