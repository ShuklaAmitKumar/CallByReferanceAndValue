# CallByReferanceAndValue
var myName = "Carlos";
function myNameIs(aName){
  aName = "Carla";
}
myNameIs(myName);
console.log(myName);

var myName1 = {};
function myNameIs1(aName){
  aName.firstName = "Carla";
}
myNameIs1(myName1);
console.log(myName1);

var myName2 = {firstName : "Carla"};
function myNameIs2(aName){
  aName = {
    lastName : "SS"
  }
}
myNameIs2(myName2);
console.log(myName2);

var myName3 = {firstName : "Carla"};
function myNameIs3(aName){
  aName.lastName = "SS"
  
}
myNameIs3(myName3);
console.log(myName3);
