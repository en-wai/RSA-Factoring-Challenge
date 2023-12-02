# Solution to RSA-Factoring-Challenge

## Algorithm

Here's a step-by-step algorithm in plain English for the given task:

1. **Read the Input File:**
   - Accept the input file path as a command-line argument.
   - Open the file and read each line, converting the content to a list of natural numbers.

2. **Factorization Function:**
   - Create a function `factorize(n)` that takes a natural number `n` as input.
   - Iterate from 2 to the square root of `n` (inclusive).
   - For each divisor `i`, check if `n` is divisible by `i`.
   - If divisible, return the pair `(i, n // i)` as factors.
   - If no divisor is found, return `(n, 1)` indicating that `n` is a prime number.

3. **Factorize Numbers:**
   - Iterate through the list of natural numbers obtained from the input file.
   - For each number, call the `factorize` function to get its factors.
   - Print the factorization in the format `n = p * q`, where `n` is the original number, and `p` and `q` are its factors.

4. **Handle File Errors:**
   - Check for file existence and handle the case where the file is not found.
   - Ensure that the content of each line in the file is a valid natural number greater than 1.
   - If any error occurs during file processing, print an error message and exit.

5. **Run the Script:**
   - If the script is executed directly (not imported as a module), run the main function.

6. **Command Line Usage:**
   - Display a usage message if the script is not provided with the correct number of command-line arguments.

7. **Run the Script:**
   - Save the script and make it executable.
   - Run the script with the provided test file or any other input file.

This algorithm outlines the basic steps for reading input, factorizing numbers, and handling errors. You can implement each step in a programming language of your choice.