# OSPecura2
# 🐑 Gestion Cheptel Pro

Application web progressive (PWA) moderne et simplifiée pour la gestion complète de cheptel d'élevage.

## ✨ Fonctionnalités

### 🐑 **Gestion des Animaux**
- ➕ **Ajout d'animaux** avec ID unique, dates, sexe, lot, emplacement et éleveur
- 📝 **Informations complètes** : date d'entrée, date de naissance, provenance
- 🗑️ **Suppression simple** avec confirmation
- 📊 **Vue d'ensemble** avec compteur temps réel

### 🌾 **Suivi Nutrition**
- 📅 **Enregistrement quotidien** des rations distribuées
- 🏠 **Par emplacement** : Bergerie 1, Bergerie 2, Tunnel 1, Tunnel 2, ou Ensemble
- 📦 **Quantités** : Foin (bottes) et Aliment (kg)
- 🗑️ **Gestion des records** avec suppression

### 📈 **Statistiques**
- 📊 **Compteurs en temps réel** : Total, Présents, Mâles, Femelles
- 📋 **Vue d'ensemble** du cheptel

### 💾 **Sauvegarde & Export**
- 🔄 **Sauvegarde automatique** dans le navigateur (localStorage)
- 📤 **Export CSV** pour Excel/LibreOffice
- 📥 **Import d'exemples** pour démarrage rapide
- 🗑️ **Remise à zéro** complète

## 🚀 Installation & Utilisation

### **📱 Utilisation directe**
1. Téléchargez le fichier `index.html`
2. Ouvrez-le dans votre navigateur web
3. L'application fonctionne immédiatement !

### **🌐 Hébergement en ligne (GitHub Pages)**
1. Créez un repository GitHub
2. Uploadez les fichiers
3. Activez GitHub Pages
4. Accédez via `https://votre-username.github.io/nom-repo/`

### **📱 Installation PWA (App mobile)**
- **Android** : Menu → "Ajouter à l'écran d'accueil"
- **iPhone** : Partager → "Sur l'écran d'accueil"  
- **PC** : Icône d'installation dans la barre d'adresse

## 📋 Guide d'utilisation

### **🐑 Ajouter un animal**

1. Cliquez sur **"✚ Ajouter Animal"**
2. Remplissez les champs :
   - **ID animal*** : Identifiant unique (ex: 001, A123)
   - **Date d'entrée** : Quand l'animal arrive
   - **Date de naissance** : Age réel de l'animal
   - **Nom éleveur** : Provenance
   - **Sexe** : Mâle/Femelle
   - **Lot*** : Classification (obligatoire)
   - **Emplacement*** : Où il est logé (obligatoire)
3. Cliquez **"💾 Sauvegarder"**

*Champs obligatoires marqués d'un astérisque

### **🌾 Enregistrer la nutrition**

1. Cliquez sur **"✚ Nouvelle Ration"**
2. Sélectionnez :
   - **Date** de distribution
   - **Emplacement** concerné
   - **Quantités** : Foin (bottes) et Aliment (kg)
3. Cliquez **"💾 Sauvegarder"**

### **📊 Consulter les statistiques**

- Onglet **"📈 Stats"** : Vue d'ensemble avec compteurs
- **En-tête** : Nombre total d'animaux en temps réel

## 🔧 Données gérées

### **🐑 Informations Animal**
```
- ID unique
- Date d'entrée dans le cheptel
- Date de naissance
- Sexe (Mâle/Femelle)
- Lot (Béliers moins 1 an, Béliers plus 1 an, Agnelles de pensions, Béliers adultes de pension)
- Emplacement (Bergerie 1/2, Tunnel 1/2)
- Nom de l'éleveur d'origine
```

### **🌾 Données Nutrition**
```
- Date de distribution
- Emplacement (ou Ensemble)
- Foin en bottes
- Aliment en kilogrammes
```

## 🎯 Fonctionnalités avancées

### **📥 Import d'exemples**
- Bouton **"⬇ Import Exemples"** charge des données de test
- Parfait pour découvrir l'application
- Aucun doublon créé

