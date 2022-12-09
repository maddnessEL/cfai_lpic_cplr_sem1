# OpenSuse LEAP
![](https://i.imgur.com/opAO1al.png)

### Les avantages de OpenSUSE:
- **Compatibilité binaire avec SLES**: 

OpenSUSE Leap est basé sur les paquets de SUSE Linux Enterprise Server (SLES) de l’entreprise de Nuremberg. Depuis lors, la base de code des deux systèmes d’exploitation est identique et les distributions sont compatibles binaires. 

- **Stabilité et sécurité:** 

L’une des principales raisons du succès d’openSUSE Leap dans le monde est la stabilité du système d’exploitation. La distribution Linux, considérée comme extrêmement sûre, convient donc aussi à une utilisation dans les domaines qui ne tolèrent aucune erreur ni problème.

- **YaST:** 

YaST (pour « Yet another Setup Tool ») basé sur RPM, est un outil qui facilite considérablement les tâches administrateur. YaST permet de procéder plus rapidement et surtout plus clairement aux installations, configurations, et paramétrages de services sur les serveurs, entre autres.

- **Live Patching:** 

Live Patching permet d'appliquer des correctifs et des mises à jour critiques au noyau Linux sans redémarrer le système et les applications. Optimisez la disponibilité et effectuez des mises à jour de sécurité critiques et des corrections à la volée pour de nombreuses applications.



### **Esaie de yast :**

Dans mon cas, j'ai essayé la TUI de yast2, depuis YaST, vous pouvez effectuer à peu près n’importe quelle tâche d’administration du système. Par exemple :

- Installer et supprimer des logiciels
- Configurer les paramètres système (date/heure, langue, réseau...)
- Configurer votre pare-feu
- Activer ou désactiver les services du système
- Gérer le partitionnement de vos disques
- Gérer les groupes et utilisateurs
- Éventuellement ajouter une couche de virtualisation, type KVM

YaST2 est intuitif et est utilisable dès lors que l'on rentre la commande :
```bash=
sudo yast2
```
Voici à quoi ressemble l'interface TUI de YaST2 :

![](https://i.imgur.com/udepTtY.png)

### **Installation d'un service avec YaST :**

Nous allons nous rendre dans **Logiciel > Installer et supprimer des logiciels** et faites les étapes suivantes :

```yaml
    Étapes:
        - 1: "Rechercher le logiciel nginx"
        - 2: "On descend sur nginx et on appuie sur la touche espace afin d'afficher le +"
        - 3: "Cliquer sur accepter"
```

![](https://i.imgur.com/BN8NDu0.png)

Cliquer sur **Terminer** et Nginx est maintenant installé.

Nous allons maintenant vérifier que le service est activé et mettre le démarrage automatique au lancement d'OpenSuse, pour cela on va se rendre dans  **Système > Gestionnaire de services** et faire les étapes suivantes :

```yaml
    Étapes:
        - 1: "Descendre pour trouver le service [nginx]"
        - 2: "Se rendre sur [Mode de démarrage] et passer la valeur à [Au démarage du système]"
        - 3: "Ensuite cliquer sur [Démarrer] pour démarrer le service"
        - 4: "Enfin cliquer sur [Appliquer] et [OK]"
```
![](https://i.imgur.com/eLosxe5.png)

Pour finir nous allons éditer le pare-feu afin d'autoriser les flux **HTTP** et **HTTPS**, pour ce faire rendez-vous dans **Sécurité et Utilisateurs > Pare-feu** et suivez les étapes suivantes :

```yaml
    Étapes:
        - 1: "Aller dans la zone [public]"
        - 2: "Sélectionner [http] et [https]"
        - 3: "Ensuite cliquer sur [Ajouter]"
        - 4: "Enfin cliquer sur [Accepter]"
```
![](https://i.imgur.com/L5Fx5KS.png)

Le logiciel Nginx est maintenant fonctionel et est accessible depuis l'ip de la machine.

![](https://i.imgur.com/VRuktkK.png)