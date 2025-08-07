<a href="https://discord.gg/8tuuGjuEE9"><img src="https://img.shields.io/badge/discord-brightgreen.svg?style=for-the-badge&logo=discord&colorA=23272a&colorB=7289da" alt="Discord!"></a>

# HuhLoco
a unity vr/xr locomotion system using physics to move around by moving your hands on the ground like the game Gorilla Tag


# Setup
**Make sure you have XR Inputs installed for it to work if you dont get it from** https://github.com/HuhMonk/XRInputs/releases                   
When you import HuhLoco unity package into unity open the folder you imported called Physics Rig
then open Prefabs and drag in the HuhLoco (PID) prefab into your scene and then setups is done
remember that for best networking on your multiplayer manager right and left hands should be the physics hands

# Recommended Settings
Settings I Would Recommend for what type of hand physics you want : **This is on the PhysicsHand Script**

for bouncy like the vr game Capuchin Settings:
- Climb Force: 1000
- Climb Drag: 500

for slight bounce i would recommend:
- Climb Force: 3000
- Climb Drag: 1000

for non bouncy i would recommend
- Climb Force: 5000
- Climb Drag: 1500

# Documentation

for using any of these things remember to add this into your script
```csharp
using HuhLoco;
```

### Movement Restrictions
i aded a enum to The Physics Hands Called MovementAllowment where if its allowed then player can move else if its restricted player wont be able to move its mostly made for teleporting scripts but yeah

## Events

this is for physics grabbing since its the only one made so far with events some heres the example
```csharp
void Awake()
{
    GrabbingHand.OnGrab.AddListener(Grabbing);
    GrabbingHand.OnGrab.OnRelease(Release);
}

void Grabbing()
{
    Debug.Log("Grabbed");
}

void Release()
{
    Debug.Log("Released");
}
```
