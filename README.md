# Rose's Utilities
Adds a collection of useful utilities that enhance both vanilla and modded ARK experiences.

## Installing the Mod
Log into Steam, go to [Rose's Utilities](https://steamcommunity.com/sharedfiles/filedetails/?id=2939004410), and subscribe to the mod. Then launch ARK and the mod should automatically download.

## GameUserSettings.ini Configuration
First close your game/server. Then in the GameUserSettings.ini file, find the [RosesUtilities] section and change the settings you want changed and save the file. When you restart your game/server, the new settings should be applied.

The following section should add itself to the bottom of your GameUserSettings.ini file, but if it doesn't, copy it into the bottom of the file.

```
[RosesUtilities]
BasePalletStackSize=8
PalletBaseWeight_MetalIngotPallet=100.000000
PalletBaseWeight_ScrapMetalIngotPallet=100.000000
PalletBaseWeight_CrystalPallet=50.000000
PalletBaseWeight_WoodPallet=25.000000
PalletBaseWeight_FungalWoodPallet=25.000000
PalletBaseWeight_CorruptedWoodPallet=25.000000
PalletBaseWeight_StonePallet=25.000000
PalletBaseWeight_ObsidianPallet=50.000000
PalletBaseWeight_ElementShardPallet=25.000000
PalletBaseWeight_CharcoalPallet=12.500000
PalletBaseWeight_FlintPallet=2.500000
```

## S+ Pull Resource Config
Add the following to the end of the **PullResourceAdditions=** line in your **GameUserSettings.ini** file under the **\[StructuresPlus\]** section to enable S+ resource pulling for Rose's Utilities items. If the config line already has items in it from other mods, seperate those items from the Rose's Utilities items with a comma.

```
/Game/Mods/RosesUtilities/Items/Consumables/TeamBuildingBook/PrimalItemConsumable_TeamBuildingBook.PrimalItemConsumable_TeamBuildingBook,/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Crude/PrimalItemConsumable_ArmorRepairKitCrude.PrimalItemConsumable_ArmorRepairKitCrude,/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Basic/PrimalItemConsumable_ArmorRepairKitBasic.PrimalItemConsumable_ArmorRepairKitBasic,/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Advanced/PrimalItemConsumable_ArmorRepairKitAdvanced.PrimalItemConsumable_ArmorRepairKitAdvanced,/Game/Mods/RosesUtilities/Items/Consumables/ArmorRepairKit/Universal/PrimalItemConsumable_ArmorRepairKitUniversal.PrimalItemConsumable_ArmorRepairKitUniversal,/Game/Mods/RosesUtilities/Items/Consumables/V-Mate/PrimalItemConsumable_V-Mate.PrimalItemConsumable_V-Mate,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_MetalIngot.PrimalItemResourcePallet_MetalIngot,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_ScrapMetalIngot.PrimalItemResourcePallet_ScrapMetalIngot,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Crystal.PrimalItemResourcePallet_Crystal,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Wood.PrimalItemResourcePallet_Wood,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_FungalWood.PrimalItemResourcePallet_FungalWood,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_CorruptedWood.PrimalItemResourcePallet_CorruptedWood,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Stone.PrimalItemResourcePallet_Stone,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Obsidian.PrimalItemResourcePallet_Obsidian,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_ElementShard.PrimalItemResourcePallet_ElementShard,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Flint.PrimalItemResourcePallet_Flint,/Game/Mods/RosesUtilities/Items/Resources/Pallets/PrimalItemResourcePallet_Charcoal.PrimalItemResourcePallet_Charcoal
```
	
## Added Items:
### Consumables:
#### Team Building Book
<details><summary>------- Info ---------</summary>

When used while riding a dinosaur, adds 25-50% imprint quality and sets the imprinter to the rider.

Cannot be used on dinosaurs fully imprinted to you.
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Items/Consumables/TeamBuildingBook/PrimalItemConsumable_TeamBuildingBook.PrimalItemConsumable_TeamBuildingBook'" 40 0 false
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

Requires electricity from a Generator or Tek Generator. 

Designed to facilitate the use of intermediate and mobile bases.
```
cheat giveitem "Blueprint'/Game/Mods/RosesUtilities/Structures/Packager/PrimalItemStructure_Packager.PrimalItemStructure_Packager'" 1 0 false
```
</details>
