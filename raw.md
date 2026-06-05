
Mods documentation
Intrudoction
Quick start
Simple decorative mod
Tools
3D editor
Text editor
Graphics editor
Creation of 3D models
Textures
Structure of a mod
info.json
Wheel mod
Custom Size Wheel mod
Functional mods (lua)
Introduction
Start
Scripting
Hello world
Connection points
Evertech Sandbox API
The content of es
es.TimeScale - the scale of time (default is 1)
es.DeltaTime - the time since previous frame (Update)
es.FixedDeltaTime - the interval between FixedUpdate calls
es.SetSoundVolume(float volume) - set sound volume of the current item
es.SetSoundLoop(bool value) - if the sound should loop
es.PlaySound(string path) - play the sound, path - the path to a sound file (only .wav)
es.Player - functions related to a player
es.MultiBlock - returns the MultiBlock object of the current mod item.
es.Quaternion - contains functions for work with quaternions.
es.CreateMultiblock
es.FindMultiBlock
es.TryGetMultiBlock - getting the multiblock with help of raycast
es.TryGetMultiBlockFromConnection - get multiblock from connection
es.ConnectConnections - connect two multiblock connections
es.DisconnectConnections - disconnect two multiblock connections
es.Raycast - measure a distance
Saving and reading the data to and from a save file.
Saving
Reading saved data
Deleting the key
GUI
Textures
Mesh
MultiBlock
Root
Block
Transform
Rigidbody
Player
Switch
Sign
ModBlock
Mods documentation
Intrudoction
This document describes all possibilities of Evertech Sandbox Mod API.

Evertech Sandbox - is a mobile game, a physics sandbox, where players may create complex constructions and mechanisms from simple blocks.

With help of mods players can extend the possibilities of the game and add new items with different look and functionality.

Quick start
Simple decorative mod
Tools
In order to create the most simple decorative mod you will need:

3D editor
Text editor
Graphics editor
3D editor
You can use any 3D editor which can export 3D models as .obj files. But better if it can also allow you to edit UV layout.

If you are on a PC then the choice of 3D editors is huge, the most popular is Blender3d. If you have only Android phone, then the best choice is Spacedraw.

Text editor
If you are on a PC then it can be ordinary notepad. But I use Sublime Text. If you are on Android, then I can recommend QuickEdit

Graphics editor
There are many editors. The most popular for PC is Photoshop, but there are other free alternatives like Gimp.

Also for texture creation the true proffesionals use software like Substance Painter, but I cannot suggest anything here, because I am just a programmer and I cannot create 3d models :)

Creation of 3D models
As I already said, I am not a 3d Modeller, so I can't teach you to create 3d models. But there are many tutorials in the internet, so if you can't make 3d models you can learn it with help of google. When you create your 3d model, position it right in the center of the world.

After you created a 3d model, export it as .obj file.

Textures
Most likely you 3d models should have a texture.

The game uses PBR (Physically based rendering)

