# Proiect Mini-Scenă 3D: Insula Plutitoare

Acest proiect este o mini-scenă 3D interactivă realizată pentru a demonstra utilizarea conceptelor de bază din grafica pe calculator. Scena reprezintă o "Insulă Plutitoare" (Floating Island) care conține elemente de mediu și arhitectură simplificată (low-poly).

## Tehnologii Utilizate

Proiectul a fost dezvoltat exclusiv cu tehnologii web standard și biblioteci 3D:
* **HTML5 / CSS3:** Pentru structura și stilizarea de bază a paginii web care găzduiește canvas-ul.
* **JavaScript (ES6 Modules):** Limbajul de programare utilizat pentru logica scenei.
* **Three.js:** O bibliotecă JavaScript open-source puternică, folosită pentru a crea și randa grafica 3D în browser prin intermediul WebGL. Am ales Three.js deoarece abstractizează complexitatea WebGL și oferă funcții intuitive pentru lumini, materiale și geometrie.
* **OrbitControls:** Un add-on din ecosistemul Three.js care permite utilizatorului să interacționeze cu scena (zoom, pan, rotate) folosind mouse-ul.

## Structura și Implementarea Scenei

Scena este compusă din următoarele elemente construite din primitive geometrice:
1.  **Baza Insulei & Iarba:** Realizate folosind `CylinderGeometry` cu număr redus de segmente (pentru aspectul low-poly).
2.  **Căsuța:** Construită dintr-un `BoxGeometry` (baza) și un `ConeGeometry` (acoperișul).
3.  **Copacul:** Format dintr-un trunchi (`CylinderGeometry`) și o coroană stilizată (`DodecahedronGeometry`).
4.  **Iluminare:** Am folosit o combinație de `AmbientLight` (pentru a ilumina uniform umbrele) și `DirectionalLight` (pentru a simula lumina soarelui și a genera umbre dinamice).

## Cum se rulează proiectul

Proiectul nu necesită instalarea unor servere locale sau a altor dependențe (librăria Three.js este importată via CDN).
1. Descărcați sau clonați acest repository.
2. Deschideți fișierul `index.html` în orice browser web modern.
3. Folosiți click-stânga pentru a roti camera și scroll-ul pentru zoom.

## Previzualizare

![Screenshot Scena 3D](./screenshot.png)
