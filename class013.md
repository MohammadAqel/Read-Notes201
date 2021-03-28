## LOCAL STORAGE FOR WEB APPLICATIONS :
 
*Cookies were invented early in the web’s history : they have three potentially *
1. Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the
same data over and over.
2. Cookies are included with every HTTP request, thereby sending data unencrypted over the internet.
3. Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.
   
### A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5:
   
*userData allows web pages to store up to 64 KB of data per domain, in a hierarchical XML-based structure.*
*In 2002, Adobe introduced a feature in Flash 6 that gained the unfortunate and misleading name of Flash cookies.*
*Brad Neuberg developed an early prototype of a Flash-to-JavaScript bridge called AMASS (AJAX Massive Storage System).*
*In 2007, Google launched Gears, an open source browser plugin aimed at providing additional capabilities in browsers.*
*By 2009, dojox.storage could auto-detect Adobe Flash, Gears, Adobe AIR, and an early prototype of HTML5 storage that was only implemented in older versions of Firefox.*
   
   
### INTRODUCING HTML5 STORAGE :
   
*“HTML5 Storage” is a specification named Web Storage, which was at one time part of the HTML5 specification proper, but was split out *
*into its own specification for uninteresting political reasons.*
*it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even *
*after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike all previous attempts at providing persistent local storage.*
     
### USING HTML5 STORAGE :
   
*HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key.*
*the data is actually stored as a string.anything other than strings, you will need to use functions like parseInt() or parseFloat() to coerce your retrieved data.*
     
### LIMITATIONS IN CURRENT BROWSERS :
*5 megabytes is how much storage space each origin gets by default.*