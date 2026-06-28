# BET261 Predictor

Application web de prédiction intelligente pour les paris sportifs basée sur l'IA.

## 🚀 Démarrage rapide

### Installation locale

```bash
# Cloner le repository
git clone https://github.com/nomenan97-sys/Virtualisation.git
cd Virtualisation
git checkout bet261-predictor

# Créer un environnement virtuel
python -m venv venv
source venv/bin/activate  # Sur Windows: venv\Scripts\activate

# Installer les dépendances
pip install -r requirements.txt

# Lancer l'application
python app.py
```

L'application sera disponible sur `http://localhost:5000`

### Déploiement sur Render

1. Fork ce repository
2. Aller sur [render.com](https://render.com)
3. Créer un nouveau "Web Service"
4. Connecter votre repository
5. L'application se déploiera automatiquement avec la configuration `render.yaml`

## 📋 Fonctionnalités

- 🎯 Prédiction basée sur l'IA
- 📊 Analyse des cotes
- 💰 Calcul du retour sur investissement
- 📱 Interface responsive
- 🚀 Déploiement facile

## 🛠️ Technologies

- **Backend**: Flask (Python 3.11)
- **Frontend**: HTML5, CSS3, JavaScript
- **Deployment**: Render, Gunicorn

## 📦 Requirements

- Python 3.11+
- Flask >= 3.0
- Gunicorn >= 21.2

## 🔧 Configuration

### Variables d'environnement

Créer un fichier `.env` pour les configurations locales :

```
FLASK_ENV=development
DEBUG=True
```

## 📝 API Endpoints

### POST /api/predict

Fait une prédiction basée sur les paramètres fournis.

**Request:**
```json
{
  "team1": "Manchester United",
  "team2": "Liverpool",
  "odds1": 1.5,
  "odds2": 2.5,
  "betAmount": 100
}
```

**Response:**
```json
{
  "status": "success",
  "prediction": "Équipe 1 gagne",
  "confidence": 0.85
}
```

### GET /health

Vérifier l'état de l'application.

## 🤝 Contribution

Les contributions sont les bienvenues ! N'hésitez pas à ouvrir une issue ou une pull request.

## 📄 Licence

Ce projet est sous licence MIT - voir le fichier [LICENSE](LICENSE) pour plus de détails.

## 👨‍💻 Auteur

Créé par [nomenan97-sys](https://github.com/nomenan97-sys)

---

⭐ Si vous trouvez ce projet utile, n'oubliez pas de lui donner une étoile !
