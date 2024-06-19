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

Après avoir lançé les programmes fournis, on obtient à quelques détails près l'affichage ci-dessous.

```python
INFO: Created TensorFlow Lite XNNPACK delegate for CPU.
Choisir la source :
0 : webcam0
1 : webcam1
2 : fichier image
3 : fichier video
```

### Détection de visages

https://ai.google.dev/edge/mediapipe/solutions/vision/face_detector/python?hl=fr

```python
python faces_visu.py
```

```python
INFO: Created TensorFlow Lite XNNPACK delegate for CPU.
Choisir la source :
0 : webcam0
1 : webcam1
2 : fichier image
3 : fichier video
```


### Reconnaissance de gestes

https://ai.google.dev/edge/mediapipe/solutions/vision/hand_landmarker/python?hl=fr

```python
python mains_visu.py
```

```python
INFO: Created TensorFlow Lite XNNPACK delegate for CPU.
Choisir la source :
0 : webcam0
1 : webcam1
2 : fichier image
3 : fichier video
```

### Détection d'objets

https://ai.google.dev/edge/mediapipe/solutions/vision/object_detector/python?hl=fr

```python
python objets_visu.py
```

```python
INFO: Created TensorFlow Lite XNNPACK delegate for CPU.
Choisir la source :
0 : webcam0
1 : webcam1
2 : fichier image
3, 4, 5 : fichier video
```

### Détection des points de repère sur le visages

https://ai.google.dev/edge/mediapipe/solutions/vision/face_landmarker/python?hl=fr


```python
python visage_visu.py
```

```python
WARNING: Logging before InitGoogleLogging() is written to STDERR
W20240619 16:49:42.567196 10260 face_landmarker_graph.cc:168] Face blendshape model contains CPU only ops. Sets FaceBlendshapesGraph acceleration to Xnnpack.
INFO: Created TensorFlow Lite XNNPACK delegate for CPU.
Choisir la source :
0 : webcam0
1 : webcam1
2 : fichier image
3 : fichier video
```


