```
nextNumber = previousNumber + previousPreviousNumber
```

If the sequence starts with 0.

```
0
```

The next number is just 1

```
0, 1
^  ^
```

Since there are now two numbers, the next number is the first and second position added together `0 + 1`

```
0, 1, 1
   ^  ^
```

The next number is `1 + 1`

```
0, 1, 1, 2
```

And so on

```
0, 1, 1, 2, 3, 5, 8, 13 ...
```

The typical recursive function that is asked of interviewees is to calculate the next number in the sequece, or to calculate position `n`.

```javascript

function fib(n){
	...
}
```

```javascript
fib(0) = 0
fib(1) = 1
fib(2) = 1
fib(3) = 2
fib(4) = 3
...
```

See if you can solve it!

[SPOILER]

```javascript
function fib(n){
	if (n === 0) return 0
	if (n === 1) return 1
	
	return fib(n-1) + fib(n-2)
}
```

[/SPOILER]