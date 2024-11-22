# %once <fn>

	Returns a fragment that will call fn with the arguments given to the frament once, all subsequent calls will result the values.

# Example

```
; fn foo <={%once {|a b| result `($a + $b)}}
; echo <={foo 4 5}
9
; echo <={foo theatre props}
9
```
