<h1>Garbage Detection: Leading the way to cleaner cities</h1>

<p>Ever saw the streets of your hometown littered with trash and wished you could do something? Well, we've been there too! We created this web application with the hopes of helping everyone come together as a community and keep our cities clean.</p>
<br>

<h2>Step 1: Identifying the Garbage</h2>
<p>With the help of delivery/transport services such as Uber, Zomato, we can identify the littered areas of the city by fixing an inference machine with a gps tracker and a smart camera that is customized to identify trash on the go. We've used YOLO for the object detection. The litter identified can be further classified by the to be cardboard, glass, metal, paper, plastic, and trash where trash includes wrappers and other indecipherable litter.</p>

<h2>Step 2: Getting the Location & the Hardware</h2>
<p>The frames where garbage was detected would be sent along with the GPS co-ordinates of the location where the frame was taken and sent to Node-RED, a service provided by IBM that makes connecting IoT devices to web applications simple.</p>


<h2>Step 3: Working with the Location</h2>
<p>The cordinates are then marked and displayed in a map using (name of the api) API and displayed in our web application to make it easier to identify which parts of the city needs to be cleaned</p>
<h3>Alternative:</h3>
