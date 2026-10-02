# Architecture — Smart Home & Capteur IoT

## 1. Smart Home

Le prototype repose sur un kit IoT permettant de collecter des données environnementales, de les transmettre vers des services cloud et de les afficher sur un dashboard.

```text
Capteurs
   ↓
Arduino Explore IoT Kit Rev2
   ↓
Réseau / connectivité
   ↓
Arduino IoT Cloud + Firebase
   ↓
Dashboard temps réel
   ↓
Commande des appareils
```

Le prototype prévoit la commande de deux lampes et de deux prises.

## 2. Capteur IoT multifonction

Le second dispositif est conçu autour d'un ESP32 S3 et de capteurs, notamment un DHT22 et un MQ-7. Le projet prévoit également la conception d'un PCB sous KiCad.

```text
DHT22 / MQ-7 / autres capteurs
              ↓
           ESP32 S3
              ↓
       Acquisition des données
              ↓
       Post-traitement / stockage
              ↓
          Exploitation
```

## 3. Principe logiciel

```text
Initialisation
     ↓
Lecture des capteurs
     ↓
Traitement des mesures
     ↓
Transmission des données
     ↓
Affichage / exploitation
     ↓
Nouvelle acquisition
```

> Les détails de câblage et les broches ne sont volontairement pas imposés dans cette documentation : ils doivent correspondre au montage effectivement réalisé.
