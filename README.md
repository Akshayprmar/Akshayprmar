## Interview Question :-

Q:1:

```
let race = function() {
  setTimeout(() => console.log("timeout"), 0);
  setImmediate(() => console.log("immediate"));
  process.nextTick(() => console.log("nextTick"));
  console.log("current event loop");
}
race()
```
O/P:
```
current event loop
nextTick
timeout
immediate
```

Q2: Find Target Value
```
function findPair(array,target){
  array.sort(function(a,b){return a-b})
  console.log(array)
  let firstIndex=0
  let lastIndex =array.length-1
  let finalArray=[]
  while(firstIndex<lastIndex){
      let sum =array[firstIndex]+array[lastIndex]
      console.log("sum",sum)
      if(sum===target){
          finalArray.push(`${array[firstIndex]},${array[lastIndex]}`)
          console.log("target",sum)
          firstIndex++
          lastIndex--
      }else if(sum<target){   
          firstIndex++
          console.log("firstIndex",firstIndex)
      }else{
          lastIndex--
          console.log("lastIndex",lastIndex)
      }
  }
    console.log(finalArray) 
}

findPair([1,2,3,4,5,6,7,9],10)
```

