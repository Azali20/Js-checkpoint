Initialize an empty array to hold the distinct elements from both sets.
Initialize a variable sum to zero.
For each element e1 in Set 1:
Check if e1 is not already in the distinct elements array.
If e1 is not in the array, add it to the array and add e1 to sum.
For each element e2 in Set 2:
Check if e2 is not already in the distinct elements array.
If e2 is not in the array, add it to the array and add e2 to sum.
Return sum.

**Here's the implementation of the algorithm in JavaScript:

// function sumOfDistinctElements(set1, set2) {
//   const distinctElements = [];
//   let sum = 0;

//   for (const e1 of set1) {
//     if (!distinctElements.includes(e1)) {
//       distinctElements.push(e1);
//       sum += e1;
//     }
//   }

//   for (const e2 of set2) {
//     if (!distinctElements.includes(e2)) {
//       distinctElements.push(e2);
//       sum += e2;
//     }
//   }

//   return sum;
// }



We can then test for the function with the following example given in the problem statement below:


// const set1 = [3, 1, 7, 9];
// const set2 = [2, 4, 1, 9, 3];

// console.log(sumOfDistinctElements(set1, set2)); // Output: 13



SECOND PROBLEM


Define a function called dotProduct that takes two vectors as input and returns their dot product.
Define a function called isOrthogonal that takes two vectors as input and returns true if they are orthogonal, false otherwise. The function should call the dotProduct function to compute the dot product of the two vectors and return true if the dot product is zero, false otherwise.
Define two arrays v1 and v2 of length n to hold the vectors.
Use nested loops to input the elements of the vectors from the user.
For each pair of vectors, call the isOrthogonal function to determine whether they are orthogonal or not.
Print the result for each pair of vectors.


function dotProduct(v1, v2) {
    // calculates the dot product of v1 and v2 and returns it
    let ps = 0;
    for (let i = 0; i < v1.length; i++) {
        ps += v1[i] * v2[i];
    }
    return ps;
}

function isOrthogonal(v1, v2) {
    // returns true if v1 and v2 are orthogonal, false otherwise
    return dotProduct(v1, v2) === 0;
}

// main algorithm
const n = // number of vectors
const vectors = [];

for (let i = 0; i < n; i++) {
    // input elements of v1
    const v1 = [];
    for (let j = 0; j < n; j++) {
        v1.push(/* input element */);
    }

    // input elements of v2
    const v2 = [];
    for (let j = 0; j < n; j++) {
        v2.push(/* input element */);
    }

    // determine if the vectors are orthogonal
    if (isOrthogonal(v1, v2)) {
        console.log("v1 and v2 are orthogonal");
    } else {
        console.log("v1 and v2 are not orthogonal");
    }
}


In the above algorithm, the dotProduct function takes two arrays as input and returns their dot product, while the isOrthogonal function takes two arrays as input and returns true if they are orthogonal, false otherwise. The main algorithm inputs the vectors using nested loops,


