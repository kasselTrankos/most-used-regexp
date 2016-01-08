# most-used-regexp

For found and replace urls in plain text:
```javascript
str.replace(/\b(?:https?|ftp):\/\/[a-z0-9-+&@#\/%?=~_|!:,.;]*[a-z0-9-+&@#\/%=~_|]/gim, '<a href="$&">$&</a>');
```
For found and replace twitter accounts: 
```javascript
str.replace(/@([a-z\d_]+)/ig, ' <a href="http://www.twitter.com/$1" target="blank">@$1</a>');
```
For found and replace hashtags:
```javascript
str.replace(/(^|\s)#(\w+)/g, ' <a href="https://twitter.com/hashtag/$2?src=hash" target="blank">#$2</a>');
```







