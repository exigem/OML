# OML | ORlib Media Library #

A simple Booknote Manager to Organise Links, Notes, Borred or other stuff aside your real Books. \n
At the time OML is only available in German Language.


## Dependencies ##

- PHP4 better PHP5
- PHP XML-DomDocument 


## Installation ##

Get last version from github.com by following command:

> git clone git://github.com/vaddi/OML.git OML

Edit verify.php to change username and password.
Make sure the "xml" Folder is writeable by Webserver (often www-data) otherwise change Permissions by Hand: 

> chown www-data:www-data xml


## Usage ##

On Empty xml Folder you will get a Link to the createArticle Site (You will be loged in first). Now you can create Booknotes to your own fits. You can remind yourself when you have borred a book to someone. You can simple Organize hints like ISBN, Color or Links. 
Shortform, Content, Index and Colophone (all textforms) will be formated by a simple BBCode style:

1.  &#91;b&#93;TEXT&#91;/b&#93; => &lt;b&gt;TEXT&lt;/b&gt;, All simple HTML-Tags (e.g. "i" or "u")
2.  &#91;url=TEXT1&#93;TEXT2&#91;/url&#93; => &lt;a href="TEXT1"&gt;TEXT2&lt;/a&gt;, Textlink or URL
3.  &#91;img&#93;TEXT&#91;/img&#93; => &lt;img src="TEXT" alt="TEXT" /&gt;, Images
4.  All URLs (http://domain.tld/) will be formated to clickable href links


## Idea ##

Based on a small [PHP XML CMS][] writen by Tom Myer and a [PHP-Libary][] by Alexandre Alapetite that make OML automaticly usable on PHP4 or PHP5 Webservers.
The Baseidea should be a simple Note for a [O'Reilly Media Books][]. Beside the maincoding the Idea grown up by more and more Features:

- write down a native linkadress, it will be saved in same format, but will be displayed as a clickable href link
- BBCode Shortcode style to get a litle bit more formating
- All Content and Pageination will be get from xml Files
- Have to be very userfriendly by simple Structure and Usage


## OnGoing ##

Nice to have things:

- A nice Idea for index Pageination for better viewing a lot of Books
- CodeMirror should be for a better Syntax highlighting on Input
- Sortable Linklist Elements
- handheld CSS File
- ReBuild OOP Class based, so Users are able to add own Nodes, Attributes and Content dynamicly


## Issuses ##

- The Add-Link on create and edit Pages are stil brocken. The new javascript var wouldn't saved by submit. 
- A h1 Element will breake the padding of the whole Entry


## Credits ##

1.  [PHP XML CMS][]
2.  [PHP-Libary][]
3.  [O'Reilly Media Books][]

[PHP XML CMS]: http://www.sitepoint.com/management-system-php/
[PHP-Libary]: http://alexandre.alapetite.fr/doc-alex/domxml-php4-php5/
[O'Reilly Media Books]: http://oreilly.com/
