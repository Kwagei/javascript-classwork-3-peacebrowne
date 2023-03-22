# Javascript Classwork #3

You are to carefully read the instructions and complete all of the PSETs below. After testing your solutions in the browser console, kindly write your code in the codeblock below each PSET. PEST 0 should serve as a guide as to how you go about writing your solutions.

0. Write a for loop that prints from 50 to 1.

    ```javascript
      for(let i = 50; i >= 1; i--){
            console.log(i)
       }
    ```

1. Write a function named `checkOrder` that takes three numbers as arguments and returns "Increasing" if the numbers are in increasing order, "Decreasing" if the numbers are in decreasing order, and "Neither" if the numbers are neither increasing nor decreasing.

    ```javascript
        function checkOrder(num1, num2, num3){
    
            if(num1 < num2 & num2 < num3){
                return'Increasing'
            }else if(num1 > num2 & num2 > num3){
                return'Decreasing'
            }else{
                return'Neither'
            }

        }
    ```

2. Write a JavaScript function that takes three numbers as arguments and returns the largest number.

    ```javascript
    function largestNumber(num1, num2, num3){
    
        if(num1 > num2 && num1 > num3){
            return num1
        }else if(num2 > num1 && num2 > num3){
            return num2
        }else if(num3 > num1 && num3 > num2){
            return num3
        }
        else{
            return num1, num2, num3
        }
    }
    ```

3. Create an object representing a person with the following properties: name, age, and occupation.

```javascript
    const person = {
        name: 'Peace Browne',
        age: 17,
        occupation: 'Student'
    }
```

4. Add a new property to the object created in Problem Set 3, representing the person's email address.

```javascript
    person.email = 'peacebrowne@gmail.com'
```

5. Write a function that takes an array of integers as input and returns the sum of all the integers in the array. Use a for loop to iterate over each element in the array and add it to a running total. Return the total at the end of the loop.

```javascript
    function sumArray(items){

        let sum = 0;

        for(let i = 0; i < items.length; i++){
            sum += items[i]
        }

        return `Running Total: ${sum}`;
    }
```

6. Write a function that takes an integer as input and returns a string representing a multiplication table for that number from 1 to 10. Use a for loop to iterate over the numbers 1 through 10 and multiply each number by the input integer. Add each result to a new string in a formatted table. Return the table string at the end of the loop.

```javascript
    function timesTable(n){

    let table = ";
    for (let i = 1; i <= 10; i++) {

        table += ` ${n} x ${i} = ${n * i} \n`
        
    }

    return table
}
```

7. Print even numbers between 1 and 20 using a for loop.

```javascript
    function evenNumbers(){
        for (let i = 1; i <= 20; i++) {
            
            if(i % 2 === 0){
                console.log(`Even: ${i}`)
            }
            
        }
    }
```

8.  Create an object representing a shopping cart with properties such as items and totalPrice. Also, add methods for adding items and calculating the total price.

```javascript
const shoppingCart = {

    items: [],

    totalPrice : 0,

    calculateTotalPrice: function(){

        for (let i = 0; i < this.items.length; i++) {

            const price = this.items[i].price
            this.totalPrice += price;

        }

        return this.totalPrice;
    },

    addItems: function(name,cost){
        this.items.push({
            item: name,
            price: cost
        })
    }

}

```
9. Create an object representing a calculator with methods for addition, subtraction, multiplication, and division.

```javascript
const calculator = {
    addition: function(n1,n2){
        returnn1 + n2;
    },
    subtraction: function(n1,n2){
        returnn1 - n2;
    },
    multiplication: function(n1,n2){
        returnn1 * n2;
    },
    division: function(n1,n2){
        returnn1 / n2;
    }
}

```

10. Write a function named `fizzBuzz` that prints from 1 - 100 and prints "Fizz" if the number is divisible by 3, "Buzz" if the number is divisible by 5, "FizzBuzz" if the number is divisible by both 3 and 5, and the number itself if none of these conditions are met.

```javascript
function fizzBuzz(){
    for (let i = 1; i <= 100; i++) {
        if(i % 3 === 0 && i % 5 === 0){
            console.log('fizzbuzz')
        }else if(i % 3 === 0){
            console.log('fizz')
        }else if( i % 5 === 0){
            console.log('fuzz')
        }else{
            console.log(i)
        }
    }
}

```

11. Create an object representing a car with properties such as make, model, and year. Also, add a method that returns the car's make and model.

```javascript
// Example
const car = {
    make: 'Honda',
    model: 'Civic',
    year: 2023,
    getMakeAndModel: function(){
        return `Output: ${this.make} ${this.model}`;
    }
}

console.log(car.getMakeAndModel()); // Output: 'Honda Civic'
```
