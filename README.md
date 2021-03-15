<div align="center"><h1>IE modding tips</h1>

<h3>Collection de diverses fonctions et macros WeiDU pour faciliter le code<h3>
</div><br>


<hr>


## Convertir les fichiers BAM d'inventaire au format EE

&#10173; <ins>gw_convert_inventory_bam_to_ee.tpa</ins>

<img align="left" src="images/fr-flag-32.png"> Cette fonction permet de modifier les fichiers BAM d'icônes d'inventaire afin que les jeux améliorés (EE) affichent à la fois leurs grandes et leurs petites icônes. Ces fichiers comportent deux séquences, la première représentant la grande icône et la seconde la petite. Résultat: Les fichiers BAM du répertoire /bam répondant à ces caractéristiques sont modifiés et sauvegardés dans le répertoire override.

<img align="left" src="images/uk-flag-32?png"> This function attempts to modify traditional inventory BAMs so that both the large and small icons are utilized by the EE games. The inventory BAM files must have two sequences, the first containing the "large" inventory icon frame and the second containing the "small" inventory icon frame to be processed. Result: Inventory icon BAMs in the /bam folder that meet these requirements are patched and saved back to the override folder.


<hr>

## Convertir les fichiers BAM d'inventaire au format EE (gw_convert_inventory_bam_to_ee.tpa)

&#10173; <ins>gw_functions.tpa</ins>

><span style="margin-left: 50px;"><a href="#0">FUNCTION GW_WRITE_EE_ITM_DESCRIPTIONS</a></span></br>
><span style="margin-left: 50px;"><a href="#1">FUNCTION GW_UPDATE_ITM_DESCRIPTION_TO_EE</a></span></br>
><span style="margin-left: 50px;"><a href="#2">MACRO GW_ADJUST_TOOLTIP</a></span></br>
><span style="margin-left: 50px;"><a href="#3">MACRO GW_READ_COL_TOOLTIP</a></span></br>
><span style="margin-left: 50px;"><a href="#4">FUNCTION GW_ADD_ITEM_TOOLTIPS</a></span></br>
><span style="margin-left: 50px;"><a href="#5">FUNCTION GW_ALTER_ITEM_ALTER_HEADER_FLAGS</a></span></br>
><span style="margin-left: 50px;"><a href="#6">FUNCTION GW_ITEM_RESTRICT_USABILITY_EE</a></span></br>
><span style="margin-left: 50px;"><a href="#7">FUNCTION GW_FIND_DLG_RESPONSE_STRING</a></span></br>

------------------------

<a name="0" id="0"></a>&#10173; **FUNCTION GW_WRITE_EE_ITM_DESCRIPTIONS**

<img align="left" src="images/fr-flag-32.png"> Cette fonction écrit les descriptions des objets au format Enhanced Edition après les avoir modifiées si nécessaire.

<img align="left" src="images/uk-flag-32?png"> This function writes item descriptions in ITM files according to the game (classical or EE) after updating them to EE format if needed.

## 

<a name="1" id="1"></a>&#10173; **FUNCTION GW_UPDATE_ITM_DESCRIPTION_TO_EE**

<img align="left" src="images/fr-flag-32.png"> Appelée par la fonction `GW_WRITE_EE_ITM_DESCRIPTIONS`, cette fonction ajuste les descriptions des objets au format Enhanced Edition.

<img align="left" src="images/uk-flag-32?png"> Called by `GW_WRITE_EE_ITM_DESCRIPTIONS` function, this function modifies item descriptions to EE format.

## 

<a name="2" id="2"></a>&#10173; **MACRO GW_ADJUST_TOOLTIP**

<img align="left" src="images/fr-flag-32.png"> Cette macro ajoute de nouvelles colonnes au fichier tooltip.2da.

<img align="left" src="images/uk-flag-32?png"> This macro adds new columns in tooltip.2da file if needed.

## 

<a name="3" id="3"></a>&#10173; **MACRO GW_READ_COL_TOOLTIP**

<img align="left" src="images/fr-flag-32.png"> Cette macro compte le nombre de colonnes du fichier tooltip.2da.

<img align="left" src="images/uk-flag-32?png"> This macro reads tooltip.2da file number of columns.

## 

<a name="4" id="4"></a>&#10173; **FUNCTION GW_ADD_ITEM_TOOLTIPS**

<img align="left" src="images/fr-flag-32.png"> Cette fonction ajoute une nouvelle entrée dans le fichier tooltip.2da.

<img align="left" src="images/uk-flag-32?png"> This function adds a new entry in tooltip.2da. file.

## 

<a name="5" id="5"></a>&#10173; **FUNCTION GW_ALTER_ITEM_ALTER_HEADER_FLAGS**

<img align="left" src="images/fr-flag-32.png"> Cette fonction ajoute, supprime ou modifie les flags des headers des objets spécifiques à EE ou à ToBEx.

<img align="left" src="images/uk-flag-32?png"> This function adds, emoves or alters items headers EE and ToBEx specific flags.

## 

<a name="6" id="6"></a>&#10173; **FUNCTION GW_ITEM_RESTRICT_USABILITY_EE**

<img align="left" src="images/fr-flag-32.png"> Cette fonction permet de modifier les flags d'utilisation ou de restriction des objets (jeux Enhanced Edition).

<img align="left" src="images/uk-flag-32?png"> This function defines special item usability restrictions (EE games).

## 

<a name="7" id="7"></a>&#10173; **FUNCTION GW_FIND_DLG_RESPONSE_STRING**

<img align="left" src="images/fr-flag-32.png"> Cette fonction recherche dans un dialogue un state et une transition correspondant à un strref.

<img align="left" src="images/uk-flag-32?png"> This function looks for state and transition numbers matching a strref in a dialog.
