Given the string, check if it is a palindrome.

```javascript

function checkPalindrome(inputString) {
     var l = inputString.length;
    for (var i = 0; i < l / 2; i++) {
        if (inputString.charAt(i) !== inputString.charAt(l - 1 - i)) {
            return false;
        }
    }
    return true;
}    
```
