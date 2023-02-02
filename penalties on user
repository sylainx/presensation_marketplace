
# Fichiers à modifier `admin.php`
---

## Fichier admin.php

###### 1- Ajouter les constantes à l'interieur de  `/*TODO:: WORK ON ALERT USER*/`

![[constantes-img.png]]

Codes à ajouter

```php

/* TODO:: WORK ON ALERT USER */
define("ALERT_CONFIG_SUB_MENU", 7747997626554);
define("UTILISATEURS_SIGNALES_ENDPOINT", 58712426554);
include_once "include/features/General_Helpers.php";
/* TODO:: END WORK ON ALERT USER */
```


##### 2- Après l'importation du fichier `setCookieConnect.php` & avant function `verifiaccessfunction(...)`

![[img-verification-alert-config.png]]

Code à ajouter

```php
/* TODO:: WORK ON ALERT USER */
require_once "include/features/alertOnUsers/traitement_adm_alert_config.php";
include_once "include/features/alertOnUsers/verify_availability_colis.php";
/* TODO:: END WORK ON ALERT USER */
```

##### 3- Au bas du menu 
	- après `Query / Replies` 
	- juste avant  la fermeture du tag `</section>` qui termine le menu

![[img-fin du menu.png]]

Code à ajouter

```php
/* TODO:: WORK ON ALERT USER */
if ($infosUser['tous'] == 1) {
echo "<a href='admin.php?admin=6538269&&action=" . UTILISATEURS_SIGNALES_ENDPOINT . "'>
<i class='fa fa-file-excel-o'></i>
Packages not retrieved
<span><i class='fa fa-angle-right'></i>
</span>
</a>";
echo "<a href='admin.php?admin=6538269&&action=" . ALERT_CONFIG_SUB_MENU . "'>
<i class='fa fa-file-excel-o'></i>
Config not retrieved
<span><i class='fa fa-angle-right'></i>
</span>
</a>";
}
/* TODO:: END WORK ON ALERT USER */
```

##### 5- Au meme endroit où l'on avait l'habitude d'inclure nos travaux
	- juste avant
		`} else if (isset($_GET['action']) && $_GET['action'] == 74947493829) {`

![[img-insertion-nos-modules.png]]

Code à ajouter
```php
/* TODO:: WORK ON ALERT USER */
} else if (isset($_GET['action']) && $_GET['action'] == ALERT_CONFIG_SUB_MENU) {
include('include/features/alertOnUsers/alert_config.php');
} else if (isset($_GET['action']) && $_GET['action'] == UTILISATEURS_SIGNALES_ENDPOINT) {
include('include/features/alertOnUsers/list_alert.php');
/* TODO:: END WORK ON ALERT USER */
```

