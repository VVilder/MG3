# MG3
## Devlog
1. The inspector showed 0 for the float and int. The bool was unchecked and the string was empty so defaults are 0, 0, false, and an empty string.
2. Unity calls it by itself on every frame of the active component that has an update method. So if I write what i want to happen each frame unity will run it for me. 
3. KickWeapon only last a split second because when the player presses space, ActivateKick turns the kick on and calls BeginTimer with _lifetimeSeconds. Since it's only 0.2 seconds, the Timer’s Update subtracts Time.deltaTime from the time left, and KickWeapon’s own Update checks IsFinished. Then the kick is turned back off once the timer is finished

## Open-Source assets
- [Cat fighter spritesheet](https://opengameart.org/content/cat-fighter-sprite-sheet)
- [Food sprites](https://rcpstd.itch.io/pixel-food-pack)