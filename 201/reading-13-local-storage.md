# Local Storage and How To Use It On Websites

This section describes what local storage is and how to use it on your websites.

## Questions

Why would a developer use local storage for a web application?

local storage can have a save state that should bring you back when returning to the site. If you frequent the site often it can help load the page faster if you have already stopped by. you could view the page offline keeping some or most functionality of the page.

What information should not be stored in local storage?

You should not store anything with PII, session data, any security parameters, and large amounts of data (5-10MB for each domain) or anything sensitive. Most of this stuff should live in the server-side with more securty.

Local storage can store what type of data? How would you convert it to that type before storing?

Local storage can store data in strings. You can set the item in local strage by using the `JSON.stringify` method:

```
let myObject = { key: "value" };
localStorage.setItem("myObject", JSON.stringify(myObject));
```

to revert them you would use the JSON.parse method. the parsedObject below with have the newly retreived data:

```
let storedObject = localStorage.getItem("myObject");
let parsedObject = JSON.parse(storedObject);
```

## Things I want to know more about

I'm just going to assume you can't use local storage to serve as a secured login method because it increases the risk of theft or unauthorized access.