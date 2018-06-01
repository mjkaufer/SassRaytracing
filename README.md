# Raytracing with SASS

## Usage

* Define whatever spheres you want to raytrace in `spheres.scss`
* Define what lights to use in `lights.scss`
* If you want to change the dimensions, make sure they stay square, and be sure to update the variables in `consts.scss` and in the JavaScript code inside `index.html`
	* The JavaScript is only there to generate the divs - see the TODO for a thought to get around this
* Run `npm run build-css` to build the css one time, or `npm run watch-css` to continuously build
* Open `public/index.html` to see your beautiful shapes!

## TODO

* Support for more shapes
	* Cylinders, cubes
* Phong shading support?
* Non-square dimension support
* Spheres further from origin look ovally
    * Something to do with perspective; I lowered FOV and it looked a little better
* Write custom base64 encoding for the pixels to create a URI, and set that as a background picture of a single div, to totally eliminate JavaScript for rendering
