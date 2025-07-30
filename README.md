# better-stack
Better-stack Hello There

Steps:
1. First I define a method with one parameter 'columnName'.
2. Declare a result variable with a starting value of 0
3. Iterate over the length of the string
4. Read the character at the given position



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
