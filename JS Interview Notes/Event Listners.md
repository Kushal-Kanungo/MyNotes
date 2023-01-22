We attach a **callback** function with an event and whenever that event occurs that function is called.

```js
document.getElementById('myButton').addEventListner('click', ()=>{
	console.log("This function will be called whenever the click event will occur")
})
```


### Why do we need to remove event listeners ? 
**Ans**: 
- Event Listners are heavy means that they take high memory so it is a good practice to remove the eventlistner whener they are not required so that garbage collector can collect it.
- They do not release memory beacuse they are just waiting for the event to occur. So they cannot release memory by their own.