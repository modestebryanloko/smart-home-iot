# 🏠 Smart Home & Capteur IoT multifonction

## Présentation

Ce projet porte sur la **mise en place d'un système de domotique** et la **conception d'un capteur IoT multifonction**.

La partie Smart Home consiste à récupérer des données environnementales en temps réel et à permettre la commande à distance de plusieurs appareils domestiques. La partie capteur IoT consiste à concevoir un dispositif connecté pour la collecte et le post-traitement de données.

## 🎯 Objectifs

- Mesurer des paramètres environnementaux en temps réel.
- Centraliser les données sur un système IoT.
- Afficher les mesures dans un dashboard.
- Commander à distance des appareils domestiques.
- Concevoir un dispositif IoT adapté à un environnement d'atelier.
- Préparer le traitement et l'exploitation des données collectées.

## 🔧 Matériel et technologies

- Arduino Explore IoT Kit Rev2
- Arduino IoT Cloud
- Firebase
- ESP32 S3
- DHT22
- MQ-7
- Capteurs environnementaux
- PCB conçu avec KiCad
- Connectivité Wi-Fi / 5G selon l'architecture utilisée

## 🏠 Système Smart Home

Le prototype de maison connectée récupère des données environnementales et permet la commande de **quatre appareils domestiques : deux lampes et deux prises**.

Les données suivies comprennent notamment la température, l'humidité, la pression et la qualité de l'air. Un dashboard permet de visualiser les informations et un autre de commander les appareils.

## 📡 Capteur IoT multifonction

Une seconde partie du projet consiste à concevoir un dispositif IoT propre, destiné au recueil de données dans un atelier.

Le travail comprend :

1. Rédaction du cahier des charges.
2. Vérification du matériel disponible.
3. Tests des composants.
4. Intégration des fonctionnalités.
5. Conception du PCB sous KiCad.
6. Collecte et post-traitement des données.

## ⚙️ Architecture générale

```text
       CAPTEURS
          │
          ▼
   ESP32 / Arduino
          │
          ▼
   Connexion réseau
          │
     ┌────┴────┐
     ▼         ▼
  Firebase   IoT Cloud
     │         │
     └────┬────┘
          ▼
      Dashboard
          │
          ▼
 Commande des appareils
```

## 💻 Exemple de logique de programmation

```text
Démarrer
   ↓
Initialiser les capteurs
   ↓
Lire les mesures
   ↓
Envoyer les données
   ↓
Afficher sur le dashboard
   ↓
Vérifier une commande utilisateur
   ↓
Commander l'appareil concerné
   ↓
Recommencer
```

Le fichier `src/smart_home_example.ino` est un exemple documentaire destiné à illustrer cette logique. Les broches et bibliothèques exactes doivent être adaptées au montage réellement utilisé.

## 📁 Structure du dépôt

```text
smart-home-iot/
├── README.md
├── docs/
│   └── architecture.md
├── images/
│   ├── kit-iot.jpg
│   ├── capteur-iot.jpg
│   ├── capteur-multifonction.jpg
│   ├── dashboard-iot.png
│   └── pcb-iot.png
└── src/
    └── smart_home_example.ino
```

## 🔮 Perspectives

- Améliorer la fiabilité des mesures par étalonnage.
- Ajouter d'autres capteurs.
- Améliorer le dashboard temps réel.
- Ajouter davantage d'appareils commandables.
- Optimiser la connectivité.
- Exploiter davantage les données collectées.

## 👨‍💻 Auteur

**Modeste LOKO**
