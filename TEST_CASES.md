TEST_CASES

Test #id: 1
Title: Rotation

Given: Game is running and no platform has been rotated
When: press 'a'
Then: platform gets rotated and none of the paltforms can be rotated again afterwards

Test #id: 2
Title: Platform gets cut correctly

Given: Platform is coming from one of the sides
 When: Left click is pressed and platform is not alinged (out of bounds)
 Then: Platform gets cut so that it's within bounds

Test #id: 3
Title: Next platform is resized correctly after cut

Given: Platform has been cut
 When: New platform gets spawned to the scene
 Then: New platform has the same size as the cut version

Test #id: 4
Title: Platform cut correctly after rotation

Given: Platform has been rotated
 When: Gets cut
 Then: Platform gets cut so that it's within bounds

Test #id: 5
Title: Platform resized correctly after rotation

Given: Rotated platform gets cut
 When: New platform spawns
 Then: New platform has the same size as the cut version

Test #id: 6
Title: Placing and rotating at the same time

Given: Platform is coming from the side
 When: Place and rotate simultaneously
 Then: It gets placed and rotated; nothing out of the ordinary happens

Test #id: 7
Title: Particles appear when platform is alinged correctly

Given: Platform incoming
 When: Alinged correctly
 Then: Particles appear around the platform's sides

Test #id: 8
Title: Particles appear when rotated

Given: Platform hasn't been rotated
 When: Platform gets rotated
 Then: Particles appear to show the area for alinging the platform

Test #id: 9
Title: Score gets updated correctly

Given: Platform incoming
 When: Gets placed and game is not lost
 Then: Score gets updated by one

Test #id: 10
Title: Time to break it

Given: Game is running
 When: Do whatever you like in order to break it somehow
 Then: See if you can find a way to break it