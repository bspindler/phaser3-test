# Testing out phaser 3 HTML5 Game Framework
https://phaser.io/tutorials/making-your-first-phaser-3-game 

# Phaser 3 Game
everything is in public/index.html and public/assets

## Examples
- https://labs.phaser.io/index.html

## References
- https://github.com/digitsensitive/phaser3-typescript

# See the game
- `npm start`
- open http://localhost:3000 

# Notes on Phaser 3 Game Development

> Phaser3 is very simple to get started with, simply add the following to your .html file
```
<head>
    <script src="//cdn.jsdelivr.net/npm/phaser@3.6.0/dist/phaser.min.js"></script>
</head>
```

> Basic structure of an app:

```
var config = {
    type: Phaser.AUTO,
    width: 800,
    height: 600,
    scene: {
        preload: preload,
        create: create,
        update: update
    }
};

var game = new Phaser.Game(config);

function preload ()
{
}

function create ()
{
}

function update ()
{
}
```
> Refactoring to Scenes
Unbeknownst to you maybe, you were creating a scene with that code above: 
```
    scene: {
        preload: preload,
        create: create,
        update: update
    }
```
