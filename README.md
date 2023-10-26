###reading-notes-class-4<br>
Reading notes and questions from class 4<br>
<br>
I. Learn HTML Creating hyperlinks><br>
  Hyperlinks allow us to link document to other documents and resources.<br>
  Most web content can be converted to hyperlink when clicked goes to different URL<br>
  a url can point to html files, text files, images tex document, video/audio files.<br>
1. Anatomy of a link<br>
A link is created by wraps the text or other content inside an < a > tag (anchor0 and using an href or attribute is Hypertext Reference or target the contains the web address<br> 
a) See notes<br>
3. Block level links anything even block level links, make heading level element link 		wrap in a tag. <b>
Notes for image<br>
Image links have image to make into link use < a >  and wrap image file refer with < img > below shows only locally stored image<br>
Adding supporting information with title.<br>
Attribute to add to links is title, contains info about link like what page has on it. Or things to be aware of on website. 
	     d)    Quick primer on urls an paths<br>
		(1) URLS use paths to find files, paths spec where the file is located in file system. See following page for details https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Creating_hyperlinks about 1/3 of way down.<br>

e) Document Fragments
		(1) possible to link just part of html doc (doc frag) rather than just top of doc. To do need to assign id attribute to element<br>

f) absolute versus relative urls
		1. Absolute points to location defined by absolute location on the we incl. protocol and domain name. <br>
		2 relative point to a location that is relative to the file you are linking from. Like linking from your directory<br> 

g. Use clear link wording<br> 
		1. Make links accessible to all readers <br>
			a) screen readers jump around<br>
			b) search engines use link text to target files <br>
			c. Visual reader skim over the page rather than reading every word. <br>
	
h. Linking to non-html resources leave signposts. <br>
I. Use the download attribute when linking to a download. <br>
j. Email links possible to creat links or buttons that open new outgoing mail message other than linking to resource page use < a > and mailto;<br>

k. Specifying details you can provide other info to start email head field the can be added to mailto: <br>


II. CSS Layout Normal Flow Css layout positions<br>
	A. Normal flow<br>
		1. How are elements laid out by default. <br>
			a. Process starts as boxes of individual elements laid out in such a way that any padding borderer margin they happen to have is added to content. BOX MODEL <br>
			b. By default block-level-element content fills available inline space of parent element contain it <br>
				1. The size of inline-level elements is just size of content can set width or height on some elements that have default display.<br> 
				2. Want to change display proper of an inline-level element use css to set to behave like block level element with display: block; or display: inline block<br> 
				3. Block level elements are laid out in the block flow direction based on the parents writing mode initial: horizontal-tb each element appears on ne line below last one. <br>
					a) inline elements behave diff they don’t appear on new lines they all sit on the same line. If two vertical adjacent elements both have a margin set on them and their margin touch the larger of the two margin remains and the smaller one disappears. This I margin collapse<br>
	B. Positioning / allows you to take element out of normal doc flow and make behave diff. Ex by sitting on top of one another or by always remaining in the same place inside the browser viewport. <br>
	1. Intro to positioning
		a) positioning allow us to produce intersting results by overriding normal doc flow. <br>
		b) static positioning/ is the default that every element gets means put it where it normally goes<br> 
. can use top, bottom, left, right can spec where to move the positioned items to. <br>
                                Top: 30px<br>
                                Left: 30px<br>
Think about the above as an invisible force  that pushes box moving in opposite direction like the force moves it it downward by 30px<br>
2. Absolute positioning / an absolutely positioned element no longer exist in the normal document flow. It sits on it’s own layer independent of everything else. <br>
 
3. Positioning contexts/ if no ancestor elements have their position property explicitly defined/ default ancestor elements have static position/ result is the absolutely positioned element will be contained in the initial containing block initial contain clock has dimensions of the viewport and is also block that contains the < html > elements<br>
                a) the positioned element is nested inside the body. Can change positioning contest/ element the absolutely positioned element is positioned relative to. <br>
 
                b. result of absolute post element will be contain in the initial contain block
                                1. initial containing block has dimension of viewport also block that contains < html> element<br>
                                2. absolutely positioned element will be displayed outside the html element and positioned relative to initial viewport. <br>
 
4. Introing z-index used to change stack order, using z index which is reffing z-axis the surface of the webpage towards your face x axis is horizontal and y axis is vertical<br>
 
