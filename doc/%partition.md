# %partition <fn> <list>

	`inc list`

	Returns two `%constantly` fragments, the first contains the list of items that are filtered on true from fn, the second contains the rest

# example

```
; (A B) = <={%partition {|x| ~ $x ???} foo bar baz 1337 33}
; echo <=$A
foo bar baz
; echo <=$B
1337 33

```
