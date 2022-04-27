## Simple Pig Latin
function pigIt(str){
  //Code here
  let newArr = [],
      strArr = str.split(" ")
  strArr.forEach(x => {
    let wordArr = x.split("")
    wordArr.push(wordArr[0], 'ay'), wordArr.shift()
    if(x === "!" || x === "?" || x === "."){
      newArr.push(x)
    }else{
      newArr.push(wordArr.join(""))
    }
  })
  return newArr.join(" ")
}

## Counting duplicates
function duplicateCount(text){
  return text.toLowerCase().split('').filter(function(val, i, arr){
    return arr.indexOf(val) !== i && arr.lastIndexOf(val) === i;
  }).length;
}

## Decode the Morse Code
decodeMorse = function(morseCode){
  return morseCode
    .trim()
    .split(/  | /)
    .map( (code) => MORSE_CODE[code] || ' ')
    .join('');
}
