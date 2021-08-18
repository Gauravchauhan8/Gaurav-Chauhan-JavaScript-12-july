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

Ans3.
