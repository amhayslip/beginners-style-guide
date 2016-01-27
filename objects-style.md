# Objects Style Guide
When writing Javascript, it's important that we have propert "style" (number of space, indentation, etc.) becuase it will make our code easier to read, and at times, it's the difference between working code and errors.

## Declaring Empty Objects
When declaring an empty object, we declare it like we would any other variable. Good and bad examples are below:

good
```javascript
var myObject = {};
```
<br>
bad - improper spacing
```javascript
var myObject={};
```
<br>
bad - improper spacing and missing semicolon
```javascript
var myObject= {}
```

## Declaring Objects with Properties

good
```javascript
var car = {
  color: "red",
  wheels: 4
};
```
<br>
bad - missing comma
```javascript
var car = {
  color: "red"
  wheels: 4
};
```
<br>
bad - properties are on the same line 
```javascript
var car = {
  color: "red", wheels: 4
};
```
<br>
good - if the object is small enough, it's fine for everything to be on the same line
```javascript
var car = { color: "red", wheels: 4 };
```
<br>

## Objects Inside of Arrays
It's common to see an "array of objects" (one array, that has several objects in it). Remember, arrays can contain anything.

good
```javascript
var cars = [
  { make: "mazda", model: "3" },
  { make: "ford", model: "F-150" },
  { make: "ferrari", model: "Spyder" }
];
```
<br>
bad - this array is too long to be on one line
```javascript
var cars = [{ make: "mazda", model: "3" },{ make: "ford", model: "F-150" },{ make: "ferrari", model: "Spyder" }];
```
<br>
bad - the objects are not indented properly and should not be on one line
```javascript
var cars = [
{ make: "mazda", model: "3" },{ make: "ford", model: "F-150" },{ make: "ferrari", model: "Spyder" }
];
```
<br>

## Declaring Object Properties by Setting Them After Creation
good
```javascript
var car = {
  color: "red",
  wheels: 4
};

car.make = "ferrari";
```
<br>
bad - no space around the <strong>=</strong> and no semicolon at the end
```javascript
var car = {
  color: "red",
  wheels: 4
};

car.make="ferrari"
```
<br>
good
```javascript
var car = {
  color: "red",
  wheels: 4
};

car['make'] = "ferrari";
```

