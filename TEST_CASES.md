TEST_CASES

**Test Case #1: Rotation**

**Given** the game is running and no platform has been rotated

**When** the player presses 'A'

**Then** the current platform rotates

**And** no other platforms can be rotated afterward
______________________________________________

Test Case #2: Platform Gets Cut Correctly

**Given** a platform is incoming from one of the sides

**When** the player left-clicks while the platform is not aligned (out of bounds)

**Then** the platform gets cut so it fits within the bounds
______________________________________________

**Test Case #3: Next Platform is Resized Correctly After Cut**

**Given** a platform has been cut

**When** a new platform spawns

**Then** the new platform has the same size as the cut version
______________________________________________

**Test Case #4: Platform Cut Correctly After Rotation**

**Given** a platform has been rotated

**When** it gets cut

**Then** the cut keeps the platform within bounds
______________________________________________

**Test Case #5: Platform Resized Correctly After Rotation**

**Given** a rotated platform has been cut
**When** a new platform spawns
**Then** the new platform has the same size as the cut version
______________________________________________

**Test Case #6: Placing and Rotating at the Same Time**

**Given** a platform is coming from the side
**When** the player places and rotates the platform simultaneously
**Then** it gets placed and rotated normally
**And** no abnormal behavior occurs
______________________________________________

**Test Case #7: Particles Appear When Platform is Aligned**

**Given** a platform is incoming
**When** it becomes perfectly aligned
**Then** particles appear around the platform’s edges
______________________________________________

**Test Case #8: Particles Appear When Rotated**

**Given** the platform has not been rotated

**When** the player rotates it

**Then** particles appear to indicate the alignment area
______________________________________________

**Test Case #9: Score Gets Updated Correctly**

**Given** a platform is incoming

**When** it is placed and the game is not over

**Then** the score increases by 1
______________________________________________

**Test Case #10: Time to Break It**

**Given** the game is running

**When** the player performs unexpected or extreme actions (e.g., spamming rotation/placement, overlapping, boundary cases)

**Then** verify if any crashes, freezes, or logic bugs occur




