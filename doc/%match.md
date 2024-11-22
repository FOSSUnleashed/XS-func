# %match <list>

	Create a matcher function for a list of globs

# Notes

```
; fn match {|glob| result '{|x| ~ $x '^$glob^\} }
//workstation4k/R ~/repos/XS-func (fo.github.com:FOSSUnleashed/XS-func)
; echo <={%filter <={match '????'} $list}
1999
//workstation4k/R ~/repos/XS-func (fo.github.com:FOSSUnleashed/XS-func)
; echo <={%filter <={match '??'} $list}
42 33 55 88 80 55
//workstation4k/R ~/repos/XS-func (fo.github.com:FOSSUnleashed/XS-func)
; echo <={%filter <={match '??' '???'} $list}
42 33 55 88 80 55
//workstation4k/R ~/repos/XS-func (fo.github.com:FOSSUnleashed/XS-func)
; fn match {|glob| result '{|x| ~ $x '^$^glob^\} }
//workstation4k/R ~/repos/XS-func (fo.github.com:FOSSUnleashed/XS-func)
; echo <={%filter <={match '??' '???'} $list}
42 33 55 88 80 55
//workstation4k/R ~/repos/XS-func (fo.github.com:FOSSUnleashed/XS-func)
; echo <={%filter <={match '??' '????'} $list}
42 33 55 88 1999 80 55
//workstation4k/R ~/repos/XS-func (fo.github.com:FOSSUnleashed/XS-func)
; echo <={%filter <={match '* *'} foo bar 'foo bar'}
foo bar foo bar
//workstation4k/R ~/repos/XS-func (fo.github.com:FOSSUnleashed/XS-func)
; echo <={%filter <={match '*\ *'} foo bar 'foo bar'}
foo bar

```
