# aaaa
A)  function sumDigits(n) {
    if (n === 0) return 0;  // Base case
    return (n % 10) + sumDigits(Math.floor(n / 10));  // Recursive case
}

// Example usage:
console.log(sumDigits(123));  // Output: 6
console.log(sumDigits(9876)); // Output: 30

B)  function power(base, exponent) {
    if (exponent === 0) return 1; // Base case
    return base * power(base, exponent - 1); // Recursive case
}

// Example usage:
console.log(power(2, 3));  // Output: 8
console.log(power(5, 0));  // Output: 1

C)  function reverseWords(sentence) {
    let words = sentence.split(" ");
    if (words.length === 1) return sentence;  // Base case
    return words.pop() + " " + reverseWords(words.join(" "));  // Recursive case
}

// Example usage:
console.log(reverseWords("Hello world"));  // Output: "world Hello"
console.log(reverseWords("I love JavaScript"));  // Output: "JavaScript love I"

D) Recursion is less efficient than iteration when recursion depth is too large which can cause stack overflow error 
   And iteration is better while finding fibonacci of large number

E)  function sumDigitsIterative(n) {
    let sum = 0;
    while (n > 0) {
        sum += n % 10;
        n = Math.floor(n / 10);
    }
    return sum;
}

// Example usage:
console.log(sumDigitsIterative(123));  // Output: 6
console.log(sumDigitsIterative(9876)); // Output: 30

   COMPARISON IS THAT ITERATIVE APPROACH IS FAST FOR LARGE NUMBERS BECAUSE IT AVOIDS STACK USAGE

 F) function reverseString(str) {
    if (str.length <= 1) return str;  // Base case
    return str[str.length - 1] + reverseString(str.slice(0, -1));  // Recursive case
}

// Example usage:
console.log(reverseString("JavaScript"));  // Output: "tpircSavaJ"
console.log(reverseString("Recursion"));   // Output: "noisruceR"
  
