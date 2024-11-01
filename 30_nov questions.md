```javascript

let arr=[75,45,67,89,66]
arr.forEach((ele)=>
    console.log(ele))
// create an array of ur favrt fruit and print each fruit
let fruits=["Mango","Orange","Apple"]
fruits.forEach((ele)=>
    console.log(ele))

// given an array  of num [1,2,3,4,5], access and print the third element
arr=[1,2,3,4,5]
console.log(arr[2])

// array of colors , change  2nd color to blue:
color=["pink","white","red","black"];
color[1]="blue";
console.log(color)

// find & print length of an array
arr=[10, 20, 30, 40, 50]
console.log(arr.length)


// Create an array of animals. Add a new animal to the end, remove the first animal, and print the updated array.
animals=["Dog","Cat","Lion","Elephant"]
animals.push("Tiger")
animals.shift()
console.log(animals)

//Concatenate two arrays of colors and print the resulting array.
let colorA=["green","pink","white"]
let colorB=["black","blue"]
finallist=colorA.concat(colorB)
console.log(finallist)

//  Create an array of numbers from 1 to 5. Loop through the array and print each number multiplied by 2.
let a=[1,2,3,4,5]
a.forEach((ele)=>
    console.log(ele*2))

// Check if a certain element (e.g., 3) exists in an array [1, 2, 3, 4, 5] .
[3,  4, 5]
arr=[1,2,3,4]
console.log(arr.indexOf(3)!==-1)

//: Given an array [1, 2, 3, 4, 5] , create a new array containing onlythe last three elements.
a=[1,2,3,4,5]
b=a.splice(-3);
console.log(b);

//Remove the third element from an array of names and print the updated array.
let names=["Anu","Riya","Anaisha", "anusha"]
names.splice(2,1);
console.log(names)

//: Write a function to find the maximum value in an array of numbers

a = [1, 2, 3, 4, 5];
max = a[0];
for (i = 0;  i<a.length; i++) {
    if (a[i] > max) {
        max = a[i];
    }
}
console.log(max);
 
// 2. Finding Minimum Value
a=[1,2,3,4,5,9,10,11];
min=a[0];
for(i=0;i<a.length;i++){
    if(a[i]<min){
        min=a[i];
    }
}
console.log(min);
 
 
 
// 3. Sum of Array Elements:
a = [1, 2, 3, 4, 5];
sum = 0;
for (i = 0; i < a.length; i++) {
    sum += a[i];
}
console.log(sum);
 
// 4. Average of Array Elements:
a = [1, 2, 3, 4, 5];
sum = 0;
for (i = 0; i < a.length; i++) {
    sum += a[i];
}
average = sum / a.length;
console.log(average);



/////////////////////////////string/////////////////////
//create a string

let a ='abc,def';
let b ="abc,def";
let c =`abc,def`;
console.log(typeof(a))
console.log(typeof(b))
console.log(typeof(c))

//concat st1 and str2
let s1 = "Hello, ";
let s2 = "World!";
let concatenated = s1.concat(s2);
console.log(concatenated); 

//Given a string str , find and print its length.
let s = "hello";
console.log(s.length); 

//Write a function getFirstAndLastChar(str) that returns the first and last characters of a string
function getFirstandLast(str){
    console.log(str[0]);
    console.log(str[str.length-1]);
  }
  getFirstandLast("Anusha");

// Create a function toUpperAndLower(str) that converts a string to uppercase and lowercase.
function ToUpperAndLower(str){
    console.log(str.tolowerCase())
    console.log(str.toUpperCase())
}
getToUpperAndLower("AnuSha")

/////////////////Intermediate////////////
//  Given a name variable, use a template literal to create a greeting: "Hello, [name]!" .
let name = "Anusha"
console.log(`Hello ${name}!`)
 
// : Write a function findFirstAndLast(str, char) that returns the first and last positions of a character in a string.

function findFirstAndLast(str, char) {
    let first = str.indexOf(char);
    let last = str.lastIndexOf(char);
    
    console.log(`First position is ${first}`);
    console.log(`Last position is ${last}`);
}

findFirstAndLast("banana", "a"); 
 
 
// Write a function getSubstring(str, start, end) that extracts a substring from str between the start and end indices
function getSubstring(str,start,end){
    console.log(str.substring(start,end))
}
let fname= "Anusha"
getSubstring(fname,1,5)
 


```
