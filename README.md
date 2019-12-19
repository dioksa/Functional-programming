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

<strong>Explanation</strong> 

'map' takes each element of array and do some actions, in our case it multiply each element by two

<h3>Example 2:</h3>

```
let possibleNumbers = ["1", "2", "three", "///4///", "5"]

let mapped = possibleNumbers.map (Int.init)
```

<i>print([Optional(1), Optional(2), nil, nil, Optional(5)]) /// -> returns array with optional Int-s and nil values</i>
