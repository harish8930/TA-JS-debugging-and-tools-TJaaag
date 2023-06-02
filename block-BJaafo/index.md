
let fullname = getFullname("Harish","Kumar");
console.log(fullname);
//let expected = "Harish kumar"

if(fullname!==expected){
  throw new Error(`${fullname} is not equal to ${expected}`)
}*/


function totalAmount(amount= 1,taxrate= 1){
let result = amount+(amount*taxrate)/100;
return result;
}

let addedtax = totalAmount(1000,5);
//console.log(addedtax);
 let expected = 1050;


 if (addedtax!== expected){
  throw new Error(`${addedtax} is not equal to ${expected}`)
 }


 if (addedtax === expected){
  throw new Error(`${addedtax} is not equal to ${expected}`)
 }


