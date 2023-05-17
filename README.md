# ItemStackBuilder

Créer simplement un ItemStack côté serveur grâce à cette class.

__Installation :__

Vous devez simplement copier/coller la classe ou son contenu dans votre projet.

__Usage :__

`ItemStack itemStack = 
new ItemBuilder(Material.WOOL).setAmount(10).setData(15).setName("Nom customisé de l'item").setLore("Ligne 1", "Ligne 2", "Ligne 3").buildItem();`

__Explication :__

► `new ItemBuilder(Material)`: Définit le bloc/item.

► `.setAmount(Integer)`: (*Optionel*) Définit le montant de l'item 
(Dans une limite de 64, par défaut 1).

► `.setData(Integer)`: (*Optionel*) Définit la metadata de l'Item 
(Exemple Laine noir = metadata 15).

► `.setName(String)`: (*Optionel*) Définit un nom custom à votre item.

► `.setLore(String...)`: (*Optionel*) Définit un "lore" à votre item. 
Vous pouvez mettre autant de String que vous souhaitez, 
il suffit de faire une séparation avec une **,**

Exemple : `.setLore("Ligne 1", "Ligne 2")` ou `.setLore("Ligne 1", "Ligne 2", "Ligne 3", "Ligne 4")`

► `.buildItem()` : Obligatoire et à mettre à la fin de votre déclaration, ceci permet de "construire" 
votre item et le retourner pour l'assigner à une **variable ItemStack**.

