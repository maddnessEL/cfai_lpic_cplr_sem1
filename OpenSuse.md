# OpenSuse LEAP
![](https://i.imgur.com/opAO1al.png)

### Les avantage de OpenSUSE:
- **Compatibilité binaire avec SLES**: 

OpenSUSE Leap est basé sur les paquets de SUSE Linux Enterprise Server (SLES) de l’entreprise de Nuremberg. Depuis lors, la base de code des deux systèmes d’exploitation est identique et les distributions sont compatibles binaires. 

- **Stabilité et sécurité:** 

L’une des principales raisons du succès d’openSUSE Leap dans le monde est la stabilité du système d’exploitation. La distribution Linux, considérée comme extrêmement sûre, convient donc aussi à une utilisation dans les domaines qui ne tolèrent aucune erreur ni problème.

- **YaST:** 

YaST (pour « Yet another Setup Tool ») basé sur RPM est un outil qui facilite considérablement les tâches administrateur. YaST permet de procéder plus rapidement et surtout plus clairement aux installations, configurations, et paramétrages de services sur les serveurs, entre autres.

- **Live Patching:** 

Live Patching permet d'appliquez des correctifs et des mises à jour critiques au noyau Linux sans redémarrer le système et les applications. Optimisez la disponibilité et effectuez des mises à jour de sécurité critiques et des corrections à la volée pour de nombreuse applications 



### **Esaie de yast :**

Dans mon cas j'ai essayé la TUI de yast2, depuis YaST, vous pouvez effectuer à peu près n’importe quelle tâche d’administration du système. Par exemple :

- Installer et supprimer des logiciels (voir chapitre suivant)
- Configurer les paramètres système (Date/heure, langue, réseau...)
- Configurer votre pare-feu
- Activer ou désactiver les services du système
- Gérer le partionnement de vos disques
- Gérer les groupes et utilisateurs
- Eventuellement ajouter une couche de virtualisation, type KVM

YaST2 est intuitif et est utilisable des lors que l'on rentre la commande :
```bash=
sudo yast2
```
Voici à quoi ressemble l'interface TUI de YaST2 :

![](https://i.imgur.com/udepTtY.png)
