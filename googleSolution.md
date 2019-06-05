## Has Pair With Sum
```javascript
function hasPairWithSum(arr, sum) {
  let comp = {};
  for(let i = 0; i < arr.length; i++) {
    if(comp[arr[i]]){
      return true;
    } else {
      comp[sum - arr[i]] = true;
    }   
  }
  return false;
}
```
