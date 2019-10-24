# SnakeGame

## Why?

So I have been quite bored recently, and to combat that I found myself playing a lot of good old [snake](https://www.coolmathgames.com/0-snake). FYI my highscore is 471 if you want to beat it.  

That was going all well for a while but I was eventually bored of playing that too. 
Then my friend suggested, "why not create your own snake game with JS and host it in your recently bought domain (iiqrah.com)?" 

At first, it sounded really lame because it seems super simple but at the same time I don't know where to begin. 
However, after a few minutes of thinking, I thought might as well try it out. 

So this is me documenting my snake game.

## How?

I will be using HTML, CSS and JavaScript to create the game. 
This is the repository that will contain all my code and documentation. 
I will be hosting the game with the help of gitHub Pages and hopefully have a link of it on my website too.  


## So let's get started.

First things first.

### Blank Folder and File Creation

- Create a folder called Snake.
- Create a blank file called snake.html 

- Create two folders inside Snake called css and js

- Inside css, create a blank file called styles.css
- Inside js, create a blank file called snake.js

### Add the bare bone html code

```html

<!DOCTYPE html>
<html lang="en" dir="ltr">
  <head>
    <meta charset="utf-8">
    <title>Snake Game || iiqrah</title>
  </head>

  <body>
    
    <h1> My Snake Game </h1>
    
  </body>
</html>
```

- If you are using Atom, type 'html' + Enter to get the basic html structure code


### Linking CS and JS with HTML

- Link the css file with html by adding <link rel="stylesheet" type="text/css" href="css/style.css"> right before the </head>
- Link the js file with html by adding <script src="js/snake.js"></script> right before the </body>

### Creation of gameScreen

- Add the canvas tag, <canvas id="gameScreen" width="300" height="300"></canvas> , right after the <body> but before the <script>
  
### Add a bit of CSS 

- Lets add some simple style to <h1> and <canva> to check if we have linked our css file correctly
- Add the following code in styles.css:

```css
h1{
  color: red;
  text-align: center;
}

canvas{
  display: block;
  margin: 0 auto;
}
```

### Add a bit of JS 

- Lets add some js code to test if we have linked our js script correctly
- Add the following code in snake.js:

```javascript
  /** CONSTANTS **/
  const CANVAS_BORDER_COLOUR ='black';
  const CANVAS_BACKGROUND_COLOUR ="green";

  // Get the canvas element
  var gameScreen = document.getElementById("gameScreen");
  // Return a two dimensional drawing context
  var ctx = gameScreen.getContext("2d");

  //  Select the colour to fill the canvas
  ctx.fillStyle=CANVAS_BACKGROUND_COLOUR;
  //  Select the colour for the border of the canvas
  ctx.strokestyle=CANVAS_BORDER_COLOUR;

  // Draw a "filled" rectangle to cover the entire canvas
  ctx.fillRect(0, 0, gameScreen.width, gameScreen.height);
  // Draw a "border" around the entire canvas
  ctx.strokeRect(0, 0, gameScreen.width, gameScreen.height);
```

## Code Preview

- If all goes well, this is how it should look like. 

![Screenshot of how the project should look like atthis point](https://i.imgur.com/07y34Xd.png)


  





