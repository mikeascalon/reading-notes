# Reading Notes

## Local Storage and How To Use It On Websites

Why would a developer use local storage for a web application?

* help reduce server load and improve performance.

What information should not be stored in local storage?

Local storage is not suitable for storing sensitive or critical information, as it has limitations and security considerations that make it less secure than other storage methods

Local storage can store what type of data? How would you convert it to that type before storing?

 Modify the localStorage object in JavaScript. You can do that directly or (and this is probably cleaner) use the setItem() and getItem() method

* Strings: You can store plain text strings directly as values in local storage

```javascript
 localStorage.setItem('username', 'john_doe'); 
```

Numbers: Numbers should be converted to strings before storing them in local storage. You can use the toString() method or the String() constructor to convert numbers to strings:

```javascript
localStorage.setItem('score', String(100));
// or
localStorage.setItem('age', (42).toString());
```

* Booleans: Booleans should be converted to strings as well, using the String() constructor or toString() method:

```javascript
localStorage.setItem('isLogged', String(true));
// or
localStorage.setItem('isAdmin', false.toString());
```

* Arrays and Objects: Arrays and objects can be stored in local storage, but they need to be converted to JSON strings using the JSON.stringify() method before storing and then parsed back using JSON.parse() when retrieving them:

```javascript
const data = [1, 2, 3];
localStorage.setItem('data', JSON.stringify(data));

// To retrieve and parse the array:
const storedData = JSON.parse(localStorage.getItem('data'));
```

### Resources

[Local Storage](https://www.smashingmagazine.com/2010/10/local-storage-and-how-to-use-it/)

ChatGPT
