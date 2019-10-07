
# Description

Up until now, you've looked at regexes to do literal matches of strings. But sometimes, you might want to also match case differences.

Case (or sometimes letter case) is the difference between uppercase letters and lowercase letters. Examples of uppercase are "A", "B", and "C". Examples of lowercase are "a", "b", and "c".

You can match both cases using what is called a flag. There are other flags but here you'll focus on the flag that ignores case - the iflag. You can use it by appending it to the regex. An example of using this flag is /ignorecase/i. This regex can match the strings "ignorecase", "igNoreCase", and "IgnoreCase".


# Instruction

Write a regex fccRegexto match "freeCodeCamp", no matter its case. Your regex should not match any abbreviations or variations with spaces.


# Tests

Your regex should match freeCodeCamp
Your regex should match FreeCodeCamp
Your regex should match FreecodeCamp
Your regex should match FreeCodecamp
Your regex should not match Free Code Camp
Your regex should match FreeCOdeCamp
Your regex should not match FCC
Your regex should match FrEeCoDeCamp
Your regex should match FrEeCodECamp
Your regex should match FReeCodeCAmp


# Challenge seed
let myString = "freeCodeCamp";
let fccRegex = /change/; // Change this line
let result = fccRegex.test(myString);


# Solution
let myString = "freeCodeCamp";

let fccRegex = /FreeCodeCamp/i; // Change this line

let result = fccRegex.test(myString);
