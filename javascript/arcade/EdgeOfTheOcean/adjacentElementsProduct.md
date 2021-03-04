Given an array of integers, find the pair of adjacent elements that has the largest product and return that product.

```javascript
function adjacentElementsProduct(inputArray) {
    let max = -Infinity;
    for (i = 1; i < inputArray.length; i++){
        max = Math.max(inputArray[i] * inputArray[i-1], max);
    }
    return max;
}
```
