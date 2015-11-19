Markdown is a minimal markup language which provides a way to write and style content for the web. It is designed to be easy to use and read. Markdown is often used as a text-to-HTML conversion tool. text on a web page, which is then converted to HTML when the page is compiled.


Paragraph
	Each line is a paragraph

Italics: surround a word with underscore(_) -> _this_ or *this*

Bold: surround a word with two asteriks (**) -> **really** or __really__ (two underscores)

You can make words both bold and italic: **_hey there_**

Headers
There are six types of headers, in decreasing sizes
	To make a headers in Markdown, you preface the phrase with a hash mark (#). You place the same number of hash marks the size of the header you want.
	header one <h1> -> # Header One
	header three <h3> -> ### Header Three

Hyperlinks
	There are two different link types in Markdown, but both of them render the same exact way.
	Inline Link
		Wrap the link text in brackets ( [ ] )
		Wrap the link in parenthesis ( ( ) )
		e.g. [Visit GitHu!](www.github.com)
		[You're **really, really** going to want to see this.]( www.dailykitten.com)
	Reference Link (a reference to another place in the document)
		An advantage of the reference link style is that multiple links to the same place only need to be updated once.
		Reference links don't apper on the rendered markdown.
		You defined them by providing the same tag name wrapped in brackets ( [ ] ), followed by a colon ( : ), followed by a link.
		     Here's [a link to something else][another place].
		     Here's [yet another link][another-link].
		     And now back to [the first link][another place].

		     [another place]: www.github.com
		     [another-link]: www.google.com
	Images 
		Images are prefaced with an exclamation point( ! ), followed by the two brackets ( [ ] ), and a pair of parentheses ( ( ) ) containing the image URL.
		Within the brackets you can place some "alt text"
		![A representation of Octdrey Catburn](http://octodex.github.com/images/octdrey-catburn.jpg)
		You can also use reference links for images (same patterns as hyperlinks)
		![The first father][First Father]

		![The second first father][Second Father]

		[First Father]: http://octodex.github.com/images/founding-father.jpg
		[Second Father]: http://octodex.github.com/images/foundingfather_v2.png

Blockquotes 
	A blockquote is a sentence or paragraph that's been specially formatted to draw attention to the reader.
	To create a block quote, all you have to do is preface a line with the "greater than" caret (>)
		>Your blockquote.

	You can also place a caret character on each line of the quote.
		> His words seemed to have struck some deep chord in his own nature. Had he spoken of himself, of himself as he was or wished to be? Stephen watched his face for some moments in silence. A cold sadness was there. He had spoken of himself, of his own loneliness which he feared.
		>
		> —Of whom are you speaking? Stephen asked at length.
		>
		> Cranly did not answer.
	Notice that even blank lines must contain the caret character. This ensures that the entire blockquote is grouped together.

Lists 
	Unordered Lists
		To create an unordered lists, you'll want to preface each item in the list with an asterik ( * ). You can also use + or - interchangebly. There has to be a space between the asterik and word. Each list item also gets its own line.
			* Milk
			* Eggs
			* Salmon
			* Butter
	Ordered Lists
		Prefaced with numbers, instead of asteriks
			1. Crack three eggs over a bowl
			2. Pour a gallon of milk into the bowl
			3. Rub the salmon vigorously with butter
			4. Drop the salmon into the egg-milk bowl
	Nested Lists
		Occasionally, you might find the need to make a list with more depth, or, to nest one list within another. Have no fear, because the Markdown syntax is exactly the same. All you have to do is to remember to indent each asterisk one space more than the preceding item.
		* Tintin
		 * A reporter
		 * Has poofy orange hair
		 * Friends with the world's most awesome dog
		* Haddock
		 * A sea captain
		 * Has a fantastic beard
		 * Loves whiskey
		   * Possibly also scotch?
	Tricks 
		1. Crack three eggs over a bowl.

		 Now, you're going to want to crack the eggs in such a way that you don't make a mess.

		 If you _do_ make a mess, use a towel to clean it up!

		2. Pour a gallon of milk into the bowl.

		 Basically, take the same guidance as above: don't be messy, but if you are, clean it up!

		3. Rub the salmon vigorously with butter.

		   By "vigorous," we mean a strictly vertical motion. Julia Child once quipped:
		   > Up and down and all around, that's how butter on salmon goes.
		4. Drop the salmon into the egg-milk bowl.

		   Here are some techniques on salmon-dropping:

		   * Make sure no trout or children are present
		   * Use both hands
		   * Always have a towel nearby in case of messes
  
Formatting Paragraphs
	soft break (creating a new line)
	Place two spaces at the end of the sentence (they are invisible)
	You can accomplish this by inserting two spaces _after_ each new line. This is not possible to see, since spaces are invisible, but it'd look something like this (each dot represents a space on the keyboard):
		Do I contradict myself?··
		Very well then I contradict myself,··
		(I am large, I contain multitudes.)

Code
	In a regular paragraph, you can create code span by wrapping text in backtick quotes. ' '

