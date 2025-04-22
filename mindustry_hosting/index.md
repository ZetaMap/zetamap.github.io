[<-- Home Page](/) <br>
![Visitor Badge](https://visitor-badge.laobi.icu/badge?page_id=ZetaMap.zetamap-github-io.mindustry_hosting) <br>
Dernière mise à jour : **22/04/2025**

# Comment jouer avec des amis ? - Tutoriel
Pour pouvoir jouer avec des amis, je vous propose un tuto où vous pourrez choisir entre plusieurs logiciels. Ce que je propose est valable pour mobile et PC.

⚠️ Lisez bien tout le tutoriel pour bien tout comprendre. ⚠️


## SOMMAIRE
* [PRÉSENTATION DES LOGICIELS](#présentation-des-logiciels)
  * [CLaJ](#claj)
  * [MiniUPNPC](#miniupnpc)
  * [Hamachi](#hamachi)
  * [Termux](#termux)
* [TUTOS](#tutos)
  * [Solution CLaJ](#solution-claj)
  * [Pour PC](#pour-pc)
    * [Solution MiniUPNPC](#solution-miniupnpc)
    * [Solution Hamachi](#solution-hamachi)
  * [Pour Mobile](#pour-mobile)
* [CONTACT](#contact)
  * [Remercîments](#remercîments)


## PRÉSENTATION DES LOGICIELS
### CLaJ
[CLaJ](https://github.com/xpdustry/claj) (Copy Link and Join) est un système utilisant un serveur distant pour créer des salons, partager le lien à vos amis, et rejoindre votre partie de manière transparente et anonyme. <br>
C'est un système similaire à Hamachi, mais intégré à Mindustry pour une utilisation pour simple et sans compte à créer.

C'est l'outil parfait pour les personnes ne souhaitant pas s'attarder sur la création d'un serveur ou l'exécution d'étapes fastidieuses.


### MiniUPNPC
[MiniUPNPC](http://miniupnp.free.fr/) est open source et complètement modulable selon vos envies, il communique avec la box pour rediriger les connexions d'un port sélectionné au PC du demandeur, cette pratique s'appelle le Port Forwarding.

C'est un logiciel très petit, très simple d'utilisation, rapide, efficace, et il n'y a que l'hébergeur du serveur qui doit être sur PC : les autres peuvent être sur la plateforme de leur choix. <br>
De plus, il ne collecte aucune donnée personnelle, vous en avez un total contrôle, et il n'y a pas de limite de place dans le réseau.

Cependant, son plus gros défaut est d'être peu sécurisé, car cela utilise votre IP publique; vous serez donc vulnérable aux attaques. <br>
Il est donc important de ne pas donner son IP à n'importe qui. <br>
En outre, si vous n'êtes pas sûr de ce que vous faites ou que vous vivez dans un quartier mal vu, je vous déconseille ce logiciel.


### Hamachi
[Hamachi](https://www.vpn.net/) est un service qui, en principe, fait la même chose que [MiniUPNPC](#miniupnpc), mais de manière plus sophistiquée et sécurisée. Sauf qu'il faut avoir un compte Hamachi. =/

Il est simple d'utilisation, avec une belle interface graphique au lieu de commandes, et est très efficace. <br>
De plus, il est sécurisé, donne la possibilité de sauvegarder plusieurs réseaux à la fois, et de définir un mot de passe sur un réseau pour en contrôler les accès.

Cependant, pour pouvoir l'utiliser il faut avoir créé un compte Hamachi, qui est certes gratuit, mais dont on ne sait pas où seront stockées les données de connexions et de trafic. <br>
Dans leurs [conditions générales d'utilisation](https://www.goto.com/fr/company/legal), ils stipulent bien que des données personnelles seront collectées, mais ne précisent pas quelles données. <br>
Par ailleurs, il faut que l'hébergeur, ainsi que toutes les personnes qui veulent s'y connecter, soient sur Windows, car le logiciel n'est disponible que sur cette plateforme. <br>
Les places disponibles dans un réseau sont limitées à 5 : pour palier à cela, la société propose des formules payantes et très chères. <br>
Enfin, lors de son installation, il ajoute un service au démarrage de l'ordinateur, ce qui est un peut intrusif.


### Termux
[Termux](https://termux.com/) est un logiciel libre et open source disponible à l'installation sur [Github](https://github.com/termux/termux-app), [F-droid](https://f-droid.org/en/packages/com.termux/), et sur [Play Store](https://play.google.com/store/apps/details?id=com.termux). <br>
C'est tout simplement le meilleur terminal de commande Linux pour mobile au monde. Il donne la possibilité d'installer des applis, contrôler son téléphone, installer les émulateurs Python ou Java, et bien d'autres fonctionnalités.  <br>
L'application ne transmet aucune donnée personnelle à des sociétés tierces, si ce n'est les rapports de bugs aux développeurs avec votre consentement, et dispose de quelques modules installables pour personnaliser son terminal.

**Note:** Pour mobile, il sera nécessaire d'installer cette application pour pouvoir utiliser [MiniUPNPC](#miniupnpc). <br>
Vous pouvez directement l'installer en [cliquant ici](https://f-droid.org/repo/com.termux_118.apk) pour la version *0.118*, et pour d'autres versions [ici](https://github.com/termux/termux-app/releases).


## TUTOS
### Solution CLaJ
Cette solution est dédiée à Mindustry, utilisant le mod CLaJ, disponible dans le navigateur de mods. <br>
**Note:** le mod doit être installé pour tout le monde, sinon les autres ne pourront pas rejoindre la partie.

Une fois le mod installé, vous devez d'abord héberger un serveur. Pour cela, lancez une carte ou votre campagne, puis dans le menu pause, faites ``Héberger une partie multijoueur`` puis ``Héberger``. <br>
Maintenant vous devez créer un salon, pour cela dans le menu pause, cliquez sur ``Gérer le salon CLaJ`` puis sélectionnez un serveur (ou ajoutez le votre), cliqez sur ``Cléer le salon``, attendez un peu et cliquez sur ``Copier le lien``. <br>
Le lien du salon a normalement été copié dans votre presse-papier, il vous reste plus qu'à le coller et l'envoyer à vos amis.

Pour rejoindre un salon, rien de plus simple, copiez le lien que votre ami vous a envoyé, puis allez dans ``Jouer`` **>** ``Rejoindre une partie`` **>** ``Rejoindre via CLaJ``, collez le lien, puis cliquez sur ``OK``. <br>
Normalement, si tout s'est bien passé, vous pouvez jouer de manière transparente avec vos amis.


### Pour PC
#### Solution MiniUPNPC
Tout d'abord, il faut télécharger le logiciel qui se [trouve ici](http://miniupnp.free.fr/files/upnpc-exe-win32-20220515.zip), ensuite dézippez le (je conseille de le faire dans le dossier de votre jeu, pour ne pas le perdre).

Maintenant il faut ouvrir un terminal de commande pour effectuer la suite du tuto, pour cela, vous pouvez faire : TOUCHE WINDOWS + R, et taper ``"cmd"`` ou rechercher ``"cmd"`` dans la barre de recherche Windows. <br>
Ensuite il faut se déplacer à l'endroit où le logiciel a été dézippé, pour ce faire, tapez ``"cd <emplacement du dossier>"`` dans le terminal.

Pour ouvrir le port de la box, exécutez la commande ``"upnpc-static.exe -r 6567 TCP 6567 UDP"``. Attendez un moment puis regardez la ligne **ExternalIPAddress**, c'est l'adresse IP publique de la box qu'il faut donner aux autres. <br>
Lorsque vous avez fini de jouer avec vos amis, tapez la commande ``"upnpc-static.exe -d 6567 TCP 6567 UDP"``, puis regardez la dernière ligne. Si elle affiche **UPNP_DeletePortMapping() returned : 0**, c'est que le port a bien été refermé.

**Info :** Pour vérifier que le port a bien été ouvert ou fermé, vous pouvez utiliser [cet outil](https://www.yougetsignal.com/tools/open-ports/), en indiquant le port *6567* dans le cadre **Port Number**. <br>
Lors du test d'ouverture du port, assurez-vous qu'au préalablement le serveur a été hébergé : si vous utilisez la version serveur de Mindustry, tapez la commande ``host`` pour l'héberger, sinon allez dans le menu pause et cliquez sur le bouton ``Héberger un serveur`` puis ``Héberger``.

**Note :** Lors de la vérification de l'ouverture du port, le site peut des fois indiquer le port comme fermé alors qu'il est bien ouvert.


#### Solution Hamachi
Premièrement, il faut installer l'installateur du client [disponible ici](https://www.vpn.net/) : suivez les étapes d'installation puis reprenez le tutoriel... <br>
Une fois que le logiciel est installé et lancé, suivez les étapes pour créer un compte Hamachi puis reprenez le tutoriel.

Une fois fait, cliquez sur ``Réseau`` en haut au milieu de la fenêtre, puis ``Créer un réseau...``. Il vous sera ensuite demandé un *ID* de réseau ainsi qu'un mot de passe et une confirmation de ce-dernier. <br>
L'ID de réseau sera son nom qui devra être communiqué aux autres personnes, et vous pouvez ne pas mettre un mot de passe si vous le souhaitez.

Pour pouvoir se connecter à un réseau, c'est très simple : il vous suffira de cliquer sur ``Réseau`` puis ``Rejoindre un réseau...``. 
Une page de connexion s'affichera, vous demandant l'ID du réseau (son nom) ainsi que son mot de passe (ou rien s'il n'y en a pas). <br>
Et normalement, dans votre jeu, le serveur devrait apparaitre dans la catégorie ``Serveurs Locaux``, dans le menu ``Jouer`` **>** ``Rejoindre une partie``.


### Pour Mobile
Avant de commencer, il faut avoir téléchargé l'application Termux (les étapes sont [ici](#termux)) et l'avoir lancé. <br>
Puis avoir téléchargé le *package* MiniUPNPNC. Pour cela, utilisez la commande ``"pkg install miniupnpc"`` et attendez que l'installation se termine en regardant si la dernière ligne ressemble à ``~ $``. <br>

Les étapes restantes ne sont pas bien différentes de la version PC : seule la syntaxe change. <br>
Pour ouvrir le port, tapez la commande ``"upnpc -r 6567 TCP 6567 UDP"`` et regardez la ligne **ExternalIPAddress** : c'est l'adresse IP publique de la box qu'il faut donner aux autres. <br>
Pour refermer le port, tapez la commande ``"upnpc -d 6567 TCP 6567 UDP"`` et vérifiez bien que la dernière ligne affiche **"UPNP_DeletePortMapping() returned : 0"** pour savoir s'il a été bien refermé. <br>
Et pour quitter l'application, tapez la commande ``"exit"``.

Pour savoir si le port a été bien ouvert ou fermé, regardez la partie **Info** des [étapes pour PC](#solution-miniupnpc).

**Note :** Héberger un serveur sur mobile est souvent une mauvaise idée, surtout s'il est public. Un téléphone n'est jamais fixe dans un réseau... <br>
Cette solution fonctionne, mais est instable; vous pouvez vous attendre à des déconnexions répétées. <br>
Toutefois, si vous possédez un PC chez vous, effectuez les [étapes pour PC](#solution-miniupnpc) tout en jouant sur mobile, cela sera plus stable.


## CONTACT
Si vous avez des difficultés à réaliser ce tutoriel, n'hésitez pas à m'envoyer un message privé sur discord : ``@zetamap``. <br>
Pas de spam ou de demandes inutiles svp, sinon je ne répondrai plus aux messages. Merci =)

#### Remercîments
Je remercie [xorblo-doitus](https://github.com/xorblo-doitus) pour m'avoir aidé sur la correction des fautes, et sur la formulation des phrases. ;)
