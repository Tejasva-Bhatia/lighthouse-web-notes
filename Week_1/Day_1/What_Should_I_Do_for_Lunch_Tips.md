### Tips

Try experimenting with the comparison operators (`<`, `>`, `===`, etc.) in the node REPL, which you can launch using the `node` command in Vagrant.

Work on your code iteratively – that means in small pieces. 

To help you figure out how to use `hungry` and `availableTime` inside your function, try outputting their values to the Terminal as follows.

``` javascript
const whatToDoForLunch = function(hungry, availableTime) {

  let result = "";
  if (!hungry)
    result = "Get back to work";

  if (hungry) {
    if (availableTime < 20)
      result = "Pick something up and eat it in the lab";

    if (availableTime >= 20 && availableTime <= 30)
      result = "Try a place nearby";

    if (availableTime > 30)
      result = "Reconsider how much time we actually have to spare";

  }

  console.log(result);

};

```