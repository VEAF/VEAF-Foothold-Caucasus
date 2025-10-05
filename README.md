# VEAF Foothold Caucasus v2.2.0

## Presentation

This is a modification of the original [Foothold Caucasus](https://www.digitalcombatsimulator.com/en/files/3341245/) mission by Lekaa, that I adapted to make it load all the script files and config directly from the server.

**Done using the latest version updated on 2025.10.05.**

## Update

### Triggers

Add this triggers on MissionStart:

name: `mission start - dynamic`
do_script:
```lua
MA_DYNAMIC_PATH = [[C:\Users\veaf\Saved Games\DCS.missions\foothold\MA_Foothold_Caucasus\Modern\]]
env.info("DYNAMIC MA LOADING")
assert(loadfile(MA_DYNAMIC_PATH .. "VEAF_MA_loader.lua")) ()
```

Change the path to xxx\Coldwar for the cold war version

## Things to do

- [x] silence all ATC
- [x] add VEAF radio presets
- [ ] check why the wind is sometimes wrong (0 kn instead of 10-15 kn)
- [x] disable the no fly zone (or make it less punitive)
- [ ] no waypoints for an f18 spawned on cvn74
- [ ] limited spawn spots on Batumi
- [ ] stats de la session (vs stats globales)
- [x] ajouter Senaki aux presets
- [x] ajouter les waypoint# aux presets
