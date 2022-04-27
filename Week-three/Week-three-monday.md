## Who likes it

function likes(names) {
  // TODO
  const likesArray = []
  
  for (const name of names){
    likesArray.push(name)
  }

  if(likesArray.length < 1){
    return "no one likes this"
  }else if(likesArray.length === 1){
    return `${likesArray[0]} likes this`
  }else if(likesArray.length === 2){
    return `${likesArray[0]} and ${likesArray[1]} like this`
  }else if(likesArray.length === 3){
    return `${likesArray[0]}, ${likesArray[1]} and ${likesArray[2]} like this`
  }else{
    return `${likesArray[0]}, ${likesArray[1]} and ${likesArray.length - 2} others like this`
  }
}

## Bit Counting

var countBits = function (n) {
    return n
      .toString(2)
      .split('')
      .reduce((Acc, currValue) => Acc + Number(currValue), 0);
  };

## Your order, please
function getWordNumber(word) {
  for (let i = 0; i < word.length; i++) {
    if (!Number.isNaN(Number(word[i]))) return word[i];
  }
}

function cleanUndefined(array) {
  let result = [];
  for (let i = 0; i < array.length; i++) {
    if (array[i] != undefined) result.push(array[i]);
  }
  return result;
}

function order(words) {
  let sortedArray = [];
  let wordsArray = words.split(' ');
  for (let i = 0; i < wordsArray.length; i++) {
    let wordNumber = getWordNumber(wordsArray[i]);
    sortedArray[wordNumber] = wordsArray[i];
  }
  return cleanUndefined(sortedArray).join(' ');
}
