# LAB-1-Mise-en-place-du-lab-Mobexler-snapshot-clean-

# Mobexler – VirtualBox Configuration

## Objectif
Configurer la machine Mobexler dans VirtualBox pour les tests de sécurité mobile Android.

---

## Étape 1 – Importer l’OVA
1. Ouvrir VirtualBox
2. File → Import Appliance
3. Sélectionner le fichier `Mobexler.ova`
4. Cliquer sur Import
5. ![Import OVA](https://github.com/user-attachments/assets/e23ff433-7a78-4dc6-99a1-5f313ffea07f)


---

## Étape 2 – Configuration réseau
Après l’importation :

1. Sélectionner la VM Mobexler
2. Settings → Network

### Adapter 1
- Type : **NAT**
- Rôle : Accès Internet (updates, outils)

### Adapter 2
- Type : **Host-Only Adapter**
- Rôle : Réseau isolé pour communiquer avec la cible Android

---

## Définition
- **NAT** : Permet à la VM d’avoir accès à Internet de manière stable.
- **Host-Only** : Réseau local isolé entre l’hôte et la VM pour le laboratoire.

---

## Remarque
Si le Host-Only Adapter n’apparaît pas :
1. VirtualBox → Tools
2. Network Manager
3. Host-Only Networks → Create

---

## Étape suivante
Démarrage de la VM et vérification de la connectivité réseau.
