# %partialRight <fn> <list>

	`inc util`

	Returns a new fragement, which will call fn with arguments to the frament, followed by the list

# Example

```
; double = <={%partialRight {|a b| result `($a * $b) } 2}
; echo <={double 5}
10
```
