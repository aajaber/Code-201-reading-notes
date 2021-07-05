# Read: 13 - Local Storage


**Persistent local storage:** is one of the areas where native client applications have held an advantage over web applications. 

For native applications, the operating system typically provides an abstraction layer for storing and retrieving application-specific data like preferences or runtime state.



## * Cookies:

web applications have had none of these luxuries. Cookies were invented early in the web’s history, and indeed they can be used for persistent local storage of small amounts of data. But they have three potentially dealbreaking downsides:

- Cookies are included with every HTTP request, thereby slowing down your web application by needlessly transmitting the same data over and over

- Cookies are included with every HTTP request, thereby sending data unencrypted over the internet (unless your entire web application is served over SSL)

- Cookies are limited to about 4 KB of data — enough to slow down your application (see above), but not enough to be terribly useful

** What we acctully need :**
- a lot of storage space
- on the client
- that persists beyond a page refresh
- and isn’t transmitted to the server



## * HTML5 Storage:
So what is **HTML5 Storage?** Simply put, it’s a way for web pages to store named key/value pairs locally, within the client web browser. Like cookies, this data persists even after you navigate away from the web site, close your browser tab, exit your browser, or what have you. Unlike cookies, this data is never transmitted to the remote web server (unless you go out of your way to send it manually). Unlike all previous attempts at providing persistent local storage, it is implemented natively in web browsers, so it is available even when third-party browser plugins are not.


### * Accessing HTML5 Storage from JavaScript:
-we can use **Modernizr** to detect support for HTML5 Storage.

    if (Modernizr.localstorage) {
      // window.localStorage is available!
    } else {
      // no native support for HTML5 storage :(
      // maybe try dojox.storage or a third-party solution
    }



### * Using HTML5 Storage:
HTML5 Storage is based on named key/value pairs. You store data based on a named key, then you can retrieve that data with the same key.

- key  => String.
- Data => can be any data type supported by JavaScript ( String , Bool.... etc).

*all the data will be stored as String , and to retrieve it based on it actual type , we'll end up using functins like 
**parseInt** & **parseFloat**.


### * HTML5 STORAGE IN ACTION:
**Ex:**

     function saveGameState() {
          if (!supportsLocalStorage()) { return false; }
          localStorage["halma.game.in.progress"] = gGameInProgress;
          for (var i = 0; i < kNumPieces; i++) {
        localStorage["halma.piece." + i + ".row"] = gPieces[i].row;
        localStorage["halma.piece." + i + ".column"] = gPieces[i].column;
          }
          localStorage["halma.selectedpiece"] = gSelectedPieceIndex;
          localStorage["halma.selectedpiecehasmoved"] = gSelectedPieceHasMoved;
          localStorage["halma.movecount"] = gMoveCount;
          return true;
      }