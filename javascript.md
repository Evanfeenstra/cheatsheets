# javascript

In javascript, variables dont have to be "typed"... but underneath, they still have a type

- Boolean: true/false
- String: 'hello'
- Number: 10
- Array: []
- Object: {}
- Function: ()=>{}

### functions
```js
// function definition
function adder(a, b){
    return a + b
}
// function call
adder(2,3) // returns 5

// this is exactly the same
var adder = (a,b) => (a + b)

// asynchronous functions
async function(){
    // you can use "await" in here
}
```

### arrays
```js
var a = [1,2,3]

a[0] // returns "1"

// loop
a.map((item,index)=>{
    console.log(item,index)
})

// filter (will return [2,3])
var b = a.filter((item,index)=>{
    return item>1
})

// sort (return a number)
a.sort((item1,item2)=> item1-item2)
```

### objects
```js
var obj = {
    hi:'hello',
    arr:[7,8],
    child:{
        name:'Evan',
        age:31,
        sayHi:function(){
            console.log('hi')
        }
    }
}

// object properties are access with dot 
obj.child.sayHi()

// OR you can use square brackets also
obj['child']['sayHi']()
```