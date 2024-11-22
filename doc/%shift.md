# %shift <list>

	`inc list`

	Return the list with last item moved to the first item.  Meant to be used to complete the push/pop/shift/unshift set.

# Examples:

```
	list = a b c d e

	# push
	list = $list f

	#pop
	(x list) = <={%shift $list}

	#shift
	(x list) = $list

	#unshift
	list = a $list
```
