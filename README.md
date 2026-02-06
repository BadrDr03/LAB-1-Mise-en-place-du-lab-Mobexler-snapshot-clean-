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
![Import OVA](https://github.com/user-attachments/assets/b625f16e-55dd-4aa0-a73d-f59e9b33e454)

### Adapter 2
- Type : **Host-Only Adapter**
- Rôle : Réseau isolé pour communiquer avec la cible Android
![Import OVA](https://github.com/user-attachments/assets/b889f7ce-e4f2-47b3-bf5f-d7ed9e6c67a8)
---

## Définition
- **NAT** : Permet à la VM d’avoir accès à Internet de manière stable.
- **Host-Only** : Réseau local isolé entre l’hôte et la VM pour le laboratoire.

---

## Étape 3 — Premier démarrage + connexion

![Import OVA](https://github.com/user-attachments/assets/fdf0969e-3b32-4a25-b23b-79466708ef67)


## Étape 4 — Vérifier le réseau (tests “santé”)

![Import OVA](https://github.com/user-attachments/assets/c6b8e1ae-cb1a-4275-94e7-e9bda4dce97a)

![Import OVA](https://github.com/user-attachments/assets/7fc77fc4-fa2b-44df-81d3-f21072a4bc9d)

![Import OVA](https://github.com/user-attachments/assets/54605e38-ac52-465c-b073-23f3dae0603c)



## Étape 5 — Créer le snapshot “CLEAN” (baseline)

![Import OVA](https://github.com/user-attachments/assets/e01ab967-2dbd-40b3-a0b0-0a62d4cce9b1)

