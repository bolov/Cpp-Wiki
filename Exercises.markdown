# C++ Exercises

# Table Of Contents

<!-- TOC depthFrom:1 depthTo:4 withLinks:1 updateOnSave:0 orderedList:0 -->

- [V: Variables](#v-variables)
	- [V.1 Swap](#v1-swap)
- [CF: Control Flow](#cf-control-flow)
	- [CF.Seq Operations on a sequence. Multiple Inputs](#cfseq-operations-on-a-sequence-multiple-inputs)
		- [CF.Seq.1 Product of `n` numbers](#cfseq1-product-of-n-numbers)
		- [CF.Seq.2 Average of numbers read until `0`](#cfseq2-average-of-numbers-read-until-0)
		- [CF.Seq.3 Maximum of numbers (read until end of stream)](#cfseq3-maximum-of-numbers-read-until-end-of-stream)
		- [CF.Seq Various operations on a sequence](#cfseq-various-operations-on-a-sequence)
		- [CF.Seq.4 Arithmetics](#cfseq4-arithmetics)
		- [CF.Seq.5 Min/Max](#cfseq5-minmax)
		- [CF.Seq.6 Count positives/even numbers](#cfseq6-count-positiveseven-numbers)
		- [CF.Seq.7 More odd/even](#cfseq7-more-oddeven)
		- [CF.Seq.8 Min/Max divisible by 7](#cfseq8-minmax-divisible-by-7)
		- [CF.Seq.9 Strictly increasing](#cfseq9-strictly-increasing)
		- [CF.Seq.10 Order](#cfseq10-order)
		- [CF.Seq.11 2<sup>nd</sup> Min/Max](#cfseq11-2supndsup-minmax)
		- [CF.Seq.12 Longest substring](#cfseq12-longest-substring)
		- [CF.Seq.13 Longest increasing substring](#cfseq13-longest-increasing-substring)
		- [CF.Seq.14 Count Max value](#cfseq14-count-max-value)
		- [CF.Seq.15 The largest value smaller than](#cfseq15-the-largest-value-smaller-than)
	- [CF.Dig: Digits](#cfdig-digits)
		- [Read a positive number `n`. Determine:](#read-a-positive-number-n-determine)
		- [CF.Dig.1 The number of digits](#cfdig1-the-number-of-digits)
		- [CF.Dig.2 The most significant (leftmost) digit](#cfdig2-the-most-significant-leftmost-digit)
		- [CF.Dig.3 The Sum of all the digits](#cfdig3-the-sum-of-all-the-digits)
		- [CF.Dig.4 The number or trailing `0`s](#cfdig4-the-number-or-trailing-0s)
		- [CF.Dig.5 Reverse](#cfdig5-reverse)
		- [CF.Dig.6 Palindrome](#cfdig6-palindrome)
		- [CF.Dig.7 LSD/MSD Swap](#cfdig7-lsdmsd-swap)
		- [CF.Dig.8 Lose middle digit(s)](#cfdig8-lose-middle-digits)
		- [CF.Dig.9 Reverse first half](#cfdig9-reverse-first-half)
		- [CF.Dig.10 Lose odd digits](#cfdig10-lose-odd-digits)
- [CArr: C-style arrays](#carr-c-style-arrays)

<!-- /TOC -->

# V: Variables

## V.1 Swap

Complete the following code snippet so that the variables `a` and `b`
end up with their values swapped

```
int a, b;
cin >> a >> b;

// ...

cout << a << b << endl;
```

##### Requirements

variables

##### Concepts

- variables can hold one value at a time
- this has the consequence that when you assign a new value to a variable, the old value is lost
- when you want to *save* a value for latter use, one solution is to assign it to another variable

# CF: Control Flow

All numbers should be `int`, unless specified otherwise.

## CF.Seq Operations on a sequence. Multiple Inputs

##### Requirements

Control Flow; IO (stdin, stdout); Operators; [Data Types]

##### Note

You are not allowed to store the entire sequence (e.g. in an array or vector)

### CF.Seq.1 Product of `n` numbers

First read a number `n`. Then read `n` numbers. Print the product of these `n` numbers.

##### Note

* `n` represents the number of numbers that will be input
  (`n` is the cardinal of the sequence)
* We call it `n` in the problem statement,
  but there is absolutely no need for the C++ variable in the code to be named `n`.
  Please make a distinction between the variable named in the assignments and the variables
  used in code. In code you can have `int n` or `int count` or `int number_of_numbers` that
  holds the `n` in the problem statement.<br/>
  In some situations you don't even need a C++ variable
  for the variable in the problem statement.

### CF.Seq.2 Average of numbers read until `0`

Read numbers until you read the value `0`. Print the arithmetic mean of those numbers.

##### Note

- The sentinel
    - the value `0` signals the end of the sequence
    - it is sometimes called a sentinel value
    - it doesn't necessary have to be the value `0`.<br/>
      it can be any value that cannot be part of the sequence
    - it is not part of the sequence
- this way of reading numbers (until a sentinel) is used mostly as a teaching method.
- the numbers read are of integral type. The result (average) is of floating point type.

### CF.Seq.3 Maximum of numbers (read until end of stream)

Read numbers from the standard input. Print the maximum value.

##### Note

The end of stream is signaled by `EOF` (end of file).<br/>
However `while(EOF was not read)` (pseudocode) is not a recommended way to determine if the end of stream was reached.<br/>

See the solution to this problem.<br/>
You can read here: http://stackoverflow.com/questions/5431941/why-is-while-feof-file-always-wrong
for a discussion about the problems with checking for `EOF`

### CF.Seq Various operations on a sequence

Read multiple numbers. You have 3 ways of doing this (choose one for each problem):
  - read `n` (the cardinal) first
  - read until a sentinel (e.g. `0`)
  - read until `EOF`

Perform these calculation on the input sequence:

### CF.Seq.4 Arithmetics

Compute the sum, product,  arithmetic mean, harmonic mean

### CF.Seq.5 Min/Max

Determine the minimum and the maximum value.

### CF.Seq.6 Count positives/even numbers

Count how many positive numbers and even numbers there are in the sequence

### CF.Seq.7 More odd/even

Determine if there were more even or more odd numbers.

### CF.Seq.8 Min/Max divisible by 7

Determine the maximum/minimum number divisible by 7

### CF.Seq.9 Strictly increasing

Determine if the sequence is strictly increasing

### CF.Seq.10 Order

Determine if the sequence is:
  - increasing
  - strictly increasing
  - decreasing
  - strictly decreasing
  - constant or
  - has no order

### CF.Seq.11 2<sup>nd</sup> Min/Max

Determine the second maximum value / second minimum value

### CF.Seq.12 Longest substring

Determine the length of longest [substring](https://en.wikipedia.org/wiki/Substring)
containing only the value `0`

##### Example:

input

```
3 4 0 0 5 0 7 0 0 0 0
              ^~~~~~~
              longest substring
```

output

```
4
```

### CF.Seq.13 Longest increasing substring

Determine the length of the longest increasing substring

##### Example

input

```
5 4 2 3 8 1 5 6 6 10 15 3
          ^~~~~~~~~~~~~
          longest increasing substring
```

output

```
6
```

### CF.Seq.14 Count Max value

Determine how many times the maximum values repeats

##### Example

input

```
4 5 1 5 9 2 1 9 4 9 3
        ^     ^   ^
```

output

```
3
```

explanation: The maximum value is `9` and it appears `3` times in the sequence

### CF.Seq.15 The largest value smaller than

Read another number `x` (before reading the sequence). Determine the largest value in the sequence that is smaller than `x`

## CF.Dig: Digits

##### Requirements

Control Flow; Operators;

### Read a positive number `n`. Determine:

### CF.Dig.1 The number of digits

### CF.Dig.2 The most significant (leftmost) digit

### CF.Dig.3 The Sum of all the digits

### CF.Dig.4 The number or trailing `0`s

(with how many `0` the number ends with)

### CF.Dig.5 Reverse

Determine the number with the digits reversed

### CF.Dig.6 Palindrome

Determine if the number is a [palindrome](https://en.wikipedia.org/wiki/Palindrome)

### CF.Dig.7 LSD/MSD Swap

Determine the number formed by swapping the least significant with the most significant digit

##### Example

`12345` -> `52341`

### CF.Dig.8 Lose middle digit(s)

Determine the number formed by loosing the middle digit(s).

- If it has an odd number of digits it looses the middle digit
- If it has an even number of digits it looses the 2 middle digits

##### Example:

- `12345` -> `1245`
- `123456` -> `1256`

### CF.Dig.9 Reverse first half

Determine the number formed by reversing the left half of it

If the number has an odd number of digits you may choose whether or not the middle digit is
part of the left half or not. Implement both.

##### Example:

- `123456` -> `321456`
- `1234567` -> `3214567` or/and `4321567`

### CF.Dig.10 Lose odd digits

Determine the number formed by loosing all the odd digits

##### Example:

`145783` -> `48`

# CArr: C-style arrays

TBA
