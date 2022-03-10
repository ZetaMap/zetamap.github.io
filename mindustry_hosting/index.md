[<-- Home Page](/)

# Comment jouer avec des amis ? - Tutoriel
Pour pouvoir jouer avec des amis, je vous propose un tuto o� vous pourrez choisir entre plusieurs logiciels, se que je propose et est valable pour mobile et PC.

**/!\\** Lisez bien tout le tutoriel pour bien tout comprendre. **/!\\**



## SOMMAIRE
* [PR�SENTATION DES LOGICIELS](#pr�sentation)
    * [MiniUPNPC](#miniupnpc)
    * [Hamachi](#hamachi)
    * [Termux](#termux)
* [TUTOS](#tutos)
     * [Pour PC](#pc)
      * [Solution MiniUPNPC](#solution-miniupnpc)
      * [Solution Hamachi](#solution-hamachi)
     * [Pour Mobile](#mobile)
* [CONTACT](#contact)



## PR�SENTATION DES LOGICIELS <a id="pr�sentation"></a>
### MiniUPNPC <a id="miniupnpc"></a>
[MiniUPNPC](http://miniupnp.free.fr/) est open source et est compl�tement modulable selon vos envies, il communique avec la box pour rediriger les connexions d'un port s�lectionn� au PC du demandeur, cette pratique s'appelle le Port Forwarding.
* **Avantages :** C'est un logiciel tr�s petit, tr�s simple d'utilisation, rapide, efficace, et il n'y a que l'h�bergeur du serveur qui doit �tre sur PC, les autres peuvent �tre sur la plateforme de leurs choix. De plus, il ne collecte aucune donn�e personnelle, vous en avait un total contr�le, et il n'y a pas de limite de place dans le r�seau.
* **D�fauts :** Son plus gros d�faut est que c'est peut s�curiser, car cela utilise ton IP publique, vous serez donc vuln�rable aux attaques des Hackers. Il est donc important de ne pas donner son IP � n'importe qui, de plus si vous n'�tes pas s�r de ce que vous faites ou que vous vivez dans un quartier mal vu, je vous d�conseille ce logiciel.
* En savoir plus [ici](http://miniupnp.free.fr/).

### Hamachi <a id="hamachi"></a>
[Hamachi](https://www.vpn.net/) est un service de *"client tunnelling"*, en principe, il fait la m�me chose que [MiniUPNPC](#miniupnpc) mais de mani�re plus sophistiqu�e et s�curiser, sauf qu'il faut avoir un compte Hamachi.
* **Avantages :** Il est simple d'utilisation, avec une belle interface graphique au lieu de commandes, et est tr�s efficace. De plus, il est s�curis�, donne la possibilit� de sauvegarder plusieurs r�seaux � la fois, et de d�finir un mot de passe sur un r�seau pour en contr�ler les acc�s.
* **D�fauts :** Pour pouvoir l'utiliser il faut avoir cr�� un compte Hamachi qui est serte gratuite, mais dont on ne sait pas o� seront stocker les donn�es des connexions. Dans leur [condition g�n�rale d'utilisation](https://www.goto.com/fr/company/legal), ils stipulent bien que des donn�es personnelles seront collect�es, mais ne disent pas quelles donn�es. De plus, il faut que l'h�bergeur ainsi que toutes les personnes qui veulent si connecter, soient sur PC ainsi que sur Windows, car le logiciel n'est disponible que sur cette plateforme. Les places disponibles dans un r�seau sont limit�s � 5, pour palier a cela, la soci�t� propose des formules payantes et tr�s ch�res. Pour finir, lors de son installation, il ajoute un service qui d�marrera � chaque d�marrage de l'ordinateur.
* En savoir plus [ici](https://vpn.net/).

### Termux <a id="termux"></a>
[Termux](https://termux.com/) est un logiciel libre et open source disponible � l'installation sur [Github](https://github.com/termux/termux-app), [F-droid](https://f-droid.org/en/packages/com.termux/), et sur [Play Store](https://play.google.com/store/apps/details?id=com.termux). C'est un terminal de commande Linux pour mobile et est tout simplement le meilleur au monde. Il donne la possibilit� d'installer des applis, contr�ler son t�l�phone, installer les �mulateurs Python ou Java, et bien d'autres fonctionnalit�s. L'application ne transmet aucune donn�e personnelle � des soci�t�s tierces si ce n'est que les rapports de bugs aux d�veloppeurs avec votre consentement, et dispose que quelques modules installables pour personnaliser son terminal.
* **Avantages :** Sais tout faire, tout simplement.
* **D�fauts :** Aucuns d�fauts si ce n'est qu'il n'est plus mis � jour sur le Play Store du a des petites demandes de changement de la part de Google (si vous voyez ce que je veux dire ;) ).
* Pour les mobiles, il sera n�cessaire d'installer cette application pour pouvoir utiliser [MiniUPNPC](/MiniUPNPC). Vous pouvez directement l'installer en [cliquant ici](https://f-droid.org/repo/com.termux_118.apk) pour la version *0.118*, et pour d'autres versions [ici](https://github.com/termux/termux-app/releases).



## TUTOS <a id="tutos"></a>
### Pour PC <a id="pc"></a>
#### Solution MiniUPNPC <a id="solution-miniupnpc"></a>
**1-** Tout d'abord, il faut t�l�charger le logiciel qui se [trouve ici](http://miniupnp.free.fr/files/download.php?file=upnpc-exe-win32-20150918.zip), ensuite d�zippe le (je conseille de le faire dans les dossiers de ton jeu pour ne pas le perdre).

**2-** Maintenant il faut ouvrir un terminal de commande pour effectuer la suite du tuto, pour cela, vous pouvez faire : TOUCHE WINDOWS + R, et taper ``"powershell"`` puis entrer.

**3-** Ensuite il faut se d�placer � l'endroit o� le logiciel a �t� d�zipp�, pour se faire tape ``"cd <emplacement du dossier>"`` dans le terminal.

**4-** Maintenant pour ouvrir le port de la box, ex�cute la commande ``"upnpc-static.exe -r 6567 TCP 6567 UDP"``. Attendez un moment puis regarde la ligne **ExternalIPAddress**, c'est l'adresse IP publique de la box qu'il faut donner aux autres.

**5-** Et lorsque vous avez fini de jouer avec vos amis, tapez la commande ``"upnpc-static.exe -d 6567 TCP 6567 UDP"``, puis regarde la derni�re ligne. Si elle affiche **UPNP_DeletePortMapping() returned : 0**, c'est que le port a bien �t� referm�.


**Info : **
Pour v�rifier que le port a bien �t� ouvert ou ferm�, vous pouvez utiliser [cet outil](https://www.yougetsignal.com/tools/open-ports/), en indiquant le port *6567* dans le cadre **Port Number**. Lors du test d'ouverture du port, assurez-vous qu'au pr�alablement le serveur a �t� h�berg� : si vous utilisez la version serveur de Mindustry, tapez la commande **host** pour l'h�berger. Et si vous ne l'utilisez pas, allez dans le menu pause et cliquez sur le bouton **H�berger un serveur**.

**Note : **
Lors de la v�rification de l'ouverture du port, le site peut des fois indiquer le port comme fermer alors qu'il est bien ouvert.

#### Solution Hamachi <a id="solution-hamachi"></a>
**1-** Premi�rement, il faut installer l'installateur du client [disponible ici](https://www.vpn.net/), suivez les �tapes d'installation puis reprenez le tutoriel... Une fois que le logiciel est install� et lanc�, suivez les �tapes pour cr�er un compte Hamachi puis reprenez le tutoriel...

**2-** Cliquez sur **R�seau** en haut au milieu de la fen�tre, puis **Cr�er un r�seau...**, il vous sera ensuite demander un *ID* de r�seau ainsi qu'un mot de passe et une confirmation de ce dernier. L'ID de r�seau sera son nom qui devra �tre communiqu� aux autres personnes, et vous n'�tes pas oblig� de mettre un mot de passe si vous le souhaitez.

**3-** Pour pouvoir se connecter � un r�seau, c'est tr�s simple, il vous suffira de cliquer sur **R�seau** puis **Rejoindre un r�seau...**. Une page de connexion s'affichera vous demandant l'ID du r�seau (son nom) ainsi que son mot de passe, avec une petite note de ne pas en mettre s'il n'y en a pas.

**4-** Il vous suffira d'h�berger votre serveur et les gens connect�s a votre r�seau verront le serveur dans la cat�gorie **Serveurs Local**.


### Pour Mobile <a id="mobile"></a>
**1-** Avant de commencer il faut avoir t�l�charg� l'application Termux, les �tapes sont [ici](#termux), et l'avoir lanc�.

**2-** Maintenant il faut t�l�charger le *package* MiniUPNPNC, pour ce faire tapez ``"pkg install miniupnpc"`` et attendez que l'installation se termine. Pour savoir si le package a �t� installer, regardez si la derni�re ligne ressemble � **~ $ **.

**3-** Le reste des �tapes ne sont pas bien diff�rentes que dans la version PC, juste la syntaxe qui change. Pour ouvrir le port, tapez ``"upnpc -r 6567 TCP 6567 UDP"`` et regardez la ligne **ExternalIPAddress**, c'est l'adresse IP publique de la box qu'il faut donner aux autres.

**4-** Et pour refermer le port, tapez ``"upnpc -d 6567 TCP 6567 UDP"`` et v�rifiez bien que la derni�re ligne affiche **UPNP_DeletePortMapping() returned : 0** pour savoir s'il a �t� bien referm�. Et pour quitter l'application, tapez ``"exit"`` puis entrer.

**5-** Pour savoir si le port a �t� bien ouvert ou ferm�, regardez la partie **Info** des [�tapes pour version PC](#solution-miniupnpc).


**Note :**
H�berger des serveurs sur mobile est souvent une mauvaise id�e surtout publique, un t�l�phone n'est jamais fixe dans un r�seau. Cette solution fonctionne, mais est instable, vous pouvez vous attendre � des d�connexions r�p�t�es, mais toutefois si vous poss�dez un PC chez vous, effectuez les [�tapes pour PC](#solution-miniupnpc) tout en jouant sur mobile, cela sera plus stable.



## CONTACT <a id="contact"></a>
Si vous avez des difficult�s � r�aliser ce tutoriel, n'h�sitez pas � m'envoyer un message priv� sur discord : ``[BTA] ZetaMap#5093``. 

Pas de spam ou de demandes inutiles svp, sinon je ne r�pondrai plus aux messages. Merci =)