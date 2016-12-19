#AutoGlitch#

__Package__ : com.danehansen.display
__Class__ : public class AutoGlitch
__Inheritance__ : AutoGlitch > Glitch > Object

Instances of this class will automatically glitch out a random amount for random amounts of times

##Public Properties##

* __cleanTime__ : Number
Maximum duration in milliseconds that the image will remain clean while activated.
* __glitchTime__ : Number
Maximum duration in milliseconds that the image will remain glitched while activated.
* __fuckLimit__ : uint
Maximum amount of fucked that the image will get while activated.

##Public Methods##

* __AutoGlitch__(element:Element, cleanTime:Number = 1500, glitchTime:Number = 100, fuckLimit:uint = 5)
Creates an AutoGlitch object, using a provided image element or other element with a background-image applied.
* __activate__()
Activates the instance, starts the glitching timeouts.
* __deactivate__()
Deactivates the instance by killing the timeouts and returning the image to its clean state.

```javascript
// example
import Glitch from 'image-glitch'
const image = new Glitch(document.getElementById('target'), 3000, 100, 26)
```

# Credit

All code, ideas, and everything written by @danehansen. I just repackaged it and published to npm so I could use it.
