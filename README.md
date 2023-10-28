NOT UPDATED TO LATEST VERSION, WIP

# Rose's Utilities
Adds a collection of useful utilities that enhance both vanilla and modded ARK experiences.

## Installing the Mod
Log into Steam, go to [Rose's Utilities](https://steamcommunity.com/sharedfiles/filedetails/?id=2939004410), and subscribe to the mod. Then launch ARK and the mod should automatically download.

## GameUserSettings.ini Configuration
First close your game/server. Then in the GameUserSettings.ini file, find/add the [RosesUtilities] section below and change the settings you want changed and save the file. When you restart your game/server, the new settings should be applied.

The settings are as follows:
- InfiniteFoodBuffBlacklist: Comma seperated list of creatures that cannot have the infinite food items used on them
- ShockAbsorbersDamageCap: Max amount of fall damage taken when Shock Absorbers are applied
- ShockAbsorbersDamagePercent: Max percent of fall damage taken when Shock Absorbers are applied

```
[RosesUtilities]
InfiniteFoodBuffBlacklist=Daeodon_Character_BP_C,Daeodon_Character_BP_Eden_C
ShockAbsorbersDamageCap=1000
ShockAbsorbersDamagePercent=1
```

## S+ Pull Resource Config
Add the following to the end of the **PullResourceAdditions=** line in your **GameUserSettings.ini** file under the **\[StructuresPlus\]** section to enable S+ resource pulling for Rose's Utilities items. If the config line already has items in it from other mods, seperate those items from the Rose's Utilities items with a comma.

```
/Game/Mods/RosesUtilities/Items/Consumables/TeamBuildingBook/PrimalItemConsumable_TeamBuildingBook.PrimalItemConsumable_TeamBuildingBook,/Game/Mods/RosesUtilities/Items/Consumables/Self-ImprovementBook/PrimalItemConsumable_Self-ImprovementBook.PrimalItemConsumable_Self-ImprovementBook,/Game/Mods/RosesUtilities/Items/Consumables/SurvivalKit/PrimalItemConsumable_SurvivalKit.PrimalItemConsumable_SurvivalKit,/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Crude/PrimalItemConsumable_ArmorRepairKitCrude.PrimalItemConsumable_ArmorRepairKitCrude,/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Basic/PrimalItemConsumable_ArmorRepairKitBasic.PrimalItemConsumable_ArmorRepairKitBasic,/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Advanced/PrimalItemConsumable_ArmorRepairKitAdvanced.PrimalItemConsumable_ArmorRepairKitAdvanced,/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Universal/PrimalItemConsumable_ArmorRepairKitUniversal.PrimalItemConsumable_ArmorRepairKitUniversal,/Game/Mods/RosesUtilities/Items/Consumables/V-Mate/PrimalItemConsumable_V-Mate.PrimalItemConsumable_V-Mate,/Game/Mods/RosesUtilities/Items/Consumables/ShockAbsorbers/PrimalItemConsumable_ShockAbsorbers.PrimalItemConsumable_ShockAbsorbers,/Game/Mods/RosesUtilities/Items/Consumables/FruitOfGrisaia/PrimalItemConsumable_FruitOfGrisaia.PrimalItemConsumable_FruitOfGrisaia,/Game/Mods/RosesUtilities/Items/Consumables/FleshOfOuroboros/PrimalItemConsumable_FleshOfOuroboros.PrimalItemConsumable_FleshOfOuroboros,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_MetalIngot.PrimalItemResourcePallet_MetalIngot,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_ScrapMetalIngot.PrimalItemResourcePallet_ScrapMetalIngot,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Crystal.PrimalItemResourcePallet_Crystal,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Wood.PrimalItemResourcePallet_Wood,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_FungalWood.PrimalItemResourcePallet_FungalWood,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_CorruptedWood.PrimalItemResourcePallet_CorruptedWood,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Stone.PrimalItemResourcePallet_Stone,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Obsidian.PrimalItemResourcePallet_Obsidian,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_ElementShard.PrimalItemResourcePallet_ElementShard,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Flint.PrimalItemResourcePallet_Flint,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Charcoal.PrimalItemResourcePallet_Charcoal
```
	
## Added Items:
### Consumables:
#### Team Building Book
<details><summary>------- Info ---------</summary>

When used while riding a creature, adds 25-50% imprint quality and sets the imprinter to the rider.

Cannot be used on creatures fully imprinted to you.
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/TeamBuildingBook/PrimalItemConsumable_TeamBuildingBook.PrimalItemConsumable_TeamBuildingBook'" 100 0 false
```
</details>

#### Self-Improvement Book
<details><summary>------- Info ---------</summary>

When used in a creature's inventory, resets the tamed levels of that creature, allowing them to be respeced by the player.
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/Self-ImprovementBook/PrimalItemConsumable_Self-ImprovementBook.PrimalItemConsumable_Self-ImprovementBook'" 100 0 false
```
</details>

#### Tiered Armor Repair Kits
<details><summary>------- Info ---------</summary>
	
A collection of tools and materials that makes repairing armor a cinch.

Use to instantly repair the first damaged or broken piece of armor in your inventory, with equipped armor having priority.

Has 4 tiers with each tier able to repair more types of armor than the previous tier, along with the previous tier's types.
| Tier | Additional Armor Types |
| --- | --- |
| Crude | Cloth, Hide |
| Basic | Fur, Desert, Ghillie, Chitin |
| Advanced | Flak, Hazard, SCUBA(minus chest), Riot |
| Universal | All |

```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Crude/PrimalItemConsumable_ArmorRepairKitCrude.PrimalItemConsumable_ArmorRepairKitCrude'" 40 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Basic/PrimalItemConsumable_ArmorRepairKitBasic.PrimalItemConsumable_ArmorRepairKitBasic'" 40 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Advanced/PrimalItemConsumable_ArmorRepairKitAdvanced.PrimalItemConsumable_ArmorRepairKitAdvanced'" 40 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Universal/PrimalItemConsumable_ArmorRepairKitUniversal.PrimalItemConsumable_ArmorRepairKitUniversal'" 40 0 false
```
</details>

#### V-Mate
<details><summary>------- Info ---------</summary>
	
Are your dinos feeling lonely because they don't have a mate? Worry not, for we have the technology! The patent-pending V-Mate provides your lonely dinosaurs with their very own virtual mate! Just use it on a dinosaur and watch them recieve all the benefits of a mate, without actually needing one!

Works on all dinosaur genders (or lack thereof), because everyone deserves love!
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/V-Mate/PrimalItemConsumable_V-Mate.PrimalItemConsumable_V-Mate'" 1 0 false
```
</details>

#### Survival Book
<details><summary>------- Info ---------</summary>
	
Every seasoned survivor knows how tedious the first few minutes on a new ARK can be what with having to craft and unlock all the basics every time. The Primal Tool Set addresses this issue by giving you all the tools you need to get going without needing to craft each individually. 

When used gives you: 
- 1 Stone Pick
- 1 Stone Hatchet
- 1 Torch
- 1 Spear
- 1 Bow
- 10 Arrows
- 1 Campfire
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/SurvivalBook/PrimalItemConsumable_SurvivalBook.PrimalItemConsumable_SurvivalBook'" 1 0 false
```
</details>

### Resources
#### Resource Pallets
<details><summary>------- Info ---------</summary>
	
Compact packages of resources which are lighter and more space efficient than their unpackaged contents. 

Crafted in the [Packager](https://github.com/Daniel0Widing/RosesUtilities#packager), and unpacked by using in an inventory. 

Types: 
- Metal Ingot
- Scrap Metal Ingot
- Crystal
- Wood
- Fungal Wood 
- Corrupted Wood
- Stone
- Obsidian
- Element Shards
- Flint
- Charcoal

*May not be compatibile with stack mods. If you only want to change the stack size of items, use the Game.ini settings instead of a stack mod. If you also want the weight reduction from a stack mod, then the Packager and Resource Pallets are redundant and shouldn't be used.*
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_MetalIngot.PrimalItemResourcePallet_MetalIngot'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_ScrapMetalIngot.PrimalItemResourcePallet_ScrapMetalIngot'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Crystal.PrimalItemResourcePallet_Crystal'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Wood.PrimalItemResourcePallet_Wood'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_FungalWood.PrimalItemResourcePallet_FungalWood'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_CorruptedWood.PrimalItemResourcePallet_CorruptedWood'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Stone.PrimalItemResourcePallet_Stone'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Obsidian.PrimalItemResourcePallet_Obsidian'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_ElementShard.PrimalItemResourcePallet_ElementShard'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Flint.PrimalItemResourcePallet_Flint'" 1 0 false
```
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Charcoal.PrimalItemResourcePallet_Charcoal'" 1 0 false
```
</details>

### Structures:
#### Packager
<details><summary>------- Info ---------</summary>

An advanced machine that creates pallets from raw and refined resources. 

Requires electricity from a Generator or Tek Generator and cannot be picked up after being activated. 

Designed to encourage the use of intermediate and mobile bases.
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Structures/Packager/PrimalItemStructure_Packager.PrimalItemStructure_Packager'" 1 0 false
```
</details>

#### Honey Barrel
<details><summary>------- Info ---------</summary>

Did you know that honey never expires if stored properly? Of course not, because you've just been leaving it around in dusty storage boxes and moldy fridges! Put your honey in the specially constructed Honey Barrel and it'll never expire!
	
*This statement has not been approved by the FDA and does not imply food safety.*
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Structures/HoneyBarrel/PrimalItemStructure_HoneyBarrel.PrimalItemStructure_HoneyBarrel'" 1 0 false
```
</details>
