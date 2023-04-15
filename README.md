Prompt #4 response

uniqueness - are all elements in a string unique? returns boolean
Input = "hello"
Output = false
Input = "copyright"
Output = true

// loop through string checking if string at string[0] === string[x], x will increment by 1 
// if at any return trus, we'll exit and return false
// if index === str.length -1, then we'll return true

Edge cases
	if (typeof str !== 'string')
  if (str === "")
  
Base case 
	if (str.length === 1)
  
Input = "helLo"
Output = false
Input = "copyright"
Output = true

const index = 1;

const checkUnique = (str) => {
	return (index) => {
  
  if (typeof str !== 'string') {
  	return;
  } else if (str === "") {
  	return;
  } else if (str.length === 1) {
  	return true;
  }	else if (str[0] === str[index] || str[0] === str[index].toLowerCase || str[0] === str[index].toUpperCase {
  	return false;
  }	else if (index === str.length - 1) {
  	return checkUnique(str.substring(1))(1);			// "hello" "ello" "llo"
  } else {
  	return checkUnique(str)(index+1);
  }
}