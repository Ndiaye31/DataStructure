# 🚀 Pack d'Exercices Avancés - Python Data Structures

## 📋 **Données de Base pour TOUS les Exercices**

```python
# Dataset e-commerce complet
ecommerce_data = [
    {
        "user_id": "U001", "name": "Alice", "age": 25, "city": "Paris",
        "orders": [
            {"order_id": "O1", "date": "2024-01", "items": [("laptop", 999, 1), ("mouse", 25, 2)], "status": "delivered"},
            {"order_id": "O2", "date": "2024-02", "items": [("keyboard", 75, 1)], "status": "pending"},
            {"order_id": "O3", "date": "2024-03", "items": [("monitor", 300, 1), ("webcam", 50, 1)], "status": "delivered"}
        ]
    },
    {
        "user_id": "U002", "name": "Bob", "age": 35, "city": "Lyon", 
        "orders": [
            {"order_id": "O4", "date": "2024-01", "items": [("laptop", 999, 1)], "status": "delivered"},
            {"order_id": "O5", "date": "2024-02", "items": [("mouse", 25, 1), ("pad", 15, 3)], "status": "delivered"}
        ]
    },
    {
        "user_id": "U003", "name": "Charlie", "age": 28, "city": "Paris",
        "orders": [
            {"order_id": "O6", "date": "2024-01", "items": [("keyboard", 75, 2), ("mouse", 25, 1)], "status": "cancelled"},
            {"order_id": "O7", "date": "2024-03", "items": [("laptop", 999, 1), ("monitor", 300, 2)], "status": "delivered"}
        ]
    }
]

# Dataset réseau social
social_network = [
    {"user": "Alice", "posts": [{"content": "Hello world", "likes": 15, "tags": ["tech", "python"]}, 
                                {"content": "Data science rocks", "likes": 23, "tags": ["data", "ml"]}],
     "following": ["Bob", "Diana"], "followers": ["Bob", "Charlie", "Eve"]},
    {"user": "Bob", "posts": [{"content": "Morning coffee", "likes": 8, "tags": ["life"]},
                              {"content": "Python tutorial", "likes": 45, "tags": ["tech", "python", "tutorial"]}],
     "following": ["Alice", "Charlie"], "followers": ["Alice", "Frank"]},
    {"user": "Charlie", "posts": [{"content": "Weekend vibes", "likes": 12, "tags": ["life", "weekend"]}],
     "following": ["Alice"], "followers": ["Alice", "Bob"]}
]
```

---

## 🔥 **SECTION 1: LIST COMPREHENSIONS AVANCÉES**

### **Ex 1.1 - Triple Nested (★★★☆☆)**
Extrayez tous les produits achetés par des utilisateurs parisiens avec quantité > 1, format: `[("Alice", "mouse", 2), ...]`

### **Ex 1.2 - Conditional Logic (★★★★☆)**
Calculez le "score de fidélité" par utilisateur: `nombre_commandes * 10 + total_dépensé * 0.1`, mais seulement pour les utilisateurs avec au moins 2 commandes livrées.

