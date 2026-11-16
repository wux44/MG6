# MG6

1. The entire for loop completes before the Update method finishes. It does not automatically spread its iterations across multiple frames. If the loop takes too long, the game will lag or freeze.
2. One issue is that the cat can pass through walls or ceilings while jumping upward. The code disables the cat’s entire collider whenever its vertical velocity is greater than zero. This disables collisions with all objects using that collider, instead of only allowing the cat to pass through the underside of platforms. The collider is enabled again when the cat stops rising or starts falling.