### **📤 Export CSV**
- Format Excel/LibreOffice compatible
- Toutes les données avec en-têtes
- Nom de fichier avec date automatique

### **🔧 Debug & Diagnostic**
Ouvrez la console navigateur (F12) et utilisez :
```javascript
debugCheptel.animals()    // Voir tous les animaux
debugCheptel.feeding()    // Voir toute la nutrition  
debugCheptel.save()       // Forcer la sauvegarde
debugCheptel.test()       // Remplir formulaire test
```

## 🛠️ Technologies utilisées

- **HTML5** - Structure moderne
- **CSS3** - Design responsive et professionnel
- **JavaScript Vanilla** - Logique métier sans dépendances
- **localStorage** - Sauvegarde locale automatique
- **PWA** - Installation comme application mobile

## 💡 Avantages

### ✅ **Simplicité**
- Interface intuitive et épurée
- Pas de compte utilisateur requis
- Fonctionne hors-ligne

### ✅ **Fiabilité** 
- Sauvegarde automatique à chaque action
- Validation des données obligatoires
- Messages d'erreur clairs

### ✅ **Flexibilité**
- Export pour analyse externe
- Fonctionne sur tous appareils
- Données jamais perdues

### ✅ **Performance**
- Chargement instantané
- Aucune dépendance externe
- Consommation mémoire minimale

## 📱 Compatibilité

### **✅ Navigateurs supportés**
- Chrome/Chromium (recommandé)
- Firefox
- Safari
- Edge

### **✅ Appareils**
- 📱 Smartphones Android/iOS
- 💻 Ordinateurs Windows/Mac/Linux  
- 📱 Tablettes
- 🖥️ Tous écrans (responsive)

## 🔐 Confidentialité & Sécurité

- 🔒 **Données locales uniquement** - Aucun envoi sur internet
- 🏠 **Stockage navigateur** - Vos données restent sur votre appareil
- 🚫 **Aucun tracking** - Respect total de la vie privée
- 💾 **Contrôle total** - Vous gérez vos propres sauvegardes

## 🆘 Support & Dépannage

### **❓ L'animal ne se sauvegarde pas**
1. Vérifiez que les champs obligatoires sont remplis (ID, Lot, Emplacement)
2. Ouvrez la console (F12) pour voir les messages d'erreur
3. Vérifiez que le localStorage n'est pas plein

### **❓ Données perdues**
- Les données sont automatiquement sauvegardées
- En cas de problème, utilisez "Import Exemples" pour redémarrer
- Exportez régulièrement en CSV pour sauvegarder

### **❓ Application lente**
- Videz le cache navigateur
- Vérifiez l'espace disque disponible
- Redémarrez le navigateur

## 🎓 Exemple d'utilisation

### **Scénario typique :**

1. **Matin** : Consultation des statistiques
2. **Arrivée d'animaux** : Ajout avec toutes les infos
3. **Distribution** : Enregistrement des rations
4. **Fin de semaine** : Export CSV pour suivi

### **Données d'exemple incluses :**
```
Animaux:
- 001 : Bélier moins 1 an, Bergerie 1 (Jacques SANTINI)
- 002 : Agnelle de pension, Bergerie 2 (Marie ROSSI)  
- 003 : Bélier plus 1 an, Tunnel 1 (Pierre MARTIN)

Nutrition:
- 20/06/2024 : Bergerie 1, 2 bottes foin, 150kg aliment
- 21/06/2024 : Bergerie 2, 1 botte foin, 100kg aliment
- 22/06/2024 : Ensemble, 3 bottes foin, 250kg aliment
```

## 📞 Contact & Contribution

Cette application est open-source et peut être librement modifiée selon vos besoins spécifiques.

### **🔧 Personnalisation possible :**
- Ajout de nouveaux lots
- Modification des emplacements  
- Nouveaux champs de données
- Interface couleurs/design

---

## 📄 Licence

**MIT License** - Utilisation libre pour usage personnel et commercial.

---

**🐑 Gestion Cheptel Pro** - La solution simple et efficace pour votre élevage ! 

*Version 2.0 - Juin 2024*
