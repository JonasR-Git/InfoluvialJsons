# InfoluvialJsons

Any help is appreciated, but here are a few guidelines to make our job easier:

For the Affinity and Class Jsons:
Name and Image: already correct and shouldn't be changed!
MultiplierBonus, Innate and Synergy. For writing in a new line you need to type \n. And for a empty line you need to write \n\n. Every space writen after \n is also displayed, so avoid this. <br />
As an example: <br />
```[2] 200 Area Energy Damage \n[3] 300 Area Energy Damage \n[4] 400 Area Energy Damage```:
  
  [2] 200 Area Energy Damage <br />
  [3] 300 Area Energy Damage <br />
  [4] 400 Area Energy Damage <br />
  
  and 
  
  ```Water Illuvials gain 3 Energy Regen last for 5 seconds and refresh every 15 seconds \n\nFire Illuvials gain 20 Energy Damage ...```:
  
  
  Water Illuvials gain 3 Energy Regen last for 5 seconds and refresh every 15 seconds
  
  Fire Illuvials gain 20 Energy Damage ...
  
  ![image](https://user-images.githubusercontent.com/44968998/178755235-334a9790-f339-4cdb-81e7-7334c1335720.png)
  
  
  It would save us a lot of time if you could mentioned it and try to fill the json right. If we see any problem, we will change it then. 
  
  
**Now for the big thing:**
  
To fill in the json, you have to write copy the whole array for a single Illuvial and just put it under the last one and seperate them with a commy, like in the example file. <br />
Try to fill in everything you could. <br />
Everything should be written in lowe case, expect the Describtion. The strings should be still strings ("") and the numbers should be numbers like in the example. <br />
Only fill in what we know, the rest should be empty for the string or a "null" for the numbers. 

    {
        "Id": 0,
        "Name": "Atlas",
        "Tier" : 1,
        "Stage":  1,
        "SizeUnits": 5,
        "MasteryPoints": 30,
        "Region": ["", ""],
        "Image:": "https://ik.imagekit.io/2zcxm4xvo/tr:w-186,h-186/Gallery/Website/IlluvialCards/Atlas.png"",
        "Line": {
            "Name":"Axolotl",
            "LinkTier1": "",
            "ImageTier1": "https://ik.imagekit.io/2zcxm4xvo/tr:w-186,h-186/Gallery/Website/IlluvialCards/Atlas.png",
            "LinkToPageTier1":"",
            "LinkTier2": "",
            "ImageTier2": "https://ik.imagekit.io/2zcxm4xvo/tr:w-186,h-186/Gallery/Website/IlluvialCards/Axon.png",
            "LinkToPageTier2":"",
            "linkTier3": "",
            "ImageTier3": "https://ik.imagekit.io/2zcxm4xvo/tr:w-186,h-186/Gallery/Website/IlluvialCards/Axodon.png",
            "LinkToPageTier3":""
        },
       "CombatAffinity": {
            "Main": "water",
            "Affinities": ["water", "", ""]
        },
        "CombatClass": {
            "Main": "bulwark",
            "Classes": ["bulwark", "", ""]
        },
        "Stats": {
            "MaxHealth": 900,
            "StartingEnergy": 0,
            "EnergyCost": null,
            "PhysicalResist": 30,
            "EnergyResist": 40,
            "Grit": null,
            "Resolve": null,
            "Precision": 25,
            "AttackPhysicalDamage": 25,
            "AttackEnergyDamage": null,
            "AttackPureDamage": null,
            "AttackSpeed": 120,
            "Savagery": null,
            "OmegaPower": 100,
            "AttackRange": 3,
            "HealthRegeneration": null,
            "EnergyRegeneration": null
        },
        "BasicAttack":
        {
            "Name": "",
            "Targeting": "target",
            "Effects": {
                "Describtion": "Atlas attacks his current target",
                "DamageType": "physical",
                "Amount": "25"
            }
        },
        "Omega": {
            "Name": "",
            "Targeting": "target",
            "Effects": {
                "Describtion": " Atlas generates a (20% Max Health + 100*OP) shield that last for up to 5 seconds. While shielded, attacks, deal (40*OP) additional energy damage.",
                "DamageType": "energy damage",
                "Amount": "40 * OP"
            }
        },
        "Hyper": {
            "Name": "",
            "Targeting": "",
            "Effects": {
                "Describtion": "",
                "Amount": ""
            }
        }
    }


The options for targeting should be the following: nearest, target, farthest, lowest Health, highest Health. <br />
If I miss something please ping me @Jonas. <br />
For the Images, just take the exact same link and just replace the name from the illuvial with the right one. Like made with Atlas, Axon and Axodon. <br />
Illuvials such as Mah'Mut should be written as MahMut and spaces should be replaced with a - so Komodo Dragon -> Komodo-Dragon.png.
