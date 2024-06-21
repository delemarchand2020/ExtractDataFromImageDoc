Le notebook "PoC_extraction_avec_VLM.ipynb" met en œuvre le modèle VLM de Microsoft, Phi3-Vision, pour l'extraction de données depuis des images de documents. 
Voici les détails :

1. **Installation des librairies** nécessaires telles que `torch` et `transformers`.
2. **Chargement des images** au format .png.
3. **Configuration et chargement du modèle** : Le modèle `microsoft/Phi-3-vision-128k-instruct` est configuré pour une quantization en 4 bits, prête à être utilisée si nécessaire, bien que non essentielle avec un GPU L4 sur Google Colab.
4. **Inférence** : La fonction `model_inference` gère l'extraction de texte à partir des images, préparant les entrées pour le modèle et exécutant l'extraction. Les résultats sont ensuite décodés.
5. **Tests d'extraction** : Des tests sont effectués sur différentes images pour démontrer l'efficacité du modèle à extraire les informations.

**Termes techniques** :
- **OCR** : Processus de conversion d'images de texte en texte codé par machine.
- **Quantization** : Réduction de la précision des nombres pour optimiser les performances, utilisable en certaines circonstances.
- **VLM**: "Vision Language Model". C'est un type de modèle d'intelligence artificielle qui combine des techniques de vision par ordinateur et de traitement du langage naturel pour comprendre et générer des réponses en se basant sur des entrées visuelles et textuelles. Ces modèles sont entraînés sur de vastes ensembles de données comprenant des images et des descriptions textuelles, leur permettant de réaliser des tâches comme la description d'images, l'extraction de données textuelles à partir d'images, et la réponse à des questions basées sur le contenu visuel.
