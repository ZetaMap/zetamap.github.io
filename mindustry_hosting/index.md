[<-- Home Page](/)

# Comment jouer avec des amis ? - Tutoriel
Pour pouvoir jouer avec des amis, je vous propose un tuto où vous pourrez choisir entre plusieurs logiciels. Ce que je propose est valable pour mobile et PC.

⚠️ Lisez bien tout le tutoriel pour bien tout comprendre. ⚠️



## SOMMAIRE
* [PRÉSENTATION DES LOGICIELS](#présentation)
  * [MiniUPNPC](#miniupnpc)
  * [Hamachi](#hamachi)
  * [Termux](#termux)
* [TUTOS](#tutos)
   * [Pour PC](#pc)
      * [Solution MiniUPNPC](#solution-miniupnpc)
      * [Solution Hamachi](#solution-hamachi)
   * [Pour Mobile](#mobile)
* [CONTACT](#contact)



## PRÉSENTATION DES LOGICIELS <a id="présentation"></a>
### MiniUPNPC <a id="miniupnpc"></a>
[MiniUPNPC](http://miniupnp.free.fr/) est open source et complètement modulable selon vos envies, il communique avec la box pour rediriger les connexions d'un port sélectionné au PC du demandeur, cette pratique s'appelle le Port Forwarding.
* **Avantages :** C'est un logiciel très petit, très simple d'utilisation, rapide, efficace, et il n'y a que l'hébergeur du serveur qui doit être sur PC : les autres peuvent être sur la plateforme de leur choix. De plus, il ne collecte aucune donnée personnelle, vous en avez un total contrôle, et il n'y a pas de limite de place dans le réseau.
* **Défauts :** Son plus gros défaut est d'être peu sécurisé, car cela utilise votre IP publique : vous serez donc vulnérable aux attaques des Hackers. Il est donc important de ne pas donner son IP à n'importe qui. En outre, si vous n'êtes pas sûr de ce que vous faites ou que vous vivez dans un quartier mal vu, je vous déconseille ce logiciel.
* En savoir plus [ici](http://miniupnp.free.fr/).

### Hamachi <a id="hamachi"></a>
[Hamachi](https://www.vpn.net/) est un service de *"client tunnelling"*. En principe, il fait la même chose que [MiniUPNPC](#miniupnpc), mais de manière plus sophistiquée et sécurisée, sauf qu'il faut avoir un compte Hamachi.
* **Avantages :** Il est simple d'utilisation, avec une belle interface graphique au lieu de commandes, et est très efficace. De plus, il est sécurisé, donne la possibilité de sauvegarder plusieurs réseaux à la fois, et de définir un mot de passe sur un réseau pour en contrôler les accès.
* **Défauts :** Pour pouvoir l'utiliser il faut avoir créé un compte Hamachi qui est certes gratuit, mais dont on ne sait pas où seront stockées les données des connexions. Dans leurs [conditions générales d'utilisation](https://www.goto.com/fr/company/legal), ils stipulent bien que des données personnelles seront collectées, mais ne précisent pas quelles données. Par ailleurs, il faut que l'hébergeur, ainsi que toutes les personnes qui veulent s'y connecter, soient sur PC ainsi que sur Windows, car le logiciel n'est disponible que sur cette plateforme. Les places disponibles dans un réseau sont limitées à 5 : pour palier à cela, la société propose des formules payantes et très chères. Enfin, lors de son installation, il ajoute un service qui démarrera à chaque démarrage de l'ordinateur.
* En savoir plus [ici](https://vpn.net/).

### Termux <a id="termux"></a>
[Termux](https://termux.com/) est un logiciel libre et open source disponible à l'installation sur [Github](https://github.com/termux/termux-app), [F-droid](https://f-droid.org/en/packages/com.termux/), et sur [Play Store](https://play.google.com/store/apps/details?id=com.termux). C'est tout simplement le meilleur terminal de commande Linux pour mobile au monde. Il donne la possibilité d'installer des applis, contrôler son téléphone, installer les émulateurs Python ou Java, et bien d'autres fonctionnalités. L'application ne transmet aucune donnée personnelle à des sociétés tierces, si ce n'est les rapports de bugs aux développeurs avec votre consentement, et dispose de quelques modules installables pour personnaliser son terminal.
* **Avantages :** Sait tout faire, tout simplement.
* **Défauts :** Aucun défaut, si ce n'est qu'il n'est plus mis à jour sur le Play Store, dû a des petites demandes de changement de la part de Google (si vous voyez ce que je veux dire ;) ).
* Pour les mobiles, il sera nécessaire d'installer cette application pour pouvoir utiliser [MiniUPNPC](/MiniUPNPC). Vous pouvez directement l'installer en [cliquant ici](https://f-droid.org/repo/com.termux_118.apk) pour la version *0.118*, et pour d'autres versions [ici](https://github.com/termux/termux-app/releases).



## TUTOS <a id="tutos"></a>
### Pour PC <a id="pc"></a>
#### Solution MiniUPNPC <a id="solution-miniupnpc"></a>
**1-** Tout d'abord, il faut télécharger le logiciel qui se [trouve ici](http://miniupnp.free.fr/files/download.php?file=upnpc-exe-win32-20150918.zip), ensuite dézippez le (je conseille de le faire dans les dossiers de votre jeu pour ne pas le perdre).

**2-** Maintenant il faut ouvrir un terminal de commande pour effectuer la suite du tuto, pour cela, vous pouvez faire : TOUCHE WINDOWS + R, et taper ``"powershell"`` puis entrer.

**3-** Ensuite il faut se déplacer à l'endroit où le logiciel a été dézippé, pour ce faire, tapez ``"cd <emplacement du dossier>"`` dans le terminal.

**4-** Maintenant, pour ouvrir le port de la box, exécutez la commande ``"upnpc-static.exe -r 6567 TCP 6567 UDP"``. Attendez un moment puis regardez la ligne **ExternalIPAddress**, c'est l'adresse IP publique de la box qu'il faut donner aux autres.

**5-** Lorsque vous avez fini de jouer avec vos amis, tapez la commande ``"upnpc-static.exe -d 6567 TCP 6567 UDP"``, puis regardez la dernière ligne. Si elle affiche **UPNP_DeletePortMapping() returned : 0**, c'est que le port a bien été refermé.


**Info :**
Pour vérifier que le port a bien été ouvert ou fermé, vous pouvez utiliser [cet outil](https://www.yougetsignal.com/tools/open-ports/), en indiquant le port *6567* dans le cadre **Port Number**. Lors du test d'ouverture du port, assurez-vous qu'au préalablement le serveur a été hébergé : si vous utilisez la version serveur de Mindustry, tapez la commande **host** pour l'héberger. Et si vous ne l'utilisez pas, allez dans le menu pause et cliquez sur le bouton **Héberger un serveur**.

**Note :**
Lors de la vérification de l'ouverture du port, le site peut des fois indiquer le port comme fermé alors qu'il est bien ouvert.

#### Solution Hamachi <a id="solution-hamachi"></a>
**1-** Premièrement, il faut installer l'installateur du client [disponible ici](https://www.vpn.net/) : suivez les étapes d'installation puis reprenez le tutoriel... Une fois que le logiciel est installé et lancé, suivez les étapes pour créer un compte Hamachi puis reprenez le tutoriel...

**2-** Cliquez sur **Réseau** en haut au milieu de la fenêtre, puis **Créer un réseau...**, il vous sera ensuite demandé un *ID* de réseau ainsi qu'un mot de passe et une confirmation de ce-dernier. L'ID de réseau sera son nom qui devra être communiqué aux autres personnes, et vous n'êtes pas obligé de mettre un mot de passe si vous le souhaitez.

**3-** Pour pouvoir se connecter à un réseau, c'est très simple : il vous suffira de cliquer sur **Réseau** puis **Rejoindre un réseau...**. Une page de connexion s'affichera, vous demandant l'ID du réseau (son nom) ainsi que son mot de passe, avec une petite note de ne pas en mettre s'il n'y en a pas.

**4-** Il vous suffira d'héberger votre serveur et les gens connectés a votre réseau verront le serveur dans la catégorie **Serveurs Locaux**.


### Pour Mobile <a id="mobile"></a>
**1-** Avant de commencer, il faut avoir téléchargé l'application Termux (les étapes sont [ici](#termux)) et l'avoir lancé.

**2-** Maintenant, il faut télécharger le *package* MiniUPNPNC. Pour ce faire, tapez ``"pkg install miniupnpc"`` et attendez que l'installation se termine. Pour savoir si le package a été installé, regardez si la dernière ligne ressemble à **\~ \$** .

**3-** Les étapes restantes ne sont pas bien différentes de la version PC : seule la syntaxe change. Pour ouvrir le port, tapez ``"upnpc -r 6567 TCP 6567 UDP"`` et regardez la ligne **ExternalIPAddress** : c'est l'adresse IP publique de la box qu'il faut donner aux autres.

**4-** Pour refermer le port, tapez ``"upnpc -d 6567 TCP 6567 UDP"`` et vérifiez bien que la dernière ligne affiche **"UPNP_DeletePortMapping() returned : 0"** pour savoir s'il a été bien refermé. Et pour quitter l'application, tapez ``"exit"`` puis entrer.

**5-** Pour savoir si le port a été bien ouvert ou fermé, regardez la partie **Info** des [étapes pour version PC](#solution-miniupnpc).


**Note :**
Héberger un serveur sur mobile est souvent une mauvaise idée, surtout s'il est public. Un téléphone n'est jamais fixe dans un réseau. Cette solution fonctionne, mais est instable : vous pouvez vous attendre à des déconnexions répétées, mais toutefois, si vous possédez un PC chez vous, effectuez les [étapes pour PC](#solution-miniupnpc) tout en jouant sur mobile, cela sera plus stable.



## CONTACT <a id="contact"></a>
Si vous avez des difficultés à réaliser ce tutoriel, n'hésitez pas à m'envoyer un message privé sur discord : ``[BTA] ZetaMap#5093``. 

Pas de spam ou de demandes inutiles svp, sinon je ne répondrai plus aux messages. Merci =)
#### Remercîment
Je remercie [xorblo-doitus](https://github.com/xorblo-doitus) pour m'avoir aidé sur la correction des fautes, et sur la formulation des phrases. ;)
