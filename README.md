## Load Depth Map

```
THREE.ImageUtils.loadDepthMap = function (url, callback, filter) {}

THREE.ImageUtils.loadDepthMap("path/to/image.file", function (depthData) {

}, function (pixel) {
	
	var brightness = 0.34 * pixel.r + 0.5 * pixel.g + 0.16 * pixel.b;

	// red
	pixel.r = brightness;
	// green
	pixel.g = brightness;
	// blue
	pixel.b = brightness;
	
	// pixel.a is used for the alpha
	
	return pixel;
})

```

