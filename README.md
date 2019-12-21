# Map(_:) -> Use map to loop over a collection and apply the same operation to each element in the collection

<h3>Example 1:</h3>

```
let arrayOfNumbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

func multiplyByTwo(_ x: Int) -> Int {
    return x * 2
}

let multiplyResult = arrayOfNumbers.map (multiplyByTwo)
```

<i>print([2, 4, 6, 8, 10, 12, 14, 16, 18, 20])</i>

<strong>Explanation:</strong> 

'map' takes each element of array and do some actions, in our case it multiply each element by two

<h3>Example 2:</h3>

```
let possibleNumbers = ["1", "2", "three", "///4///", "5"]

let mapped = possibleNumbers.map (Int.init)
```

<i>print([Optional(1), Optional(2), nil, nil, Optional(5)])</i>
    
<strong>Explanation:</strong>   

returns array with optional Int-s and nil values

<h3>Example 3:</h3>

```
struct Car {
    let name: String
    let speed: Int
}

let fastCar = Car(name: "Ferrari", speed: 380)
let slowCar = Car(name: "Some car", speed: 100)

let cars = [fastCar, slowCar]
let speedArray = cars.map { $0.speed }
```

<i>print([380, 100])</i>

<strong>Explanation:</strong> 

we created array of all cars and with the help of 'map' create another array only with speed values