The mod can have 3 types of textures (but don't be afraid, in a simple case you can use just one diffuse texture):

Diffuse or albedo
Normal map
Metallic Map (https://docs.unity3d.com/Manual/StandardShaderMaterialParameterMetallic.html)
Diffuse map stores the color.

Normal map allows objects to look like if they had more polygons then in reality. The normal map describes the direction in which the light should reflect from the surface.

Metallic map

(https://docs.unity3d.com/Manual/StandardShaderMaterialParameterMetallic.html)

The game is made in Unity3d, so the metallic map consists of two maps (metallic and smoothness). The are united to save a memory. They are stored in different channels of the texture. The red channel is used to store a metallic values. The alpha channel is used to store the smoothness values. Metallic values just describe which parts of the texture are metallic and which not. White pixels are metallic, black are not metallic and ususally you should escape intermediate values but for some materials they also can be used but I am not going to describe it in more details because I don't know them myself. smoothness values - describe how smooth is the surface. White pixels means 100% mirror surface and very glossy, and black pixels will not reflect at all.

Structure of a mod
So, you hav a 3d model in an .obj format and a set of textures.

In order to create a mod you need to create a folder, put your meshes and textures in it and create a file info.json to describe a mod. The mod has the following structure:

picture of a file structure

As an example download this birch mod download birch mod (bereza.zip)

mod preview

If you download bereza.zip and unpack it, you will see a file inside called info.json, and two directories "meshes" and "textures". In a textures folder there are 3 files: Bereza.png (a texture for a 3d model), icon.png (an icon of an item, which will be shown in inventory), preview.png (preivew of a mod which is displayed in mods catalog). In a meshes folder you can see a 3d model in a format of OBJ, also there is a .mtl but the game doesn't read it and you can safely remove it.

info.json
Let's look at the content of info.json

{
    "name" : "Birch Tree",
    "preview" : "textures/preview.png",
    "version" : "1.0.0",
    "author" : "Darwin",
    "description" : "Birch tree from Low Poly Trees collection. Author: https://vk.com/2much4",

    "simpleblocks" : [
        {
            "uuid" : "025df71c-1c0e-4394-8bd2-94f583886d66",
            "name" : "Birch tree",
            "description" : "Tree from Low Poly Trees collection.",
            "icon" : "textures/icon.png",
            "dif" : "textures/Bereza.png",
            "nor" : "",
            "normScale" : 1,
            "met" : "",
            "smoothness" : 0.0,
            "mesh" : "meshes/bereza.obj",
            "scale" : 2.7
        }
    ]
}
The content of info.json must be in a json format. It has the following fields:

name - the name of the mod
preview - a picture, which will be shown in a mods catalog
version - version name
author - creator of the mod
description - the description of the mod which will be shown in a mods catalog
simpleblocks - an array of items this mod adds to the game
Every item of an array simpleblocks has the following fields:

uuid - the unique identifier of an item IMPORTANT - it should be unique for every item. Don't copy it from other mods otherwise there will be conflicts when installing several mods. To generate a uuid go to www.uuidgenerator.net and copy it from there, to generate a new uuid just refresh the page.
name - the name of the item
description - description of an item
icon - the icon which will be shown in the inventory
dif - the texture. Ordinary diffuse texture. Also known as albedo
nor - the normal map. If you have it.
normScale - the scale of a normalmap effect from 0 to 1
met - the metallic map if you have it.
smoothness - the smoothness of a surface from 0 to 1
mesh - the path to a 3d model
scale - the scale of a 3d model. For models from blender it is usually 1
Wheel mod
To make a wheel mod you do everything like the above but add a new field "collider" and set it's value to "wheel" and this mod will have a collider in a shape of a cylinder with a size of 3х3.

In the process of creating a 3d model put it in the center and orient it horizontally like in this screenshot..

a wheel in a blender3d

Example:

wheelmod2.7z

There is a .psd in the archive, it can be safely removed, it is just a source of the texture in case somebody wants to edit it.

screenshot

Custom Size Wheel mod
Starting from recent versions, you can create wheel mods with custom sizes using the "collider": "sizable_wheel" option. This gives you full control over the wheel dimensions and positioning.

When using sizable_wheel, you can specify:

colliderOptions - controls the physical collider (collision shape):

SizeX - width of the wheel collider
SizeY - thickness of the wheel collider
SizeZ - diameter/height of the wheel collider
OffsetX - horizontal offset of the collider (rarely needed)
OffsetY - vertical offset of the collider
OffsetZ - depth offset of the collider (rarely needed)
meshOptions - controls the visual mesh positioning (works for all collider types):

OffsetY - vertical offset of the visual mesh (independent from collider offset)
This separation allows you to adjust the visual appearance independently from the physical collision shape, which is useful when your wheel mesh doesn't perfectly align with the center. Note that meshOptions can be used with any collider type, not just sizable_wheel.

Example:

{
    "uuid" : "YOU SHOULD GENERATE A UNIQUE ID HERE",
    "name" : "Tank wheel",
    "description" : "Tank wheel",
    "icon" : "textures/ti.jpg",
    "dif" : "textures/t.jpg",
    "collider" : "sizable_wheel",
    "colliderOptions" : {
        "SizeX": 2.98,
        "SizeY": 0.35,
        "SizeZ": 2.98,
        "OffsetY": 0.15
    },
    "nor" : "textures/tn.png",
    "normScale" : 1,
    "met" : "textures/1m.jpg",
    "smoothness" : 0.5,
    "mesh" : "meshes/twheel.obj",
    "scale" : 1,
    "meshOptions": {
        "OffsetY": 0.15
    }
}
Tips:

Use SizeZ to control the wheel diameter (the main rolling dimension)
Use SizeY to control wheel thickness/width
Use SizeX for the lateral dimension (usually equals SizeZ for round wheels)
The OffsetY in both colliderOptions and meshOptions is often needed to align the wheel properly with the attachment point
Functional mods (lua)
Introduction
Functional mods are mods which contain scripts in lua programming language. For example destruction mod or a rope mod. With help of scripts you can add any functionality to the game as far as your imagination can go or as far as API will let you. If you need more methods in mod API, send me a message to vitaly.sumin+mods@gmail.com

Start
I hope you already know how to make decorative mods or at least read about it, if no then go up of this page.

To add a script to your mod you need to create a .lua file and add a reference to it in a info.json file.

Let's look how it is made in a propeller mod:

{
    "name" : "Propeller mod",
    "preview" : "textures/preview.jpg",
    "version" : "2.1",
    "author" : "Own Guest & Veka",
    "description" : "For activation, you must install a switch on the screw itself",

    "simpleblocks" : [
        {
            "uuid" : "fe8f4eb0-bca1-44b1-bee4-35d3f65a5365",
            "name" : "Propeller",
            "description" : "Propeller",
            "icon" : "textures/Prop.jpg",
            "dif" : "textures/texture.png",
            "nor" : "textures/texturen.png",
            "normScale" : 1,
            "met" : "textures/texturem.jpg",
            "smoothness" : 0.5,
            "mesh" : "meshes/propeller.obj",
            "scale" : 0.5,
            "script" : "script.lua"
        }
    ]
}
In the description of an item there is a new field "script", the value of this field is the path to a script. I recommend creating a special folder for scripts called "scripts" and if you put your scripts inside this folder the path would look like this: scripts/script.lua

Scripting
The game will call certain methods from your scripts. At present moment there are 4 such methods:

funcion onPlace()

end

function start()

end

function update()

end

function fixedUpdate()

end
If your script contains these methods, the game will call them:

onPlace - is called when the player placed this item
start - is called in the moment of creation of an item (after the player placed the item, or after loading a saved world)
update - is called every frame, 30-60 times per second depending on fps
fixedUpdate - is called 50 times per second and is used for physics simulation
Hello world
Let's write our first program called Hello world

function onPlace()
    print('Hello world')
end
If you create such script and set it in info.json you will see a "Hello world" message in the logs when you place the item.

To activate a console, pause the game. Go to Settings -> Lua Settings and press the button "Show console". Or just swipe with two fingers down and the console should appear. Another way to see these messages is to go to settings, common settings and check a tickbox "Debug info". After that you will see last 5 messages in the top left corner.

Now if you created this mod and turned on logs and placed this item you will see a message: LUA: Hello world

lua console

Also this console will show errors of lua scripts.

Connection points
You can create modified items which have a connection point like other ingame items have (engine, button, sensor). The player can connect a button to this point and your mod can do something special when player presses the button. Actually the item can have several connection points, so in info.json it is described as an array (connections)

To create a connection point you must describe it in info.json

Example:

{
    "name" : "Propeller mod",
    "preview" : "textures/preview.jpg",
    "version" : "2.1",
    "author" : "Own Guest & Veka",
    "description" : "For activation, you must install a switch on the screw itself",    

    "simpleblocks" : [
        {
            "uuid" : "fe8f4eb0-bca1-44b1-bee4-35d3f65a5365",
            "name" : "Propeller",
            "description" : "Propeller",
            "icon" : "textures/Prop.jpg",
            "dif" : "textures/texture.png",
            "nor" : "textures/texturen.png",
            "normScale" : 1,
            "met" : "textures/texturem.jpg",
            "smoothness" : 0.5,
            "mesh" : "meshes/propeller.obj",
            "scale" : 0.5,
            "script" : "script.lua",
            "connections" : [
                {
                    "type" : "signalReceiver", //signalReceiver, signalSender, signalReceiverSender
                    "color" : "#ff0000",
                    "connectionsLimit" : 1,
                    "relativePosition" : {"X":0, "Y":1, "Z":0}
                }
            ]
        }
    ]
}
Note: // - it is just a comment, everything after it is ignored by a compiler.

As you can see in info.json there is a field "connections". It is an array, where each element is a description of a connection point. Currently the connection point can have one of three types (type):

signalReceiver
signalSender
signalReceiverSender
signalReceiver - this connection point can only receave a signal.

signalSender - this point can only send a signal.

signalReceiverSender - this point can receave and send a signal.

Next field (color), it has a format of html color. It starts with a symbol # and then there is a hex-value of a color. In this example it is #ff0000 a red color.

Next field "connectionsLimit" determines how many incoming connections this point allows.

Next field "relativePosition" describes a position relative of the center of the item.

So we now know how to describe a connection point it info.json, now we need to learn how to use it in the code.

You will need to add couple of methods to your script.

The first method, which you need to add is a method/function, which allows the game to understand if it can connect some item with your modified item.

function canConnect(itemType, thisConnectionIndex, otherConnectionIndex, reverse)
    
    if (itemType == "PushButton" or 
        itemType == "Sensor" or
        itemType == "Switch" or
        itemType == "Timer"


        ) and thisConnectionIndex == 1 and otherConnectionIndex == 1 then
        
        return true
    end

    return false
end
Let's look at the arguments of a function. There is 4 arguments:

itemType - it is a type of an item to which the player is trying to connect your mod. If it is a mod then it will equal to uuid of another mod.

thisConnectionIndex - it is an index of a connection point of this mod, for example if the mod only have one connection point then the index will equal to 1. If there are more points then the order is determined by the order in which they were described in info.json.

otherConnectionIndex - it is an index of connection point of another item.

reverse - true if the player started to connect from the current item to another and false if otherwise. (probably I missed something here...)

If this method returns false the line between these points will not be created, but if it returns true the line is created.

If your item has a point of connection which can receive a signal you should create a method to process the incoming signal.

function onSignalReceived(value, fromGuid, toConnectionIndex)
    switchOn = value
end
This method has 3 parameters.

value - It is a value of the signal (true or false)

fromGuid - each point of connection has it's unique identifier GUID. If your point of connection allows connecting of more then one connections then it might be useful for you.

toConnectionIndex - it's an index of a connection point to which the signal came. (you might use it in case your item has more then one point)

And one more method, which is called when the line between connection points is removed, so you can turn your item off for example.

function onInputRemoved(fromGuid, toConnectionIndex)
    switchOn = false
end
If your item must send a signal, then you need to call this method

es.SetConnectionOutput(output, index)
where "output" - it is a "true" or a "false", the output value, and index is an "index" of a connection point

Evertech Sandbox API
All methods of Evertech Sandbox API are in the object es

For example, to get the position of the player you can write:

print(es.Player.Position[1] .. ";" .. es.Player.Position[2] .. ";" .. es.Player.Position[3])
The content of es
es.TimeScale - the scale of time (default is 1)
es.DeltaTime - the time since previous frame (Update)
es.FixedDeltaTime - the interval between FixedUpdate calls
es.SetSoundVolume(float volume) - set sound volume of the current item
es.SetSoundLoop(bool value) - if the sound should loop
es.PlaySound(string path) - play the sound, path - the path to a sound file (only .wav)
es.Player - functions related to a player
es.MultiBlock - returns the MultiBlock object of the current mod item.
Read more about MultiBlock later in this documentation

es.Quaternion - contains functions for work with quaternions.
Quaternion is a way to store a rotation of an object. It is a complex mathematical thing, and we need help function to work with it.

Quaternion es.Quaternion.Euler(x, y, z) - returns the quaternion from 3 euler angles. Euler angles are the angles by 3 axises.
Quaternion es.Quaternion.LookRotation(Vector3 forward) - returns the quaternion by direction
Quaternion es.Quaternion.LookRotation(Vector3 forward, Vector3 upwards) - you can pass the up direction
Vector3 es.Quaternion.ToEulerAngles(Quaternion rotation) - converts quaternion into euler angles
Quaternion es.Quaternion.FromToRotation(Vector3 fromDirection, Vector3 toDirection) - returns rotation, which rotates fromDirection to toDirection
Quaternion es.Quaternion.Inverse(Quaternion rotation) - retunrs inverted rotation
Quaternion es.Quaternion.Multiply(Quaternion a, Quaternion b) - multiplies rotation a with rotation b
Quaternion es.Quaternion.MultiplyByVector(Quaternion a, Vector3 vector) - multiplies quaternion a by vector
Quaternion es.Quaternion.RotateTowards(Quaternion from, Quaternion to, float maxDegreesDelta) - rotates rotation in direction of another rotation limited by maximum delta in degrees (for smooth rotation)
Quaternion es.Quaternion.AngleAxis(float angle, Vector3 axis) - Creates a rotation which rotates angle degrees around axis.
es.CreateMultiblock
string es.CreateMultiblock(string itemType, Root root, Vector3 relativePosition, Quaternion relativeRotation) - creates a multiblock
string es.CreateMultiblock(string itemType, Root root, Vector3 relativePosition, Quaternion relativeRotation, string moduuid) - creates a multiblock with additional parameter moduuid. To create a cubic modblock use itemType = SimpleModBlock, for a wheel mod - WheelModBlock This method returns a guid of newly created multiblock, but it is not guaranteed to create a multiblock. Use the returned guid to find a multiblock. If you can't find a multiblock then possibly it failed to create it.
es.FindMultiBlock
MultiBlock es.FindMultiBlock(string guid) - find a multiblock by it's guid, if not found then it returns nil
es.TryGetMultiBlock - getting the multiblock with help of raycast
es.TryGetMultiBlock(Vector3 pos, Vector3 dir, float rayLength) - pos - position of the start of the ray, dir - direction, rayLength - the lenght of the ray, the more the rayLength the lower the fps
es.TryGetMultiBlockFromConnection - get multiblock from connection
es.TryGetMultiBlockFromConnection(int connectionPointIndex, bool incoming, int connectionIndex) - returns MultiBlock or nil, arguments: connectionPointIndex - index of a connection point of the current item, incoming - incoming or outcoming connection (these are different lists), connectionIndex - index of the connection. Indices start with 1.
es.ConnectConnections - connect two multiblock connections
bool es.ConnectConnections(string multiblockAguid, int connectionAindex, string multiblockBguid, int connectionBindex) - connects two connection points between multiblocks. Returns true if connection was successful, false otherwise. Parameters: multiblockAguid - GUID of first multiblock, connectionAindex - connection point index of first multiblock (1-based), multiblockBguid - GUID of second multiblock, connectionBindex - connection point index of second multiblock (1-based).
es.DisconnectConnections - disconnect two multiblock connections
void es.DisconnectConnections(string multiblockAguid, int connectionAindex, string multiblockBguid, int connectionBindex) - disconnects two connection points between multiblocks. Parameters: multiblockAguid - GUID of first multiblock, connectionAindex - connection point index of first multiblock (1-based), multiblockBguid - GUID of second multiblock, connectionBindex - connection point index of second multiblock (1-based).