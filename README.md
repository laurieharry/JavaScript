# JavaScriptPalindromes
freecodecamp exercise

//NEEDS CLEANUP 
function palindrome(str) { 
  var str1 = str.replace(/[^0-9a-z]/gi, '').toLowerCase();//make the string alphanumeric first
  console.log(str1, "<--string1 alphanumeric");
  var str2 = str1.split('');//turn it into an array
  console.log(str2, "<--string two arr")
  
  if (str2.reverse() == str1.split()){
      console.log("TRUE");
  }//check if palindrome
  console.log(str2, "<--str2 reveresed")
  
  str2 = str2.join('')
  console.log(str2, "<--str2 joined")
  
  if(str2 == str1){ // check if it's a palindrome 
      console.log("true");
      return true;
  }else{
      console.log("false");
      return false;
  }
  
}



palindrome("eye");
//palindrome("race car");
//palindrome("eyeE29479%%)")
palindrome("_tree");
