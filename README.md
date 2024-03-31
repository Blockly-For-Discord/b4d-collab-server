# NodeJS Server Software
While multiple people can work on a project at the same time, you won't see their changes till another user leaves the project. Therefore as a much cleaner solution we provide a software to enable live collaboration to be able to see the changes other people make LIVE as you code allowing for a much smoother experience.


## Installation
1. Download the Software from our releases, and unzip the files onto your NodeJS Server. In your Index.js file write this:
```js
const b4d = require('./software.js');


b4d.server(config);

var config = {
  "port": 8080,
  "password": "",
  "allowedUsers": ["@user1"],
  "blacklist": ["@user2", "127.0.0.1"] 
}
```
2. Start the server

It's as easy as that

## Config
| setting         | description                                                             |
|----------------|---------------------------------------------------------------------------------------------------------|
| `port`         | The port to listen to                                                                                   |
| `password`     | (optional) You can add a password so only people with the password can enter                            |
| `allowedUsers` | An array of people that are allowed to start live collaborations on your server. Leave empty for anyone |
| `blacklist`    | People that are blacklisted from starting a collaboration or joining one  (can be an ip)                |
