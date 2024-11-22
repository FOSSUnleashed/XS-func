# %common <pack.listA> <pack.listB>

	`inc list`

	Return the common values between two packed lists.

# Example

```
	fA = <={%constantly one two three four five}
	fB = <={%constantly two four six eight}

	echo <={%common $fA $fB}
```

Prints `two four`
