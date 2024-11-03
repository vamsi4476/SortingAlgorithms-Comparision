# Sorting Algorithm Comparisons

This Java program compares the performance of various sorting algorithms by measuring the number of comparisons required to sort arrays of increasing sizes. The algorithms included are:

- Insertion Sort
- Quick Sort
- Shell Sort with different gap sequences (Shell, Hibbard, Knuth, Gonnet, Sedgewick)
- Heap Sort
- Merge Sort

It also calculates the theoretical `N log N` value for each array size, providing a comparison with expected time complexity.

## Features

- **Comparison of Sorting Algorithms**: Measures the number of comparisons made by each sorting algorithm on arrays of different sizes.
- **Gap Sequences for Shell Sort**: Includes several gap sequences (Shell, Hibbard, Knuth, Gonnet, and Sedgewick) to observe their impact on Shell Sort performance.
- **N log N Calculation**: Computes `N log N` for each array size, showing a theoretical baseline for comparison.
- **Detailed Output**: Outputs the comparison counts for each algorithm and array size, allowing for analysis and comparison.

## Project Structure

- `Assignment5_final.java`: Main class that implements sorting algorithms and comparison counting.
- Sorting Methods:
  - **Insertion Sort**: Simple sorting algorithm for comparison.
  - **Quick Sort**: Recursive divide-and-conquer algorithm.
  - **Shell Sort**: Implemented with different gap sequences.
  - **Heap Sort**: Sorting based on binary heap data structure.
  - **Merge Sort**: Divide-and-conquer sorting algorithm.

## Sorting Algorithms and Methods

### Insertion Sort
A basic sorting algorithm that builds the sorted array one element at a time.

### Quick Sort
Uses a pivot to partition the array into smaller parts, then recursively sorts each part. The `partition` method selects a pivot and arranges elements around it, and the `quickSort` method recursively applies the sort.

### Shell Sort
An optimization of insertion sort that uses gap sequences to sort elements. Various gap sequences are implemented:
- **Shell**: Divides array based on halving.
- **Hibbard**: Sequence of the form `2^k - 1`.
- **Knuth**: Sequence of the form `(3^k - 1) / 2`.
- **Gonnet**: Sequence that reduces by approximately a factor of 2.2.
- **Sedgewick**: Combination of powers of 4 and 2 for gaps.

### Heap Sort
Transforms the array into a binary heap, then extracts elements one by one, maintaining the heap property with `heapify`.

### Merge Sort
A recursive sorting algorithm that divides the array, sorts each half, and merges them.

## Installation and Execution

1. **Compile the Program**:
   `javac Assignment5_final.java`

2. **Run the Program**:
   `java Assignment5_final`

3. **Output**:
   The program will print the comparison counts for each sorting algorithm for arrays of different sizes. It also calculates and displays the value of `N log N` for each size.

## Key Methods and Functions

- `generateRandomArray(int size)`: Generates an array of random integers of the specified size.
- `quickSort(int[] arr, int low, int high)`: Implements Quick Sort using the `partition` method.
- `shellSort(int[] arr, String sequenceType)`: Sorts an array using Shell Sort with different gap sequences.
- `heapSort(int[] arr)`: Sorts an array using Heap Sort and `heapify`.
- `mergeSort(int[] arr, int l, int r)`: Sorts an array using Merge Sort and the `merge` method.
- `calculateNLogN(int n)`: Computes the theoretical `N log N` value for a given size `n`.

## Example Output

The program will output the number of comparisons for each sorting algorithm and array size. Example output for array sizes of 1000 to 10000:

Array size: 1000 <br /> 
Insertion Sort comparisons: 262474  <br /> 
Shell Sort (shell) comparisons: 7406 <br /> 
Shell Sort (Hibbard) comparisons: 6963 <br /> 
Shell Sort (Knuth) comparisons: 8785 <br /> 
Shell Sort (Gonnet) comparisons: 7074 <br /> 
Shell Sort (Sedgewick) comparisons: 7406 <br /> 
Heap Sort comparisons: 19064 <br /> 
Merge Sort comparisons: 8738<br /> 
Quick Sort comparisons: 10570<br /> 
Value of N log N : 9965.784284662086<br /> 
<br /> <br /> 
Array size: 2000<br /> 
Insertion Sort comparisons: 1000912<br /> 
Shell Sort (shell) comparisons: 19607<br /> 
Shell Sort (Hibbard) comparisons: 16545<br /> 
Shell Sort (Knuth) comparisons: 20868<br /> 
Shell Sort (Gonnet) comparisons: 14380<br /> 
Shell Sort (Sedgewick) comparisons: 19607<br /> 
Heap Sort comparisons: 42376<br /> 
Merge Sort comparisons: 19427<br /> 
Quick Sort comparisons: 23836<br /> 
Value of N log N : 21931.568569324176<br /> <br /> <br /> 

