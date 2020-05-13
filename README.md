# display-text
Displays text based on an encoded and somewhat encrypted URL.

The purpose of this web page is to make it easy to link to a certain message/text without having to host it somewhere, or spoil the message within the URL. 

The "decrypting" is done by subtracting 1 from the charcode for ever character. 

## Encrypt text 
To encrypt and encode a message you might use this javascript code:
```javascript
var input = "Text to encrypt";//change this
var output = "";
input.split("").forEach(a => {output += (String.fromCharCode(a.charCodeAt(0)+1))});
console.log(encodeURI(output));
```
You can then add it to this URL https://isakisreserv.github.io/display-text/#YOUR-TEXT-HERE
