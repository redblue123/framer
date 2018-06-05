button1.states.a =
	options:
		time: 1
		curve: Spring(tension: 200,friction: 25)
	
	x: 304
	scale: 1.2
	
bj.states.a =
	backgroundColor: "rgba(84,161,253,1)"
	
button1.states.animationOptions = 
	curve: Spring(tension: 200,friction: 25)
	time: 1
	
bj.states.animationOptions = 
	curve: Spring(tension: 200,friction: 25)
	time: 1
	
button1.onClick ->
	button1.stateCycle()
	bj.stateCycle()
bj.onClick ->
	button1.stateCycle()
	bj.stateCycle()	
```
- #####气泡

![演示图.gif](https://upload-images.jianshu.io/upload_images/2666102-90a5ee7a4d4f7cbf.gif?imageMogr2/auto-orient/strip)

```

layerA.states.rotate =
	rotation: 180
	animationOptions:
		time: 1
		curve: Spring
		
 
layer2.states.csale =
	scale: 0
	y: -74
	x: 257
	opacity: 0.00

layer2.states.animationOptions = 
	curve: Spring

layerA.states.animationOptions = 
	curve: Spring	
		
layerA.onTap ->
	layerA.stateCycle()
	layer2.stateCycle()
