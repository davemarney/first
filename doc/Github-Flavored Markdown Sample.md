Our API Documentation approach
------------------------------

Definition: An "API Document" is a multi-page document formatted like a book with chapters, a table of contents, etc. One document per API.

* API Documents are written in Markdown, and generated as HTML and PDF at release.
* A standard, github-compatible Markdown dialect is adopted.
* GUI Markdown editors are provided for those who want them, otherwise people edit the text directly.
* API Documents are hosted in repositories alongside the API source code, where they can be versioned, diffed, forked, cloned, etc.Standard naming conventions are followed.
* The following typographic features are supported in the Markdown code:
	* A title page (document title, author, version, date last updated, table of contents) 
	* A definitions page (contains terms and definitions, for example, a name of a parameter and its definition.) Tools will be provided to scan source code for parameter comments and automatically generate/update the definitions.
	* Multiple content pages, containing
		* Standard Markdown content tags
		* Heading text (up to four levels)
		* Paragraphs
		* Inline bold, italic, underline, and strikethrough 
		* Lists (bulleted and numbered)
		* Tables
		* Images (with optional thumbnails linking to full-size versions.)
		* Anchors and Links (named link targets on a page, and links to pages, terms, and external resources.)
		* Definition expansions (inline replacement of a reference to a term with its definition.)
		* Code text with multi-language syntax highlighting. Code text may contain additional Markdown attributes indicating that the code can be used as a Code Sample. Code Samples are parsed at build time to generate QA tests, and at release time to generate "Try It" console functionality on the XE Registry web site.
* At release: 
	* API Documents are emitted in PDF and zipped HTML formats. 
	* For the HTML version, Code Samples embedded in the API document are extracted and used to generate "Try It" interfaces.
	* They are distributed along with the rest of the documentation, and uploaded to the Ellucian XE Registry website hosted on Salesforce. 
	* We will add steps to hand-off API Document sources for translation to additional languages in a later phase.

A test of code highlighting
==================

```javascript
function (a) {
	var x = document.getElementById('foo');
	console.log x;
}
````

The afterward.
