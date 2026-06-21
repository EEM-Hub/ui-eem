---
source: sources/wiki-Gesture_recognition.md
source_url: https://en.wikipedia.org/wiki/Gesture_recognition
---

## Gesture Recognition in Human-Computer Interaction

Gesture recognition is a field within computer science and computer vision that uses mathematical algorithms to detect, interpret, and classify human gestures — primarily from hands and faces — enabling touchless interaction with computing devices. It spans input methods from camera-based tracking to wearable sensors, with applications in gaming, sign language translation, home automation, defense, and consumer electronics.

## Key Concepts

- **Gesture recognition** is a subdiscipline of computer vision that interprets human body language computationally, going beyond traditional text or GUI interfaces.
- **Two gesture types in interfaces**: *offline gestures* (processed after interaction completes, e.g., drawing a circle to open a menu) and *online gestures* (real-time direct manipulation, e.g., pinch-to-zoom, rotate).
- **Touchless User Interface (TUI)**: device control via body motion/gestures without physical contact with any input surface.
- **Kinetic User Interface (KUI)**: interaction through motion of objects and bodies (e.g., Wii, Kinect).
- **3D model-based approaches** use volumetric or skeletal models to represent body parts in 3D space; computationally expensive but geometrically rich.
- **Skeletal-based algorithms** simplify 3D models to joint angles and segment lengths — faster, suitable for real-time analysis, and enable pattern matching against template databases.
- **Appearance-based models** derive parameters directly from images/video using template matching (e.g., deformable 2D templates, silhouettes, contours); easier to process but less generalizable.
- **Electromyography (EMG)-based models** classify gestures from electrical signals produced by muscles; advantage is no camera requirement, enabling greater freedom of movement.
- Key pointers are typically represented in a **3D coordinate system**, and gesture detection accuracy depends on input quality and algorithm design.

## Commands and Syntax

No CLI commands or configuration syntax — this is a conceptual/theoretical domain. Key technical procedures include:

- **Depth map generation**: Use structured-light or time-of-flight cameras to produce short-range 3D representations for hand gesture detection.
- **Stereo camera calibration**: Establish spatial relationship between two cameras using a positioning reference (e.g., infrared emitter) to approximate 3D scene geometry.
- **Skeletal tracking pipeline**: Compute virtual skeleton → map body parts to segments → analyze joint angles and segment orientations → classify gesture.
- **Template matching (appearance-based)**: Capture binary silhouette or contour image → compare against hand/gesture template database → infer matching gesture.
- **EMG classification**: Capture muscle electrical signals via wearable band → classify arm muscle activation patterns → map to gesture input.

## Relationships

- **Computer vision / Image processing**: Parent disciplines providing the foundational techniques (tracking, pose estimation, feature extraction).
- **Sign language translation**: Major application area; Kinect-based systems have been used for real-time sign language recognition.
- **Emotion recognition**: Overlapping subfield that derives emotional state from facial expressions and hand gestures.
- **Activity recognition / Pose estimation**: Broader fields that gesture recognition feeds into and draws from (articulated body pose estimation, 3D pose estimation).
- **Augmented/Virtual Reality**: Skeletal hand tracking is actively developed for AR/VR interaction without controllers.
- **HCI and form factors**: Gesture recognition connects to mobile device design, wearable computing, and public installation interaction paradigms, each with distinct social acceptability constraints.
- **Wi-Fi sensing**: Emerging non-visual approach to gesture detection using wireless signal perturbation.

## Exam-Relevant Points

- **Offline vs. online gestures**: Offline = post-interaction processing (e.g., context menu activation); Online = real-time direct manipulation (e.g., scaling, rotating).
- **Three main algorithmic approaches**: 3D model-based (volumetric/skeletal), appearance-based (template matching from images), and EMG-based (muscle signal classification).
- **Skeletal models are preferred for real-time** because they use fewer parameters (joint angles + segment lengths) than volumetric models, which require intensive computation of complex 3D surfaces (NURBS, polygon meshes).
- **Appearance-based models trade generality for simplicity** — easier to process than 3D models but typically lack the generalization needed for robust HCI.
- **EMG advantage over vision-based**: User does not need to face a camera; non-invasive wearable bands connect via Bluetooth.
- **Key input devices**: Wired gloves (DataGlove was first commercial), depth-aware cameras (structured light / time-of-flight), stereo cameras, gesture-based controllers, single 2D cameras, Wi-Fi sensing, mouse gesture tracking.
- **Major challenges**: Image noise, inconsistent lighting, background clutter, occlusions (partial/full), camera variability, distance/resolution effects, and **social acceptability** of performing gestures in public.
- **Arm fatigue ("gorilla arm")** contributed to the decline of early touch-screen interfaces in the 1980s; measured via a technique called **Consumed Endurance**.
- **Social acceptability factors**: Gestures resembling natural/everyday actions are more accepted; body placement matters (forearm/wrist most acceptable for wearables; waist/groin least acceptable).
