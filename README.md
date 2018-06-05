box.states = 
	one:
		borderRadius: 14
		rotation: 15
		scale: 1.5
		backgroundColor: "rgba(255,255,255,1)"
		
	two:
		scale:.75
		rotation: -15
		x: 86
		y: 143
		width: 203
		height: 203
		backgroundColor: "rgba(255,185,0,1)"
		
	three:
		rotation: 0
		scale: 1
		backgroundColor: "rgba(255,255,255,1)"
		
box.animationOptions =
	curve: Spring(damping: 0.5)

box.onTap ->
	box.stateCycle("one","two","three")
