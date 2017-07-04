---
layout: default
---

# WMT Mission Framework


## Les modules

| **Module**                | Description                            	|
|-------------------------	|----------------------------------------	|
| **Main**                	| Paramètres de base de la mission       	|
| **Time**                	| Réglages des contraintes temporelles   	|
| **Start Position**      	| Choix de la position de départ         	|
| **Task: Point**         	| Réglage de zones de défense/capture    	|
| **Task: Capture Point** 	| Capturer un certain nombre de zones    	|
| **Task: Arrived**       	| Livrer un objet dans une zone          	|
| **Task: Destroy**       	| Destruction d'objet                    	|
| **Task: VIP**           	| Destruction de VIP(s) dans une zone    	|
| **Task: Compose**       	| Permet d'assigner des tâches multiples 	|


### Main module

<table border="0">

<thead>

<tr>

<th scope="col" align="center" width="35%">Paramètre</th>

<th scope="col" align="center" width="65%">Description</th>

</tr>

</thead>

<tbody>

<tr>

<td valign="top">:black_small_square: `View distance`</td>

<td valign="top">Distance de vue maximale que le joueur peut définir dans ses paramètres.  

**Valeur possible:**  
*   **NUMBER** - de 100 à 12000</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: ` js Heavy losses ratio `</td>

<td valign="top">Indique le seuil du nombre de joueurs restants avant que la missions s'arrête. La mission se termine lorsque le nombre joueurs tombe en dessous du pourcentage déterminé.  

