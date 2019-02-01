# BuildSystem
A simple Modular Building System for Unity 3D

In the repo you will find a Unity Package. The package contains all scripts, models, and prefabs that I used to build the system in the tutorial video. 

Below you will find a quick guide on how to set up your models. Remember you will need 2 different models for each thing you want to build. One will be the actual model you player can walk on and interact with in your game. The other will be the "preview" that the player can position in your game. 


<h1>Setup</h1>

 <h2>-------Tags and Layers------</h2>
 <br/>-You will need to make a different Tag for each snap point type, such as Foundation_SnapPoints, Wall_SnapPoints.....
 <br/>-Create a new layer for you preview gameobject. This is important and if you skip this step it will glich out 

<h2>--------SnapPoint--------</h2>
<br/>SphereCollider -> Radius = 0.25
<br/>SphereCollider -> IsTrigger = True

<h2>--------Prefab-----------</h2>
<br/>-Just add a material so it stands out(if using a primitive)
<br/>-No tag
<br/>-No layer

<h2>--------Preview GameObject--------</h2>
<br/>Layer -> Set it to somthing like BuildLayer(or whatever you want it to be)
<br/>Box Collider -> IsTrigger = True
<br/>Rigidbody -> useGravity = False
<br/>Rigidbody -> isKinematic = true
<br/>Add the Preview Script 
