# Diff-Two-Arrays

#FreeCodeCamp JavaScript Algorythms and Data structure certification

Diff Two Arrays

Compare two arrays and return a new array with any items only found in one of the two given arrays, but not both. In other words, return the symmetric difference of the two arrays.

Note: You can return the array with its elements in any order.

--- Here's the code ---

function diffArray(arr1, arr2) {
  const newArr = [];
  arr1.concat(arr2).filter(elt => {
    if(!arr1.includes(elt) || !arr2.includes(elt)){
      newArr.push(elt)
    }
  })
  return newArr
}

diffArray([1, 2, 3, 5], [1, 2, 3, 4, 5]);
