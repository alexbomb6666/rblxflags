# rblxflags
Just the fork of [luavfv's](https://github.com/luafv/rbxflags/tree/master?tab=readme-ov-file) abusive fastflags (fuck putting them under a paywall)

# Physics (Abusive)
## Tool Desync
```json
{
    "DFIntSimBlockLargeLocalToolWeldManipulationsThreshold": "-1"
}
```

## Remap R6 to R15 Rigs/Weird Movement
```json
{
    "FFlagRemapAnimationR6ToR15Rig": "True"
}
```

## Weird Leg Movement
```json
{
    "DFFlagAnimatorPostProcessIK": "True"
}
```

## Adjust Hip Height Clamps
```json
{
    "DFIntHipHeightClamp": "-48"
}
```

## Random High Jumps
```json
{
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```

## Drunk
```json
{
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
    "DFFlagSimHumanoidTimestepModelUpdate": "True"
}
```

## No Animations
> [!NOTE]
> Stops the game from trying to replicate your animations in the server. You dont have animations in the server but you do for your client
```json
{
    "DFIntReplicatorAnimationTrackLimitPerAnimator": "-1"
}
```

## Stick unanchored parts to you
> [!TIP]
> - = up, + = down
```json
{
    "DFIntSolidFloorPercentForceApplication": "-1000",
    "DFIntNonSolidFloorPercentForceApplication": "-5000"
}
```

## Max Raycast Distance
> [!NOTE]
> Raycasting is the use of intersection tests to solve problems in Roblox. The most common use of raycasting is to determine the first object intersected by a ray. This is done by casting a virtual ray from a certain point in a direction and determining the first surface it intersected with.
> [!TIP]
> Break legs collision from 2 to -inf, kinda break camera on values over 3 noclip cam on 3
```json
{
    "DFIntRaycastMaxDistance": "3"
}
```

## Possible Super Jump
```json
{
    "DFIntNewRunningBaseGravityReductionFactorHundredth": "1500"
}
```

## Change DataSender Rate
> [!NOTE]
> A.k.a does not let you load games
```json
{
    "DFIntDataSenderRate": "-1"
}
```

## Disable Touch Events (semi-useful on obby games)
```json
{
    "DFIntTouchSenderMaxBandwidthBps": "-1"
}
```

## Fake Lag
```json
{
    "DFIntS2PhysicsSenderRate": "1"
}
```

## Invisible 1
> [!NOTE]
> Stops the physics on your character froms sending to the server so your character doesn't move for the server. You can move on your client.
```json
{
    "DFIntS2PhysicsSenderRate": "-30"
}
```

## Invisible 2
>[!NOTE]
>Locks your character's position on the server to (0, 0, 0), having the side effect of turning you invisible. This only affects the server and other clients, not you. server-sided things that rely on your position, like clicking to get tools, will not function. In some games these can be abusable.
```json
{
    "DFIntGameNetPVHeaderTranslationZeroCutoffExponent": "10"
}
```

## Invisible 3
>[!NOTE]
>Restricts the client from sending any physics-related information. This means other people can topple you over.
```json
{
    "DFIntPhysicsSenderMaxBandwidthBps": "1",
    "DFIntPhysicsSenderMaxBandwidthBpsScaling": "0"
}
```

## Clientsided Invisible
```json
{
    "FIntParallelDynamicPartsFastClusterBatchSize": "-1"
}
```

## Warp & Slowmotion
```json
{
    "DFIntMaxMissedWorldStepsRemembered": "1"
}
```
```json
{
    "DFIntMaxMissedWorldStepsRemembered": "1000"
}
```

## Noclip 1
> [!TIP]
> Adjust the value so you don't fall through the ground
```json
{
    "DFIntAssemblyExtentsExpansionStudHundredth": "-50"
}
```

## Noclip 2
> [!TIP]
> Adjust the value so you don't fall through the ground
```json
{
    "DFIntSimBroadPhasePairCountMax": "50"
}
```

## Noclip 3
> [!IMPORTANT]
> Found by @burgerboxer & @dis_spencer
```json
{
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntMaximumFreefallMoveTimeInTenths": "1000",
    "DFIntDebugSimPrimalStiffness": "0"
}
```

## Freeze (?)
```json
{
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntDebugSimPrimalLineSearch": "0"
}
```

## Hip Height
>[!NOTE]
>Very controllable bounce, only works with negative values
>[!TIP]
>0 allows you to hover
```json
{
    "DFIntMaxAltitudePDStickHipHeightPercent": "-200"
}
```

## Wallglide
>[!TIP]
>Adjust the value for the gliding to be faster (switches the direction if set to positive)
```json
{
    "DFIntUnstickForceAttackInTenths": "-4"
}
```

## Network Ownership
>[!NOTE]
>better [network ownership](https://create.roblox.com/docs/physics/network-ownership) of parts
>[!CAUTION]
>This might get you banned in some games with anticheats (Limbobbia)
```json
{
    "DFIntMinClientSimulationRadius": "2147000000",
    "DFIntMinimalSimRadiusBuffer": "2147000000",
    "DFIntMaxClientSimulationRadius": "2147000000"
}
```

## Low Gravity 1
>[!NOTE]
>`FFlagDebugSimDefaultPrimalSolver : True`
>This flag enables the new simulation engine or whatever it is.

>[!CAUTION]
>`DFIntDebugSimPrimalLineSearch : 1`
>This setting is a poor man's gravity/flight. The default value is 100:
>
>- Above 0: Low gravity.
>- Below 1 to -1: Will make gameplay weird, especially with physics.
>- Below -1: Acts as a poor man's fly mode (not really usable).

>[!IMPORTANT]
>Found by [@Amity](https://www.youtube.com/watch?v=5M411LL17B0)
```json
{
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntDebugSimPrimalLineSearch": "3"
}
```

## Void Unanchored Parts
```json
{
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntDebugSimPrimalLineSearch": "222"
}
```

## Low Gravity 2
>[!CAUTION]
>This is more buggy
```json
{
  "FFlagDebugSimDefaultPrimalSolver": "True",
  "DFIntDebugSimPrimalPreconditioner": "100",
  "DFIntDebugSimPrimalPreconditionerMinExp": "100",
  "DFIntDebugSimPrimalNewtonIts": "1",
  "FFlagDebugSimDefaultPrimalSolver": "True",
  "DFIntDebugSimPrimalWarmstartVelocity": "-150",
  "DFIntDebugSimPrimalWarmstartForce": "-775",
  "DFIntDebugSimPrimalToleranceInv": "1"
}
```

## Low Gravity 2 Control on Parts Improvement
```json
{
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntDebugSimPrimalNewtonIts": "1",
    "DFIntDebugSimPrimalPreconditioner": "15",
    "DFIntDebugSimPrimalPreconditionerMinExp": "10",
    "DFIntDebugSimPrimalToleranceInv": "1",
    "DFIntDebugSimPrimalWarmstartForce": "-150",
    "DFIntDebugSimPrimalWarmstartVelocity": "100"
}
```

## Tool Fly
```json
{
    "DFIntMinimalSimRadiusBuffer": "2147000000",
    "DFIntMinClientSimulationRadius": "2147000000",
    "DFFlagSimHumanoidTimestepModelUpdate": "True",
    "DFIntMaxClientSimulationRadius": "2147000000",
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFIntNonSolidFloorPercentForceApplication": "-12000",
    "DFIntDebugSimPrimalPreconditioner": "100",
    "DFIntDebugSimPrimalPreconditionerMinExp": "100",
    "DFIntDebugSimPrimalNewtonIts": "2",
    "DFIntDebugSimPrimalWarmstartVelocity": "-150",
    "DFIntDebugSimPrimalWarmstartForce": "-775",
    "DFIntDebugSimPrimalToleranceInv": "1"
}
```

## Backwards SpeedHax
>[!WARNING]
>Bugginess and speed depend on the value of `DFIntDebugSimPrimalWarmstartForce`. Recommended values are `775` and the value I ([luafv](https://github.com/luafv/rbxflags/tree/master?tab=readme-ov-file])) put.

>[!TIP]
>For `DFIntDebugSimPrimalWarmstartVelocity`, it’s recommended to use a value of `150`. However, it might be difficult to control.

>[!NOTE]
>I ([luafv](https://github.com/luafv/rbxflags/tree/master?tab=readme-ov-file])) may not have found this first, but I discovered this by myself.
```json
{
  "DFIntDebugSimPrimalNewtonIts": "1",
  "DFIntDebugSimPrimalPreconditioner": "69",
  "DFIntDebugSimPrimalPreconditionerMinExp": "69",
  "DFIntDebugSimPrimalToleranceInv": "1",
  "DFIntDebugSimPrimalWarmstartForce": "-885",
  "DFIntDebugSimPrimalWarmstartVelocity": "-350",
  "FFlagDebugSimDefaultPrimalSolver": "True"
}
```

## Vehicle Speed 1
```json
{
    "DFIntDebugSimPrimalWarmstartForce": "40",
    "DFIntDebugSimPrimalWarmstartVelocity": "102",
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntDebugSimPrimalLineSearch": "41"
}
```

## Vehicle Speed 2
>[!TIP]
>Adjust `DFIntDebugSimPrimalWarmstartVelocity` or `DFIntBulletContactBreakOrthogonalThresholdPercent` and find the best values for you
```json
{
    "DFIntDebugSimPrimalLineSearch": "50",
    "DFIntDebugSimPrimalWarmstartVelocity": "103",
    "DFIntDebugSimPrimalStiffness": "300",
    "DFIntBulletContactBreakOrthogonalThresholdPercent": "10000"
}
```

## GRAH GRAH (???)
```json
{
    "DFIntDebugSimPrimalLineSearch": "1",
    "DFIntDebugSimPrimalWarmstartForce": "160",
    "DFIntDebugSimPrimalWarmstartVelocity": "102",
    "FFlagDebugSimDefaultPrimalSolver": "True"
}
```

## Spin 1
>[!IMPORTANT]
>Found by @bloodraven
```json
{
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "FIntDebugSimPrimalGSLumpAlpha": "-2147483647",
    "DFIntDebugSimPrimalPreconditioner": "1100",
    "DFIntDebugSimPrimalPreconditionerMinExp": "1000",
    "DFIntDebugSimPrimalNewtonIts": "2",
    "DFIntDebugSimPrimalWarmstartVelocity": "102",
    "DFIntDebugSimPrimalWarmstartForce": "-800",
    "DFIntDebugSimPrimalToleranceInv": "1"
}
```

## Speed 2
>[!NOTE]
>Not backwards but more buggy
```json
{
    "DFIntDebugSimPrimalWarmstartForce": "-285",
    "DFIntDebugSimPrimalWarmstartVelocity": "750",
    "FIntDebugSimPrimalGSLumpAlpha": "-2147483647",
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "DFIntDebugSimPrimalPreconditioner": "100",
    "DFIntDebugSimPrimalPreconditionerMinExp": "1000",
    "DFIntDebugSimPrimalNewtonIts": "1",
    "DFIntDebugSimPrimalToleranceInv": "10",
    "DFFlagSimHumanoidTimestepModelUpdate": "True",
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFIntDebugSimPrimalLineSearch": "100"
}
```

# Abusive visuals
##Semi Fullbright
>[!NOTE]
>Might make some shaders in games go haywire. Disable/delete it from the active fflag list when not used.
```json
{
    "FFlagFastGPULightCulling3": "True",
    "FIntRenderShadowIntensity": "0",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "2147483647",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "2147483647",
    "FFlagNewLightAttenuation": "True",
    "FIntRenderShadowmapBias": "-1",
    "DFFlagDebugPauseVoxelizer": "True"
}
```

## Draws a circle under avatars
```json
{
    "FFlagDebugAvatarChatVisualization": "True",
    "FFlagEnableInGameMenuChromeABTest2": "False"
}
```

## Humanoid Outline
>[!NOTE]
>Draws an outline around every part and every humanoid
```json
{
    "DFFlagDebugDrawBroadPhaseAABBs": "True"
}
```

## fflag above but more complex
>[!NOTE]
>Draws an outline around every body part
```json
{
    "DFFlagDebugDrawBvhNodes": "True"
}
```

## Buggy ZPlane Camera
```json
{
    "FIntCameraFarZPlane": "1"
}
```

## Collision Highligher
>[!NOTE]
>Adds an UI in game, which highlights any part player touches (like ground, Meshes etc.). It's a non-functioning UI too. Also adds a blue circle to your humanoid.
```json
{
    "FFlagDebugHumanoidRendering": "True"
}
```

## Xray
```json
{
    "DFIntCullFactorPixelThresholdMainViewHighQuality": "10000",
    "DFIntCullFactorPixelThresholdMainViewLowQuality": "10000",
    "DFIntCullFactorPixelThresholdShadowMapHighQuality": "10000",
    "DFIntCullFactorPixelThresholdShadowMapLowQuality": "10000"
}
```

# Abusive Game Specific Presets
## Fling Things and People
### Send people to hell (aint posting those emojis)
```json
{
    "DFIntSimAdaptiveHumanoidPDControllerSubstepMultiplier": "-999999",
    "DFFlagSimHumanoidTimestepModelUpdate": "True",
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "FFlagSimAdaptiveTimesteppingDefault2": "True",
    "DFIntDebugSimPrimalWarmstartVelocity": "-10",
    "DFIntDebugSimPrimalWarmstartForce": "1750",
    "DFIntDebugSimPrimalPreconditioner": "-20",
    "DFIntDebugSimPrimalPreconditionerMinExp": "1000",
    "DFIntDebugSimPrimalNewtonIts": "2",
    "DFIntDebugSimPrimalToleranceInv": "2"
}
```

### Send people to hell V2
>[!TIP]
>Modify warmstart to change speed
```json
{
    "DFIntDebugSimPrimalNewtonIts": "2",
    "DFIntDebugSimPrimalPreconditioner": "1100",
    "DFIntDebugSimPrimalPreconditionerMinExp": "1000",
    "DFIntDebugSimPrimalToleranceInv": "1",
    "DFIntDebugSimPrimalWarmstartForce": "-800",
    "DFIntDebugSimPrimalWarmstartVelocity": "102",
    "FFlagDebugSimDefaultPrimalSolver": "True",
    "FIntDebugSimPrimalGSLumpAlpha": "-2147483647"
}
```

### Send people to heaven
```json
{
    "DFIntDebugSimPrimalNewtonIts": "1",
    "DFIntDebugSimPrimalPreconditioner": "15",
    "DFIntDebugSimPrimalPreconditionerMinExp": "10",
    "DFIntDebugSimPrimalToleranceInv": "1",
    "DFIntDebugSimPrimalWarmstartForce": "-150",
    "DFIntDebugSimPrimalWarmstartVelocity": "100",
    "FFlagDebugSimDefaultPrimalSolver": "True",
}
```

That should be it.
