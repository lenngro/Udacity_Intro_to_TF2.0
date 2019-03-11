# Merantix Automotive Assignment
Assignment for Merantix Automotive Applicants

## Base task
Given a list of integers, find the consecutive subsequence with the highest _sum_.

## Context
Nowadays, conventional vehicles are already equipped with a variety of sensors.
These sensors collect an enormous amount of data every second.
To make use of this large pool of sensory data in our pipeline, we need to identify interesting subsequences.
The task is an abstraction of this, with the list of integers representing the sensor data and the sum is the metric to evaluate if a subsequence is interesting.

## Usage
### Input:
A file path to a file with a single line that contains the integer sequence separated by space, e.g.,
```
3 -5 1 2 -1 4 -3 1 -2
```

### Output:
The command should print to stdout the _sum_ of the desired subsequence, e.g., for the input above the output would be `6` from the subsequence `1 2 -1 4`.


## Extension tasks

After finishing the first task, the following other tasks should be tackled:
* The input is extended by a second parameter `n` that restricts the maximum length of the subsequence to n.
* The input is extended by a third parameter which changes how the metric is calculated.
  Instead of the _sum_ of the values we want to find the highest _sum_ of the absolute values of the differences of neighboring pairs.
  As an example, for the input above the absolute differences would be: `8 6 1 3 5 7 4 3` and therefore the output should be `16` for `n = 4` as `-1 4 -3 1` result in the absolute differences of `5 7 4` which adds up to `16`.
  The expected input parameter is `values` for the original behavior and `differences` for the new one.

## Examples
You can find example input files in the data folder.


```
python find_subsequence.py data/input_1.txt 9 values
>> 6
```

```
python find_subsequence.py data/input_1.txt 4 differences
>> 16
```

```
python find_subsequence.py data/input_2.txt 10 values
>> 27
```

```
python find_subsequence.py data/input_2.txt 5 differences
>> 58
```

```
python find_subsequence.py data/input_3.txt 30 values
>> 44
```

```
python find_subsequence.py data/input_3.txt 10 differences
>> 40
```

## Deliverables
* Code:

    * A _compressed_ (`tar.gz`) folder with the __Python__ (version 3.7) source file(s).
      The main function should be in a file called `find_subsequence.py` and be callable as demonstrated in the examples.
      Our goal is to check your software engineering capabilities, so while this is a small task, please also think about overall common best practices such as readability, maintainability and more.
    * The necessary library requirements should be in a `requirements.txt` file next to the python sources.
    * Any additional information should reside in a `README.md` file also included in the folder.

* Time (this will not be taken into account, but will only be used to improve this exercise)
# Udacity_Intro_to_TF2.0
