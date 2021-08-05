### Local Storage :

##### COOKIES SideEffects:

* Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
* Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).
* Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.


##### INTRODUCING HTML5 STORAGE :
* local storage :it’s a way for web pages to store named key/value pairs locally.within the client web browser like cookies
* this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you
* From your JavaScript code, you’ll access HTML5 Storage through the localStorage object on the global window object.


##### USING HTML5 STORAGE :
* HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.
* Calling `setItem()` with a named key that already exists will silently overwrite the previous value. 
*  Calling `getItem()` with a non-existent key will return null rather than throw an exception.
* Calling `removeItem()` for removing the value for a given named key.
* If you call` key()` with an index that is not between 0–(length-1), the function will return null
 


##### TRACKING CHANGES TO THE HTML5 STORAGE AREA
* The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something.
* to hook the storage event, you’ll need to check which event mechanism the browser supports. 

* The handle_storage callback function will be called with a StorageEvent object, except in Internet Explorer where the event object is stored in window.event.


PROPERTY |TYPE |DESCRIPTION
---------|-----|-----------
key	|string | the named key that was added, removed, or modified
oldValue | any	| the previous value (now overwritten), or null if a new item was added
newValue | any	| the new value, or null if an item was removed
url* |	string	| the page which called a method that triggered this change



##### LIMITATIONS IN CURRENT BROWSERS 
* the flag for whether there is a game in progress (gGameInProgress) is a Boolean. In the saveGameState() function, we just stored it and didn’t worry about the datatype:
`localStorage["halma.game.in.progress"] = gGameInProgress;`

*  in the `resumeGame()` function, we need to treat the value we got from the local storage area as a string and manually construct the proper Boolean value ourselves:
`gGameInProgress = (localStorage["halma.game.in.progress"] == "true");`

* the number of moves is stored in gMoveCount as an integer. In the saveGameState() function, we just stored it:
`localStorage["halma.movecount"] = gMoveCount;`

* But in the resumeGame() function, we need to coerce the value to an integer, using the parseInt() function built into JavaScript:
`gMoveCount = parseInt(localStorage["halma.movecount"]);`
