# Sullien's Comments
[I recently realized the comments in Sullien's original .json may become an issue at some point](https://github.com/denismattos/Future-Expansion-Continued/blob/main/forewords.md##4.1.3).  
So I'm doing a cleanup of the files and moving all comments within every file to this separate file, here.
## [Buildings.json](https://github.com/denismattos/Future-Expansion-Continued/blob/main/jsons/Buildings.json)
Buildings.json's comments were used to divide additions and modifications by eras and categories.
### "Ancient"
Palace
### "Medieval"
Forge
### "Renaissance"
No additions or modifications.
### "Industrial"
* Museum
* History Museum
* Public School
* Factory
* Coal Plant
* Hospital
* Stock Exchange
* Hydro Plant
### "Modern"
* Stadium
* Broadcast Tower
* Research Lab
### "Atomic"
* Medical Lab
* International Pass
* Nuclear Plant
* Recycling Center
* Electrical Grid
### "Information"
* Foreign Center
* Branch Office
* Entrepeneur Venue
* Spaceship Factory
* Virtual Space
* Private Grid
* Defense Complex
### "Future"
* Bio Facility
* Nano-Factory
* Energy Reactor
* Space Station
* Composite Factory
* Adaptive Base
* Energy Barrier
* Space Colony
### "National Wonders"
* Utopia Project
* Nuclear Testing Site
* Information Warfare
* Time Machine Blueprints
* Monolith Portal
### "World Wonders"
* Manhattan Project
* Pentagon
* Cristo Redentor
* Apollo Program
* Hubble Space Telescope
* United Nations
* Fusion Reactor
* Living Castle
* Space Elevator
* World Alliance
* Teleport Station
### "Corporations"
* Electrical Corporation
* Engineering Corporation
* Tourism Agency
* Defense Force Agency
* Social Network Company
* World Delivery Company
* Space Organization
* Holy Organization
### "Perks"
* SP-Innovation
* SP-Water Power
* SP-Supply Chains
* SP-Corporate Chains
* SP-Medical Labs
* SP-Nuclear Arsenal
* SP-Modern Medicine
* SP-Green Energy
* SP-Enviromentalism
* SP-Future Power
* AP-Excavations
* AP-Art Guilds
* AP-Museum Host
* AP-Music
* AP-World Tour
* AP-World Competitions
* AP-Foreign Exchange
* AP-Press Media
* AP-New Age
* AP-Space Combat
* EP-First Pioneers
* EP-Extractor
* EP-Early Vehicles
* EP-Distillery
* EP-Recycling
* EP-Civil Planning
* EP-Advanced Machinery
* EP-Energy Contractors
* EP-Genetic Engineering
* EP-Cyber Engineering
* MP-Expropiation
* MP-Public Transport
* MP-Arms Dealer
* MP-Entertainment
* MP-Branch Companies
* MP-International Aid
* MP-Entrepeneur Aid
* MP-Virtual Age
* MP-Desalination
* MP-Eternal Gold
* PP-Church Institute
* PP-New Church
* PP-Church Taxes
* PP-Ideology War
* PP-Independent Church
* PP-Faith Censor
* PP-Global Broadcast
* PP-Peace Mediator
* PP-New Millenium
* PP-Hegemony
* GP-Modernization
* GP-Great Conquests
* GP-Great War
* GP-Navy First
* GP-Conscription
* GP-Finest Hour
* GP-National Defense
* GP-Stealth Operatives
* GP-Hovercombat
* GP-Energy Weapons
### "Effect-Based"
* Cloning Facility
* Free Iron
* Free Oil
* Free Power
* Corporate Slot
* No Corporation
* Solar Plant
## [Eras.json](https://github.com/denismattos/Future-Expansion-Continued/blob/main/jsons/Eras.json)
* Ancient era's `"startingSettlerCount": 1` line was commented:  
"These values should not include the values given in Difficulties.json."
* Information era's `"startPercent": 80` line was commented (Presumably referring to its `"startingObsoleteWonders"` attribute.):  
"So, theoretically, this is always just all the wonders at least 2 eras old. So we could just use that.  
But where is the modularity? The excluding of very specific wonders? That is no fun.  
So we just write down the entire long list (sorted by era!), instead."
## [TileImprovements.json](https://github.com/denismattos/Future-Expansion-Continued/blob/main/jsons/TileImprovements.json)
Some of TileImprovements.json's improvements were divided by categories using comments.
### "Modern Upgrades"
* Excavation Site
* Concert Venue
* Industry
* Wind Farm
* Solar Farm
* Offshore Wind Farm
* Resort
### "Resource-Specific"
* Pasture
* Oil well
* Offshore Platform
* Plantation
* Camp
* Quarry
* Fishing Boats
### "Infraestructure"
* Power Plant
* Supply Route
* Water Tower
* Industrial Complex
* Residential
### "Great Improvement"
* Academy
* Landmark
* Manufactory
* Customs house
* Holy site
* Citadel
* Space Platform
### "Civilization-Unique"
* Moai
* Terrace farm
* Polder
## [TileResources.json](https://github.com/denismattos/Future-Expansion-Continued/blob/main/jsons/TileResources.json)
TileResources.json's comments were used to divide resources by categories.
### "Bonus"
Natural Appeal
### "Perks"
* Scientist Perk
* Artist Perk
* Engineer Perk
* Merchant Perk
* Prophet Perk
* General Perk
### "Strategic"
* Power
* Composites
* Aluminum
* Fossil
### "Corporation"
* Corporation Slot(Total)
* Corporation Slot
* Electrical Stock
* Engineering Stock
* Tourism Stock
* Defense Force Stock
* World Delivery Stock
* Social Network Stock
* Space Stock
* Holy Stock
## [UnitPromotions.json](https://github.com/denismattos/Future-Expansion-Continued/blob/main/jsons/UnitPromotions.json)
Some of UnitPromotions.json's promotions were divided by categories using comments.
### "Effects"
* Stealth
* Amphibious
* Hovering
* Rocket Launcher
* Firewall
* Heat Sensor
* Implants
* Scan Visor
* Energy Weapons
* Gravity Generator
* In Orbit
* Energy Shield
* Teleportation
* Support Unit
* Skirmish
### "Carrier"
* Armor Plating I
* Armor Plating II
* Armor Plating III
* Flight Deck I
* Flight Deck II
* Flight Deck III
## [Units.json](https://github.com/denismattos/Future-Expansion-Continued/blob/main/jsons/Units.json)
Most of Units.json's comments were used to divide units by eras and categories.  
Additionally, Battleship was commented:  
"Does **actually** upgrade to Missile Cruiser, now."
### "Ancient"
* Worker
* Work Boats
* Scout
### "Renaissance"
No units.
### "Industrial"
* Archaeologist
* Recon
* Medic
* Rifleman
* Mehal Sefari
* Carolean
* Norwegian Ski Infantry
* Cavalry
* Cossack
* Hussar
* Observation Balloon
* Artillery
### "Modern"
* Great War Infantry
* Triplane
* Great War Bomber
* Biplane
* Landship
* Battleship
* Musician
* Corporate
* Supply Agent
* Destroyer
* Anti-Aircraft Gun
* Tank
### "Atomic"
* Marine
* Bomber
* Paratrooper
* Architect
* Carrier
* Anti-Tank Gun
* Atomic Bomb
* Rocket Artillery
* Mobile SAM
* Guided Missile
* Helicopter Gunship
### "Information"
* Nuclear Submarine
* Nuclear Missile
* Drone
* Missile Cruiser
* Hacker
* Mechanized Infantry
* Modern Armor
* Jet Fighter
* Tactical Supplier
* Stealth Hacker
* Jet Bomber
* Stealth Bomber
### "Future"
* Bio-Infantry
* Hovertank
* Future Soldier
* Hovertillery
* Hover-SAM
* Combat Robot
* Seeker
* Synthethic Plant
* Energy Infantry
* Future Copter
* Orbital Carrier
* Orbital Jet
* Orbital Bomber
* Giant Death Robot
* Future Submarine
* Orbital Strike
### "Great Persons"
* Great Spacefarer
* Great General
* Khan
### "Time Machine Parts"
* Photon Generator
* Causality Matrix
* Dimensional Shifter
* Entropy Phaser
### "Barbarians"
* Terrorist
* Outlaw
* Hit Squad
### "Aliens"
* Body Snatcher
* Monolith Body Snatcher
* Brainiac
* Monolith Brainiac
* UFO
* Monolith UFO
### "Civ-Exclusive"
* Norwegian Ski Infantry
* Carolean
* Mehal Sefari
* B17
### "Spaceship"
* SS Booster
* SS Cockpit
* SS Engine
* SS Stasis Chamber
## [UnitTypes.json](https://github.com/denismattos/Future-Expansion-Continued/blob/main/jsons/UnitTypes.json)
UnitTypes.json's comments were used to divide unit types by expansions.
### "G&K"
* Civilian
* Sword
* Gunpowder
* Archery
* Ranged Gunpowder
* Scout
* Mounted
* Armored
* Siege
* Civilian Water
* Melee Water
* Ranged Water
* Submarine
* Aircraft Carrier
* Fighter
* Bomber
* Atomic Bomber
* Missile
* Helicopter
### "Future Expansion"
* Support