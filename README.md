# Mystery Function

What does the `mystery()` function in the following piece of code do? Add your
answer to this markdown file.

```javascript
function mystery(a) {
    if(a.length == 1) return a[0];
    var foo = mystery(a.slice(1, a.length))
    if(foo > a[0]) return foo;
    else return a[0];
}
```

## Plagarism Statement

All exercises must contain the following statement:
“I certify that I have listed all sources used to complete this exercise, including the use
of any Large Language Models. All of the work is my own, except where stated
otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is
suspected, charges may be filed against me without prior notice.”
15

## Answer

The `mystery()` function will return the largest element in an array. 
This happens through a recursive "telescoping" action that slices the first array into sub arrays.
The previous value of foo is compared to the first element in the sub array.
The larger value between foo and the current first element in the sub array will be the next value for foo.
Process repeats until all sub arrays are checked for the largest value.
This results in an ouput of the largest element in the array.


