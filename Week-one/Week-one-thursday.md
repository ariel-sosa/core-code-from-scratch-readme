
<h2>Print special numbers</h2>

```
for (let i = 0; i <= 100; i++){
    if(i % 2 === 0){
        console.log(i)
    }
}

```
<h2>Bad code</h2>
<p>The code is not working because 'cond' is being assigned to true within the conditional, instead the comparison operator '===' might be used or alternatively you can enter just the variable name for Javascript to check whether the value is true or false </p>
<p>Revised code:</p>

```
var cond = false;

if (cond) {
  console.log('The cond variable is true');
} else {
  console.log('The cond variable is false');
}
```
<h2>Bad code 2</h2>

<p>Revised code:</p>

```
var n = 100

if(n === 100){
    console.log('This is a special number')
}else if((n < 1000 && n % 10 === 0 && n !== 100 )){
    console.log("This number is almost special")
}else{
    console.log("Just a regular number")
}
```
