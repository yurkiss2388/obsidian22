spread - разворачивает объекты и массивы   
rest - остаток 

***spread
1 применение :
```js 
const normalWork = ["инженер", "деловод","токарь"]
const work ={...normalWork,"блогер", "инста модель"};
console.log(work);
```

2 применение :
```js
const worker = {
	"name" : "Yura"
	"job" : "front"
}

const SlySoft = {
	...worker,
	"position" : "Jun"
}
console.log(SlySoft);
```

***rest

применение:

```js
const num = (...args) => args;
console.log(num(1,2)); //можно вызвать с любым количеством аргументов 
```


