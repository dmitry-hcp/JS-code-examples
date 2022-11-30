**Write a function that takes a string and outputs a strings of 1's and 0's where vowels become 1's and non-vowels become 0's.**

**All non-vowels including non alpha characters (spaces,commas etc.) should be included.**

**Examples:**
```
vowelOne( "abceios" ) // "1001110"

vowelOne( "aeiou, abc" ) // "1111100100"
```
**Solution:**
```
function vowelOne(s){
  let vowel = ['a','e','i','o','u','A','E','I','O','U'];
    let arr = Array.from(s); 
    let res = [];
    for (i = 0; i < arr.length; i++) {
        if (vowel.includes(arr[i])) {
            res.push(1);
        } else {
            res.push(0)
        }
    }
    return res.join('');
}
```