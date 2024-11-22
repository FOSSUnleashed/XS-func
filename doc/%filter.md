# %filter <fn> <list>

	`inc list`

	Filters a list, applying a boolean verification function

# Example

```
	list = a.c b.c c.c foo.a bar.a

	echo <={%filter {|x| ~ $x *.c} $list}
	# prints `a.c b.c c.c`
```