**Valeur possible:**  
*   **NUMBER** - de 0 à 1  
(Exemple : avec 0,1 * nombre de joueurs = 0,1 * 60 = 6 : en dessous de 3 joueurs la missions s'arrête  
:warning: Si vous spécifiez 0, la fonction est désactivée. Si vous spécifiez une valeur très faible de 0,001, la mission prendra fin lorsque tous les joueurs seront tués.  
:warning: le nombre initial de joueurs est considéré après la fin du warm-up, ou 60 secondes après le début de la mission.  
:warning: le pop-up de fin est généré automatiquement  
:warning: les victimes civiles ne sont pas comptées  
:warning: **Non pris en charge !** <strike>`wmt_hl_sidelimits = [0,0,0];`</strike>  
:warning: **Non pris en charge !** <strike>`wmt_hl_ratio = [0.1,0.2,0.1];`</strike></td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Thermal image`</td>

<td valign="top">Permet de configurer les cameras thermiques.  

**Valeur possible:**  
*   Désactivé dans les véhicules*   Désactivé*   Activé  
:warning: Cela désactive également certaines visées infrarouges.  
</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Extended briefing`</td>

<td valign="top">Ajoute les informations suivante au briefing:  
*   Equipement*   Equipement ennemi*   Groupes*   Mon équipe*   Paramètres de la mission  
**Valeur possible:**  
*   Activé*   Désactivé  
:warning: affiche la position de départ des véhicules et groupes</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Nametags`</td>

<td valign="top">Affiche le nom du joueur au centre de l'écran.  

**Valeur possible:**  
*   Activé*   Désactivé  
:warning: Pas compatible avec ACE Nametags (je conseille donc de le désactiver)</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Identify bodies`</td>

<td valign="top">Affiche le nom des morts via l'`action menu`. **Désactivation recommandée**.  

**Valeur possible:**  
*   Activé*   Désactivé</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Show frequencies`</td>

<td valign="top">Ajoute un onglet affichant les fréquences radio dans le briefing.  

**Valeur possible:**  
*   Activé*   Désactivé</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `AI`</td>

<td valign="top">Permet de désactiver ou d'activer les IA.  

**Valeur possible:**  
*   Activé*   Désactivé</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Show statistics`</td>

<td valign="top">Affiche les statistiques après la mort en cliquant sur <kbd>End</kbd>.  

**Valeur possible:**  
*   Activé*   Désactivé  
:warning: les statistiques ne sont pas toujours correctes (explosion, bleedout, ...)</td>

</tr>

</tbody>

</table>

### Fonctionnalités incluses

<table border="0">

<thead>

<tr>

<th scope="col" align="center" width="35%">Fonction</th>

<th scope="col" align="center" width="65%">Description</th>

</tr>

</thead>

<tbody>

<tr>

<td valign="top">:black_small_square: `Menu du jeu`</td>

<td valign="top">Ajoute le menu WMT, accessible avec la touche <kbd>Home</kbd>.  

**Menu:**  
*   Réglage du viewdistance*   Panneau d'administration*   Rétroaction à l'administrateur ? (обратная связь с администратором)</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Marqueurs side`</td>

<td valign="top">Il offre la possibilité de définir des marqueurs à afficher uniquement pour une camp en particulier, par le biais de l'ajout d'un préfixe au nom:  
*   `wmt_west_`*   `wmt_east_`*   `wmt_res_`*   `wmt_civ_`  
:warning: **civilian** Ne sont pas considérés comme des alliés par aucun camp.  
:warning: sensible à la casse  

**Exemple:**  
`wmt_west_marker`</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Marqueurs temporaires (retirés après le briefing)`</td>

<td valign="top">Les marqueurs dont le nom commence par `wmt_` et se termine par `_del sont automatiquement rendu invisible à la fin du briefing.  
:warning: sensible à la casse  

**Exemple:** 
`wmt_marker_del`</td>

</tr>

</tbody>

<tbody><tr>
<td valign="top">:black_small_square: `Rating control`</td>
<td valign="top">Does not allow to set rating bellow 0 and change side to **enemy**.</td>
</tr></tbody>

</table>

<table border="0"><caption>

# Module Time

</caption>

<thead>

<tr>

<th scope="col" align="center" width="35%">Paramètre</th>

<th scope="col" align="center" width="65%">Description</th>

</tr>

</thead>

<tbody>

<tr>

<td valign="top">:black_small_square: `Mission time`</td>

<td valign="top">La mission se termine à la fin du temps.  

**Valeur possible:**  
* **NUMBER** - temps en minutes  
:warning: Le timer commence à la fin du briefing  
:warning: Le timer est en temps réel (pas en temps de jeu)</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Winner side`</td>

<td valign="top">Indique le temps qui gagne à la fin du temps.  

**Valeur possible:**  
*   personne*   BLUFOR*   OPFOR*   INDEP*   CIV</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Message`</td>

<td valign="top">Le message apparaît à la fin du temps quand la mission est terminée.  

**Valeur possible:**  
*   **STRING** - Message texte</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Prepare time`</td>

<td valign="top">Indique le temps alloué au briefing.  

**Valeur possible:**  
*   **NUMBER** - temps en minutes  
:warning: Durant le briefing, les joueurs ne peuvent pas tirer, quitter la zone ou démarrer les véhicules</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Size of start zone`</td>

<td valign="top">Définit la taille de la zone de départ.  

**Valeur possible:**  
*   **NUMBER** - distance en mètres</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Remove bots`</td>

<td valign="top">Temps à partir duquel la mission supprime les emplacements vides.  

**Valeur possible:**  
*   **NUMBER** - Temps en minutes  
:warning: Si activé, les bots seront supprimés après le briefing  
:warning: If you take slot and relog to other slot from menu, bot will be set as playable and won't be deleted  
:warning: squad leader can deny bot deletion</td>

</tr>

</tbody>

</table>

### Task: Point

<table border="0">

<thead>

<tr>

<th scope="col" align="center" width="35%">Параметр</th>

<th scope="col" align="center" width="65%">Описание</th>

</tr>

</thead>

<tbody>

<tr>

<td valign="top">:black_small_square: `Маркер`</td>

<td valign="top">Маркер определяет границы зоны  

**Возможные значение:**  
*   Zone1*   Zone2_a, Zone2_b</td>

</tr>

<tr>

<td valign="top">:black_small_square: `Сторона по-умолчанию`</td>

<td valign="top">Определяет принадлежность зоны одной из сторон при старе миссии  

**Возможные значение:**  
*   Никто*   Запад*   Восток*   Независимые*   Гражданские</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Сообщение`</td>

<td valign="top">Сообщение при захвате зоны.  

:warning: сообщение видно всем, включая спектатор  
:warning: сообщение не появляется, если оставить поле пустым  
</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Кол-во для защиты`</td>

<td valign="top">Задает минимальное число обороняющих  

:warning: если число больше или ровно заданному числу, то захват зоны не возможен  
</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Кол-во для захвата`</td>

<td valign="top">Задает минимальное число атакующих  

:warning: если число больше или ровно заданному числу, то при условии нахождение в зоне не достаточного число обороняющихся происходит захват зоны  
</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Блокировка`</td>

<td valign="top">Блокирует зоны после одного захвата(потери) зоны  

**Возможные значение:**  
*   Включено*   Выключено</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Легкий захват`</td>

<td valign="top">Возможность захвата зоны любым количеством атакующих при условии отсутвия в зоне обороняющих  

**Возможные значение:**  
*   Включено*   Выключено</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Минимальная высоты`</td>

<td valign="top">Задает нижнюю границу по высоте отсносительно повехрности.  

:warning: дает возможность делать зоны на воде или на верхних этажах зданий :warning: на земле высота считается относительно повехности земли :warning: на воде высота считается относительно повехности воды</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Максимальная высоты`</td>

<td valign="top">Задает верхнюю границу по высоте отсносительно повехрности.  

:warning: делает невозможным захват зоны парашутистами или воздушной техникой :warning: на земле высота считается относительно повехности земли :warning: на воде высота считается относительно повехности воды</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Автоматическая потеря`</td>

<td valign="top">При отсутсвии в зоне обороняющих, зона автоматически становится ничейной  

:warning: если включена блокировка зоны, то после потери зоны захватить зону будет невозможно</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Таймер`</td>

<td valign="top">Задает промежуток времени при захвате или потери зоны  

:warning: таймер распространяется на все случаи смены владельца зоны  
</td>

</tr>

</tbody>

<tbody>

<tr>

<td valign="top">:black_small_square: `Условие`</td>

<td valign="top">Дополнительное условие которое должны быть выполнено, для захвата или потери зоны  

:warning: если вы не знаете точно, что делаете, не трогайте  
:warning: проверяейте правильность условие перед использоваем  
</td>

</tr>

</tbody>

</table>

##Fonctions:
* [WMT_fnc_BoundingBoxMarker](#wmt_fnc_boundingboxmarker)
* [WMT_fnc_BriefingMap](#wmt_fnc_briefingmap)
* [WMT_fnc_EndMission](#wmt_fnc_endmission)
* [WMT_fnc_IsTheUnitInsideMarker](#wmt_fnc_istheunitinsidemarker)
* [WMT_fnc_ProgressBar](#wmt_fnc_progressbar)
* [WMT_fnc_ShowTaskNotification](#wmt_fnc_showtasknotification)
* [WMT_fnc_ZoneCaptured](#wmt_fnc_zonecaptured)

***

###WMT_fnc_BoundingBoxMarker
##### Параметры:
* 0 - OBJECT
* 1 - COLOR: цвет маркера
* 2 - SCALAR: прозрачность маркера

##### Описание:
Добавляет маркер на объект.
Функция является локальной.

##### Пример:
`[this] call WMT_fnc_BoundingBoxMarker`

`[this,"ColorRed"] call WMT_fnc_BoundingBoxMarker`

`[this,"ColorGrey",0.5] call WMT_fnc_BoundingBoxMarker`

***

###WMT_fnc_BriefingMap
##### Параметры: 
-
##### Описание:
* Добавляет карту на время брифинга тем, у кого ее нету
* Дает возможность использовать карту близкого союзника или карту из техники с GPS 
* Функция должна вызываться в `init.sqf`

##### Пример:
`[] call WMT_fnc_BriefingMap;`

***
###WMT_fnc_EndMission
##### Параметры: 
* 0 - SIDE: выигрывавшая сторона 
* 1 - STRING: сообщение

##### Описание:
Функция для завершения миссии с выводом сообщения. 
Функция является локальной.

##### Пример:
`[east, "Восток победил"] call WMT_fnc_EndMission;`

***

###WMT_fnc_IsTheUnitInsideMarker
##### Параметры: 
* 0 - OBJECT
* 1 - MARKER

##### Описание:
Проверяет нахождения объекта в маркере.
Возвращает BOOL.

##### Пример: 
`[car,"zone_1"] call WMT_fnc_IsTheUnitInsideMarker`

***

###WMT_fnc_ProgressBar
##### Параметры: 
* 0 - BOOL: показать/скрыть бар 
* 0 - SCALAR: установить положение бара

##### Описание:
Показывает прогресс выполнения какого-либо действия.

Важно: при использовании функции необходима проверка значение `WMT_mutexAction `и вызывать функцию, только если значение равно `false`.

##### Пример: 
1. `for "_i" from 0 to 100 do {`
2. `   if(!WMT_mutexAction) then {`
3. `      [_i/100] call WMT_fnc_ProgressBar;`
4. `   };`
5. `   sleep 0.1;`
6. `};`
7. `[false] call` WMT_fnc_ProgressBar;`

***

###WMT_fnc_ShowTaskNotification
##### Параметры:
* 0 - SIDE: сторона для которой задание считается выполненным 
* 1 - STRING: сообщение

##### Описание:
Вывод сообщение.

##### Пример: 
`[east,"Объект уничтожен"] call WMT_fnc_ShowTaskNotification`

`["Объект уничтожен"] call WMT_fnc_ShowTaskNotification`

***

###WMT_fnc_ZoneCaptured
##### Параметры: 
* 0 - SIDE: сторона захватившая зону
* 1 - STRING: сообщение о захвате во всплывающем окне
* 2 - ARRAY: список маркеров обозначающих зону

##### Описание:
Выводит сообщение о захвате зоны и изменяет цвета маркера на карте.

##### Пример: 
`[east, "CSAT захватил зону",["Zone_1"]] call WMT_fnc_EndMission;`











[back](./)
