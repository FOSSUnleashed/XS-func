# %constantly <list> 

	`inc list`

	Returns a function that returns list F(A) -> (F() -> A)

# Examples

	func = <={%constantly $list}

	list = <=$func
