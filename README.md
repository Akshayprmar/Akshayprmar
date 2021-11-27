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
Q:
```
const promise1 = Promise.resolve(3)

async function abc () {
  let data = await promise1
  console.log(data) //3
  return data
}
console.log('****', abc()) //Promise { <pending> }
```
Other Topics

```
Event loop
concurrency
io
close
non blocking io
API
protocol
url Desiging
Hosting
promise and .all and fail cases
Object key finding Complexity - O(N)
HATEOAS

From <https://www.vinaysahni.com/best-practices-for-a-pragmatic-restful-api> 



Indexing
DynamoDB
Global Positionining Indexing
Single Table Desiging
IIFE
Micro Service Architecture


-OLAP and OLDP
-ideapotenstional such as GET,PUT,DELETE
- API Standard Rules
-Optimize API RESPONSE
   - DATABASE
-Caching

js
node js
react js
typescript
docker
aws
tdd- jest/jasmine/karma- equivalent
scrum environment
postgresql- DB
hands on on ds/algos
 
 
no sql db- mongo, dynamo
radis cache
kafka/ rabbit/ kinesis- msg streaming services
vue js- good to have
 
 
good to know jenkins and kubernetes
 
 
services
deployment
unit test cases- write own
closures/ scope- js
js is oops? it support oops
current trends in js
current ecma script standard
```

