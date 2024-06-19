# Essais avec MediaPipe

## Introduction

[MediaPipe](https://ai.google.dev/edge/mediapipe/solutions/guide?hl=fr) est un environnement permettant notamment d'appliquer rapidement des techniques d'intelligence artificielle (IA) et de machine learning (ML).

Installation :
```python
pip install mediapipe
```

Les programmes proposés font aussi appel à [Opencv](https://pypi.org/project/opencv-python/), donnant accès à la gestion et au tratement des images et des vidéos.

Installation :
```python
pip install opencv-python
```
 
Les programmmes mentionnés ci-après sont dans le fichier archive [mediapipe.zip](Data/mediapipe.zip) (dossier Data).

Dans ce fichier archive :
- dossier **code** : les programmes Python lançant les exemples
- dossier **images_vidéos** : quelques images et vidéos pour tester les méthodes
- dossier **tflite_task** : les fichiers fournis par MediaPipe pour construire les détecteurs

## Les exemples

### Mode d'emploi sommaire

Après avoir lançé les programmes décris ci-après, on obtient à quelques détails près l'affichage ci-dessous.

```python
INFO: Created TensorFlow Lite XNNPACK delegate for CPU.
Choisir la source :
0 : webcam0
1 : webcam1
2 : fichier image
3 : fichier video
```

On peut alors choisir une source vidéo directe (webcam) ou un fichier image ou vidéo.

### Détection de visages

[Description](https://ai.google.dev/edge/mediapipe/solutions/vision/face_detector/python?hl=fr)

Programme à lancer
```python
python faces_visu.py
```

### Reconnaissance de gestes

[Description](https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker/python?hl=fr)

Programme à lancer
```python
python mains_visu.py
```

### Détection d'objets

[Description](https://ai.google.dev/edge/mediapipe/solutions/vision/object_detector/python?hl=fr)

Programme à lancer
```python
python objets_visu.py
```

### Détection des points de repère sur le visages

[Description](https://ai.google.dev/edge/mediapipe/solutions/vision/face_landmarker/python?hl=fr)

Programme à lancer
```python
python visage_visu.py
```
