## THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS

Persistent local storage is one of the areas where native client applications have held an advantage over web applications. The native applications's operating system provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.

Three potentially dealbreaking downsides of Cookies:

 1- Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over

 2- Cookies are included with every HTTP request, thereby sending data unencrypted over the internet 

 3- Cookies are limited to about 4 KB of data — enough to slow down your application 



<!-- ## A BRIEF HISTORY OF LOCAL STORAGE HACKS BEFORE HTML5

DHTML Behaviors is one of the things that Microsoft invented and included it to the Internet Explorer , and one of these behaviors was called userData.

UserData allows web pages to store up to 64 KB of data per domain (Trusted domains, such as intranet sites, can store 10 times that amount. And hey, 640 KB ought to be enough for anybody.) -->

## INTRODUCING HTML5 STORAGE

“**HTML5 Storage**” is a specification named **Web Storage**, also known as “Local Storage” or “DOM Storage.”
HTML5 storage *is a way for web pages to store named key/value pairs locally, within the client web browser*. The data persists even after you navigate away from the web site, close your browser tab, exit your browser. 
Also, unlike cookies,the data is never transmitted to the remote web server (unless you go out of your way to send it manually).
It is implemented natively in web browsers, so it is available even when third-party browser plugins are not.

## USING HTML5 STORAGE

HTML5 Storage is based on named **key/value pairs**. You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. And the data can be any type that is supported  by JS. 

But the *data is actually stored as a string*. If you are storing and retrieving anything other than strings, you will need to use functions like **parseInt()** or **parseFloat()** to coerce your retrieved data into the expected JavaScript datatype.

Calling **setItem()** with a named key that already exists will silently overwrite the previous value. Calling **getItem()** with a non-existent key will return null rather than throw an exception.

Like other JavaScript objects, you can treat the **localStorage** object as an associative array. Instead of using the **getItem() and setItem() methods**, you can simply use **square brackets**. 


## TRACKING CHANGES TO THE HTML5 STORAGE AREA

To track programmatically of when the storage area changes, you can trap the storage event. The storage event is fired on the window object whenever setItem(), removeItem(), or clear() is called and actually changes something. The storage event is supported everywhere the localStorage object is supported.

## LIMITATIONS IN CURRENT BROWSERS

**“5 megabytes”** is how much storage space each origin gets by default. <br>
 One thing to keep in mind is that you’re storing strings, not data in its original format. If you’re storing a lot of integers or floats, the difference in representation can really add up. Each digit in that float is being stored as a character, not in the usual representation of a floating point number.

## HTML5 STORAGE IN ACTION

With HTML5 Storage, we can save the progress locally, within the browser itself. Example on this is if I have a game and made a few moves, then closed the browser tab, then re-opened it. If your browser supports HTML5 Storage, the demonstration page should magically remember your exact position within the game, including the number of moves you’ve made, the position of each of the pieces on the board, and even whether a particular piece is selected.

And need to pay attention that as mentioned before that any data type will be saved as a string so If you are storing something other than a string, you’ll need to coerce it yourself when you retrieve it.


**References:**

[THE PAST, PRESENT & FUTURE OF LOCAL STORAGE FOR WEB APPLICATIONS](http://diveinto.html5doctor.com/storage.html)