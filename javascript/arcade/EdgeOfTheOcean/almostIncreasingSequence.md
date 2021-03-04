Given a sequence of integers as an array, determine whether it is possible to obtain a strictly increasing sequence by removing no more than one element from the array.

```javascript
function almostIncreasingSequence(sequence) {
    var bad = 0;
    for (i = 1; i < sequence.length; i++){
        if (sequence[i] <= sequence[i - 1]){
            bad++
            if(bad > 1){
                return false
            }
            if(sequence[i + 1] <= sequence[i - 1] && sequence[i] <= sequence[i - 2]){
                return false
            }
        }
    }
    return true
}
```
