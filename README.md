# Merchant-Villager-standalone-Inventory-API


Hey Guys The Owner here,


This API adds a Villager like Inventory Type that can be Accessed and Displayed in any Method and Event, there's no need for a Custom or modified Villager anymore.
This API got tested on Spigot 1.11.2 and should work on any 1.11 Version. Tests and modifications need to be done for Versions below that and will only happen on Request.
If you like our work feel free to buy us a coffe the only thing that can still keep us awake 0.0: <br>
[![paypal](https://www.paypalobjects.com/en_US/i/btn/btn_donateCC_LG.gif)](https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=JFHPNTUJMDD8G)




###Instructions:
The added Inventory Type is called Merchant and can be created easily like this:

```Java
Merchant testMerchant = new Merchant();
```


But The Inventory needs something to Display of course. This is how you can create an Offer. Make sure that empty Fields have to be filled with a ItemStack with the Meterial.AIR, otherwise you will get an error and the Offer will not be Displayed inside the Inventory.

```Java
MerchantOffer testOffer = new MerchantOffer(new ItemStack(Material.BED, 1), new ItemStack(Material.AIR, 1), new ItemStack(Material.ANVIL, 1));
```				


To add an Offer to the MerchantInventory just do:

```Java
testMerchant.addOffer(testOffer);
```


To open the Inventory for a Player you have to first set the Customer and than open the Menue manually:

```Java
testMerchant.setCustomer(Player);
testMerchant.openTrading(Player);
```




Thanks for Choosing our API :)

With Friendly Greetings,
The Owner
