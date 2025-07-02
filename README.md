# Pourquoi c'est problématique ? – Site Collaboratif

Bienvenue sur le site Pourquoi c'est problématique ? Ce site a pour but de référencer les idées problématique et d’y répondre de façon claire, sourcée et pédagogique.

---

## 🚀 Contribuer au site

Ce projet est **ouvert à toutes et tous** ! Tu peux participer simplement en ajoutant une nouvelle question ou en améliorant les réponses existantes.

### Comment contribuer ?

1. **Fork** ce dépôt depuis GitHub.

2. **Ajoute ta question** dans un nouveau fichier Markdown (`.md`) dans le dossier [`src/content/questions/`](./src/content/questions).

   - Respecte la structure frontmatter (exemple ci-dessous) :

   ```md
   ---
   title: "Titre clair de ta question"
   shortAnswer: "Une réponse courte qui résume la réponse."
   sources:
     - label: "Nom de la source"
       url: "https://lien-vers-la-source"
   nextQuestion:
     label: "Titre d’une question liée"
     url: "/q/slug-question-liée"
   ---

   Ici, tu peux écrire ta réponse détaillée en Markdown, avec des titres, listes, liens, etc.
3. **Enregistre ton fichier** avec un nom clair en minuscule, sans espaces, par exemple racisme-inverse.md.

4. **Teste ta question** pour vérifier qu’elle s’affiche bien :

    - **Option simple (sans installation) :**
    Tu peux utiliser un visualiseur Markdown en ligne, comme Dillinger ou StackEdit, pour vérifier que ton fichier s’affiche correctement (titres, liens, listes, etc.).
    Attention : cette méthode ne montre pas la mise en forme exacte du site, mais permet de s’assurer que le Markdown est bien formé.

    - **Option avancée (recommandée)** :
    Si tu te sens à l’aise avec un peu de technique, tu peux tester ta question directement dans le site :

        1. Clone le dépôt en local sur ton ordinateur.

        2. Installe Node.js si ce n’est pas déjà fait (https://nodejs.org).

        3. Ouvre un terminal, navigue dans le dossier du projet et lance :
            ``` sh
            npm install
            npm run dev
            ```

        4. Ouvre ton navigateur à l’adresse indiquée (souvent http://localhost:4321).

        5. Vérifie que ta question apparaît bien dans la liste ou à l’URL correspondante (/q/nom-de-ta-question).

        6. Si tu rencontres un souci, vérifie la syntaxe Markdown et la structure frontmatter.

5. **Crée une Pull Request** vers la branche principale (main ou master) de ce dépôt.

## 📚 Règles de bonne conduite

- **Sois factuel·ve et précis·e** : base tes réponses sur des sources fiables et reconnues.

- **Évite les propos offensants ou polémiques** : ce site vise à informer et apaiser les débats.

- **Reste concis·e et clair·e,** les réponses doivent être accessibles à tous·tes.

- **Merci d’indiquer au moins une source vérifiable** dans le frontmatter.

## 🛠️ Pour les développeur·se·s

Le site est construit avec Astro et utilise les fichiers Markdown pour générer les pages automatiquement.

- Les questions sont dans src/content/questions/*.md.

- Les pages sont générées dynamiquement à partir des fichiers Markdown.

- Le style utilise Tailwind CSS avec DaisyUI pour l’interface.

## 🙏 Merci pour ta contribution !

Chaque nouvelle question enrichit le site et aide à mieux comprendre et combattre le racisme au quotidien.