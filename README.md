# 🤖 AI CMD Hub - Mode Claude

Plateforme IA pour analyser des dossiers Python/Code complets et générer du code.

## 🚀 Installation

```bash
git clone https://github.com/Qays67/ai-cmd-hub.git
cd ai-cmd-hub
npm run install-all
```

## 🎯 Utilisation

**Terminal 1 - Backend:**
```bash
npm start
```

**Terminal 2 - Frontend:**
```bash
cd client && npm run dev
```

**Terminal 3 - CLI:**
```bash
npm link
ai-cmd help
```

## 📋 Commandes CLI

```bash
# Créer une IA
ai-cmd create "Mon IA" "Tu es un expert Python"

# Lister les IA
ai-cmd list

# Ajouter un dossier entier
ai-cmd add-folder [AI_ID] /chemin/vers/dossier

# Analyser le dossier
ai-cmd analyze [AI_ID] [FOLDER_ID] "Analyse ce code"

# Générer du code
ai-cmd generate [AI_ID] Python "Crée une fonction pour..."

# Exécuter du Python
ai-cmd exec [AI_ID] "print('Hello')"

# Voir historique
ai-cmd history [AI_ID]

# Supprimer une IA
ai-cmd delete [AI_ID]
```

## 🔌 API Endpoints

- `POST /api/ai/create` - Créer une IA
- `GET /api/ai/list` - Lister les IA
- `POST /api/ai/:id/add-folder` - Ajouter un dossier
- `POST /api/ai/:id/analyze-folder` - Analyser
- `POST /api/ai/:id/generate-code` - Générer du code
- `POST /api/ai/:id/execute-python` - Exécuter Python
- `DELETE /api/ai/:id` - Supprimer

## 💡 Exemple d'utilisation

```bash
# 1. Créer une IA spécialisée
ai-cmd create "CodeAnalyzer" "Tu es expert en optimisation Python"

# 2. Ajouter un dossier de projet
ai-cmd add-folder [ID] ./mon-projet

# 3. Analyser la structure
ai-cmd analyze [ID] [FOLDER_ID] "Identifie les problèmes de performance"

# 4. Générer une solution
ai-cmd generate [ID] Python "Optimise les fonctions lentes"
```

## ⚙️ Configuration

Créer `.env`:
```
PORT=5000
OPENAI_API_KEY=sk-xxx
```

**License:** MIT | Made by Qays67
