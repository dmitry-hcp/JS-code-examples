**Write a function that returns only the decimal part of the given number.**

**You only have to handle valid numbers, not Infinity, NaN, or similar. Always return a positive decimal part.**

**Examples**
```
getDecimal(2.4)  === 0.4
getDecimal(-0.2) === 0.2
```
**Solution:**
```
function getDecimal(n){
  n = String(n);
    if (n.indexOf('.') === -1) {
        return 0;
    } else {
        let pos = n.indexOf('.');
        let substr = n.slice(pos);
        return +substr;
    } 
}
```