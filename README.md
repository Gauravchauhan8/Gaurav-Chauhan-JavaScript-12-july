# Gaurav-Chauhan-JavaScript-12-july
Assessment answers
Q1. var dateobj =
var dateToday = new Date('October 15, 1996 05:35:32:77 GMT+11:00');
How to fetch the millisecond according to universal time from a given Date object?

Ans1. By using function name as DateObj.getUTCMilliseconds() we are able to get the milliseconds,
Output- 77

Q2.
Write a JavaScript program to display the reading status (i.e. display book name, author
name and reading status) of the following books.
var library = [
{
author: 'Bill Gates',
title: 'The Road Ahead',
readingStatus: true
},
{
author: 'Steve Jobs',
title: 'Walter Isaacson',
readingStatus: true
},
{
author: 'Suzanne Collins',
title: 'Mockingjay: The Final Book of The Hunger Games',
readingStatus: false
}];

Ans2. If the book is already read:
Already read '<book_name>' by <author_name>.

If the book is unread:
You still need to read '<book_name>' by <author_name>.

function displayInformation() {
}
var library = [
{
author: 'Bill Gates',
title: 'The Road Ahead',
readingStatus: true
},
{
author: 'Steve Jobs',
title: 'Walter Isaacson',
readingStatus: true
},
{
author: 'Suzanne Collins',
title: 'Mockingjay: The Final Book of The Hunger Games',
readingStatus: false
}];
displayInformation();


Q3. What will be the output of the following code?
var Employee =
{
company: 'Rohit'
}
var Emp1 = Object.create(employee);
delete Emp1.company Console.log(emp1.company);

Ans3.wecannot delete a variable that declared with var.
For the deletion following command is compatible.
delete Employee.company




Q4. Consider the two functions below. Will they both return the same thing? Why or why

not?

function foo1()
{
return {
bar: "hello"
};
}
function foo2()
{return
{
bar: "hello"
};
}



Ans4. these two functions will not return the same thing. 
The reason for this has to do with the fact that semicolons are technically optional in JavaScript (although omitting them is generally really bad form). 
As a result, when the line containing the return statement (with nothing else on the line) is encountered in foo2(), a semicolon is automatically inserted immediately after the return statement.




Q5.
var arr = [2, 56, 78, 34, 65];
var new_arr = arr.map(function(num) {
return num / 2;
});
print(new_arr);
What will be the output for the above code?

Ans5. Output-1, 28, 39, 17, 32.5

Q6.
const set = new Set(['Beethoven', 'Mozart', 'Chopin', 'Chopin'])
How to delete 'Beethoven' from set?

Ans 6. By using this function set.delete('Beethoven'); we are able to perform deletion operation.



Q7. Create a nested array object called operatingSystem and add below key and values
Name - Ubuntu , version - 18.4 , license - open source


Ans7. const operatingSystem = {
    name: 'Ubuntu',
    version: 18.04,
    license: 'Open Source'
};

// Get the object key/value pairs
const entries = Object.entries(operatingSystem);

console.log(entries);


Q8.
const name = { firstName: 'Philip',
lastName: 'Fry' };
const details = {
job: 'Delivery Boy',
employer: 'Planet Express'
};
How to copy values from one object to another in above mentioned example , merge and
print them?



Ans8. by using this line of code we will able to merge const character = Object.assign(name, details);





Q9.
const gimli =
{ name: "Gimli",
race: "dwarf",
weapon: "axe",
greet: function() { return `Hi, my name is ${this.name}!`; }, };
How to access and print greet function from the above object code?

Ans9. By using this function - gimli.greet()
Output
"Hi, my name is Gimli!";
we see that the string value for the object method greet() is returned.




Q10.
Consider below as an example of constructor function where we want name and level to be
referred to a function itself, is below example correct or not? Please explain?
function Hero(name, level)
{
name = name;
level = level;
}
function Hero(name, level)
{
name = name;
level = level;
console.log(name);
}
Hero();
//If an enclosed function defines a variable with the same name as a variable in the outer scope, then there is no way to refer to the variable in the outer scope again.It does not give any output because we do not assign any value. So, this is not correct.

/*Expected output                                                                                                                       
    undefined
*/
