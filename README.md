# EL-HAKIM PRO — installation et mises à jour

Logiciel de gestion de cabinet médical : patients, consultations, rendez-vous, ordonnances et documents.
Cette page sert uniquement à télécharger le programme d'installation. Elle ne contient aucune donnée de cabinet.

## Télécharger

Téléchargez la dernière version :
**[el-hakim-pro-setup.exe](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/el-hakim-pro-setup.exe)**

Toutes les versions et leurs notes sont dans [Releases](https://github.com/yacami/el-hakim-pro-releases/releases).

## Vous avez déjà EL-HAKIM PRO (version 1.4.0 ou plus récente)

Vous n'avez rien à télécharger :
- quand une nouvelle version est disponible, l'application vous le propose ;
- cliquez sur **« Mettre à jour maintenant »**. La mise à jour se fait seule : sauvegarde complète d'abord, puis
  installation. EL-HAKIM PRO se ferme puis se rouvre.
- Paramètres › **« Mises à jour et fichiers joints… »** : rechercher une mise à jour, ou désactiver la vérification
  automatique.

**Plusieurs postes au cabinet :** mettez d'abord à jour le **poste serveur**. Les autres postes proposent ensuite la
mise à jour d'eux-mêmes.

## Première installation, ou mise à jour depuis la version 1.0.4

1. **Fermez EL-HAKIM PRO** sur ce poste.
2. Lancez **el-hakim-pro-setup.exe**.
3. **Si Windows affiche « Windows a protégé votre ordinateur »** (filtre SmartScreen) :
   - cliquez sur **« Informations complémentaires »** ;
   - vérifiez que l'éditeur ou le nom du fichier correspond à EL-HAKIM PRO, puis cliquez sur
     **« Exécuter quand même »**.

   Ce message apparaît parce que le programme est encore peu téléchargé. Il ne signale pas un problème.
4. **Choisissez le dossier d'installation.** Pour une mise à jour, gardez celui qui est proposé.
5. **Choisissez l'usage du poste :**
   - **Poste unique** : EL-HAKIM PRO n'est utilisé que sur cet ordinateur ;
   - **Serveur multi-postes** : les autres ordinateurs du cabinet utilisent les données de ce poste ;
   - **Poste client** : ce poste utilise les données du serveur ; saisissez l'adresse du serveur (ex. 192.168.1.10).
6. Si Windows demande l'autorisation d'apporter des modifications, acceptez. Elle sert à installer le composant
   Visual C++ et à régler le pare-feu.

Lors d'une mise à jour, une **sauvegarde complète** (programme, base de données, documents) est faite et vérifiée
**avant** toute modification. Elle se trouve dans votre profil Windows, dossier `EL-HAKIM PRO Sauvegardes`. En cas
de problème, l'installation remet automatiquement tout comme avant.

## Vérifier le fichier téléchargé (facultatif)

Chaque version publie son empreinte SHA-256 dans `SHA256.txt`. Pour la comparer, ouvrez PowerShell dans le dossier
du fichier, puis tapez :

```
Get-FileHash .\el-hakim-pro-setup.exe -Algorithm SHA256
```

Les deux empreintes doivent être identiques.

## Licence

À la première ouverture, la page **Licence** affiche l'**identifiant du poste**. Envoyez-le à votre fournisseur :
vous recevrez une clé à coller, ou un fichier de licence à importer, dans cette même page.

## Assistance

En cas de problème, transmettez le journal d'installation au support. Il se trouve dans votre profil Windows :
`EL-HAKIM PRO Sauvegardes\journal-installation-….log`
