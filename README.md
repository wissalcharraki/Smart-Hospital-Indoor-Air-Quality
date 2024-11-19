
# SMART HOSPITAL: IAQ

**Surveillance Intelligente de la Qualité de l'Air Intérieur en Temps Réel dans un Espace Hospitalier**

## Réalisé par :
- Wissal CHARRAKI
- Adam ESSBAA
- Abdelhak AMZIL

## Encadré par :
- Pr. Abdelhalim HNINI

---

## **Contexte**
La qualité de l'air dans les espaces hospitaliers, en particulier les salles d'opération, les unités de soins intensifs et les chambres stériles, est un enjeu crucial pour :
- Réduire les risques d'infections nosocomiales.
- Améliorer la santé et le confort des patients et du personnel.
- Prévenir les impacts négatifs des contaminants et des mauvaises conditions environnementales.

---

## **Objectifs du Projet**
1. Fournir une solution de **surveillance en temps réel** de la qualité de l'air.
2. Détecter et signaler rapidement les **anomalies** environnementales.
3. Centraliser les données pour une **analyse historique** et des visualisations.
4. Automatiser le processus de surveillance pour minimiser la dépendance humaine.

---

## **Problèmes Ciblés**
### Contaminants :
- Particules fines (PM2.5, PM10)
- Gaz anesthésiques et dioxyde de carbone (CO₂)
- Contaminants microbiologiques (bactéries, moisissures)

### Conditions Environnementales :
- Température (< 18°C ou > 26°C)
- Humidité (< 30% ou > 70%)
- Défauts de ventilation et de pression d'air

### Autres Risques :
- Sur-occupation et entrées/sorties fréquentes
- Gaz inflammables et fumées toxiques

---

## **Solution Technique**
### Matériel Utilisé :
- Raspberry Pi board
- Capteurs (DHT11 pour température et humidité, MQ7 pour CO)
- Caméra pour détection d'occupation
- Affichage LCD I2C
- Divers modules électroniques (ADS7830, GPIO Extension board, etc.)

### Pipeline de Traitement :
1. **Collecte des Données** :
   - Capteurs IoT
   - Stockage dans DynamoDB
2. **Préparation des Données** :
   - Nettoyage et extraction via Python
3. **Analyse et Prédiction** :
   - Modèle LSTM (Long Short-Term Memory) pour la prédiction des anomalies environnementales
4. **Déploiement** :
   - AWS SageMaker pour la gestion des prédictions

---

## **Fonctionnalités Clés**
- **Alertes en Temps Réel** : Notifications lors de dépassements de seuils.
- **Prédiction d'Anomalies** : Utilisation du LSTM pour anticiper les variations des niveaux de CO₂, température et humidité.
- **Surveillance Continue** : Minimisation des interventions humaines grâce à l'automatisation.

---

## **Conclusion**
Ce projet offre une approche innovante pour améliorer la qualité de l'air dans les hôpitaux en intégrant les technologies IoT et IA, garantissant ainsi un environnement plus sûr pour les patients et le personnel.
"# Smart-Hospital-Indoor-Air-Quality" 
