# Lexique de l'Intelligence Artificielle

> Glossaire des termes clés de l'IA — réalisé dans le cadre de la formation CFA FORMADU / 2i Academy.

## Sommaire

- [Concepts fondamentaux](#concepts-fondamentaux)
- [Modèles et architectures](#modèles-et-architectures)
- [Entraînement et données](#entraînement-et-données)
- [Usage et interaction](#usage-et-interaction)
- [Outils et écosystème](#outils-et-écosystème)
- [Éthique, limites et réglementation](#éthique-limites-et-réglementation)

---

## Concepts fondamentaux

### Algorithme
Suite finie et non ambiguë d'instructions permettant de résoudre un problème ou d'effectuer un calcul. C'est la base de tout programme informatique, y compris des modèles d'IA.

### Intelligence Artificielle (IA)
Ensemble de techniques permettant à une machine de simuler des capacités cognitives humaines : raisonnement, apprentissage, perception, prise de décision.

### Machine Learning (Apprentissage automatique)
Sous-domaine de l'IA où un système apprend à partir de données, sans être explicitement programmé pour chaque tâche, en identifiant des motifs (patterns) statistiques.

### Deep Learning (Apprentissage profond)
Sous-domaine du Machine Learning basé sur des réseaux de neurones à plusieurs couches ("profonds"), particulièrement efficace pour le traitement d'images, de texte et de son.

### Réseau de Neurones (Neural Network)
Architecture de calcul inspirée du fonctionnement des neurones biologiques, composée de couches de neurones artificiels interconnectés qui transforment progressivement une donnée d'entrée en sortie.

### NLP — Natural Language Processing (Traitement du Langage Naturel)
Branche de l'IA dédiée à la compréhension, l'analyse et la génération du langage humain (texte ou parole) par une machine.

### Test de Turing
Expérience proposée par Alan Turing en 1950 pour évaluer si une machine peut faire preuve d'un comportement intelligent indiscernable de celui d'un humain lors d'une conversation.

### Singularité Technologique
Hypothèse selon laquelle l'IA dépasserait un jour l'intelligence humaine de façon incontrôlable, entraînant des transformations sociétales imprévisibles.

---

## Modèles et architectures

### Modèle
Représentation mathématique entraînée sur des données, capable de produire des prédictions ou des résultats à partir de nouvelles entrées.

### LLM — Large Language Model (Grand Modèle de Langage)
Modèle de deep learning entraîné sur d'immenses volumes de texte, capable de comprendre et générer du langage naturel (ex : GPT, Qwen, Llama, Mistral).

### GPT — Generative Pre-trained Transformer
Famille de modèles de langage développée par OpenAI, basée sur l'architecture Transformer, pré-entraînée puis affinée pour générer du texte.

### Qwen
Famille de LLM open-weight développée par Alibaba Cloud, utilisée notamment pour des déploiements locaux via des outils comme Ollama.

### Transformer
Architecture de réseau de neurones (2017, Google) reposant sur le mécanisme d'"attention", à la base de la quasi-totalité des LLM modernes.

### IA Générative
Catégorie d'IA capable de créer du contenu original (texte, image, son, code) à partir d'un apprentissage sur des données existantes, plutôt que de simplement classer ou prédire.

### IA Adaptative
IA capable d'ajuster son comportement en fonction du contexte, de l'utilisateur ou de retours en temps réel, sans nécessiter un nouvel entraînement complet.

### IA Générale (AGI — Artificial General Intelligence)
IA hypothétique capable d'accomplir n'importe quelle tâche intellectuelle qu'un humain peut réaliser, par opposition aux IA actuelles, spécialisées ("IA faible" ou "narrow AI").

### Agent IA
Système basé sur un LLM capable d'agir de façon autonome : planifier des étapes, utiliser des outils (API, code, recherche web) et accomplir des tâches complexes sans supervision constante.

### ChatBot
Programme conversationnel simulant un dialogue avec un utilisateur, historiquement basé sur des règles, aujourd'hui le plus souvent propulsé par un LLM.

---

## Entraînement et données

### DataSet (Jeu de données)
Ensemble structuré de données utilisé pour entraîner, valider ou tester un modèle d'IA.

### Données
Informations brutes (texte, image, son, chiffres) servant de matière première à l'apprentissage automatique.

### Big Data
Ensembles de données si volumineux, rapides ou variés qu'ils nécessitent des outils spécifiques pour être stockés, traités et analysés.

### Paramètre
Valeur numérique interne à un modèle, ajustée pendant l'entraînement, qui détermine comment il transforme une entrée en sortie. Le nombre de paramètres (ex : 7B, 70B) donne une indication de la taille d'un modèle.

### Token
Unité élémentaire de texte (mot, sous-mot ou caractère) que traite un LLM. Le texte est découpé en tokens avant d'être analysé par le modèle.

### Embedding
Représentation numérique (vecteur) d'un mot, d'une phrase ou d'un document, permettant de capturer son sens et de mesurer sa proximité sémantique avec d'autres contenus.

### Biais (Bias)
Distorsion systématique dans les résultats d'un modèle, souvent héritée des données d'entraînement, pouvant conduire à des résultats injustes ou discriminatoires.

### Fine-tuning (Affinage)
Ré-entraînement partiel d'un modèle pré-entraîné sur un jeu de données spécifique, afin de le spécialiser sur une tâche ou un domaine précis.

---

## Usage et interaction

### Prompt
Texte d'entrée fourni par l'utilisateur à un modèle d'IA générative pour obtenir une réponse ou un contenu.

### SystemPrompt
Instruction initiale, généralement invisible pour l'utilisateur final, définissant le comportement, le rôle et les contraintes d'un modèle avant toute conversation.

### Prompt Engineering
Pratique consistant à concevoir et formuler des prompts de façon précise pour obtenir les meilleurs résultats possibles d'un modèle d'IA.

### Inférence
Phase d'utilisation d'un modèle déjà entraîné : le modèle applique ce qu'il a appris pour produire une réponse à partir d'une nouvelle entrée (par opposition à l'entraînement).

### RAG — Retrieval-Augmented Generation
Technique consistant à enrichir la réponse d'un LLM en allant chercher (retrieval) des informations pertinentes dans une base de connaissances externe avant de générer (generation) la réponse, afin de la rendre plus fiable et à jour.

### Hallucination
Phénomène par lequel un modèle génère une information fausse, incohérente ou inventée, tout en la présentant avec assurance comme si elle était vraie.

### Fenêtre de contexte (Context Window)
Quantité maximale de texte (en tokens) qu'un modèle peut prendre en compte simultanément dans une conversation.

---

## Outils et écosystème

### Ollama
Outil open-source permettant de télécharger, exécuter et gérer des LLM en local, sur sa propre machine, sans dépendre d'un service cloud.

### ModelFile
Fichier de configuration utilisé par Ollama pour définir un modèle personnalisé : modèle de base, paramètres, system prompt, template de conversation.

### API — Application Programming Interface
Interface permettant à un logiciel d'interroger un modèle d'IA (ou tout autre service) de façon standardisée, souvent utilisée pour intégrer l'IA dans une application.

### MCP — Model Context Protocol
Protocole ouvert permettant à un modèle d'IA de se connecter de façon standardisée à des outils et sources de données externes (fichiers, bases de données, applications).

---

## Éthique, limites et réglementation

### European AI Act
Règlement de l'Union Européenne encadrant le développement et l'usage de l'IA selon une approche par niveaux de risque (inacceptable, élevé, limité, minimal), afin de garantir sécurité et droits fondamentaux.

### Zero-shot / Few-shot Learning
Capacité d'un modèle à réaliser une tâche sans exemple préalable (zero-shot) ou avec seulement quelques exemples fournis dans le prompt (few-shot), sans ré-entraînement.

### Surapprentissage (Overfitting)
Défaut d'un modèle qui a "trop bien" appris les données d'entraînement au point de mal généraliser sur de nouvelles données.

---

*Dernière mise à jour : à compléter au fil des ajouts.*
