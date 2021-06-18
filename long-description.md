<h1>Garbage Detection: Leading the way to cleaner cities</h1>

<p>Ever saw the streets of your hometown littered with trash and wished you could do something? Well, we've been there too! We created this web application with the hopes of helping everyone come together as a community and keep our cities clean.</p>
<br>
<p>Keeping in mind the Goal no. 11 of United Nation's Sustainability Goals, 'Sustainable Cities & Communities' (<i> https://sdgs.un.org/goals </i>), we propse the following idea to clean up the city and segregate waste.</p>

<h2>Step 1: Identifying the Garbage</h2>
<p>With the help of delivery/transport services such as Uber, Zomato, we can identify the littered areas of the city by fixing an inference engine with a camera and a gps tracker, that is programmed to identify trash on the go. We've used the YOLO (You Only Look Once) Algorithm for the garbage detection. The litter identified can be further classified into the following categories:
  <ul>
    <li>cardboard</li>
    <li>glass</li>
    <li>metal</li>
    <li>paper</li>
    <li>plastic</li>
    <li>trash (includes wrappers, biodegradable waste and other indecipherable litter)</li>
   </ul>
  </p>

<h2>Step 2: Getting the Location & the Hardware</h2>
<p>The frames where garbage was detected would be sent along with the GPS co-ordinates of the location where the frame was taken and sent to Node-RED via MQTT protocol, Node-RED is a service provided by IBM that makes connecting IoT devices to web applications simple.</p>


<h2>Step 3: Working with the Location</h2>
<p>On recieving the location, coordinates (latitude and longitude) are stored in a database (IBM's cloudant) where we've represented each location with a document. The cordinates are then retrieved and markers are placed on a map using python library (folium) and will be displayed in our web application. Concerned authorities can then be able to collect the garbage and treat it using appropriate techniques. </p>

<h3>Alternative:</h3>
<p>The inference machine can be directly tracked using HERE tracking to display details about the locations of garbage found.</p>
