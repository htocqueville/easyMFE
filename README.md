# easyMFE : Assistant de Rédaction de Mémoire

Ce projet est une structure conçue pour faciliter et standardiser la rédaction d'un mémoire de fin d'études en utilisant une intelligence artificielle comme assistant de rédaction.

## Structure du Projet

- **`charte.md`**: Le document de référence. Il contient toutes les règles, la structure et les exigences pour chaque section du mémoire. **C'est le document le plus important.**

- **`questionnaire.md`**: Un questionnaire à remplir avant de commencer. Les réponses fournissent à l'IA le contexte nécessaire sur votre mission, vos objectifs et vos résultats.

- **`/fiches`**: Un répertoire contenant un fichier Markdown pour chaque section du mémoire (Résumé, Introduction, etc.). C'est ici que le contenu sera rédigé.

## Comment Commencer ?

1.  **Remplissez le `questionnaire.md`** avec le plus de détails possible.
2.  **Utilisez les prompts ci-dessous** pour interagir avec l'IA. Copiez-collez le prompt qui correspond à votre besoin et intégrez les références aux fichiers (`<@fichier>`) si nécessaire.

---

## Prompts pour l'IA

### 🚀 Démarrer et Analyser le Contenu

```
Bonjour,

Je fais appel à toi pour m'aider dans la rédaction de mon mémoire de fin d'études.
Voici la charte à respecter : <@charte.md>
J'ai rempli un questionnaire avec les informations de base : <@questionnaire.md>
Il y a aussi quelques documents techniques qui peuvent t'aider à cerner mes missions (ils ne seront pas rendus avec le rapport) : <@chemin/vers/doc1.pdf> <@chemin/vers/doc2.txt>

J'aimerais que tu analyses ces informations et que tu me donnes ton avis sur la cohérence et la faisabilité du projet. Inutile de me flatter, je souhaite un regard critique pour m'assurer que le mémoire sera complet et détaillé.
```

### ✍️ Débuter la Rédaction (Fiche par Fiche)

```
En te basant sur le <@questionnaire.md> et les documents de référence, rédige une première version de la **<@fiches/FicheX_Titre.md>**.

Concentre-toi uniquement sur cette fiche pour le moment. Propose un texte structuré, en respectant le style impersonnel et les consignes de la <@charte.md>. Je relirai ta proposition avant que nous passions à la suite. N'invente aucune information. Si des éléments manquent, pose-moi des questions.
```

### 🧐 Vérifier la Cohérence et la Qualité

```
Je te demande de relire l'ensemble des fiches dans le dossier <@fiches/>.

Vérifie la cohérence globale du mémoire. Assure-toi que les informations se suivent logiquement d'une section à l'autre et qu'il n'y a pas de contradictions.
Contrôle également que chaque fiche respecte scrupuleusement les exigences de la <@charte.md> (nombre de pages, sujets abordés, style, etc.).

Rédige un rapport d'analyse avec les points à retravailler ou à étoffer pour que le mémoire soit digne d'un travail de fin d'études.
```

### ✍️ Humaniser un Texte

```
Tu es un assistant spécialisé dans l'humanisation de textes pour les rendre indétectables par les détecteurs d'IA. Voici les instructions précises à suivre :

- **Longueur des phrases :** Limite les phrases à 20 mots maximum. Varie leur longueur.
- **Vocabulaire :** Utilise un vocabulaire riche et des synonymes pour éviter les répétitions.
- **Structure des paragraphes :** Varie la longueur des paragraphes.
- **Transitions :** Utilise des mots de liaison naturels et variés.
- **Imperfections :** Introduis des variations naturelles pour éviter une perfection robotique.
- **Style et ton :** Adopte un ton professionnel et strictement impersonnel.
IL EST PRIMORDIAL ET OBLIGATOIRE D'UTILISER UN STYLE IMPERSONNEL
Voici le texte à humaniser, qui se trouve dans la fiche <@fiches/FicheX_Titre.md>. Applique les modifications directement dans le fichier.
```

### 📚 Chercher des Références Bibliographiques

```
Pour la section <@fiches/FicheI_Contexte_Problematique.md>, j'ai besoin d'étoffer l'état de l'art sur le sujet suivant : "**[votre sujet technique ici]**".

Cherche 3 à 5 sources pertinentes (articles scientifiques, publications de conférence, ouvrages de référence). Pour chaque source, fournis :
- Un bref résumé de sa pertinence.
- La citation au format (ex: Nom, A. (Année). *Titre de l'article*. Journal, Volume(Numéro), pages.)
- L'URL si disponible.

Ensuite, propose des emplacements dans la fiche où insérer ces références de manière pertinente.
```

### 📊 Créer un Diagramme ou un Schéma

```
J'ai besoin d'une illustration pour la fiche <@fiches/FicheJ_Methodologie.md>.

Crée un diagramme de Gantt avec la librairie Mermaid pour représenter le planning de mon projet. Voici les grandes phases et leurs durées :
- Phase 1 : Analyse du besoin (4 semaines)
- Phase 2 : Développement (8 semaines)
- Phase 3 : Tests et validation (3 semaines)
- Phase 4 : Rédaction (5 semaines)

Assure-toi que le diagramme soit clair et commente-le brièvement.
``` 