Hello, i build a different Illenium-appearance for core_inventory so here is the file to make your clothes as Items :

There are some errors try to adapt the code to yours illenium-appearance, the script works well, on saving after you choosed your clothes from /pedmenu the system gives you same item to good player with the same metadata and same texture.

Basicly you can create all your clothes from illenium and import them in your inventory as cloth items on saving. 



(the system works eaven if you have/not core_clothing) 

If you see any error you can show it here i will try to give assistance for qb only

Thanks !  🎉
 by @Criphyn


MODIFICATIONS TO DO IN CONFIG.LUA FOR BAG AS ITEM CORE_INVENTORY  : 

1 :
 SyncBackpacks = false,               -- If you have a eligible backpack in your inventory it will add it on you as clothes
   EnableBackpackIntoBackpack = false, -- Enable the hability to put backpack into backpack

2 :
['bag'] = {mID = 5, mModel = 0, mTexture = 0, wID = 5, wModel = 0, wTexture = 0},

3:
 ["bag"] = {
    color = "#ff0088",
    takeSound = 'take_clothes',
     putSound = 'put_clothes'
   },

4:
   ["bag"] = {
      slots = 4,
      rows = 2,
      x = "50%",
      y = "20%",
      label = "BAG",
      restrictedTo = {'bag'},
      isHolder = true,
      alwaysSave = true
      },

DONT FORGET TO ADD YOUR CLOTH ITEMS PROVIDED IN THE PACKAGE OF CORE_INVENTORY IN TO : qb-core/shared/items !!!

ACTUAL FILE VERSIONS : 
Illenium-appearance : 5.6.1
core_inventory : 1.4.3
CUTOM SCRIPT MADED
BY CRIPHYN 
