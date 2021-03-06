
![JARACI BALANCE MOD](jaraci_big.png "Logo")

# Introduction

## About

**Jaraci balance mod** is a **Homeworld: Deserts of Kharak** modification created by AGameAnx with the help of some of the best competitive Deserts of Kharak players. The mod focuses on improving faction and unit interactions/balance throughout the game while retaining most of the intuitive Deserts of Kharak feel.

[**Please watch this quick changes summary video by Bozocow**](https://www.youtube.com/watch?v=frEmE-Iozyg)

Join [Homeworld Universe discord](https://discord.gg/homeworld) for usage help, to discuss the mod, download replays and participate in mod tournaments!

Casts of previous **Jaraci Cup** games can be found on [Bozocow's YouTube channel](https://www.youtube.com/user/Bozothcow/videos).

Deserts of Kharak unofficial ranked ladder, which also includes **Jaraci patch ranked ladder** and downloadable replays [can be found here](https://docs.google.com/spreadsheets/d/1_F2TLo5-lys_RwV6Ql6kVzlgnUqdZJTW2Kiex31WAHY).

The mod is created using [Subsystem](https://github.com/AGameAnx/Subsystem). It is not recommended to install Subsystem on its own, however. Subsystem comes as part of the more-maps mod (see [how to play](#how-to-play)).

Special thanks to Majiir and SSSS for paving the way towards a balance mod being possible, to Descara and Bozocow for being awesome support, discussion and playtest help.

## How to play

It is recommended to play Jaraci patch using the [SSSS more-maps mod](https://github.com/S5SS/dok-repo/releases/download/maps-v1.1/more-maps-v1.1.zip) (version 1.1t required)

More-maps mod allows players to load custom layouts and attribute patches directly in multiplayer lobbies. It does not affect your ability to play vanilla Deserts of Kharak games.

Use the following command in match setup chat to load the mod:

**`/p jaraci`**

If above version is not up to date with the recent changes, its version will be marked as 'Tournament version' in recent changes list. If you want the latest (experimental) changes and not the tournament version use the following command:

**`/p agame`**

## Mod releases

* Tournament: [jaraci.json](https://github.com/S5SS/dok-repo/blob/master/patches/jaraci.json)
* Development: [agame.json](https://github.com/S5SS/dok-repo/blob/master/patches/agame.json)

## Recent changes

Recent changes can be found in a [sister document HERE](jaraci_recent_changes.md)

# Table of contents

- [Introduction](#introduction)
    - [About](#about)
    - [How to play](#how-to-play)
    - [Mod releases](#mod-releases)
    - [Recent changes](#recent-changes)
- [Table of contents](#table-of-contents)
- [General changes](#general-changes)
    - [Carriers](#carriers)
        - [Power level upgrades](#power-level-upgrades)
        - [Range power systems (Gaalsien/Coalition)](#range-power-systems-gaalsiencoalition)
        - [Point defense weapons](#point-defense-weapons)
        - [Missile systems](#missile-systems)
        - [Indirect fire systems (nukes)](#indirect-fire-systems-nukes)
    - [Unit upgrades](#unit-upgrades)
        - [Medium vehicle armor](#medium-vehicle-armor)
        - [Strike craft damage](#strike-craft-damage)
        - [Strike craft damage upgrades](#strike-craft-damage-upgrades)
        - [Strike craft armor upgrades](#strike-craft-armor-upgrades)
    - [Quality of life](#quality-of-life)
        - [Fog of war reveal duration after firing](#fog-of-war-reveal-duration-after-firing)
        - [Railgun target prioritization](#railgun-target-prioritization)
        - [Unit priority as target](#unit-priority-as-target)
        - [Air sorties](#air-sorties)
    - [Generic balance changes](#generic-balance-changes)
        - [Small arms anti-air weapons](#small-arms-anti-air-weapons)
        - [Salvager](#salvager)
        - [Salvager RU hold size](#salvager-ru-hold-size)
        - [Demo pack](#demo-pack)
        - [Baserunner](#baserunner)
        - [Artillery barrages (except Khaaneph)](#artillery-barrages-except-khaaneph)
- [Coalition / Soban](#coalition--soban)
    - [Salvager](#salvager-1)
    - [Coalition carrier](#coalition-carrier)
        - [Cruise missile](#cruise-missile)
    - [Soban carrier](#soban-carrier)
        - [ALM](#alm)
        - [Microwave emitter](#microwave-emitter)
    - [Armored vehicle upgrades](#armored-vehicle-upgrades)
    - [Production upgrades](#production-upgrades)
    - [Support cruiser](#support-cruiser)
    - [Baserunner](#baserunner-1)
        - [Probe](#probe)
        - [AA turret](#aa-turret)
        - [Gun turret](#gun-turret)
        - [Targeting jammer](#targeting-jammer)
    - [LAV](#lav)
    - [AAV](#aav)
    - [Railgun](#railgun)
        - [Mag accelerator upgrade](#mag-accelerator-upgrade)
        - [Coalition railgun](#coalition-railgun)
        - [Soban railgun](#soban-railgun)
    - [Missile battery](#missile-battery)
    - [Assault cruiser](#assault-cruiser)
    - [Battlecruiser](#battlecruiser)
        - [Coalition](#coalition)
        - [Soban](#soban)
    - [Artillery cruiser](#artillery-cruiser)
    - [Fighter and gunship fabrication](#fighter-and-gunship-fabrication)
        - [Strike fighter](#strike-fighter)
        - [Gunship](#gunship)
    - [Tactical bomber](#tactical-bomber)
- [Gaalsien / Khaaneph](#gaalsien--khaaneph)
    - [Salvager](#salvager-2)
    - [Gaalsien carrier](#gaalsien-carrier)
        - [Hyper-sonic missile barrage](#hyper-sonic-missile-barrage)
    - [Khaaneph carrier](#khaaneph-carrier)
    - [Baserunner](#baserunner-2)
        - [Gaalsien baserunner](#gaalsien-baserunner)
        - [Khaaneph baserunner](#khaaneph-baserunner)
            - [Blast drone](#blast-drone)
    - [Sandskimmer](#sandskimmer)
    - [Production cruiser](#production-cruiser)
    - [Assault ship](#assault-ship)
    - [Missile ship](#missile-ship)
    - [Vehicle armor upgrade cost](#vehicle-armor-upgrade-cost)
    - [Railgun fabrication](#railgun-fabrication)
        - [Assault railgun](#assault-railgun)
        - [Heavy railgun](#heavy-railgun)
    - [Railgun armor upgrades cost](#railgun-armor-upgrades-cost)
    - [Interceptor](#interceptor)
    - [Precision bomber](#precision-bomber)
    - [Siege cruiser](#siege-cruiser)
        - [Gaalsien siege cruiser](#gaalsien-siege-cruiser)
        - [Khaaneph siege cruiser](#khaaneph-siege-cruiser)
    - [Honourguard cruiser](#honourguard-cruiser)

# General changes

## Carriers

### Power level upgrades
> *Intention of the cost rebalance is to slightly shift away: `Strike-craft-centric playstyles when using the carrier as well as reduce the incentive to power up the carrier as early as possible (it should be risky doing this on low tech). The extra hitpoints granted with carrier upgrades allows clever players to read which power upgrade the enemy is on and shifts carrier general strength away from early game and into lategame, allowing offensive capabilities to be transferred more easily into early game when needed for balance purposes, while reducing defensive ones.*

* Hitpoints granted per upgrade: `0 => 150`
* Cost:
    * Level 1: `140CU 80RU => 200CU 100RU`
    * Level 2: `280CU 160RU => 400CU 175RU`
    * Level 3: `460CU 260RU => 650CU 250RU`
    * Level 4: `720CU 400RU => 900CU 400RU`
    * Level 5: `1100CU 600RU => 1200CU 550RU`
    * Level 6: `1300CU 700RU => 1300CU 700RU`
    * Level 7: `1500CU 800RU => 1400CU 850RU`

### Range power systems (Gaalsien/Coalition)
> *All railgun and carrier ranges are reduced in the mod as part of the effort to reduce the prevalence of railgun-based strategies. Carrier ranges are reduced slightly more than railgun ranges.*

* Level 0:
    * Turret max range: `500 => 800`
* Level 1:
    * Turret max range: `500 => 900`
* Level 2:
    * Turret max range: `1100 => 1050`
    * Missile max range bonus: `600 => 550`
* Level 3:
    * Turret max range: `1400 => 1250`
    * Missile max range bonus: `900 => 750`
    * Sight and contact range: `600 => 550`
* Level 4:
    * Turret max range: `1700 => 1450`
    * Missile max range bonus: `1200 => 950`
    * Sight and contact range bonuses: `900 => 800`
* Level 5:
    * Turret max range: `2000 => 1650`
    * Missile max range bonus: `1500 => 1150`
    * Sight and contact range bonuses: `1200 => 1050`

### Point defense weapons
> *Carrier point defense weapons are some of the most unintuitively designed weapons in the game. A couple of issues include - they do very little damage even at level 5 power systems, they do very low amounts of damage so going from level 4 to level 5 weapon systems power level makes no difference in a carrier fight (even with changes they still don't, in most cases). Additionally, early in the game on some of the carriers they do almost nothing. These changes make defending against strike craft-based attacks easier in the early game which is a change forced by a particular Khaaneph Blast Drone rush.*

* Accuracy profiles:
    * Short: `5% or 100% => 50%`
    * Medium: `4.5% or 90% => 45%`
    * Long: `4% or 80% => 35%`
* Weapon damage: `8 or 10 => 20`
* Benefit from high ground: `Yes => No`
* Penetrating weapon damage: `17 => 50`
* Rate of fire: `See per-carrier changes below`
* Normalized all modifiers against different target sizes:
    * Small: `5 or 8 => 1`
    * Medium: `1, 15 or 18 => 1`
    * Large: `1 or 2000 => 1.3`
    * XLarge, Carrier: `1 or 25 => 1.3`
* Improved visuals of PDs missing their target

### Missile systems
> *Missile systems do the majority of carrier's damage, and thus the missile weapon is receiving a reduction in fire rate across all carriers.*

* Wind-up: `0 => 0.5s`

### Indirect fire systems (nukes)
> *The range change stems mostly from the fact that soban MWE can be used to extend the lead of a soban player in a really uninteractive way of spamming MWE onto enemy mining operations. Shouldn't affect 1v1 games too much but will be a pretty big change for team games.*

* Affected by high ground: `Yes => No`
* Range: `35000 to 4500`

## Unit upgrades

### Medium vehicle armor
> *Armor upgrades affect some combat situations very drastically, making certain units weaker than intended. Maximum armor on upgraded units will be reduced slightly overall, but base armor increased in select cases.*

* Armor granted: `Fixed to +1`

### Strike craft damage
> *This change is aimed at helping strike craft counter heavily upgraded railguns & increasing potential of fully upgraded strike craft strategies. This change wouldn't be a good idea on its own without the consideration of all the other mod changes. Almost all strike craft counts have seen updates/buffs, therefore it has become logical to provide a small bonus to strike-craft based strategies.*

* CU Cost: `500 => 400`

### Strike craft damage upgrades
> *Due to reduced base damage and increased rate of fire these upgrades were too powerful when granting old bonuses.*

* Damage increase per upgrade `2 => 1`
* CU cost: `400 => 300`

### Strike craft armor upgrades
> *Main ways to counter strike craft always involve area of effect but that also means that getting strike craft armor upgrades wasn't very impactful at preventing strike craft: `getting quickly wiped by their area of effect counters.*

* Added bonus: `30 extra hitpoints per upgrade`
* CU Cost: `200 => 300`

## Quality of life

### Fog of war reveal duration after firing
> *This is done to make sure slower rate of fire railguns do not cloak in fog of far after firing before firing off the next shot. Previously, soban and coalition railguns would disappear in fog of war between their shots which messes up player micro and makes enemy railguns switch targets or lose targets. Additionally, carriers have the same penalty applied to make it more dangerous to stay on max sensor power shunt and fire at the enemy from a great distance.*

* Railgun and carrier reveal duration after firing: `2.5s => 4.5s`

### Railgun target prioritization
> *Railgun target prioritization weights have been reworked to ensure more predictable and smart behavior. Range and angle make less of an impact on railgun target prioritization, but weapon effectiveness is now more important (meaning railguns will prioritize targets that have lower armor but also take high received accuracy from the railguns, which is most likely enemy railguns).*

* Weapon effectiveness weight: `increased`
* Distance weight: `decreased`
* Angle weight: `decreased`
* Auto target sticky bias: `decreased`

### Unit priority as target
> *Adjusting certain unit priority as targets to make targeting of these units more logical and less micro intensive.*
> 
> *Generally the result of automatic targeting of most units should be as follows: Strike craft > Salvagers > Small targets.*
> 
> *For railguns: Medium/Large targets > Carrier > Baserunner > Strike craft > Salvagers > Small targets*

* Baserunner: `decreased`
* Salvager: `increased`
* Strike craft: `increased`
* Railgun: `increased`
* Carrier: `increased (inconsistencies fixed)`
* Gun turret: `decreased`
* Missile turret: `decreased`
* Missile ship/missile battery: `reduced`

### Air sorties
> *The optimal way to use air is to always keep them in the air (as there is no fuel system in the game). The micro requirement for keeping air units in the air was to queue as many commands as possible to make the units fly back & forth and not return to carrier. This change should simply lessen the amount of tedious micromanagement required to use air optimally.*

* Duration: `10s => 40s`

## Generic balance changes

### Small arms anti-air weapons
> *LAV are unaffected by this change as they use the same weapon to target air as they do ground.*

* Affected by high ground: `Yes => No`

### Salvager
> *Generally speaking, salvager kills were uncommon and mostly easily replaced as they tend to happen only towards midgame and when some amount of tech is already out on the field. The new cost aims to both make salvager kills more valuable, and expanding slightly more expensive and slow. Armor is changed on salvagers and area of effect kills on salvagers are very common therefore the health is going up slightly.*

* Cost: `100CU => 150CU`
* Hitpoints: `900 => 950`

### Salvager RU hold size
> *The combination of RU hold size and mining rate makes long-hauling RUs vastly more efficient than long-hauling CUs. In order to bring the two in line so that long-hauling has the same impact on both resource types, the RU hold size would need to be reduced to 16 RUs. (This is the exact number.) However, 16 RUs would not be an ergonomic hold size. This is part of an effort to reduce the effectiveness of early game RU-based rush strategies (coalition/soban carrier rush, gaalsien railgun rush).*

* RU hold size: `40 => 20`

### Demo pack
> *The goal of these changes is to slow down expansion slightly, to move away some of the cost of expansion from the associated units (PC and SC). The damage is changed to allow demo packs to remain a relevant ability defensively (even if weak).*

* Cost: `50CU => 100CU`
* Damage: `175 => 200`
* Packets: `1 => 2`

### Baserunner
> *Early artifact pressure has become very standard meta, even after initial cost nerfs baserunner play was standard and difficult to punish. Even adjusting artifact timings wouldn't solve some of the issues which are present on certain maps where fast investment into mid-game railgun army could completely lock down the game due to extraction corridor being close enough to artifact pick up locations and main base. Extracting artifacts with multiple baserunners at a time will now require a moderate investment, hopefully reducing the size of an aforementioned railgun army. Additionally, this allows baserunner abilities and baserunner AA weapon to be tuned stronger without the concern of making it a better air counter unit than actual AA tech.*

* Cost: `250CU => 250CU 50RU`
* Max speed: `65 => 70`

**Baserunner anti-air**
> *These changes should add some soft early game anti-air to all factions. Surprise air tech can be game ending and blind teching against air is almost a necessity for almost all matchups.*

* AA weapon dmg: `5 => 17`
* Packets: `0 => 1`
* Turret rotation speed: `95(180) => 200`
* Damage against probes: `100% => 50%`
* Ranges:
    * Short: `600(300) => 700`
    * Medium: `900(600) => 1100`
* Accuracy:
    * Short: `100(75) to 90`
    * Medium: `100 to 80`
* Gaalsien BR long range: `Set to unused`
* Removed unused modifiers against ground targets

### Artillery barrages (except Khaaneph)
> *These changes don't apply to Khaaneph Siege Cruiser, although it has seen a different rework (see below). The idea behind these changes is to make immediate impact of artillery barrages lower but allow them to deny an area for longer and have a larger overall impact on the battle. This should allow artillery to better counter railgun high ground positions and better punish less attentive play.*

* Damage against small targets: `100% => 50%` 
* Damage against carriers: `100% => 60%`
* Autofire: `Has same modifiers as main barrage`
* Burst: `1s => 1.7s`
* Cooldown: `0.5s => 1.6s`

# Coalition / Soban

## Salvager

* Armor: `5 => 0`

## Coalition carrier

**General statistics**
> *Carriers should become a bit trickier to use in combat and carrier aggression should become a bit more punishable. Worth noting that these changes coincide with railgun nerfs, however. Movement speed nerf is part of an effort to fix a particularly strong early game 1 base carrier timing push.*

* Hitpoints: `15000 => 9000`
* Movement speed: `60 => 50`
* Turn radius: `150 => 65`
* Acceleration time: `2s => 1.1s`
* Braking time: `2s => 1.1s`

**Point defense weapons**
> *Lower level PD performance increased (due to BD rush), but higher level rate of fire reduced (due to damage rework of carrier PD weapons)*

* Rate of fire: `2 => 6`
* Weapon Systems power shunt PD rate of fire bonuses:
    * Level 1: `'set to 5' => 'increase by 20%'`
    * Level 2: `'set to 10' => 'increase by 35%'`
    * Level 3: `'set to 20' => 'increase by 55%'`
    * Level 4: `'set to 40' => 'increase by 80%'`
    * Level 5: `'set to 40' => 'increase by 25%'`

**Armor system power shunt**
> *Due to railgun damage reductions and other units being less numerous in numbers and generally having lower rate of fire, the insanely high armor of coalition carrier had to be reduced.*

* Level 2: `40 => 35`
* Level 3: `75 => 45`
* Level 4: `100 => 60`

### Cruise missile
> *Coalition cruise missile's destructive potential is unmatched. A reduction of its effectiveness against smaller units should make it tougher to extract very high value from it on a consistent basis while keeping overall strategic value of an expensive nuke-class weapon appropriately high.*

* Cooldown: `120s => 170s`
* Damage: `5000 => 2300`
* Damage against cruisers and carriers: `100% => 180%`

## Soban carrier

**General statistics**
> *Carriers should become a bit trickier to use in combat and carrier aggression should become a bit more punishable. The Soban carrier hitpoint nerf is larger than other carriers because it gets strong railgun weaponry from the beginning of the game and extra range for safer positioning. Movement speed and armor changes are part of an effort to fix a particularly strong early game 1 base carrier timing push*

* Hitpoints: `15000 => 8800`
* Movement speed: `60 => 50`
* Turn radius: `150 => 65`
* Acceleration time: `2s => 1.1s`
* Braking time: `2s => 1.1s`
* Base armor: `25 => 15`

**Armor system power shunt**
> *Soban carrier is particularly strong for the carrier rush. It is meant to be a long range support carrier and thus it is getting its armor reduced across all levels of armor power shunt, including the base armor*

* Level 1: `30 => 20`
* Level 2: `40 => 25`
* Level 3: `60 => 35`
* Level 4: `100 => 50`

**Point defense railguns**
> *The new iteration of these railguns works much closer to how Soban railgun units work.*

* Damage: `165 => 195`
* Number of bursts: `10 => 2`
* Burst: `1s => 0.25s`
* Cooldown: `5s => 10s`
* Reload: `10s => 15s`
* Wind-up: `1.6s => 1s`
* Range:
    * Medium: `600 => 550`
    * Long: `900 => 1000`
* Accuracy:
    * Medium: `5.3% => 5%`
    * Long: `5% => 4.5%`

**Turret network power shunt**
> *The goal is to make Soban carrier a relatively powerful brawler against armored targets, while keeping its overall damage output at bay and keeping the carrier weak against strike craft.*

* Level 1:
    * Reload: `'Set to 10s => 'decrease by 35%'`
    * Cooldown: `'Set to 5s' => 'decrease by 35%'`
    * Accuracy bonus: `10% => 15%`
* Level 2:
    * Reload: `'Set to 6s => 'decrease by 55%'`
    * Cooldown: `'Set to 3s' => 'decrease by 55%'`
* Level 3:
    * Reload: `'Set to 4s => 'decrease by 70%'`
    * Cooldown: `'Set to 2s' => 'decrease by 70%'`
    * Accuracy bonus: `40% => 35%`
* Level 4:
    * Reload: `'Set to 2s => 'decrease by 85%'`
    * Cooldown: `'Set to 1.5s' => 'decrease by 85%'`
    * Accuracy bonus: `50% => 45%`
* Level 5:
    * Reload: `'Set to 2s => 'decrease by 95%'`
    * Cooldown: `'Set to 1s' => 'decrease by 95%'`
    * Accuracy bonus: `60% => 55%`
* Fixed a number of issues with reload and cooldowns of select PD weapons being updated incorrectly
* No longer setting the damage of the dummy weapon to 160 on every power level

**Range systems power shunt**
> *Soban carrier receives slightly more range than other carriers across all power levels*

* Ranges:
    * Level 1: `800/550/300 => 1200/750/450`
    * Level 2: `1100/750/400 => 1450/1100/700`
    * Level 3: `1400/950/500 => 1650/1300/900`
    * Level 4: `1700/1150/600 => 1900/1400/1100`
    * Level 5: `2000/1350/700 => 2150/1700/1300`
* Fixed an issue where front right turret range wasn't updated correctly at Level 4 power level

### ALM
> *It's a bit too difficult to micro around ALMs and they provide too much early game safety. To offset the reload and area of effect changes ALM damage is upped considerably. World height offset change is meant to make ALM more easily targetable when placed on a small hill*

* Damage: `40 => 110`
* Damage packets: `1 => 2`
* Accuracy: `100%/90%/80% => 100%/100%/100%`
* AOE: `100 => 80`
* Target prioritization fixes:
    * Distance weight: `decreased`
    * Angle weight: `decreased`
* World height offset: `0 => 15`

**ALM power shunt**
> *Generally, ALM should be much worse at stun-locking opponent units, but also more capable at dealing damage which helps win defensive engagements (see ALM unit changes below).*

* Sensors range:
    * Level 1: `1100 => 1000`
    * Level 2: `1300 => 1100`
    * Level 3: `1600 => 1200`
    * Level 4: `1900 => 1300`
    * Level 5: `2200 => 1500`
* Contact radius: 
    * Level 1: `1400 => 1300`
    * Level 2: `1600 => 1400`
    * Level 3: `2100 => 1500`
    * Level 4: `2500 => 1700`
    * Level 5: `3000 => 1900`
* Reload time:
    * Level 1: `4s => 6.5s`
    * Level 2: `3s => 5.5s`
    * Level 3: `2s => 4.5s`
    * Level 4: `1s => 3.5s`
    * Level 5: `0.4s => 2.5s`
* Deployment range bonus:
    * Level 2: `1000 => 800`
    * Level 3: `1500 => 1000`
    * Level 4: `1800 => 1200`
    * Level 5: `2000 => 1500`
* Damage bonus:
    * Level 4: `10 => 30`
    * Level 5: `20 => 50`

### Microwave emitter
> *Microwave emitter is the weakest nuke-class weapon and therefore is receiving some buffs.*

* Cooldown: `90s => 150s`
* Cost: `500CU => 400CU`
* Impact damage falloff: `Linear => Quadratic`
* Duration: `20s => 30s`
* Damage packets: `1 => 0`
* Base damage per tick: `170 => 100`
* Burst: `1s => 0.25s`
* Damage against strike craft and salvagers: `100% => 50%`
* Damage against Carrier, XLarge and Large class targets: `100% => 120%`
* Removed the 500 damage per second status affect on friendly units

## Armored vehicle upgrades
> *Reducing strength of level 3 armor upgrade to both make railguns more susceptible to their counters throughout the game and to lower the power of AAV snowballing.*

* Vehicle armor upgrade level 3 hitpoints granted: `200 => 100`

## Production upgrades
> *It has become quite commonplace to get railgun or AAV tech just to get the last level of production for C/S factions. This will open up C/S options significantly, it will allow for more optimized and committed midgame pushes and deadlier timings. Nevertheless, extra cost and other changes will make these pushes require well designed build orders to pull off properly.*

* Requirements: `Railgun/AAV techs => None`
* Level 1 upgrade cost: `500CU => 400CU 40RU`
* Level 2 upgrade cost: `500CU => 600CU 80RU`
* Research time: => `30s => 50s`

## Support cruiser

**General stats**
> *Aim of the cost change is to slow down tech progression when expanding. Currently, there's almost no downside and slow down when expanding from 2 to 3 base, this should make the tech progression just slightly slower which could prove meaningful vs aggressive enemy strategies. Added repair rate helps C/S sustain in lategame positional battles*

* Cost: `600CU => 450CU 50RU`
* Production time: `45s => 35s`
* Hitpoints: `4100 => 3200`
* Armor: `3 => 5`
* Turn radius: `100 => 75`
* Population: `6 => 5`
* Armor: `2 => 3`
* Repair rate: `10 => 7`
* G2G weapon:
    * Damage: `3 => 15`
        * Rate of fire: `12 => 8`
    * Burst: `0.4-0.8s => 0.8-0.9s`
    * Cooldown: `2s => 0.5s`
    * Reload: `4s => 2s`
    * Accuracy: `75%/55%/35% => 45%/35%/35%`
    * Ranges: `300/600/900 => 400/600/950`
    * Can target air: `No => Yes`
    * Damage against probes: `100% => 20%`
    * Accuracy against non-small targets: `100% => 150%`
    * Benefits from high ground: `Yes => No`
    * Turret:
        * Field of fire: `8 => 360`
        * Field of view: `140 => 360`
        * Rotation speed: `75 => 160`

**Anti-air**
> *Support cruiser AA is the strongest AA in the game by a large margin. Such a high hitpoint body shouldn't have strong AA capability. This capability is also achieved through a single upgrade while SC is already a very useful and needed unit. The strength of this upgrade currently makes most other AA sources obsolete, and is a very easy and obvious choice of an upgrade to purchase. Ground to Ground weapon is now redesigned to have AA and meaningful anti-ground capabilities. This makes defending against early game rushes slightly more easier and allows other aspects of the unit to become weaker (hitpoints, repair rate).*

* Upgrade cost: `500CU 320RU => 450CU 250RU`
* Weapon:
    * Damage: `250 => 50`
    * Rate of fire: `2 => 1`
    * Burst count: `1 => 4`
    * Burst duration: `1s => 0.3s`
    * Cooldown: `0.7s => 0s`
    * Wind-up: `0ms => 50ms`
    * Range: `1550 => 1200`

## Baserunner

**General**

* Hitpoints: `3350 => 2400`

### Probe
> *Probe is slightly too fragile and it often feels random whether it dies or not when it flies into any kind of early game anti-air even if pulled back instantly. The probe is rebalanced along with production cruiser AA and baserunner AA to be more consistent in its interactions with them.*

* Hitpoints: `100 => 120`
* Sensors radius: `1000 => 1250`
* Contact radius: `1100 => 1450`
* Max movement speed: `250 => 200`

### AA turret
> *Generally using this turret is quite undesirable and almost never worth the original cost investment.*

* Anti-air turret post cost: `350CU => 200CU`

### Gun turret
> *Turrets become slightly less self-sufficient. Hitpoints is a change to prevent blast drones from 1-shotting the turret.*

* Cost: `250CU => 300CU`
* Cooldown: `60s => 110s`
* Vision range: `1200 => 1000`
* Hitpoints: `600 => 720`
* Armor: `5 => 1`

**Gun turret weapon**
> *The goal of this rework is to make baserunner turret slightly more effective against armored targets and to also fix some issues with its performance such as it firing behind dunes. This new iteration of the turret will allow for greater micro potential against it with strike craft and it'll be slightly better at countering highly upgraded tanks. With accuracy always being 100% the turret will always 1-shot skimmers which aren't upgraded with level 2 armor or aren't pulled away.*

* Damage: `30 => 54`
* Damage packets: `1 => 2`
* AOE: `0 => 75`
* AOE falloff: `None => Quadratic`
* Rate of fire: `14 => 4`
* Number of bursts: `2 => 15`
* Cooldown: `0.1s => 0`
* Burst: `0.8-1s => 0.334s`
* Reload: `2s => 1.65s`
* Range: `1200 => 1450`
* Accuracy: `95%/85%/75% => 100%/95%/60%`
* Turret rotation speed: `180 => 150`
* World height offset: `5 => 15`

### Targeting jammer
> *Extremely situational ability which wasn't very useful even when used in its perfect case scenarios.*

* Cost: `150CU => Free`
* Hitpoints: `500 => 1100`
* Max deployment range: `1100 => 1250`
* Sensors radius: `0 => 270`
* Contact radius: `0 => 400`
* Cooldown: `60s => 80s`
* Projectile: `Mine => Scanner` (increased travel speed)
* Fixed an issue of this unit always being "contacted"
* Status effect:
    * Max speed reduction: `10% => 45%`
    * Turn radius decrease: `5% => 35%`
    * Acceleration increase: `0 => 25%`
    * Added a unit behavior modifier which makes units try to keep a distance of 400 units away from their target while inside ECM field (this is to prevent AI from endlessly circling the ECM with strike craft)

## LAV
> *LAV have been revealed as a center point of effective coalition play. Oppressive early game strategies along with LAV providing a strong mid/late game defensive core for the coalition army is the main reasoning behind the reduction of overall LAV effectiveness. Production time is increased substantially due to production upgrade being available earlier and it was needed to curb the power of LAV openers in general. The base damage of the weapon is reduced to make armor more effective at protecting against it.*

* Tech:
    * Cost: `300CU => 350CU`
    * Research time: `35s => 35s`
* Build time: `8s => 12s`
* Hitpoints: `500 => 450`
* Armor: `0 => 2`
* Weapon:
    * Base damage: `15 => 16`
    * Burst: `0.8-1.2s => 0.95-1s`
    * Burst count: `4 => 2`
    * Cooldown: `0.8s => 0.45s`
    * Accuracy:
        * Short: `94% => 90%`
        * Medium: `82% => 85%`
        * Long: `56% => 61%`
    * Turret rotation speed: `180 => 250`
    * Damage against air: `50% => 70%`
    * Damage against probes: `100% => 50%`
    * Accuracy against medium, large, xlarge: `100% => 130%`
* Max speed: `110 => 120`
* Speed boost ability:
    * Speed bonus: `60% => 45%`
    * Turn radius increase: `50% => 35%`
* Upgrade research time:
    * Speed boost: `50s => 40s`
    * Damage level 1: `30s => 25s`
    * Damage level 2: `60s => 45s`

## AAV

**Survivability**
> *The hitpoints are reduced on AAV to make soft-countering them with units such as assault ships or interceptors more of an option than it previously was. Previously, AAV would drive past a lot of things to target the squishier targets such as enemy salvagers. This is still possible, but the enemy can react to it easier.*

* Hitpoints: `1400 => 940`
* Sensors: `1000 => 1100`

**Pricing**
> *AAV timing on small maps is a bit too oppressive. Due to an increase of unit's lategame utility, the base cost is going up slightly. AAV are not very effective late game units and are cheap, their population cost doesn't reflect this.*

* Tech cost: `350CU 85RU => 400CU 75RU`
* Tech research time: `50s => 60s`
* Cost: `180CU 30RU => 250CU 20RU`
* Production time: `14s => 17s`
* Population: `3 => 2`

**Weapon**
> *AAV weapon has notoriously one of the weakest late game weapons present in the game (for example, it dealt only 1 damage per shot to upgraded railguns). These changes will allow it to maintain some damage output against units with upgrades.*

* Damage: `11 => 15`
* Rate of fire: `20 => 14`
* Burst: `0.5-0.6s => 0.5-0.55s`
* Range: `800 => 1000`
* Slow effect: `50% => 35%`

## Railgun

**Tech**
> *These changes are part of an effort to fix a particularly strong early game 1 base carrier timing push. Additionally, mag accelerator is overall too much of a no-brainer upgrade and a cost increase will make it slightly more difficult to acquire, making it more of a decision in midgame to get it quickly.*

* Research cost: `450CU 135RU => 300CU 125RU`
* Research time: `50s => 60s`
* Build time: `14s => 16s`

**Movement speed**
> *Coalition and Soban railguns are generally less effective damage-wise for their cost, they needed a slight nudge but it couldn't be in their raw performance. Movement speed buff will increase early game usability and general flexibility of the unit while not affecting the blobbing style too much.*

* Max speed: `60 => 70`

**Accuracy**
> *All railguns have seen a general accuracy increase to reduce RNG of missing in railgun fights..*

* Short: `5.6% => 7%`
* Medium: `5.3% => 6.5%`
* Long: `5% => 6%`

**Range**
> *All railgun and carrier ranges are reduced in the mod as part of the effort to reduce the prevalence of railgun-based strategies.*

* Range: `2100 => 2060`

### Mag accelerator upgrade
> *The upgrade was too impactful for early game performance. Railguns are still balanced around this upgrade being present, but the lack of this upgrade in the early game is now not as impactful as before.*

* Cost: `400CU 100RU => 100CU 250RU`
* Damage bonus: `60 => 25`

### Coalition railgun
> *Railguns have seen a large redesign in the mod, where their damage per shot has been reduced, cost increased, but hitpoints also increased. Railgun battles now resolve themselves slower, and high ground advantage plays a much larger role.
Coalition railguns have also seen some reload time buffs to go alongside target priority & reveal time changes to bring cost / damage output closer to the insanely high values that gaalsien railguns have in that category.*

* Cost: `200CU 60RU => 240CU 80RU`
* Hitpoints: `670 => 750`
* Armor: `3 => 0`
* Experience value: `350 => 450`
* Damage: `225 => 155`
* Reload: `3.5s => 2.0s`

### Soban railgun
> *Railguns have seen a large redesign in the mod, where their damage per shot has been reduced, cost increased, but hitpoints also increased. Railgun battles now resolve themselves slower, and high ground advantage plays a much larger role.
> 
> *The gap between coalition and Soban railgun performance has been lessened significantly, but soban railgun remains the most cost efficient railgun in the game.*

* Cost: `210CU 60RU => 240CU 80RU`
* Hitpoints: `680 => 750`
* Armor: `4 => 0`
* Experience value: `350 => 470`
* Damage: `165 => 155`
* Cooldown: `2s => 1.3s`
* Reload: `2.5s => 4.25s`

## Missile battery

**General stats**
> *The largest factor of AA doing its work vs normal air strategies is the first shot. Increased reload duration means AA will have a much harder time quickly killing off large numbers of air and heavy air and both of those strategies are underused, however it won't affect the early game air rush situations very much. Additionally rebalancing cost, lowering armor to make out of position batteries more punishable and increasing speed to ease the use of this unit*

* Cost: `350CU 80RU => 300CU 90RU`
* Speed: `50 => 60`
* Armor: `5 => 3`
* Reload: `2s => 3s`

**Mortar ability**
> *Mortar damage was extremely polarizing. When hitting enemy units from the high ground it had the potential to make game-winning plays of wiping entire enemy strike craft forces, but when hitting normally the damage could end up irrelevant. These changes should make this ability much more consistent in its performance, killing off strike craft in the center, and damaging a good chunk around them in a healthy area of effect.*

* Benefits from high ground: `Yes => No`
* Falloff: `None => Linear`
* Damage packets: `20 => 30`
* AOE: `180 => 220`
* Damage: `450 => 660`

## Assault cruiser

**General stats**
> *Assault cruiser becomes slightly worse at brawling against other cruisers and armored vehicles but gets help in other areas such as its cost, its hitpoints and its abilities. Weapon and armor changes will allow mid-tier units to soft-counter out of position assault cruisers in some fringe situations, whereas previously assault cruisers were very hard to weed out even by much superior numbers when they were positioned behind dunes.*

* Tech research cost: `600CU 350RU => 500CU 250RU`
* Production time: `65s => 60s`
* Cost: `500CU 250RU => 400CU 220RU`
* Population: `6 => 5`
* Hitpoints: `2700 => 2900`
* Armor: `15 => 12`
* Max movement speed: `70 => 65`
* Missile barrage benefits high ground: `Yes => No`
* Cooldowns:
    * Missile barrage: `60s => 40s`
    * Overdrive: `80s => 40s`
    * Self repair: `50s => 40s`
* Overdrive armor bonus: `100% => 50%`
* Tactical missile barrage reworked:
    * Cost: `250CU => Free`
    * Damage: `200 => 180`
    * AOE: `120 => 140`
    * Falloff: `None => Quadratic`
    * Range: `1350 => 1000`
    * Damage against small targets: `100% => 60%`
* Weapon:
    * Damage: `70 => 50`
    * Rate of fire: `2 => 3`
    * Number of bursts: `2 => 4`
    * Reload: `2s => 3.5s`
    * AOE: `80 => 75`
    * Wind-up: `50ms => 0.25s`
    * Burst: `1s => 0.7s`

**AA upgrade**
> *This upgrade is very weak, especially because the AA weapon is weaker than normal AA. Cost reduction should make it more desirable.*

* Cost: `500CU 340RU => 300CU 150RU`
* Research time: `65s => 45s`

## Battlecruiser

**Common**
> *The unit is overall unreasonably expensive for utility and options that it provides for the player. Area of effect changes allow battlecruisers to deal somewhat meaningful damage against strike craft forces. Unit is receiving large tech and production cost reductions but reduced survivability*

* Tech cost: `700CU 450RU => 550CU 300RU`
* Production time: `75s => 55s`

### Coalition
> *Damage is reduced in favor of higher rate of fire. This helps the unit deal with medium vehicles easier while also curbing its insane damage potential against carriers*

* Cost: `800CU 225RU => 650CU 280RU`
* Production time: `60s => 65s`
* Hitpoints: `6500 => 2700`
* Armor `25 => 15`
* Damage: `300 => 200`
* Reload : `7s => 4.8s`
* Falloff: `Linear => Quadratic`
* AOE: `50 => 55`
* Movement dynamics:
    * Max speed: `50 => 62`
    * Turn radius: `200 => 130`
    * Acceleration time: `1.5s => 1.2s`
    * Braking time: `1s => 0.9s`

### Soban
> *Long range high damage unit. Very dangerous to have such a unit be also extremely survivable. Improving close range accuracy, this unit had higher accuracy on Distant range than Short and Medium.*

* Cost: `780CU 220RU => 650CU 280RU`
* Production time: `60s => 65s`
* Hitpoints: `6500 => 2700`
* Armor `25 => 13`
* Population: `5 => 6`
* Movement dynamics:
    * Max movement speed: `50 => 62`
    * Max speed turn radius: `200 => 160`
    * Acceleration time: `1.5s => 1.9s`
    * Braking time: `1s => 1.2s`
* Range: `1750 => 1650`
* Damage: `320 => 280`
* Reload: `5s => 8.5s`
* Cooldown: `3s => 1.2s`
* Wind-up: `0.6s => 2.2s`
* Accuracy:
	* Short: `4% => 7%`
	* Medium: `4% => 6%`

## Artillery cruiser

**General stats**
> *Getting to artillery should now be much faster and easier. This is designed this way to allow for players to play against enemy railguns without the need of using own railguns, albeit in a still risky way, especially against midgame railgun pushes. Survivability changed to make artillery battles resolve themselves much faster. This makes countering artillery with own artillery less desirable as it's more risky. Additionally, sniping artillery cruisers was too difficult overall.*

* Tech research cost: `500CU 350RU => 500CU 250RU`
* Research time: `100s => 55s`
* Cost: `450CU 250RU => 450CU 200RU`
* Population: `6 to 4
* Construction time: `70s => 60s`
* Hitpoints: `2500 => 2100`
* Armor: `5 => 6`
* Movement dynamics characteristics:
    * Max speed: `50 => 56`
    * Acceleration time: `1.5s => 1.2s`
    * Braking time: `1s => 0.9s`
    * Turn radius: `100 => 90`

**Autofire**
> *Autofire is an extremely unsatisfying mechanic, exceptionally annoying to deal with for an opposing player while requiring little-to-no effort on the part of artillery cruiser users to be effective. It'll remain useful for forcing enemy to constantly micro their units and force the opponent to displace if they are in range, but will ultimately be less punishing and easier to deal with.*

* Damage: `200 => 100`
* Packets: `2 => 1`

**Barrages**
> *Barrages were pretty difficult to use on most maps against railguns, increased range should help with artillery cruiser usability on a larger variety of maps.*

* Barrage recharge: `65s => 100s`
* Rate of fire: `4 => 3`
* Number of bursts: `8 => 6`
* Barrage and precision barrage ranges: `2400 => 2650`
* Precision barrage:
    * Benefits from high ground: `Yes => No`
    * Cooldown: `30s => 60s`
    * Now has the same modifiers as normal barrage

## Fighter and gunship fabrication

**Tech**
> *Slight cost rebalance to require higher RU commitment, RU costs of units in this tech is reduced.*

* Research cost: `500CU 200RU => 450CU 200RU`
* Research time: `70s => 65s`

### Strike fighter
> *Strike Fighter timings are extremely powerful and their numbers can grow very fast. These changes aim to reduce strike fighter timing attack strength (especially in CvC matchups, but also against gaalsien railgun openings), and make soft countering strike fighters easier (hitpoint reduction).*

* Cost: `150CU 100RU => 200CU 85RU`
* Production time: `15s => 26s`
* Hitpoints: `650 => 490`
* Armor: `2 => 4`
* Weapon:
    * Rocket count: `10 => 8`
    * Damage packets: `1 => 2`
    * Rate of fire: `2 => 3`
    * Burst: `1000ms => 667ms`
    * Reload: `3000ms => 3332ms`
    * Field of fire: `50 => 55`
    * Range: `1200 => 1250`
* Max hangar size: `15 => 12`

### Gunship
> *Increased range to make weapon work more consistently as the gunship circles its target. Unit cost rebalanced to be more of a CU sink than an RU one. Armor decreased to make PC, BR and LAV be slightly more effective at chipping away at it, but total hitpoint pool increased. Weapon packet count reduced, making it significantly more effective against lightly armored targets. Area of effect is increased but added falloff should make gunship's area damage slightly less powerful overall.*

* Cost: `380CU 250RU => 500CU 100RU`
* Production time: `55s => 45s`
* Population: `2 => 3`
* Hitpoints: `1050 => 1250`
* Armor: `10 => 9`
* Damage: `60 => 36`
* Damage packets: `4 => 1`
* AOE: `150 => 160`
* Falloff: `None => Quadratic`
* Range: `700 => 1050`

## Tactical bomber
> *Very underused unit in the metagame. Costed extremely prohibitively for what it's capable of accomplishing. The rebalanced version of the unit should be very useful at destroying clumped up mid tier army units. Damage changes are made specifically so that they can't 1 shot AA batteries and 2 bombs are not enough to destroy a production or support cruiser. Double bombers should still be a solid choice for destroying out of position cruisers, with some follow-up.*

* Research time: `75s => 55s`
* Research cost: `550CU 200RU => 550CU 150RU`
* Cost: `500CU 250RU => 350CU 160RU`
* Population: `2 to 4`
* Hitpoints: `1050 => 1350`
* Armor: `15 => 20`
* Max speed: `370 => 390`
* Turn radius: `350 => 310`
* Damage: `2500 => 1500`
* Damage against Small: `100% => 60%`
* AOE: `180 => 220`
* Wind-up: `50ms => 0ms`

# Gaalsien / Khaaneph

## Salvager

* Armor: `2 => 3`

## Gaalsien carrier

**General stats**
> *Carriers should become a bit trickier to use in combat and carrier aggression should become a bit more punishable. Worth noting that these changes coincide with railgun nerfs, however.*

* Hitpoints: `12500 => 8100`
* Armor: `40 => 20`

**Point defense weapons**
> *Lower level PD performance increased, but higher level rate of fire reduced (due to damage rework of carrier PD weapons)*

* Rate of fire: `10 => 8`
* Weapon Systems power shunt PD rate of fire:
    * Level 1: `'set to 17' => 'increase by 20%'`
    * Level 2: `'set to 24' => 'increase by 35%'`
    * Level 3: `'set to 31' => 'increase by 50%'`
    * Level 4: `'set to 38' => 'increase by 70%'`
    * Level 5: `Bonus removed (30 => 10)`

**Re-establish systems regeneration rate**
> *With railguns costing more and carrier hitpoints reduced, time to heal the carrier to full was too short.*

* Level 2: `50 => 35`
* Level 3: `70 => 50`
* Level 4: `90 => 65`
* Level 5: `110 => 80`

**Speed**
> *Slight reduction in power of this power system. Chasing down a lategame gaalsien carrier was previously extremely difficult.*

* Base: `10 => 15`
* Speed systems power shunt:
    * Level 3: `75 => 70`
    * Level 4: `95 => 85`
    * Level 5: `120 => 105`

### Hyper-sonic missile barrage
> *Nuke-style abilities have the potential to wipe big parts of enemy army without much chance for retaliation, only preemptive preparation is effective. A bigger window is required after their use so that players can have an engagement which will not involve another one. Hyper-sonic missile barrage is also one of the most inconsistent abilities, while also being extremely damaging when hitting larger targets. Damage reduced and increased area of effect should make the ability feel more consistent.*

* Cooldown: `90s => 160s`
* Damage: `600 => 240`
* Damage against carriers: `50% => 100%`
* AOE: `200 => 230`
* AOE falloff: `Linear => Quadratic`
* Missile count per weapon: `10 => 8`
* Fixed an issue where the entity which granted vision for the barrage had a population cost (`1 => 0`)

## Khaaneph carrier

**General stats**
> *Carriers should become a bit trickier to use in combat and carrier aggression should become a bit more punishable. Worth noting that these changes coincide with railgun nerfs, however. Khaaneph armor was abnormally low compared to other carrier which, combined with its slow speed, was a bit too punishable in some situations. The new mobility support makes this carrier considerably faster, adds sensors range and speed*

* Hitpoints: `12500 => 9600`
* Armor: `20 => 15`
* Sensor radius: `800 => 1200`
* Contact radius: `1000 => 1350`
* Max speed: `40 => 45`

**Cruise missiles systems**
> *Khaaneph cruise missiles have proven themselves to be extremely powerful overall and especially against enemy carriers.*

* Damage: `400 => 670`
* Packets: `1 => 5`
* AOE: `150 => 140`
* Damage against carriers: `150% => 70%`
* Affected by high ground: `Yes => No`
* Base missile warmup time: `6s => 9s`
* Range bonuses:
    * Level 2: `0 => 100`
    * Level 3: `0 => 200`
    * Level 4: `0 => 350`
    * Level 5: `36% => 500`
* Warmup time bonuses:
    * Level 2: `1 => 0`
    * Level 3: `2 => 1`
    * Level 4: `3 => 2`
    * Level 5: `4 => 3`

**Weapon systems**
> *Khaaneph carrier does not have range systems on it, meaning the range of its basic weaponry can never be increased. This meant that weapons systems power shunt was mostly useless as it could never get range on the opponent. Increasing base range of carrier weapons can be dangerous for early game therefore Khaaneph carrier is receiving some nerfs to its basic weapons for low levels. High power level PDs receive the highest available rate of fire compared to other carriers, however, to make this system more desirable.*

* PD ranges: `250/500/750 => 350/650/1100`
* PD ROF: `8 => 10`
* Missile systems range: `750 => 950`
* Missile systems wind-up: `0.25s => 0.5s`
* Power shunt now provides extra fire rate to missile systems
* Rate of fire bonuses:
    * Level 1: `'set to 17' => 'increase by 25%'`
    * Level 2: `'set to 24' => 'increase by 40%'`
    * Level 3: `'set to 31' => 'increase by 65%'`
    * Level 4: `'set to 38' => 'increase by 100%'`
    * Level 5: `'set to 38' => 'increase by 50%'`
* Fixed a bug where level 5 weapon system power shunt would decrease the range of one of the PD weapons

**Mobility support system**
> *The diameter of level 5 speed boost was larger than the range of a railgun. In team games this would allow for somewhat oppressive speed boost blobbing strategies which should now be slightly more difficult to execute correctly. Despite this, this system was generally extremely underutilized and is therefore getting secondary functionality which makes this system desirable over other systems in both a lategame head to head carrier brawl and early game skirmishing.*

* Now grants sensors range to all medium and large units (meaning entire fleet except strike craft and workers)
* Now has double effectiveness for the carrier itself
* Speed bonuses:
    * Level 1: `3 => 8%`
    * Level 2: `6 => 12%`
    * Level 3: `10 => 16%`
    * Level 4: `15 => 20%`
    * Level 5: `20 => 25%`
* AOE radius:
    * Level 1: `420 => 600`
    * Level 2: `420 => 600`
    * Level 3: `800 => 750`
    * Level 4: `800 => 750`
    * Level 5: `1200 => 1000`
* Added sensors range bonus:
    * Level 1: `+100 sensors range`
    * Level 2: `+150 sensors range`
    * Level 3: `+200 sensors range`
    * Level 4: `+250 sensors range`
    * Level 5: `+300 sensors range`

**Re-establish systems regeneration rate**
> *With railguns costing more and carrier hitpoints reduced, time to heal the carrier to full was too short.*

* Level 2: `50 => 35`
* Level 3: `70 => 50`
* Level 4: `90 => 65`
* Level 5: `110 => 80`

## Baserunner

### Gaalsien baserunner
> *Due to the healing ability being immensely powerful, gaalsien now has slightly lower hitpoint pool than other baserunners.*

* Hitpoints: `3350 => 2000`

**Heal aura ability**
> *It is no longer possible to abuse baserunner spam to quickly heal large amounts of hitpoints on targets such as the carrier, as the heal doesn't stack nearly as strongly as it used to. Overall effectiveness of this ability is increased immensely, however. The stacking portion heals 200 hitpoints in total per 10 seconds. The non-stacking portion heals 600 hitpoints per 10 seconds. Total heal amount increases from 400 to 800.*
* Recharge time: `50s => 80s`
* Rate of healing: `1 => 10`
* Amount: `40 => 2`
* Now applies a non-stacking healing over time status effect to friendly units:
    * Rate of healing: `20`
    * Healing: `3`
* Prevented from affecting air units

**Deploy sensor ability**
> *Slight ease of use improvement for this ability as it is considerably weaker than the combination of Khaaneph baserunner abilities*

* Deployment range: `2350 => 2550`
* Recharge: `200s => 140s`
* Hitpoints: `600 => 250`
* Scanner sensors radius: `1400 => 1300`

### Khaaneph baserunner

* Hitpoints: `3350 => 1700`

**Speed**
> *To improve early game scouting and improve baserunner interactions with early game units Khaaneph baserunner gets a slight speed advantage. This might also open up strong opportunities for artifact-based midgame strategies.*

* Max speed: `70 => 80`

**Smoke ability**
> *Baserunners could survive on their own a bit too much. On the other hand, the recharge of this ability was rather long and could be tuned down.*

* Recharge: `180s => 40s`
* Burst count: `4 => 3`

**Passive regen ability**
> *An unused ability in Khaaneph Baserunner has been repurposed to provide passive regeneration akin to other Gaalsien/Khaaneph units.*

* No-damage activation delay: `10s`
* Regeneration amount: `20`
* Time between regeneration ticks: `1s`

#### Blast drone
> *A 1PC skimmer together with blast drones rush was nearly impossible to stop even with perfect response and good micro. Additionally, late game BD use was limited and expensive. The new BD iteration should hopefully provide extra motivation for getting them later in the game while fixing the issues with early game rushes.*

* Construction time: `20s => 70s`
* Hitpoints: `500 => 540`
* Population: `0 => 2`
* Falloff: `None => Quadratic`
* AOE: `200 => 260`
* Damage: `650 => 620`
* Damage packets: `10 => 15`
* Max speed: `160 => 200`
* Braking time: `0.75s => 0.1s`

## Sandskimmer

**General stats**
> *Discrepancy between LAV and Skimmer hitpoints was very large and caused almost every area of effect weapon to be extremely difficult to balance. Skimmers also needed a slight decrease in power. Slightly increased sensors range should help skimmers avoid AAV and other early game threats easier.*

* Tech research time: `35s => 30s`
* Hitpoints: `650 => 540`
* Sensor radius: `1000 => 1150`
* Self regen:
    * Activation time: `3.5s => 5.5s`
    * Amount healed per tick: `16 => 20`
* Short range accuracy: `100% => 85%`

**Weapon**
> *It is generally easier to counter strike craft in the mod, the extra DPS was introduced in order to bring back the rock-paper-scissors mechanic, meaning strike craft will be capable of countering enemy railguns. The base damage of the weapon is reduced to make armor more effective at protecting against it.*

* Damage: `15 => 11`
* ROF: `3 => 7`
* Reload: `0.1s => 0.6s`
* Cooldown: `0.398s => 0.35s`
* Burst: `0.67-1s => 0.78-0.84s`
* Long range accuracy: `88.21% => 80%`

**Upgrades**
> *These changes are part of the effort of reducing supply blocking due to upgrades for gaalsien.*

* Raiding upgrade research time: `50s => 40s`
* Damage 1 upgrade research time: `30s => 25s`
* Damage 2 upgrade research time: `60s => 45s`

## Production cruiser

**Hitpoints**
> *A slight reduction because seeing PC snipes was too uncommon as a result of reduction to damage of high damage weaponry in the mod.*

* Hitpoints: `4100 => 3500`
* Armor: `5 => 6`

**Costs**
> *Strategies of quickly transitioning from heavy aggression to 3 base economy are extremely strong and need to be tuned down. This doesn't affect conventional fast expand strategies very much, early game units are getting tuned around this change. RU cost on production cruisers is there to slow down tech progression when expanding. Currently, there's almost no downside and slow down when expanding from 2 base to 3 base, this should make tech progression just slightly slower which could prove meaningful vs aggressive enemy strategies.*

* Refinery tech cost: `700CU => 600CU 80RU`
* Cost: `600CU => 600CU 60RU`

**Sensors**
> *Production cruisers can be ambushed quite easily by enemy assault ships or AAV which can cause game ending damage because production cruisers don't have high enough movement speed to escape, and even if the PC itself doesn't die, the units coming out of them do. The extra vision range makes PCs able to preemptively move back. This also helps with vision for early game pushes.*

* Sensors radius: `1000 => 1450`
* Contact radius: `1250 => 1600`

**AA weapon**
> *DPS was rebalanced slightly to be lower on short and medium range but stronger on long range, an additional slight range increase is introduced in order to help mitigate early game air plays. This should ensure that air is a bit harder to control and will most likely be bleeding hitpoints when attempting to operate close to production cruisers.*

* Rate of fire: `15 => 12`
* Range: `1100 => 1250`
* Accuracy:
    * Short: `55% => 60%`
    * Medium: `40% => 55%`
    * Long: `25% => 40%`
* Hidden accuracy modifiers against probes removed
* Damage against probes: `100% => 50%`

## Assault ship
> *Reducing tech cost to make this tech path more desirable in more situations. Range increase should help with unit usability issues as well as improve overall effectiveness, particularly against units it's intended to counter. The unit is extremely strong when it can get into position to fire, so, to reduce the impact of assault ship rushes and assault ship early game dominance, hitpoints of the assault ship are getting reduced. To mitigate midgame assault ship spam and all-in aggro strategies, their cost is getting increased. Additionally, now that assault ships have good range to do consistent damage to strike craft, their large area of effect is no longer required for them to be effective at countering them, therefore it is getting falloff.*

* Tech cost: `600CU 100RU => 450CU 80RU`
* Tech research time: `60s => 65s`
* Cost: `220CU 40RU => 300CU 35RU`
* Production time: `18s => 17s`
* Hitpoints: `1400 => 960`
* Armor: `6 => 5`
* Self regeneration per tick: `20 => 15`
* Max movement speed: `70 => 72`
* Sensors: `1000 => 1100`
* Contact radius: `1200 => 1250`
* Damage: `24 => 30`
* ROF: `5 => 4`
* Burst: `0.8-1s => 0.75s-0.85`
* AOE: `80 => 120`
* Falloff: `None => Quadratic`
* Range: `700 => 920`

## Missile ship

**Tech**
> *Even though the scouting window is existent in the mod, it was still incredibly short, despite strike fighter production time being increased drastically. Missing scouting, or being hit by an air timing attack, was unbelievably punishing as G/K. The following change is meant to reduce the impact of getting hit by air in those cases and also to make the scouting window larger.*

* Missile ship fabrication research time: `55s => 45s`

**General stats**
> *Gaalsien AA tanks take significantly lower to tech into and produce, a small production time buff should help gaalsien prepare for enemy air plays more easily. The largest factor of AA doing its work vs normal air strategies is the first shot. Increased reload duration means AA will have a much harder time quickly killing off large numbers of air and heavy air and both of those strategies are underused, however it won't affect the early game air rush situations very much.*

* Cost: `400CU 80RU => 350CU 90RU`
* Armor: `5 => 3`
* Production time: `28s => 24s`
* Reload: `1s => 2.5s`
* Range: `1400 => 1330`
* Fixed an issue where veterancy 4 rate of fire increase did nothing for the unit, it now grants a 1s reduction to reload time

**Radar guided missiles upgrade**
> *Range upgrade pretty much has never seen use in competitive play. Gaalsien AA range is strong enough to cover most of what it needs to cover and the fact that it can regenerate hitpoints generally allows it to position itself more aggressively than the coalition AA tank counterpart. With base range being reduced, radar guided missile upgrade should become more of an important upgrade when facing more committed enemy air play.*

* Radar upgrade range: `1600 => 1500`
* Research time: `30s => 20s`
* Fixed an issue where radar upgrade was reducing turret rotation speed rather than increasing it:
    * Turret field of fire: `120 => 40`
    * Base turret rotation speed: `240 => 160`
    * Upgraded turret rotation speed: `180 => 240`

**Direct missile barrage**
> *Direct missile barrage is now much better at hitting enemy strike craft and also more potent at dealing good damage to medium vehicles. The recharge upgrade was considerably underutilized and for good reason. Reducing cost and time to purchase the upgrade, making it less of a commitment and more of a quality of life upgrade to occasionally get in case there are already multiple MS out on the field.

* Weapon:
    * Recharge: `60s => 90s`
    * Damage: `150 => 140`
    * AOE: `80 => 150`
    * Falloff: `None => Linear`
    * Benefits from high ground: `Yes => No`
* Recharge upgrade cost and research time: `300CU 85RU 30s => 220CU 60RU 15s`

## Vehicle armor upgrade cost
> *Ship armor upgrades are the least used upgrades and the least useful ones. Decreasing cost and time to purchase these upgrades to make them more desirable.*

* Level 1: `200CU 100RU 15s => 150CU 100RU 15s`
* Level 2: `200CU 200RU 20s => 200CU 150RU 20s`
* Level 3: `200CU 300RU 30s => 250CU 200RU 25s`

## Railgun fabrication
> *Having research take less time makes it easier to counter various rush strategies.*

* Tech cost: `450CU 200RU => 350CU 250RU`
* Tech research time: `50s => 45s`

### Assault railgun
> *Assault railguns are pretty difficult to deal with on some maps and reaching critical mass of them is rather easy. A slight rebalance to their survivability and cost to better place the unit in terms of how it lines up with things it's supposed to counter, and its counters. Maneuverability changes should allow strike craft and other units which normally have a hard time catching them to be more capable of doing it and promotes the use of dart maneuver ability. Damage is increased but reload also lengthened to frontload the damage output, this is to address mirror matchup defensive player having a hard time capitalizing on the safe haven of the carrier. Overall AR DPS is slightly reduced with other midgame unit balancing in mind, AR were a bit too good at countering a lot of them. Wind-up time reduced (and moved to reload) to make the weapon more responsive when AR are being flanked.*

* Cost: `200CU 35RU => 240CU 45RU`
* Production time: `24s => 17s`
* Hitpoints: `550 => 600`
* Armor: `6 => 4`
* Self regeneration per tick: `13 => 7`
* Sensors range: `1000 => 1250`
* Contact radius: `1250 => 1350`
* Experience value: `610 => 350`
* Armor upgrade hitpoint bonus:
    * Level 2: `100 => 50`
    * Level 3: `200 => 100`
* Movement dynamics characteristics:
    * Max speed: `100 => 85`
    * Acceleration time: `0.85s => 1.5s`
    * Braking time: `0.85s => 1.2`
* Damage: `50 => 42`
* Burst duration: `0.1-0.1s => 0.11-0.11s`
* Number of Bursts: `3 => 5`
* Wind-up: `1s => 0.6s`
* Wind-down: `0.5s => 0.25s`
* Reload: `0.6s => 2.6s`
* Max range: `1000 => 1100`
* Accuracy: `15%/13%/11% => 20%/16%/14%`
* Dart maneuver:
    * Tech time: `60s => 30s`
    * Tech cost: `100CU 100RU => 100CU 70RU`
    * Cooldown: `60s => 30s`
    * Duration: `2s => 3s`

### Heavy railgun

**General stats**
> *Railguns have seen a large redesign in the mod, where their damage per shot has been reduced, cost increased, but hitpoints also increased. Railgun battles now resolve themselves slower, and high ground advantage plays a much larger role. All railgun and carrier ranges are reduced in the mod as part of the effort to reduce the prevalence of railgun-based strategies. All railguns have seen a general accuracy increase to reduce RNG of missing in railgun fights.*

* Cost: `280CU 90RU => 350CU 110RU`
* Population cost: `3 => 4`
* Damage: `225 => 180`
* Hitpoints: `670 => 750`
* Max speed: `62 => 65`
* Turn radius: `150 => 50`
* Experience value: `450 => 550`
* Range: `2100 => 2060`
* Accuracy:
    * Short: `6% => 7%`
    * Medium: `5% => 6.5%`
    * Long: `4% => 6%`
* Railgun armor upgrade level 3 hitpoints granted: `200 => 100`

**EMP**
> *This upgrade has seen very little use throughout the game's history. Effectiveness buffs to make it more desirable.*

* Upgrade cost: `250CU 150RU => 300CU 100RU`
* Upgrade research time: `45s => 35s`
* Recharge time: `45s => 90s`
* Disables enemy weapons and abilities: `No => Yes`
* Damage: `150 => 110`
* Wind-up: `1s => 0.75s`
* AOE: `100 => 145`
* Range: `1200 => 1300`
* Duration: `1.5s => 2.5s`
        * Stun duration: `2.2s => 2.5s`
        * Area of effect: `135 => 145`
        * Range: `1250 => 1300`

**Ranged calibration**
> *This upgrade has seen very little use throughout the game's history. Effectiveness buffs to make it more desirable.*

* Cost: `250CU 150RU => 200CU 200RU`
* Research time: `60s => 45s`
* Range bonus: `300 => 370`
* Max speed penalty: `66% => 50%`
* Turn radius penalty: `66% => 50%`

## Railgun armor upgrades cost
> *Slight cost tweaks to make railgun skimmer playstyles spend CU a bit faster.*

* Level 2 cost: `200CU 200RU => 250CU 200RU`
* Level 3 cost: `200CU 300RU => 300CU 300RU`

## Interceptor

**General stats**
> *Cost changes are part of the effort to reduce the strength of assault ship rush follow-ups, but also this will help interceptor sustain and prevent them: `bogging down the carrier production line as heavily.*

* Tech cost: `250CU 250RU => 450CU 250RU`
* Tech research time: `55s => 70s`
* Cost: `250CU 120 RU => 250CU 100RU`
* Build time: `15s => 12s`
* Armor: `1 => 2`
* Hangar size: `15 => 12`

**Weapon**
> *Interceptor reload time was abnormally short (compared to 8s reload time of strike fighters), often allowing it to fire off the start of a second volley within a single pass over its target. This also made interceptors incredibly strong in dogfights and when they would circle very large targets (carriers), or when chasing the enemy. Overall rocket count per plane isn't changed, but 4 rockets are shot per burst instead of 3, decreasing the total number of bursts from 4 to 3. These changes will decrease the overall damage payload of interceptors per sortie. It will also decrease the RNG nature of interceptors fighting ground targets as more rockets will land resulting in more fair spread of damage to the intended targets. Damage per burst is going down from 450 to 440 (intent is to not change this very much), damage per sortie is going down from 1800 to 1320. Additionally, this set of changes will help mitigate the carrier sniping strategies utilized in team games.*

* Reload: `2s => 4.5s`
* Weapon base damage: `150 => 110`
* Weapon damage packets: `1 => 2`
* Weapon rate of fire: `3 => 4`
* Area of effect: `60 => 70`
* Damage against carriers: `100 => 60`

**Afterburner upgrade**
> *Afterburner upgrade is incredibly effective and can be oppressive in situations where a player can get it while being ahead in the game. Toned down its effects and increased the cost to make this upgrade more of a commitment.*

* Cost: `350CU 90RU => 200CU 120RU`
* Research time: `60s => 40s`
* Max speed bonus: `60% => 40%`
* Turn radius reduction: `60% => 40%`

## Precision bomber

**General stats**
> *Improved accessibility of tech and the unit itself should make this tech path much more desirable. Precision bomber has incredible maneuverability parameters, curbing those to make the unit harder to control and slower to deliver follow-up bombs on target. The damage characteristics have been updated to make the bomber worse at destroying enemy AA vehicles but still potent at dealing with enemy cruisers. Area of effect improved, but modifier against small targets added to prevent the bombers from becoming too strong against strike craft and salvagers.*

* Research cost: `400CU 275RU => 300CU 175RU`
* Research time: `65s => 45s`
* Cost: `300CU 220RU => 300CU 140RU`
* Production time: `32s => 22s`
* Population: `2 => 3`
* Hitpoints: `1250 => 1050`
* Max speed: `550 => 450`
* Turn radius: `225 => 300`
* Damage: `1000 to 800`
* Reload: `1.5s => 3.5s`
* Damage against small targets: `100% => 60%`
* AOE: `60 => 140`
* Falloff: `None => Quadratic`

**Upgrades**
> *Extremely expensive to fully upgrade gaalsien bombers, making these upgrades very undesirable unless all-inning. Bomber usability falls off as counters get added to the battlefield, investing into both bomber count and their upgrades normally is a very bad idea, these changes along with other air and anti-air rebalances should help with these upgrades become more desirable.*

* Rearm upgrade:
    * Cost: `350CU 70RU => 200CU 70RU`
    * Research time: `40s => 20s`
* Payload upgrade cost: `500CU 200RU => 400CU 200RU`

## Siege cruiser

**Range upgrade**
> *This is the longest research in the game, abnormally so.*

* Research time: `135s => 50s`

### Gaalsien siege cruiser
> *Getting to artillery should now be much faster and easier. This is designed this way to allow for players to play against enemy railguns without the need of using own railguns, albeit in a still risky way, especially against midgame railgun pushes. Due to hitpoint changes, artillery battles will get resolved faster. This makes countering artillery with own artillery less desirable as it's more risky. Additionally, sniping artillery cruisers was too difficult overall. Gaalsien siege cruiser is becoming a lot less cheap and more mobile, at the cost of decreased barrage effectiveness.*

* Tech research cost: `600CU 450RU => 250CU 150RU`
* Tech research time: `90s => 55s`
* Cost: `600CU 200RU => 300CU 150RU`
* Production time: `60s => 30s`
* Population: `6 => 5`
* Hitpoints: `2500 => 1400`
* Barrage:
    * Recharge: `50s => 90s`
    * Damage: `200 => 120`
    * Packets: `2 => 1`
    * Rate of fire: `3 => 5`
    * Number of bursts: `6 => 2`
    * Burst duration: `1.7s => 1.8s`
    * Cooldown: `1.6s => 1.4s`
* Movement attributes:
    * Max speed: `55 => 60`
    * Acceleration time: `1.5s => 1.25s`
    * Braking time: `1.5s => 1.25s`

**Autofire**
> *Autofire is an extremely unsatisfying mechanic, exceptionally annoying to deal with for an opposing player while requiring little-to-no effort on the part of artillery cruiser users to be effective. It'll remain useful for forcing enemy to constantly micro their units and force the opponent to displace if they are in range, but will ultimately be less punishing and easier to deal with.*

* Autofire damage: `200 => 120`
* Reload: `4s => 10s`
* Packets: `2 => 1`

### Khaaneph siege cruiser
> *Khaaneph siege cruiser is very strong and becomes problematic when spammed in team games, besides being very strong on maps with certain topology which allows siege cruisers to constrict players completely in their base. These changes should increase the critical mass required for siege cruisers to be able to counter its counters such as railguns, and reduce the potential of providing free damage on the enemy while keeping the barrage feeling powerful. Getting hit by KSC main weapon should be slightly less punishing overall, and micro against it is easier. However, the damage is applied over a considerably larger area, making it more consistent for the situations where units are trying to dodge it. Additionally, this cruiser was impossible to weed out from behind dunes. Armor reduction means that this cruiser can get swarmed even by lower damage weapon using units.*

* Tech research time: `90s => 95s`
* Cost: `650CU 200RU => 620CU 250RU`
* Hitpoints: `3350 => 3200`
* Population: `5 => 6`
* Production time: `60s => 45s`
* Sensors radius: `1000 => 1150`
* Contact radius: `1250 => 1300`
* Armor: `15 => 12`
* Main weapon:
    * Damage: `125 => 130`
    * Reload: `2.5s => 4.5s`
    * AOE: `150 => 270`
    * Falloff: `Linear => Quadratic`
* Barrage:
    * Recharge: `50s => 140s`
    * Damage: `125 => 240`
    * Damage packets: `1 => 2`
    * Falloff: `None => Quadratic`
    * AOE: `150 => 240`
    * Damage against small targets: `100% => 65%`
    * Damage against carriers: `100% => 80%`
    * Number of bursts: `3 => 4`
    * Cooldown: `0.8s => 2.5s`

## Honourguard cruiser

**General stats**
> *It should now be easier to field honourguard cruisers and overall weapon performance is more more consistent. A rebalance to unit's hitpoint pool was required to curb the overall survivability and make it slightly easier to counter.*

* Tech time: `75s => 65s`
* Cost: `700CU 240RU => 550CU 270RU`
* Production time: `70s => 55s`
* Hitpoints: `3600 => 2700`
* Population: `5 => 7`
* Max speed: `60 => 54`

**Weapon**
> *Honourguard cruisers had the potential to one-shot enemy strike craft force from long range when firing at them from high ground, which could often end the game very quickly. The damage that the weapon had also made its overall DPS extremely low, meaning it was very bad at countering anything which had a meaningful hitpoint pool. The weapon should now perform much more consistently and feel powerful even against bulkier targets.*

* Main weapon:
    * AOE: `200 => 220`
    * Damage: `400 => 500`
    * Reload: `5s => 4.5s`
    * Falloff: `None => Linear`
    * Wind-down: `0.5s => 0.25s`
    * Target prioritization:
        * Weapon effectiveness weight: `increased`
		* Distance weight: `decreased`
		* Angle weight: `decreased`
		* Auto target sticky bias: `decreased`

**Anti-air**
> *Honourguard cruiser anti-air is relatively weak and paying such a large sum for it is almost never worth it. The long wind-up also often meant that the target would fly out of range before the weapon could fire.*

* Research time: `75s => 45s`
* Research cost: `600CU 370RU => 300CU 200RU`
* Wind-up: `3s => 1.5s`
* Reload: `0 => 3s`