### **Ex 1.3 - Complex Filtering (★★★★★)**
Trouvez les utilisateurs qui ont commandé le même produit dans différentes commandes (détection de récurrence d'achat).

---

## 🏆 **SECTION 2: NESTED DATA MANIPULATION**

### **Ex 2.1 - Matrix Operations (★★★☆☆)**
Créez une matrice user×produit avec les quantités totales achetées par chaque utilisateur pour chaque produit unique.

### **Ex 2.2 - Social Graph (★★★★☆)**
À partir du dataset réseau social, créez un dictionnaire de "mutual connections" : `{"Alice": ["Bob"], "Bob": ["Alice"], ...}`

### **Ex 2.3 - Engagement Analysis (★★★★★)**
Calculez le "taux d'engagement" par tag : `moyenne_likes_posts_avec_ce_tag / moyenne_likes_tous_posts * 100`

---

## 🎯 **SECTION 3: SET OPERATIONS & DEDUPLICATION**

### **Ex 3.1 - Customer Segmentation (★★★☆☆)**
Identifiez les clients qui ont acheté des produits en commun (intersection des achats).

### **Ex 3.2 - Recommendation Engine (★★★★☆)**
Pour chaque utilisateur, trouvez les produits achetés par des utilisateurs similaires (même ville) qu'il n'a pas encore achetés.

### **Ex 3.3 - Influence Network (★★★★★)**
Calculez le "degré de séparation" entre tous les utilisateurs du réseau social (qui suit qui, directement ou indirectement).

---

## 📊 **SECTION 4: TUPLE & NAMED TUPLE MASTERY**

### **Ex 4.1 - Data Indexing (★★★☆☆)**
Créez un système d'indexation : tuple `(user_id, order_id, item_index)` pour accéder rapidement à n'importe quel item.

### **Ex 4.2 - Temporal Analysis (★★★★☆)**
Analysez l'évolution temporelle des achats : `[(mois, nombre_commandes, chiffre_affaires), ...]` triés chronologiquement.

### **Ex 4.3 - Advanced Sorting (★★★★★)**
Triez les utilisateurs par critères multiples : 1) Total dépensé, 2) Nombre de commandes, 3) Ancienneté (première commande).

---

## 🚀 **SECTION 5: INTEGRATION CHALLENGES**

### **Ex 5.1 - Data Pipeline (★★★★☆)**
Créez un pipeline de transformation : raw_data → clean_data → aggregated_data → insights, tout en list comprehensions.

### **Ex 5.2 - Real-time Analytics (★★★★★)**
Simulez un système de métriques temps réel : calculez simultanément 5 KPIs différents en une seule comprehension.

### **Ex 5.3 - Memory Optimization (★★★★★)**
Réimplémentez vos solutions précédentes en optimisant pour la mémoire (générateurs, lazy evaluation).

---

## 🎮 **SECTION 6: GAMIFICATION CHALLENGES**

### **Ex 6.1 - Treasure Hunt (★★★☆☆)**
Cachez des "trésors" dans vos structures de données. Créez des énigmes basées sur les patterns de données.

### **Ex 6.2 - Speed Challenge (★★★★☆)**
Résolvez 3 problèmes en moins de 10 lignes de code chacun, avec performance optimale.

### **Ex 6.3 - Code Golf (★★★★★)**
Version ultra-compacte : résolvez des problèmes complexes en 1 seule ligne de comprehension (lisibilité vs concision).

---

## 🏅 **DÉFI FINAL BOSS**

### **Ex BOSS - Master Data Engineer (★★★★★)**
Créez un système complet d'analyse e-commerce qui :
1. Détecte les anomalies (commandes suspectes)
2. Prédit les prochains achats (pattern matching)
3. Optimise l'inventaire (analyse de demande)
4. Segmente les clients (clustering basique)
5. Génère un rapport exécutif (top insights)

**Contrainte :** Maximum 20 lignes de code, structures de données Python pures uniquement.

---

## 📈 **SYSTÈME DE SCORING**

- **★☆☆☆☆** : 10 points
- **★★☆☆☆** : 20 points  
- **★★★☆☆** : 30 points
- **★★★★☆** : 50 points
- **★★★★★** : 100 points
- **BOSS** : 200 points

**Bonus :**
- Code élégant : +10 points
- Solution alternative : +15 points
- Optimisation performance : +20 points
- Créativité exceptionnelle : +25 points

**Total possible : 1000+ points** 🎯

---

## 🎯 **STRATÉGIE RECOMMANDÉE**

1. **Échauffement** : Commencez par Section 1 (★★★☆☆)
2. **Montée en puissance** : Sections 2-3 (★★★★☆)
3. **Expertise** : Sections 4-5 (★★★★★)
4. **Fun & Challenge** : Section 6 + BOSS

**Prêt(e) pour l'aventure ?** 🚀