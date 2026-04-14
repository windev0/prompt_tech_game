

# ✅ PROMPT  — VERSION OPTIMISÉE POUR GÉNÉRER L’APPLI TECHGAME

**Titre :** *Créer une application web mobile-first en React nommée TechGame (quiz tech multi‑niveaux)*

## 🎯 **Objectif général**

Créer une application web **mobile-first**, moderne, rapide, nommée **TechGame**, permettant de jouer à un quiz sur la culture technologique.  
Le jeu doit proposer **3 niveaux** :

- Débutant (100 questions)
- Intermédiaire (100 questions)
- Expert (100 questions)

Les questions portent sur :

- les fondateurs d’entreprises tech  
- les créateurs d’outils / langages  
- la reconnaissance de logos  
- l’histoire de la tech  
- les frameworks, outils, protocoles, systèmes  

L’application doit être **entièrement fonctionnelle**, propre, maintenable, et codée en **React + TypeScript + TailwindCSS**.

---

## 📱 **Exigences UI/UX (mobile-first)**

- Design moderne, minimaliste, inspiré des apps mobiles  
- Navigation simple :  
  - Écran d’accueil  
  - Choix du niveau  
  - Quiz  
  - Score final  
- Animations légères (fade, slide)  
- Accessibilité (ARIA, contrastes)  
- Mode sombre automatique  

---

## 🧩 **Fonctionnalités obligatoires**

### 1. Écran d’accueil
- Nom : **TechGame**
- Bouton “Jouer”
- Bouton “Choisir un niveau”

### 2. Choix du niveau
- Débutant  
- Intermédiaire  
- Expert  

### 3. Quiz
- Une question à la fois  
- 3 ou 4 propositions  
- Feedback immédiat  
- Timer optionnel (15s)  
- Score en temps réel  
- Logos affichés via URL  
- Questions mélangées aléatoirement  

### 4. Score final
- Score total  
- Pourcentage  
- Bouton “Rejouer”  
- Bouton **“Partager en image”**  
  - Générer une image (canvas) contenant :  
    - Score  
    - Niveau  
    - Date  
    - Logo TechGame  

### 5. Architecture
- React + TypeScript  
- TailwindCSS  
- Composants réutilisables  
- Dossier `data/` contenant les 300 questions  
- Dossier `utils/` pour :  
  - shuffle  
  - export image  
  - timer  
- Dossier `components/`  
- Dossier `screens/`  

---

## 📚 **Données : 300 questions (100 par niveau)**

### Format JSON attendu

```ts
export interface Question {
  id: number;
  level: "debutant" | "intermediaire" | "expert";
  type: "text" | "image";
  question: string;
  image?: string;
  choices: string[];
  answer: string;
  source: string; // lien wikipedia
}
```

---

## 🖼️ **Ressources logos (SVG officiels)**

### Frameworks / outils
- React : `https://upload.wikimedia.org/wikipedia/commons/a/a7/React-icon.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fa%2Fa7%2FReact-icon.svg")  
- Vue.js : `https://upload.wikimedia.org/wikipedia/commons/9/95/Vue.js_Logo_2.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F95%2FVue.js_Logo_2.svg")  
- Angular : `https://upload.wikimedia.org/wikipedia/commons/c/cf/Angular_full_color_logo.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fc%2Fcf%2FAngular_full_color_logo.svg")  
- Laravel : `https://upload.wikimedia.org/wikipedia/commons/9/9a/Laravel.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F9%2F9a%2FLaravel.svg")  
- Docker : `https://upload.wikimedia.org/wikipedia/commons/4/4e/Docker_%28container_engine%29_logo.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F4%2F4e%2FDocker_%2528container_engine%2529_logo.svg")  
- Kubernetes : `https://upload.wikimedia.org/wikipedia/commons/3/39/Kubernetes_logo_without_workmark.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F3%2F39%2FKubernetes_logo_without_workmark.svg")  
- Node.js : `https://upload.wikimedia.org/wikipedia/commons/d/d9/Node.js_logo.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fd%2Fd9%2FNode.js_logo.svg")  
- Python : `https://upload.wikimedia.org/wikipedia/commons/c/c3/Python-logo-notext.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fc%2Fc3%2FPython-logo-notext.svg")  
- Java : `https://upload.wikimedia.org/wikipedia/en/3/30/Java_programming_language_logo.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fen%2F3%2F30%2FJava_programming_language_logo.svg")  
- Git : `https://upload.wikimedia.org/wikipedia/commons/3/3f/Git_icon.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F3%2F3f%2FGit_icon.svg")  

### Entreprises
- Google : `https://upload.wikimedia.org/wikipedia/commons/2/2f/Google_2015_logo.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F2%2F2f%2FGoogle_2015_logo.svg")  
- Apple : `https://upload.wikimedia.org/wikipedia/commons/f/fa/Apple_logo_black.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Ff%2Ffa%2FApple_logo_black.svg")  
- Microsoft : `https://upload.wikimedia.org/wikipedia/commons/4/44/Microsoft_logo.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F4%2F44%2FMicrosoft_logo.svg")  
- Meta : `https://upload.wikimedia.org/wikipedia/commons/0/05/Meta_Platforms_Inc._logo.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2F0%2F05%2FMeta_Platforms_Inc._logo.svg")  
- Amazon : `https://upload.wikimedia.org/wikipedia/commons/a/a9/Amazon_logo.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fa%2Fa9%2FAmazon_logo.svg")  
- Tesla : `https://upload.wikimedia.org/wikipedia/commons/b/bd/Tesla_Motors.svg` [(upload.wikimedia.org in Bing)](https://www.bing.com/search?q="https%3A%2F%2Fupload.wikimedia.org%2Fwikipedia%2Fcommons%2Fb%2Fbd%2FTesla_Motors.svg")  

---

## 🧠 **Exemples de questions (à générer automatiquement)**

### Débutant (100 questions)
- Qui a fondé Microsoft ?  
- Quel est ce logo ? (React)  
- Qui a créé Facebook ?  
- Quel langage utilise `console.log()` ?  
- Quel est le logo de Docker ?  

### Intermédiaire (100 questions)
- Qui a créé le langage Python ?  
- Quel framework utilise JSX ?  
- Quel outil a été créé par Linus Torvalds ?  
- Quel est ce logo ? (Kubernetes)  
- Qui a fondé Amazon ?  

### Expert (100 questions)
- Qui a créé le protocole TCP/IP ?  
- Quel est le créateur de PostgreSQL ?  
- Quel framework a été créé par Evan You ?  
- Quel est ce logo ? (Kubernetes, Rust, GraphQL…)  
- Qui a fondé Sun Microsystems ?  

---

## 🧱 **Livrables attendus**

1. Code complet React + TypeScript  
2. Architecture propre  
3. 300 questions générées automatiquement  
4. Fonction export du score en image  
5. UI mobile-first  
6. Animations légères  
7. Mode sombre  
8. Application entièrement fonctionnelle  

---

## 🧑‍💻 **Ton rôle**

Tu es un **développeur senior expert en React, TypeScript, UI/UX, architecture front-end**.  
Tu dois produire :

- un code propre  
- maintenable  
- scalable  
- lisible  
- optimisé  

---

## 🏁 **Objectif final**

Générer une application complète **TechGame**, prête à l’emploi, jouable, moderne, mobile-first, avec 300 questions et export du score en image.
