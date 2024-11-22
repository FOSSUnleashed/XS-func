# %uniq <pack.listA> <pack.listB>

	`inc list`

	Return the values that are unique to both lists.

# Example

```
	fA = <={%constantly one two three four five}
	fB = <={%constantly two four six eight}

	echo <={%uniq $fA $fB}
```

Prints `one three five six eight`
