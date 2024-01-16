# Fix holes and customize the map (Updated to The Chop Shop DLC)

The purpose of this script is to fix the holes in the map by loading zones that aren’t loaded by default.

This fork by TayMcKenzieNZ is to work alongside my fork of [online-interiors](https://github.com/TayMcKenzieNZ/online-interiors) which adds teleporters to and from the locations for on foot and vehicles.

-------------------

## [Wiki](https://github.com/Bob74/bob74_ipl/wiki)
- The Wiki has been created to help you customize your interiors as you wish. I have gone ahead and customised them for you however if you do not like how it is done, you can set it up the way you like using bob's wiki. It contains every function you can use for each interior.

- Each Wiki page has an example at the bottom of the page to show how you can use it in your own resource.

- Also at the bottom of the Wiki will show you the default values set by `IPL_NAME.LoadDefault()`.

------------------

# Heist Carrier 🛥️

Heist carrier has been disabled as it isn't exactly necessary with Cayo Perico. To reenable it, open `client.lua` and set `HeistCarrier.Enable(false)` to HeistCarrier.Enable(true)`.

------------------

# Pillbox Hospitial 🏥

`PillboxHospital.Enable(false)` due to this location being a popular spot for custom MLO hospitals. Setting it to true makes it so doors appear in front of your custom hospital MLO, therefore you can't access it. If you do not have any custom hospital MLOs in this location and instead have a gaping hole, set this to `PillboxHospital.Enable(true)`

------------------

# Arena Wars Arena 🏟️

Nor Bob or myself have included these IPLs. You can find and configure them [here](https://github.com/Starystars67/Titch2000_Arena) however I can not guarantee compatibility with my forks of either bob74_ipl, or online interiors.



------------------

# Install 💾

1. Download my fork of bob74_ipl
2. Extract `bob74_ipl.zip` and copy the `bob74_ipl` into your `resources` folder.
3. add `start bob74_ipl` and `start online-interiors` to your `server.cfg`

------------------

# Screenshots
- [After Hours Album](https://imgur.com/a/Qg96l0D)
- [Misc. Album](https://imgur.com/a/cs9Ip4d)
- [IPL Fix Album](https://imgur.com/a/1Sfl4)

## Changelog

<details><summary>Click to view</summary>
(DD/MM/YYYY)

---
05/12/2023 - 2.1.3
- Added missing train track near Davis Quartz (https://github.com/Bob74/bob74_ipl/pull/129 @TheIndra55)

10/01/2023 - 2.1.2
- Fix native and update native names (@NeenGame )

24/10/2022 - 2.1.1
- Fix vespucci beach wall hole
- Fix Boat House Door in Sandy Shores
- Fix GTA 5 24/7 Roof in Sandy Shores
- Fix Industrial Building near Lesters Warehouse
- Fix Collision Holes near Lost MC compound

11/10/2022 - 2.1.0a
- Make Doomsday Facility Objects non network

03/08/2022 - 2.1.0
- Added "The Criminal Enterprises" support

02/05/2022 - 2.0.15
- Reformatted code
- Removed unused .gitignore
- Bumped version in fxmanifest.lua
- Improved performance

21/04/2022 - 2.0.14
- Fix casino penthouse carpet patterns colors

12/02/2022 - 2.0.13a
- Fix Music Roof

12/02/2022 - 2.0.13
- Added Contract IPLs: Garage, Studio, Offices, Music Roof, Billboards

10/02/2022 - 2.0.12
- Fix FIB roof

07/02/2022 - 2.0.11
- Added Tuners IPLs: Garage, Meth Lab, Meetup

18/01/2022 - 2.0.10b
- Change water in yachts to be non-networked.

01/08/2021 - 2.0.10a
- Improved performance
- Fixed hole in the FIB fountain
- Fixed error appearing if casino IPL is loaded, but the game build is not sufficient
- Fixed a few typos in the README file

19/07/2021 - 2.0.10
- Added Diamond Casino IPLs: Casino, Garage, VIP garage, Penthouse
- Import: Forced refresh of CEO Garages
- Updated fxmanifest fx_version to cerulean
- Updated IPL list link in fxmanifest nad removed outdated Props list and Interior ID list
- Fixed export typo in `michael.lua`
- Removed unnecessary space in north_yankton IPL

27/05/2020 - 2.0.9a
- Fixed disabling Pillbox Hospital
- Fixed `ResetInteriorVariables`

23/04/2020 - 2.0.9
- Replaced deprecated __resource.lua with fxmanifest.lua
- Added ferris wheel on the Del Perro Pier
- Reformatted client.lua

20/10/2019 - 2.0.8
- Nightclubs: Added dry ice emitters
- Heist & Gunrunning: Added water to the yachts hot tubs (to enable/disable)
- Offices: Added a way to open and close the safes
- Facility: Added privacy glass
- Moved Bahama Mamas and PillBox Hospital in their own files
- Fixed error `ReleaseNamedRendertarget`
- Cleaned and optimized the code

22/03/2019 - 2.0.7c
- CEO Offices: Changed the default loaded garage to ImportCEOGarage4.Part.Garage2 in order to avoid Office glitches

15/01/2019 - 2.0.7b
- Nightclubs: Fixed a typo for the fake lights

15/01/2019 - 2.0.7a
- Nightclubs: Added the ability to set no podium (using `AfterHoursNightclubs.Interior.Podium.none`)

14/01/2019 - 2.0.7
- Changed the way Trevor’s trailer is handled and added a Wiki entry.
- Added a way to open or close Zancudo’s gates with a Wiki entry.

12/01/2019 - 2.0.6
- Added nightclubs interior and exteriors
- Removed Zancudo gates by default (file bob74_ipl/gtav/base.lua: RequestIpl("CS3_07_MPGates") is now commented)

29/12/2018 - 2.0.5a
- Fixed the name of the BikerClubhouse1 export

19/12/2018 - 2.0.5
- Fixed a typo that prevents the printers, security stuff, and cash piles to spawn in the counterfeit cash factory

10/11/2018 - 2.0.4
- Fixed an issue where the clubhouse2 lower walls wouldn’t be colored on the first resource start
- Fixed gang members names using an old format
- Disabled the Mod shop from CEO garage 3 (ImportCEOGarage3) because it is overlapping with CEO office 3 (FinanceOffice3)

08/11/2018 - 2.0.3
- Added biker gang’s name, missions, and members pictures
- Added CEO office organization’s name

05/11/2018 - 2.0.1
- Removed overlapping Zancudo River
- Added the trailer near Zancudo River

04/11/2018 - 2.0.0
- Plugin totally rewritten
- Support for all DLC (up to The Doomsday Heist)
- Ability to easily customize story mode and online purchasable interiors
- You can still use it as it is if you want IPL and interiors to be loaded, the plugin sets a default style for each one
- Check out the Wiki to find out how: https://github.com/Bob74/bob74_ipl/wiki

26/06/2017
- Added optional IPL
- Bunkers exteriors (enabled)
- Bunkers interior
- CEO Offices
- Bikers places (some are still buggy)
- Import/Export locations
- Removed the trick to open Lost’s safehouse since the last update already opens it

19/06/2017
- Fix hole in Zancudo River
- Fix hole in Cassidy Creek
- Add optional graffiti on some billboards (enabled by default)
- Opened Lost’s safehouse interior

14/06/2017
- Original release
</details>
