# Hand Gesture Detection and Finger Counting

The application detects hand landmarks in real-time from a webcam feed and counts the number of fingers raised on each hand. It uses the Mediapipe `Hands` module for detecting hand landmarks and OpenCV for displaying the results.

## Features

- Detect hand landmarks in images and real-time videos.
- Count the number of fingers raised for each hand.
- Draw hand landmarks and connections on the processed video frames.
- Visualize results using OpenCV and Matplotlib for images.

## Requirements

Before running the project, make sure you have the following dependencies installed:

- **OpenCV :** Utilisé pour le traitement d'images et de vidéos en temps réel, notamment pour capturer et manipuler des flux vidéo provenant de la webcam.
- **MediaPipe :** Fournit des solutions d'apprentissage automatique, ici utilisé pour la détection des mains et des landmarks (points de repère) sur les mains pour compter les doigts.
- **Pygame :** Une bibliothèque multimédia utilisée pour ajouter du son ou d'autres interactions à l'application. Cependant, elle n'est pas utilisée directement dans le script donné.
- **Matplotlib :** Utilisé pour afficher les images traitées, notamment pour visualiser les résultats des détections et des transformations.
- **Numpy :** Utilisé pour des opérations mathématiques et manipulation efficace de tableaux multidimensionnels, particulièrement avec les images.

## Project Structure

- `detectHandsLandmarks()` : Detects and draws hand landmarks on images or video frames.
- `countFingers()` : Counts the number of fingers raised for each detected hand.
- Webcam real-time feed using OpenCV to process video frames.

## How it works

- **Hand Detection:** The MediaPipe Hands model is initialized to detect hand landmarks in both static images and video.
- **Landmark Visualization:** The landmarks are drawn on top of the hand using OpenCV's drawing utilities.
- **Finger Counting:** The script identifies the position of each finger's tip and compares it with the corresponding joint landmark to determine whether the finger is raised or folded.
