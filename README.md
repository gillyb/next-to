next-to
=======

Simple jQuery plugin for aligning elements next to each other<br/>
This is a really old plugin written by me, and just now ported to github from code.google.com.<br/>
You should read my <a href="http://debuggerstepthrough.blogspot.co.il/2012/03/jquery-relative-position-plugin-nextto.html">blog post</a> about this.


<h3>What is this ?</h3>
There are so many jQuery plugins that have a nasty part of code in them just do calculations to position an element next to another element. This plugin is that piece of nasty code extracted out to a separate plugin, so that your plugin could look a little bit cleaner.

This could help you while designing a menu, a drop-down effect, rollover tooltip or whatever else comes to mind... 

<h3>Requirements :</h3>
* jQuery version 1.2.6 

<h3>Tested with :</h3>
* FireFox
* Chrome
* IE7 (and above) 

<b>Sample Usage :</b><br/>
`<script type="text/javascript">`<br/>
`  $('.PlaceThisDiv').nextTo($('.ThisOtherDiv'), {position:'right', shareBorder:'top'});`<br/>
`</script>`<br/><br/>
For more samples look in the samples directory in the source code. They're pretty much self-explanatory.

<b>About Usage :</b>

* The first element is the 'loose' element. This is the element we want to be moved next to the 'base' element.<br/>
* The 'base' element is the element passed as a parameter to the 'nextTo' method, and this element will not be moved at all.<br/>
* The object passed as the second parameter in the 'nextTo' method can have four properties :<br/>
  * `position` - 'top', 'bottom', 'left' or 'right' and this describes on what side of the 'base' element the loose element will be aligned.<br/>
  * `shareBorder` - 'top', 'bottom', 'left' or 'right'. This will align the chosen border of the base element to the same chosen border on our loose element. (Look at the samples to get a better understanding)<br/>
  * `offsetX` - the amount (in pixels) we want to move the element on the X axis.<br/>
  * `offsetY` - the amount (in pixels) we want to move the element on the Y axis.<br/>
