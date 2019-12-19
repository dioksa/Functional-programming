Map(_:) -> Use map to loop over a collection and apply the same operation to each element in the collection

// Example 1:

let arrayOfNumbers = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]

func multiplyByTwo(_ x: Int) -> Int {
    return x * 2
}

let multiplyResult = arrayOfNumbers.map (multiplyByTwo)
/// print([2, 4, 6, 8, 10, 12, 14, 16, 18, 20])

// 'map' takes each element of array and do some actions, in our case it multiply each element by two

// Example 2:
let possibleNumbers = ["1", "2", "three", "///4///", "5"]

let mapped = possibleNumbers.map (Int.init)
print(mapped) /// -> returns array with optional Int-s and nil values
