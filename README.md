<a href="https://discord.gg/8tuuGjuEE9"><img src="https://img.shields.io/badge/discord-brightgreen.svg?style=for-the-badge&logo=discord&colorA=23272a&colorB=7289da" alt="Discord!"></a>

# HuhLoco
a unity vr/xr locomotion system using physics to move around by moving your hands on the ground like the game Gorilla Tag


# Setup
**Make sure you have XR Inputs installed for it to work if you dont get it from** https://github.com/HuhMonk/XRInputs/releases                   
When you import HuhLoco unity package into unity open the folder you imported called Physics Rig
then open Prefabs and drag in the HuhLoco (Physics ) prefab into your scene and then setups is done
remember that for best networking on your multiplayer manager right and left hands should be the physics hands

# Recommended Settings
Settings I Would Recommend for what type of physics you want : **This is on the RandomPhysics Script**

- Spring = 500000
- Damper = 5000
- Velocity Limit = 10

# Documentation

for using any of these things remember to add this into your script
```csharp
using HuhLoco;
```
