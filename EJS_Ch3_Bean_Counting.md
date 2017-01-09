My Code
```
// Your code here.
function countBs(str){
  var count = 0;		
  for (var i = 0; i < str.length; i++){
    	if (str.charAt(i) === "B"){
          count ++;
        }
  	}
  return count;
}


function countChar (str, letter){
 var count = 0;		
 for (var i = 0; i < str.length; i++){
    	if (str.charAt(i) === letter){
          count ++;
        }
  	}
  return count;
  
}

console.log(countBs("BBC"));
// → 2
console.log(countChar("kakkerlak", "k"));
// → 4fdhsdh
```
Author's Code
```
function countChar(string, ch) {
  var counted = 0;
  for (var i = 0; i < string.length; i++)
    if (string.charAt(i) == ch)
      counted += 1;
  return counted;
}

function countBs(string) {
  return countChar(string, "B");
}

console.log(countBs("BBC"));
// → 2
console.log(countChar("kakkerlak", "k"));
// → 4
```
  
