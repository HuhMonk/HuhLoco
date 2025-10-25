<a href="https://discord.gg/8tuuGjuEE9"><img src="https://img.shields.io/badge/discord-brightgreen.svg?style=for-the-badge&logo=discord&colorA=23272a&colorB=7289da" alt="Discord!"></a>

# HuhLoco
a unity vr/xr locomotion system using physics to move around by moving your hands on the ground like the game Gorilla Tag


# Setup
**Make sure you have XR Inputs installed for it to work if you dont get it from** https://github.com/HuhMonk/XRInputs/releases                   
When you import HuhLoco unity package into unity open the folder you imported called Physics Rig
then open Prefabs and drag in the XR Origin Physics prefab into your scene and then setups is done
remember that for best networking on your multiplayer manager right and left hands should be the physics hands

# Recommended Settings
Settings I Would Recommend for what type of physics you want : **This is on the PhysicsRig Script**

- Spring = 5000
- Damper = 100 or 125
- Velocity Limit = 6.5
- Solver Iterations = 50
- Solver Velocity Iterations = 40

# Documentation

for using any of these things remember to add this into your script
```csharp
using HuhLoco;
```

you can use the instance from
```csharp
HuhLoco.PhysicsRig.Instance
```
