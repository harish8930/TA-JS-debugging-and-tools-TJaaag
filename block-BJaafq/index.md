function add(a,b){
return a+b;
}

function subtract(a,b){
  return a-b;
}

function test(message,callback){
try{
  callback();
  console.log(`Okay`,message)
}catch(error){
console.error(error);
console.log("X",message)
}
}

function testadd(){
let result,expected;
result = add(2,4);
expected = 6;
if(result !== expected){
  throw new Error(`${result} is not equal to ${expected}`);
}
}
test(`adding 2 and 4 `,testadd)

function testsub(){
result = subtract(20,4);
expected = 16;
if(result !== expected){
  throw new Error(`${result} is not equal to ${expected}`);
}
}

test(`subtract 20 and 4`,testsub)
