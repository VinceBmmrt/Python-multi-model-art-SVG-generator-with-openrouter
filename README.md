# Python SVG Generator with LLMs

This is a fun experimentation project that generates SVGs line by line using Large Language Models (LLMs). Unlike traditional image generators, here the AI writes each line of SVG code, giving fine-grained control and allowing for unlimited creativity.

## What is an SVG?

SVG (Scalable Vector Graphics) is a text-based format that describes vector images. It is made of XML tags, each representing a graphical element, for example:

Each tag has attributes that define its position, size, color, or other properties. 
In this project, the idea is to let an LLM write these lines like a digital artist drawing directly the blueprint of an image.

The subject to be drawn by the LLMs is stored in the variable `challenge`, which can be modified to test different prompts; by default, it is set to "Two cute cats as astronauts floating in space with stars and planets".
## Features

* Line-by-line SVG generation using multiple LLMs
* Easy comparison of models to see who draws the best
* Supports an effort parameter to influence output quality and detail
* Easy access to many models via OpenRouter

## 🎥 Demo

▶️ **[Watch the demo video](https://drive.google.com/file/d/1mCsMcy6Y04P0nWZOMaPZjusnDz_K5rbo/view?usp=sharing)**

---

## Example Usage

choose your LLM model, optionally set an effort level, and then generate the SVG. Each model produces the SVG as if an artist was drawing line by line.

## Available Models

* `openai/gpt-oss-120b`
* `openai/gpt-5-nano` (supports effort)
* `deepseek/deepseek-v3.2`
* `moonshotai/kimi-k2-thinking`
* `x-ai/grok-4.1-fast`
* `anthropic/claude-opus-4.5`
* `openai/gpt-5.2` (supports effort)
* `google/gemini-3-pro-preview`


---
## 🛠 Installation

1. Clone this repository to your local machine:
```bash
   git clone <repository-url>
   cd <repository-name>
```

2. Install **uv** from Astral:

3. Install project dependencies and synchronize environment:
```bash
   uv sync
```

4. Set up your environment variables:
   - Create a `.env` file in the project root
   - Add your OpenRouter API key:
```
     OPENROUTER_API_KEY=your-api-key-here
```

5. Run the project:
```bash
   uv run svg_generator.py
```

---


# Francais

# Générateur SVG Python avec LLMs

Il s'agit d'un projet d'expérimentation amusant qui génère des SVG ligne par ligne en utilisant de grands modèles de langage (LLMs). Contrairement aux générateurs d'images traditionnels, ici l'IA écrit chaque ligne de code SVG, offrant un contrôle précis et permettant une créativité illimitée.

## Qu'est-ce qu'un SVG ?

SVG (Scalable Vector Graphics) est un format textuel qui décrit des images vectorielles. Il est composé de balises XML, chacune représentant un élément graphique, par exemple :
Chaque balise possède des attributs qui définissent sa position, sa taille, sa couleur ou d'autres propriétés.

Dans ce projet, l'idée est de laisser un LLM écrire ces lignes comme un artiste numérique dessinant directement le plan d'une image.

## Fonctionnalités

* Génération SVG ligne par ligne utilisant plusieurs LLMs
* Comparaison facile des modèles pour voir qui dessine le mieux
* Support d'un paramètre d'effort pour influencer la qualité et le détail de la sortie
* Accès facile à de nombreux modèles via OpenRouter


## Exemple d'utilisation
Le sujet que les LLM vont dessiner est stocké dans la variable `challenge`, modifiable pour tester différents prompts ; par défaut, elle est définie sur "Two cute cats as astronauts floating in space with stars and planets".

Choisissez votre modèle LLM, définissez éventuellement un niveau d'effort, puis générez le SVG. Chaque modèle produit le SVG comme si un artiste dessinait ligne par ligne.

## Modèles disponibles

* `openai/gpt-oss-120b`
* `openai/gpt-5-nano` (supporte l'effort)
* `deepseek/deepseek-v3.2`
* `moonshotai/kimi-k2-thinking`
* `x-ai/grok-4.1-fast`
* `anthropic/claude-opus-4.5`
* `openai/gpt-5.2` (supporte l'effort)
* `google/gemini-3-pro-preview`
