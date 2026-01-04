 

SGML – Standard Generalized Markup Language
HTML
History of HTML
HTML - 1991
HTML2 - 1995
HTML3.2 - 1997
HTML4.01 - 1999
xHTML- 2000
HTML5 – 2014

DOCTYPE – it gives the information about the version of HTML
For HTML5 its <!DOCTYPE>

Basic html file structure is:
<html>
	<head>
		<meta charset=”utf-8”>
		<base href=”https://www.mywebsite.com”/>
		<title>test title</title> - displayed on browser tab, user full for search engines and users
		<link rel=”stylesheet” href=”/folder/folder/filepath.css”>
		<script>
			alert(“test”);
		</script>
	</head>
	<body>
		All content will go here…
	</body>
</html>

Tag	Description	Output/comments
<pre>	text displayed in a fixed-width and font	Its preserves both spaces and breaks
<em>	Emphasized text	Test - Similar to italic
<i>	Italic text	test
<small>	Small text	Cascade multiple small tags to make text even smaller
<sub>	Subscripted text	
<sup>	Superscripted text	
<ins>	Inserted text	text
<del>	Deleted text	text
<mark>	Marked or highlighted text	text
<q>	Short Quotation text	“text”
<abbr>	Defined as abbreviation	
<address>	Block as italic	
<bdo>	Bi-Directional override	<bdo dir=”rtl”>this is test</bdp>
Output will be: tset si siht
<a>	link	Target attributes plays vital role
Target=”_blank” – opens link in new tab
Target=”_self” – opens link in same tab
Target=”_parent” – opens link in parent tab
Target=”_top” – opens link in new full body window
<img>, <map>	To render image	Map – informs users that an interactive image is there with clickable areas
<h1>, … , <h6>	Header text	H1 is the largest text

Tables:
<table>
<thead>: headers that label the content in each column
<tbody>: the body of table
<tfoot>: describes all footer content
<tr>: table row
<td>: table cell
<th>: table header per column
<colgroup>: group column for formatting purposes
<col>: a single column of information within table
<caption>: description of table’s purpose and info it contains

e.g.,
<table>
	<colgroup>
		<col span=”2” style=””>
	</colgroup>
	<tr>
		<th>test1</th>
		<th>test2</th>
	</tr>
	<tr>
		<td>test3</td>
		<td>test4</td>
	</tr>
</table>

Objects:
<object>: describes a file type to be embedded like audio, video, PDFs etc.
Attributes are: width, height, type and usemap

<object width="100%" height="500px" data="snippet.html"></object>


iFrames:
<iframe>: an inline frame that allows external information to be embedded into a document.
Attributes are: src, width, name, srcdoc
<object width=”” height=””></object>
<iframe src=”test.html” width=”xxx” height=”xxx”></iframe>
<embed src=”test.swf” width=”” height=””></embed>

<iframe width="420" height="315"
src="https://www.youtube.com/embed/xyz">
</iframe>

List
Ordered list:
<ol>
	<li type=’1’>test</li>
</ol>
Possible values for type can be
1 for numeric
A for capital alphabet
a for small alphabet
I for roman
I for small roman

Unordered list:
<ul>
	<li type=’disc’>test</li>
</ul>
Possible values for type can be disc, circle, square and none.

Event Handlers:
There are multiple event handler attributes, few of them are: Onclick, Onerror, Ondragstart, Ondragover, Ondragenter, Ondrop etc

Forms

Tag used in <input>

Important attributes are type, value, readonly, disable (not a key-value pair attribute), size, maxlength, autocomplete, novalidation (not a key-value pair attribute), autofocus (not a key-value pair attribute), max, min, pattern and placeholder.

Type can be text, radio, submit, password, checkbox, number, date, color, range, month, week, time, daytime, daytime-local, email, search, tel and url (modern browsers identify the type and show the input keyboard accordingly)

Action attribute for submitting request:
<form action=”” method=”GET”>
	… [all input tag values will be passed as query string on submission]
</form>
Method can be GET (data passed as query string) or POST
e.g., 
<form action=”” method=”post”>
	<fieldset>
		<legend>section title</legend>
		Name: <input type=”text” name=”x”/>
		Month: 
