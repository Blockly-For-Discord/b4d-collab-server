# NodeJS Server Software
While multiple people can work on a project at the same time, you won't see their changes till another user leaves the project. Therefore as a much cleaner solution we provide a software to enable live collaboration to be able to see the changes other people make LIVE as you code allowing for a much smoother experience.


## Installation
Download the Software from our releases, and unzip the files onto your NodeJS Server. In your Index.js file write this:
```js
const b4d = require('./software.js');


b4d.server(config);

var config = {
  "port": 8080,
  "password": "",
  "allowedUsers": ["@inventionpro"],
  "blacklist": ["@hitbyathunder", "210.24.90.135"] 
}
```
