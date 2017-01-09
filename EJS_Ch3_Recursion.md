My Code
```
function isEven(x) {
	if (x === 0) {
    	return true;
    }
    else if (x === 1){
    	return false;
    }
    // Account for negative values of x (input variable)
    else if (x < 0) {
    	return (isEven(Math.abs(x - 2)));
    }
    else {
    	return isEven(x - 2);
    }
}
console.log(isEven(50));
// → true
console.log(isEven(75));
// → false
console.log(isEven(-1));
// → ??
```

Author's Solution
```
function isEven(n) {
  if (n == 0)
    return true;
  else if (n == 1)
    return false;
  else if (n < 0)
    return isEven(-n);
  else
    return isEven(n - 2);
}


console.log(isEven(50));
// → true
console.log(isEven(75));
// → false
console.log(isEven(-1));
// → false
```
