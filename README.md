# EL-HAKIM PRO — téléchargements

Logiciel de gestion de cabinet médical : patients, consultations, rendez-vous, ordonnances et documents.
Cette page sert uniquement à télécharger le programme et ses fichiers. Elle ne contient aucune donnée de cabinet.

## Télécharger

Version actuelle : **1.4.1**. Cliquez sur un fichier pour le télécharger.

| Fichier | Contenu |
|---|---|
| **[el-hakim-pro-setup.exe](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/el-hakim-pro-setup.exe)** | Programme d'installation (première installation ou mise à jour) |
| [EL-HAKIM-PRO-Guide-Installation-v1.4.1.pdf](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/EL-HAKIM-PRO-Guide-Installation-v1.4.1.pdf) | Guide d'installation et de configuration |
| [EL-HAKIM-PRO-Guide-Utilisation-v1.4.1.pdf](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/EL-HAKIM-PRO-Guide-Utilisation-v1.4.1.pdf) | Guide d'utilisation |
| [EL-HAKIM-PRO-Demarrage-Rapide-v1.4.1.pdf](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/EL-HAKIM-PRO-Demarrage-Rapide-v1.4.1.pdf) | Démarrage rapide (2 pages à imprimer) |
| [nomenclature-medicaments-juin-2026.xlsx](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/nomenclature-medicaments-juin-2026.xlsx) | Nomenclature nationale des médicaments (juin 2026), à importer dans EL-HAKIM PRO |
| [logos-specialites.rar](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/logos-specialites.rar) | Logos de spécialités (16 images) pour l'en-tête des documents |
| [guide-courbes-de-croissance.docx](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/guide-courbes-de-croissance.docx) | Guide du module Courbes de croissance |

## Vous avez déjà EL-HAKIM PRO (version 1.4.0 ou plus récente)

Vous n'avez rien à télécharger :
- quand une nouvelle version est disponible, l'application vous le propose ;
- cliquez sur **« Mettre à jour maintenant »**. La mise à jour se fait seule : sauvegarde complète d'abord, puis
  installation. EL-HAKIM PRO se ferme puis se rouvre ;
- les fichiers ci-dessus (guides, nomenclature, logos) arrivent aussi d'eux-mêmes sur le poste. Pour les ouvrir :
  **Configuration** › **« Mises à jour et fichiers joints… »** › **« Ouvrir le dossier des fichiers joints »**.

**Plusieurs postes au cabinet :** mettez d'abord à jour le **poste serveur**. Les autres postes proposent ensuite la
mise à jour d'eux-mêmes.

## Première installation, ou mise à jour depuis la version 1.0.4

1. **Fermez EL-HAKIM PRO** sur ce poste.
2. Lancez **el-hakim-pro-setup.exe**.
3. **Si Windows affiche « Windows a protégé votre ordinateur »** (filtre SmartScreen) : cliquez sur
   **« Informations complémentaires »**, vérifiez que le nom du fichier correspond à EL-HAKIM PRO, puis cliquez sur
   **« Exécuter quand même »**. Ce message apparaît parce que le programme est encore peu téléchargé. Il ne signale
   pas un problème.
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

Tout le détail est dans le **Guide d'installation et de configuration** (tableau ci-dessus).

## Licence

À la première ouverture, EL-HAKIM PRO fonctionne en période d'essai (3 jours). Dans la page
**Licence & Abonnement**, copiez le **CODE MACHINE** et envoyez-le à votre fournisseur : vous recevrez un fichier de
licence à importer, ou une clé à coller, dans cette même page.

## Vérifier le fichier téléchargé (facultatif)

L'empreinte SHA-256 du programme d'installation est publiée avec chaque version
([SHA256.txt](https://github.com/yacami/el-hakim-pro-releases/releases/latest/download/SHA256.txt)). Pour la comparer,
ouvrez PowerShell dans le dossier du fichier, puis tapez :

```
Get-FileHash .\el-hakim-pro-setup.exe -Algorithm SHA256
```

Les deux empreintes doivent être identiques.

## Assistance

En cas de problème, transmettez le journal d'installation au support. Il se trouve dans votre profil Windows :
`EL-HAKIM PRO Sauvegardes\journal-installation-….log`

---

*Les autres fichiers de la page des versions (`latest.json`, `fichiers.json`, leurs signatures `.sig`) servent aux
mises à jour automatiques du logiciel : vous n'avez pas à les télécharger.*
