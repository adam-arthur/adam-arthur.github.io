---
layout: post
---

Function hoisting gets a [bad rap](https://github.com/airbnb/javascript/issues/273). Some say it leads to code that reads "unnaturally". Others say that it obscures important implementation details. Doesn't hoisting require the reader to jump back and forth through the code to build the full context of what they're reading?

While code style is subjective to a certain extent, I've found these and other arguments against hoisting lacking in rigor. 

Function hoisting is one of the *best* features in JavaScript, and I'll explain why.

## So what is "Function Hoisting"?
Function hoisting is a language feature that essentially allows you to call a function declaration before the point at which it's declared in the code. 

<div>
{% prismc javascript %}
add(2, 2) // Returns 4. It works!

function add(number, otherNumber) {
    return number + otherNumber;
}
{% endprismc %}
</div>

This is opposed to how functions work in Python, for example:
<div>
{% prismc python %}
add(2, 2) # Fail! NameError: name 'add' is not defined

def add(number, otherNumber):
    return number + otherNumber
{% endprismc %}
</div>


## 