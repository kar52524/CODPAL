# CODPAL
cp
function printNthDigitOfPi(n) {
  // Check if n is a valid number
  if (typeof n !== 'number' || n < 0) {
    console.error('n must be a positive number');
    return;
  }

  // Get the value of Pi
  const pi = Math.PI;

  // Convert the value of Pi to a string
  const piString = pi.toString();

  // Check if the nth digit exists
  if (piString.length < n) {
    console.error('n is too large');
    return;
  }

  // Get the nth digit of Pi
  const nthDigit = piString[n];

  // Print the nth digit of Pi
  console.log(`The ${n}th digit of Pi is ${nthDigit}`);
