[Refrence Video](https://www.youtube.com/watch?v=SHINoHxvTso&list=PLlasXeu85E9cQ32gLCvAvr9vNaUccPVNP&index=16)

### Function Statement (aka Function Declaration)
```js
function myFunction(){
	console.log("It is function statement")
}
```

### Function Expression
```js
var myFunc = function(){
	console.log("It is function expression")
}
```

- The difference between `Function Statement` and `Function Expression` is **[[Hoisting]]**. The statement will have full function stored during the first run and the expression will have `undefined` value in Global Context.
- So due to hoisting if we try to call a function before declaring them `statement` will run just fine but `expression` will give us an error.
```js
a() // log : It is function statement
b() // Error: b is undefined

// Function Statement 
function a(){
	console.log("It is function statement")
}

// Function Expression 
var b = function(){
	console.log("It is function expression")
}
```


### Anonymous Function
- A function without a name is known as anonymous function.
- Ecma script donot allow us to declare an anonymous function.
- I can be used where function is treated like a values.
For Eg. 

- It can be assignment to a variable 
```rb
var b = function(){
	console.log("anonymous function assignment to a variable")
}
```

- It can be passed as a parameters
```js
setTimeout(function (){
console.log("This is an anonymous function")
}, 5000);
```

### First Class Function 
- In JS we can pass function in another function as argument.
- The ability to pass funtion as paramenter is known as first class function.
- It can also be refered as **First Class Citizen**.