Array size: 3000<br /> 
Insertion Sort comparisons: 2230695<br /> 
Shell Sort (shell) comparisons: 26922<br /> 
Shell Sort (Hibbard) comparisons: 26732<br /> 
Shell Sort (Knuth) comparisons: 33917<br /> 
Shell Sort (Gonnet) comparisons: 21378v
Shell Sort (Sedgewick) comparisons: 26922<br /> 
Heap Sort comparisons: 67228<br /> 
Merge Sort comparisons: 30900<br /> 
Quick Sort comparisons: 39757<br /> 
Value of N log N : 34652.24035614973<br /> <br /> <br /> 

Array size: 4000<br /> 
Insertion Sort comparisons: 3972148<br /> 
Shell Sort (shell) comparisons: 44748<br /> 
Shell Sort (Hibbard) comparisons: 39190<br /> 
Shell Sort (Knuth) comparisons: 53068<br /> 
Shell Sort (Gonnet) comparisons: 29479<br /> 
Shell Sort (Sedgewick) comparisons: 44748<br /> 
Heap Sort comparisons: 92572<br /> 
Merge Sort comparisons: 42832<br /> 
Quick Sort comparisons: 55490<br /> 
Value of N log N : 47863.13713864835<br /> <br /> <br /> 

Array size: 5000<br /> 
Insertion Sort comparisons: 6239182<br /> 
Shell Sort (shell) comparisons: 63249<br /> 
Shell Sort (Hibbard) comparisons: 51463<br /> 
Shell Sort (Knuth) comparisons: 60625<br /> 
Shell Sort (Gonnet) comparisons: 39352<br /> 
Shell Sort (Sedgewick) comparisons: 63249<br /> 
Heap Sort comparisons: 119232<br /> 
Merge Sort comparisons: 55219<br /> 
Quick Sort comparisons: 77105<br /> 
Value of N log N : 61438.561897747255<br /> <br /> <br /> 

Array size: 6000<br /> 
Insertion Sort comparisons: 9056934<br /> 
Shell Sort (shell) comparisons: 63669<br /> 
Shell Sort (Hibbard) comparisons: 59608<br /> 
Shell Sort (Knuth) comparisons: 80901<br /> 
Shell Sort (Gonnet) comparisons: 69694<br /> 
Shell Sort (Sedgewick) comparisons: 63669<br /> 
Heap Sort comparisons: 146246<br /> 
Merge Sort comparisons: 67881<br /> 
Quick Sort comparisons: 96206<br /> 
Value of N log N : 75304.48071229945<br /> <br /> v

Array size: 7000<br /> 
Insertion Sort comparisons: 12305744<br /> 
Shell Sort (shell) comparisons: 76680<br /> 
Shell Sort (Hibbard) comparisons: 71142<br /> 
Shell Sort (Knuth) comparisons: 102549<br /> 
Shell Sort (Gonnet) comparisons: 55979<br /> 
Shell Sort (Sedgewick) comparisons: 76680<br /> 
Heap Sort comparisons: 173508<br /> 
Merge Sort comparisons: 80628<br /> 
Quick Sort comparisons: 109852<br /> 
Value of N log N : 89411.97444703785<br /> <br /> <br /> 

Array size: 8000<br /> 
Insertion Sort comparisons: 15926222<br /> 
Shell Sort (shell) comparisons: 101180<br /> 
Shell Sort (Hibbard) comparisons: 84543<br /> 
Shell Sort (Knuth) comparisons: 116662<br /> 
Shell Sort (Gonnet) comparisons: 65733<br /> 
Shell Sort (Sedgewick) comparisons: 101180<br /> 
Heap Sort comparisons: 201416<br /> 
Merge Sort comparisons: 93733<br /> 
Quick Sort comparisons: 133500<br /> 
Value of N log N : 103726.2742772967<br /> <br /> <br /> 

Array size: 9000<br /> 
Insertion Sort comparisons: 20294464<br /> 
Shell Sort (shell) comparisons: 114403<br /> 
Shell Sort (Hibbard) comparisons: 107676<br /> 
Shell Sort (Knuth) comparisons: 129546<br /> 
Shell Sort (Gonnet) comparisons: 75952<br /> 
Shell Sort (Sedgewick) comparisons: 114403<br /> 
Heap Sort comparisons: 229434<br /> 
Merge Sort comparisons: 106976<br /> 
Quick Sort comparisons: 148203<br /> 
Value of N log N : 118221.3835749396<br /> <br /> <br /> 

Array size: 10000<br /> 
Insertion Sort comparisons: 25041282<br /> 
Shell Sort (shell) comparisons: 143200<br /> 
Shell Sort (Hibbard) comparisons: 117111<br /> 
Shell Sort (Knuth) comparisons: 155790<br /> 
Shell Sort (Gonnet) comparisons: 94932<br /> 
Shell Sort (Sedgewick) comparisons: 143200<br /> 
Heap Sort comparisons: 258112<br /> 
Merge Sort comparisons: 120440<br /> 
Quick Sort comparisons: 182621<br /> 
Value of N log N : 132877.1237954945


