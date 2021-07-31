<h1>Garbage Detection: Leading the way to cleaner cities</h1>

<p>Ever saw the streets of your hometown littered with trash and wished you could do something? Well, we've been there too! We created this web application with the hopes of helping everyone come together as a community and keep our cities clean.</p>
<br>

<p>As India and the world urbanizes, and with the pandemic, there is a sudden rise in the number of corporations providing deliveries to people in and around cities. This puts us in a unique situation wherein we can, with the help of the corporates that provide the delivery, observe locations wherein unnoticed garbage is being collected.</p>

<p>Keeping in mind the Goal no. 11 of United Nation's Sustainability Goals, 'Sustainable Cities & Communities' ( https://sdgs.un.org/goals ), we propose the following idea to clean up the city and segregate waste.</p>

<h2>Our Setup: How will this work?</h2>
<p> This project deals with Deep Learning, wherein we will have a model which is trained to identify garbage and an inference device, which will do the identification physically so as to speak. An inference engine, in the field of AI is a component of the system that applies logical rules to the knowledge base to deduce new information.</p>
<p>Our set-up would essentially be comprised of a smart camera to see the streets, GPS to detect the location and a modem to send the location to a Database server, so that the coordinates are noted and can be displayed on a map for the convenience of the concerned authorities to clean up. These authorities could be municipalities or recycling plants.</p> 
<p>Another approach, which will be more feasible with the onset of 5G and hence internet of things is to eliminate the need of pre-trained inference engines and smart cameras and instead have regular cameras sending all the footage it receives directly to a cloud for processing wherein the we will not only be able to identify the presence of garbage but also the specific type of garbage, hence making it easier for the recycling plants using the service too. The processing of the footage in a cloud will be faster and much more accurate since a cloud service could continuously learn. This approach also significantly decreases the cost of setup.</p>

<h2>Step 1: Identifying the Garbage</h2>
<p>With the help of delivery/transport services such as Uber, Zomato, we can identify the littered areas of the city by fixing our setup (discussed above), that is programmed to identify trash on the go. We've used the YOLO (You Only Look Once) Algorithm for the garbage detection. The litter identified can be further classified into the following categories:
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
<p>The frames where garbage was detected would be sent along with the GPS co-ordinates of the location where the frame was taken can be sent to IBM's Cloudant database from where we can plot them area-wise and garbage-type wise for ease of identification. Or another approach would be to use IBM's Node-RED via MQTT protocol, Node-RED is a service provided by IBM that makes connecting IoT devices to web applications simple.</p>


<h2>Step 3: Working with the Location</h2>
<p>On receiving the location, coordinates (latitude and longitude) are stored in a database (IBM's Cloudant) where we've represented each location with a document. The coordinates are then retrieved and markers are placed on a map using python library (folium) and will be displayed in our web application. Concerned authorities can then be able to collect the garbage and treat it using appropriate techniques.</p>

<h3>Alternative:</h3>
<p>The inference machine can be directly tracked using HERE tracking to display details about the locations of garbage found.</p>
