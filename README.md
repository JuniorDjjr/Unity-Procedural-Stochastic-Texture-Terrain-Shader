# Unity Procedural Stochastic Texture Terrain Shader
Procedural Stochastic Texturing for Unity URP terrain, to fix repeated tile patterns on terrain textures.  

**For other materials (Shader Graph node): https://github.com/JuniorDjjr/UnityProceduralStochasticTexturingNode**  

I'm trying to keep updated to lastest Unity/URP version, so if you use old Unity (with old URP version), check commits for old versions of this shader. My first release version was tested on Unity 2019.  

![](https://1.bp.blogspot.com/-nQy-BVqnTPM/XrnbfO7LctI/AAAAAAAAYOY/mAjoKityEYIA3fKWPGhHQ7LCDaPhVAniACK4BGAsYHg/w1175-h1170/warpunk-game-procedural-stochastic-terrain-shader-texturing-unity-urp.jpg)

**Limitation:** The UV is calculated locally at the object's UV position, so the edges of objects/terrains will not be seamless for the same texture. Someone more experienced than me can try UV randomation by world space, or you can try something like vertex color to define a mask where the effect is applied (would need to edit the terrain shader).

From [rotoscope](https://www.reddit.com/user/rotoscope-/) adaptation, based on [Thomas Deliot and Eric Heitz paper](https://drive.google.com/file/d/1QecekuuyWgw68HU9tg6ENfrCTCVIjm6l/view), implemented by me (Junior_Djjr) for Unity terrain lit shader with Universal Render Pipeline / URP.  
