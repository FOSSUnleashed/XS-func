# %partial <fn> <list>

	`inc util`

	Returns a new fragement, which will call fn with list as the arguments, but with arguments of the frament afterwards

# Example

```
; double = <={%partial {|a b| result `($a * $b) } 2}
; echo <={double 5}
10
```
