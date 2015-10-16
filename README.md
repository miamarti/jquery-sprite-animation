jQuery Sprite Animation
===========
[jquery-sprite-animation] Sprite Animation on jQuery

<p>
  <img src="https://img.shields.io/badge/jquery--sprite--animation-release-green.svg">
  <img src="https://img.shields.io/badge/version-1.0.0-blue.svg">
  <img src="https://img.shields.io/bower/v/bootstrap.svg">
</p>

## Bower install de dependency
```
$ bower install jquery-sprite-animation --save
```

## HTML Page include
```
<script src="bower_components/jquery-sprite-animation/dist/jquery-sprite.min.js"></script>
```

## Creating an animation
```
$(document).ready(function() {
    
    var config = {
        slide: 1,
        fps: 12,
        frames: 17,
        cycles: {
            '1': {
                url: 'assets/slides/slide01/Cycle-0.sprite.png'
            },
            '2': {
                url: 'assets/slides/slide01/Cycle-1.sprite.png'
            },
            '3': {
                url: 'assets/slides/slide01/Cycle-2.sprite.png'
            },
            '4': {
                url: 'assets/slides/slide01/Cycle-3.sprite.png'
            }
        },
        onPlay: function(){
        },
        onPause: function(){
        },
        onFrame: function(obj){
        }
    };
    $('.slide').sprite(config);
});
```

## Methods

### #play
Starts playing continuous animation that doesn't stop until interrupted by other methods.
```
$('.slide').play();
```

### #Pause
Pauses the current animation.
```
$('.slide').pause();
```

### #Toggle
Pauses when playing, resumes when paused.
```
$('.slide').toggle();
```

## Based on Darsa Motion
- http://darsa.in/motio/
