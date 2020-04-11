# Find-the-missing-letter
/*method that takes an array of consecutive
 (increasing) letters
 as input and that returns the missing
 letter in the array.*/
function findMissingLetter(array) {
var string = array.join('');
for(var i = 0; i < string.length; i++){
if(string.charCodeAt(i +1) - string.charCodeAt(i) !=1){
return String.fromCharCode(string.charCodeAt(i) + 1);
}}}
findMissingLetter(['a','b','c','d','f'])
