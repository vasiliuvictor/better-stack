# better-stack
Better-stack Hello There

Steps:
1. First I define a method with one parameter 'columnName'.
2. Declare a result variable with a starting value of 0
3. Iterate over the length of the string
4. Read the character at the given position
5. Read the numerical value for the character at the step above
6. Substract the value of A character which is 65, which represents the starting point of the alphabet
7. Add the + 1 after the substraction to shift the 0 to 1, meaning if the string will contain "AA" the result will be not stucked returning 0 value
8. Return result -1 to correct the above adition.



```
function excelColumnToNumber(columnName) {
  let result = 0;
  for (let i = 0; i < columnName.length; i++) {
    const char = columnName[i];
    const charValue = char.charCodeAt(0) - 'A'.charCodeAt(0) + 1;
    result = result * 26 + charValue;
  }
  return result - 1;
}

```
