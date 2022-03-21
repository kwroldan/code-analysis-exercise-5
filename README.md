# Programming Exercise

Your task is to figure out how this code works.

* Come with a test input for the function.
* Trace the flow of the program with your test input **without running the code**, keeping track of all of the variables and transformations until you can determine the output.
* Keep coming up with new inputs until you're confident until you're confident that you know how the function works.
* Write a summary of what the function does.

*SUMMARY*
1) The function takes some string input.
2) The function creates a blank string called `answer`, and uses the `for...in` loop to return the index of each character in the string. 
3) The function checks if one of the characters in the string is a period `.` and if it's not, it assigns `newCharacter` to be equal to `character` (which would be the index of the string).
4) The function concatenates each iteration of `newCharacter` and assigns it to the variable `answer`. 
5) The function returns the answer. 

```js
function (string){
  let answer = ""
  for (character in string) {
    let newCharacter = "-"

    if (character !== "."){
      newCharacter = character
    }

    answer += newCharacter
  }

  return answer
}
```

| Input | Output |
| ----- | ------ |
| "Hey" | "012"  | 
|"Help" | "0123" | 
|"Why?" | "0123" | 

<table>
  <tr>
    <th>What does this program do?</th>
    <td>The program takes input string and converts it to index and returns it as output string.</td>
  </tr>
</table>

## Rubric

* Contains a plausible collection of test cases
* Outputs are accurately derived from inputs
* Summary is plausible
