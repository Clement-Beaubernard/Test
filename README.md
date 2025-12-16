Projet K
Test 2
Équipe : Antoine, Clément, Simon, Eliott

Objectif : Développer un outil de génération de fichiers 3D modifiables et exportables pour l’impression 3D.

Fonctionnalités principales :
* Utilisation d’un prompt ou d’un plan dessiné, avec nécessité de fournir les côtes.
* Possibilité pour l’utilisateur de modifier le plan soit via un prompt, soit directement avec des ajouts de fonctionnalités principales et faciles d’utilisation.

Considérations de plateforme :
* Déterminer si l’outil sera un site web ou une application.
* Intégrer un système d’inscription.
* S’assurer de la compréhension de l’outil, même en cas de fautes d’orthographe.

Plan :
1. Convertir le prompt ou le plan en géométrie paramétrique.
2. Détecter les primitives et identifier les paramètres.
3. L’utilisateur saisit un prompt ou importe un plan.
4. L’IA analyse les paramètres géométriques.
5. L’outil génère un modèle paramétrique (script CAD).
6. Le modèle est construit et affiché.
7. L’utilisateur modifie le modèle via des commandes ou des sliders.
8. Exportation vers les formats STL ou STEP pour l’impression 3D.

Technologie :
* CadQuery est une bibliothèque Python open-source permettant de créer des modèles 3D paramétriques. Elle présente l’avantage de créer des modèles CAO 1 en BREP.

Recommandations technologiques (Chatgpt) :
* Lecture du prompt : LLM (API Chatgpt, Llama, etc.)
* Analyse du plan (dessin) : Vision OCR + détection de contours (OpenCV + modèle personnalisé)
* Moteur géométrique : CadQuery / OpenCascade
* Génération de code paramétrique : Python
* Exportation : STEP, STL

Précision :
* Travailler en millimètres, standard pour l’impression 3D.

Performance :
* Optimiser le maillage (< 100 000 triangles pour STL).

Expérience utilisateur :
* Offrir un retour visuel immédiat sur les modifications.
Validation : Vérifiez toujours que le modèle est « manifold » (étanche).
Utilisation des coordonnées pour la 3D.
Comprendre le schéma
