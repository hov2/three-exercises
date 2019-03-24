// Valerie Ho
// Techworks Cohort 5
// March 24, 2019
// 3 Exercise Solutions

// Exercise 1

// Define a function called multiplyFive which accepts a number and returns that number multiplied by 5.

function multiplyFive (number) {
  return number * 5;
}

// Exercise 2

// Create a class called Person which accepts the name of a person as a string, and his/her age as a number. The Person class should have a method called describe which returns a string with the following syntax: "name, age years old". So for example, if John is 19 years old then the function describe of his object will return "John, 19 years old".

function Person (firstName, age) {
  this.firstName = firstName;
  this.age = age;
  this.describe = function() {
    return this.firstName + ", " + this.age + " years old";
  }
}

// Exercise 3

// Create bound copies of printFullName and printDetails to person called boundPrintFullName and boundPrintDetails.

var person = { // this time I set up a sample person
  firstName: "John",
  lastName: "Smith",
  age: "33",
  occupation: "Software Developer"
};

function printFullName () {
  console.log(this.firstName + " " + this.lastName);
}

function printDetails () {
  console.log("This person is " + this.age + " years old and works as a " + this.occupation + ".");
}

var boundPrintFullName = printFullName.bind(person); // binds printFullName function to the person object

var boundPrintDetails = printDetails.bind(person); // binds printDetails function to the person object

boundPrintFullName(); // prints out "John Smith"

boundPrintDetails(); // prints out "This person is 33 years old and works as a Software Developer."
