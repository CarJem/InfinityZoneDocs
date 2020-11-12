
Platform
=======
```
TODO: Unfinished Documentation
```

**Bio:** 

Found in Almost Every Zone in Sonic Mania, this object allows Sonic to either cross gaps and get to places he otherwise couldn’t do on his own, or simply get to places without doing anything at all, lazily. However, some aren’t meant to carry sonic, some move objects, some can even hurt Sonic if you set them up correctly. There’s plenty of things you can do with platforms.

Attributes
-----------

**Type:**

Determines the Platform’s Behavior

    * 0 - Default
    * 1 - Collapsing Platform; Shortly after the player stands on this type, the platform will begin to fall. This type will respawn if the player goes far away enough as long as amplitudeX is set to 0, otherwise it will be gone until the scene is restarted.
    * 2 - Normal Up and Down Moving Platforms
    * 3 - Circular Path Moving Platforms
    * 4 - Back and Forth Moving Platforms; Move from side to side.
    * 5 - Unknown, Used with PlatformControl object
    * 6 - Player Pushable Platform
    * 7 - OOZ Moving Spike Platforms; They move back and forth when they hit walls.
    * 8 - Waiting Moving Platforms; These Wait for the Player to be on top of them, and when the player is, it will move to its destination.
    * 9 - Waiting Moving Platforms(with Bobbing); These Wait for the Player to be on top of them, and when the player is, it will move to its destination.
    * 10 - Moves when player is standing on them
    * 11 - Circular TMZ2 Style Platform Lift Thing?
    * 12 - ???
    * 13 - ???
    * 14 - ???
    * 15 - ???
    * 16 - ???

**Amplitude:**

Determines where the platform will move (relative to the place it’s placed) if it is a moving type set by the type variable.

**Speed:**

Determines how fast the platform will move if it’s a type that moves. Must be higher than 0 for the platform to able to move, the larger it is, the faster the platform will move into position.

**HasTension:**

When using Type 3, determines if you want to see the tension bars (the chains that attach the platform the it’s initial position) or not.

**FrameID:**

Determines what Texture/Frame to use. The Frames it uses can be found in the Platform.bin for the Zone in it’s Sprite Folder. Attribute has an upper limit of 127. If set to -1, it will appear Invisible, useful in combination with ChildCount.

**Collision:**

Determines how the platform will behave when an player interacts with it. Your Results may vary depending on what your Type Attribute is set to.

	* 0 - Solid on Top only
	* 1 - Solid from all sides
	* 2 - No collision
	* 3 - Hazardous from all sides
	* 4 - ???
	* 5 - Hazardous from left and right sides
	* 6 - Hazardous from bottom only
	* 7 - Hazardous from top only
	* 8 - Platform makes Sonic look like he is on a turntable
	* 9 - Sticky from all sides
	* 10 - Sticky from top only
	* 11 - Sticky from left side only
	* 12 - Sticky from right side only
	* 13 - Sticky from bottom side only
	* 14 - Platform makes Sonic look like he is on a barstool
	* 15 - ???

**TileOrigin:**

Usage Unknown

**ChildCount:**

Depending on it’s value, this attribute causes objects to move with the platform. For Example, if you set childCount to 2, and the Entity Slot is 287, Entities with a Slot of 288, and 289 will move with the platform.

**Angle:**

When Using Type 3, sets the starting point for the platform on its circular path.