<select>
	<option value=”cooking”>Cooking</option>
	<option value=”photography”>Photography</option>
		</select>
		<input type=”submit” value=”Submit”>
	</fieldset>
</form>

New in HTML5
1)	New DOCTYPE and Charset
Html 4.01 doctype: <!DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN"
            "http://www.w3.org/TR/html4/strict.dtd">
Html 5 doctype: <!DOCTYPE>

Charset examples: <meta charset=”UTF-8”>

Header <header>
Navigation <nav>
Section <section>
Article <article>	Side Navigation <aside>
Footer <footer>
2)	New Structure
a.	Sections
b.	Header
c.	Footer
d.	Nav
e.	Article
f.	Figure

3)	New elements
a)	Time
b)	Meter
c)	Progress

4)	Form element
a.	Datetime
b.	Month and year
c.	Time
d.	Number
e.	Range
f.	Email
g.	Url

5)	Audio and Video
<video width="320" height="240" controls>
  <source src="movie.mp4" type="video/mp4">
  <source src="movie.ogg" type="video/ogg">
Your browser does not support the video tag.
</video>

<audio controls>
  <source src="horse.ogg" type="audio/ogg">
  <source src="horse.mp3" type="audio/mpeg">
Your browser does not support the audio element.
</audio>

6)	Canvas and SVG
Canvas

They are used to draw graphics via scripting
a)	Drawing a line
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.moveTo(0, 0);
ctx.lineTo(200, 100);
ctx.stroke();
</script>

b)	Drawing a circle
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");
ctx.beginPath();
ctx.arc(95, 50, 40, 0, 2 * Math.PI);
ctx.stroke();
</script>

c)	Drawing circular gradient
<script>
var c = document.getElementById("myCanvas");
var ctx = c.getContext("2d");

// Create gradient
var grd = ctx.createRadialGradient(75, 50, 5, 90, 60, 100);
grd.addColorStop(0, "red");
grd.addColorStop(1, "white");

// Fill with gradient
ctx.fillStyle = grd;
ctx.fillRect(10, 10, 150, 80);
</script>

SVG – Scalable Vector Graphics

SVG defines vector-based graphics in XML format.

a)	Drawing a circle
<svg width="100" height="100">
  <circle cx="50" cy="50" r="40" stroke="green" stroke-width="4" fill="yellow" />
</svg>

b)	Drawing a rounded corner rectangle
<svg width="400" height="180">
  <rect x="50" y="20" rx="20" ry="20" width="150" height="150"
  style="fill:red;stroke:black;stroke-width:5;opacity:0.5" />
</svg>

Canvas	SVG
•	Resolution dependent
•	No support for event handlers
•	Poor text rendering capabilities
•	You can save the resulting image as .png or .jpg
•	Well suited for graphic-intensive games	•	Resolution independent
•	Support for event handlers
•	Best suited for applications with large rendering areas (Google Maps)
•	Slow rendering if complex (anything that uses the DOM a lot will be slow)
•	Not suited for game applications

7)	Geolocation
The HTML Geolocation API is used to locate a user's position.

<script>
var x = document.getElementById("demo");
function getLocation() {
  if (navigator.geolocation) {
    navigator.geolocation.watchPosition(showPosition);
  } else {
    x.innerHTML = "Geolocation is not supported by this browser.";
  }
}
function showPosition(position) {
  x.innerHTML = "Latitude: " + position.coords.latitude +
  "<br>Longitude: " + position.coords.longitude;
}
</script>

Property	Returns
coords.latitude	The latitude as a decimal number (always returned)
coords.longitude	The longitude as a decimal number (always returned)
coords.accuracy	The accuracy of position (always returned)
coords.altitude	The altitude in meters above the mean sea level (re-turned if available)
coords.altitudeAccuracy	The altitude accuracy of position (returned if available)
coords.heading	The heading as degrees clockwise from North (returned if available)
coords.speed	The speed in meters per second (returned if available)
timestamp	The date/time of the response (returned if available)

8)	Web Storages – Local Storage and Session Storage
9)	Drag and drop
10)	Caching (Manifest file)
