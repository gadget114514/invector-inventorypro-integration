# invector-inventorypro-integration (+ UMA2)
Invector and Inventory Pro integration

https://invector.proboards.com/thread/692/inventory-pro-2-5

https://www.dropbox.com/s/5pmp1sd9cug6o55/Invector_InventoryPro_2.5.unitypackage?dl=0

It causes errors for recent invector (3).
This unity package is modified to fix them.


add vThirdPersonControllerPlayer to vThirdPersonController gameobject.



The following images shows the inventory pro and invector integration example.

![(1)](https://user-images.githubusercontent.com/34733747/119249985-efc59c00-bbd7-11eb-9ce2-958e07037e6b.png)

![(2)](https://user-images.githubusercontent.com/34733747/119249993-f9e79a80-bbd7-11eb-8180-00e0eedeaf3b.png)

0. maybe the first you have to do is overwriting inventory pro by github cloning.
1. Create third person controller character.
2. Add vThirdPersonControllerPlayer
3. Add Inventory Player
4. Setup Inventory Pro Database and UIs. (add _Manager gameobject and setup UI etc)
5. Set UIs to Inventory Player and Handler to Inventory Player also.
6. Done!




# Alternative inventory pro + UMA2 integration

it is UMA2 recipe based integration; it looks easier than implemented in inventory-pro integration.

1. extract InventoryProUMA2.zip
2. it extends EquippableInventoryItem; xetype and xename; they are used for "slot" and "name" each.
3. Create EquippableInventoryItem with xetype and xename, if it is UMA2 item.
4. use UMA2CharacterEquipmentHandler instead of CharacterEquipmentHandler;  (create asset and use it in InventoryPlayer component)

Maybe this implementation impacts minimum to existed sources.
wardrope only.


![(3)](https://user-images.githubusercontent.com/34733747/120885841-f74c6280-c625-11eb-8d35-b2fcb80fc7d0.png)