5. Fixed positioning. Works exactly the same as absolute positioning one key diff, absolute fixes element in place  to nearest ancestor, fixed usually fixes an element in place relative to the visible portion of viewport<br>
 
6. sticky position basically hybrid between relative and fixed position, allows positioned item to act like it’s relatively positioned until it’s scrolled to certain threshold. <br>
                1. common use for position: sticky is to create a scrolling index page where diff heading stick to top of page as they are reached. <br>
 
IV. JS functions reusable blocks of code.<br>
	a) Functions reusable blocks of code.<br>
	b) Functions vs. Methods.<br>
		1. Functions  are a part of objects called methods.<br>
		2. Built in code used so far comes in both forms, Functions and methods can find full list in mdn standard built in objects<br>
	c) Invoking functions<br>
		1. Must call invoke function to run it. Done by including the name of the function in code somewhere and following it by paren myFunction();<br>
	d) Function parameters <br>
		1. Some functions need parameters to be invoked these are the values that need to be inside the function paraen to work.
		2. Sometimes parameters are optional. The function will adopt behavior an example the join() function is optional<br>
	c. Default parameters<br>
		1. When writing function if want to have optional can include + like function hello (name = ‘chris’) console.log(‘hello ${name}!);<br>
		2. Arrow functions COME BACK LATER THIS IS<br>
	d. Function scope and conflicts.<br>
	e. Scope- create function variables and things defined inside the unction are inside their own separate scope, are locked away in own separate compartments unreachable outside o the functions.<br>
	f top level global, accessible from anywhere<br>

##Things I want to know more about. 
	1. I just need to take more time and focus on things.<br>


HTML<br>
To create a basic link, we wrap text or other content inside what element?<br>
To create a basic link we wrap it in a an anchor tag <a><br>
The href attribute contains what information?<br>
The href contains the target/ web address of the link you are creating.<br>
What are some ways we can ensure links on our pages are accessible to all readers?<br>
Use clear link wording so it is easier for screen readers, search engines, and visual readers.<br>
Don’t use part of the URL to link text. Keep it short! Try not to duplicate copies of text that are linked to different places.<br>
CSS<br>
What is meant by “normal flow”?<br>
Normal flow is how block and inline elements are shown on the page before any changes are made to the layout. It is the default layout.<br>
What are a few differences between block-level and inline elements?<br> https://www.w3schools.com/html/html_blocks.asp<br>
Block level elements always star on a new line. The browser auto adds space, before and after element.<br>
Block elements take up all the available width. Inline does not start on a new line, and inline element only takes up the space necessary.<br>
___ positioning is the default for every html element.<br>
Static is the default position of every html element.<br>
Name a few advantages to using absolute positioning on an element.<br>
With absolute positioning the element is in/on it’s own layer so it can be isolated for it’s own independent means. <br> 
What is a key difference between fixed positioning and absolute positioning?<br>
Fixed and absolute are very similar according to the MDN docs absolute position fixes itself to the nearest ancestor.<br> 
Fixed positioning usually fixes an element in place relative to what is viewable on screen, it make is possible to make things like menus that are visible no matter how deep you scroll.<br> 

JS<br>
Describe the difference between a function declaration and a function invocation.<br>
A function declaration is where you declare the function, or create the function.<br>
The function invocation is just calling the function it is putting it where you want it to run.<br>
What is the difference between a parameter and an argument?<br>
A parameter is the bit of the function inside the parentheses, you need it to call/invoke a function, it is a variable.<br>
An arguments are the actual values of the variable or parameter <br>
https://www.w3schools.com/js/js_function_parameters.asp#:~:text=Function%20Parameters%20and%20Arguments&text=Function%20parameters%20are%20the%20names,and%20received%20by)%20the%20function.<br>

Misc<br>
Pick 2 benefits to pair programming and reflect on how these benefits could help you on your coding journey.<br>
		1. It is always good to get a second set of eyes on a problem everyone solves problems differently and someone else can help you see something you were unable to get past or identify before.<br>
  It is very helpful to rubber duck your code, to sit down and explain what it is doing to someone else, sometimes that’s all it takes to really solve something on your own is to hear it out loud<br>
  or to write it down as you would explain it.<br> It is so helpful not to be alone in anything that is difficult be it life or programing.<br>
