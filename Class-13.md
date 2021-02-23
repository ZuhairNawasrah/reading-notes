# Local Storage

## INTRODUCING HTML5 STORAGE

Persistent local storage is one of the areas where **Native Client Applications** have held an advantage over **Web Applications**.For native applications,data can be stored in the **registry**, **INI files**, **XML files**, or some other place according to platform convention. Historically, web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealBreaking downsides:

- Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over.
- Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL).
- Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful.


Before HTML5, all attempts to create database with specific features were ultimately unsatisfactory in different ways.“HTML5 Storage”,“Local Storage” or “DOM Storage.” all of these are different names to a **Web Storage**. It’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually).

You store data based on a named key, then you can retrieve that data with the same key. The named key is a string. The data can be any type supported by JavaScript, including strings, Booleans, integers, or floats. However, the data is actually stored as a string. If you are storing and retrieving anything other than strings, you will need to use functions like `parseInt()` or `parseFloat()` to coerce your retrieved data into the expected JavaScript datatype.

## LIMITATIONS IN CURRENT BROWSERS

limitations of the now-standardized HTML5 Storage is “**5 megabytes**,” “**QUOTA_EXCEEDED_ERR**,” and “**no**.”
1. “**5 megabytes**”: Is how much storage space each origin gets by default. This is surprisingly consistent across browsers, but remember that you’re storing strings, not data in its original format. If you’re storing a lot of integers or floats, the difference in representation can really add up.
2. “**QUOTA_EXCEEDED_ERR**”: Is the exception that will get thrown if you exceed your storage quota of 5 megabytes.
3. “**No**”: Is the answer to the next obvious question, “Can I ask the user for more storage space?”.
