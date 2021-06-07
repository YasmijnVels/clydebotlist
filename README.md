## Installation
*If you have trouble with the installation, please feel free to visit our [discord](https://clydebotlist.com/dc) & [Website](https://clydebotlist.com/) address.*
- `npm i clydebotlist.js`

```js
const clydebotlist = require("./clydebotlist.js");
const dbl = new clydebotlist("TOKEN-HERE", client);

client.on("ready", async () => {
  dbl.serverCount(); // => Note: Only discord.js.
  // console.log("Server count posted")
  
  let hasVote = await dbl.hasVoted("714451348212678658");
  if(hasVote === true) {
    console.log("Voted")
  } else {
    console.log("Vote please.")
  }
  
  
  let search = await dbl.search("779641401482805289")
  console.log(search)
});
```

