---
source: https://en.wikipedia.org/wiki/Gesture_recognition
fetched: 2026-06-20
---

Topic in computer science and language technology 
|  | This article'stone or style may not reflect theencyclopedic toneused on Wikipedia.See Wikipedia'sguide to writing better articlesfor suggestions.(November 2016)(Learn how and when to remove this message) |
| --- | --- |

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/d/de/Gesture_Recognition.jpg/330px-Gesture_Recognition.jpg)](./File:Gesture_Recognition.jpg)A child's hand location and movement being detected by a gesture recognition algorithm 

**Gesture recognition** is an area of research and development in [computer science](./Computer_science) and [language technology](./Language_technology) concerned with the recognition and interpretation of human [gestures](./Gesture). A subdiscipline of [computer vision](./Computer_vision),[*[citation needed](./Wikipedia:Citation_needed)*] it employs mathematical [algorithms](./Algorithm) to interpret gestures.[[1]](./Gesture_recognition#cite_note-Kobylarz-1)

 

Gesture recognition offers a path for computers to begin to better understand and interpret [human body language](./Computer_processing_of_body_language), previously not possible through [text](./Text_user_interface) or unenhanced [graphical user interfaces](./Graphical_user_interfaces) (GUIs).

 

Gestures can originate from any bodily motion or state, but commonly originate from the [face](./Face) or [hand](./Hand). One area of the field is [emotion recognition](./Emotion_recognition) derived from facial expressions and hand gestures. Users can make simple gestures to control or interact with devices without physically touching them.

 

Many approaches have been made using cameras and [computer vision](./Computer_vision) algorithms to interpret [sign language](./Sign_language), however, the identification and recognition of posture, gait, [proxemics](./Proxemics), and human behaviors is also the subject of gesture recognition techniques.[[2]](./Gesture_recognition#cite_note-2)

 

## Overview

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/9/91/Linux_kernel_and_gaming_input-output_latency.svg/330px-Linux_kernel_and_gaming_input-output_latency.svg.png)](./File:Linux_kernel_and_gaming_input-output_latency.svg)Middleware usually processes gesture recognition, then sends the results to the user. 

Gesture recognition has application in such areas as:

 
- Automobiles
- Consumer electronics
- Transit
- Gaming
- Handheld devices
- Defense[[3]](./Gesture_recognition#cite_note-3)
- [Home automation](./Home_automation)
- [Automated sign language translation](./Automated_sign_language_translation)[[4]](./Gesture_recognition#cite_note-4)

 

Gesture recognition can be conducted with techniques from [computer vision](./Computer_vision) and [image processing](./Image_processing).[[5]](./Gesture_recognition#cite_note-5)

 

The literature includes ongoing work in the computer vision field on capturing gestures or more general human [pose](./Pose_(computer_vision)) and movements by cameras connected to a computer.[[6]](./Gesture_recognition#cite_note-6)[[7]](./Gesture_recognition#cite_note-7)[[8]](./Gesture_recognition#cite_note-8)[[9]](./Gesture_recognition#cite_note-9)

 

The term "gesture recognition" has been used to refer more narrowly to non-text-input handwriting symbols, such as inking on a [graphics tablet](./Graphics_tablet), [multi-touch](./Multi-touch) gestures, and [mouse gesture](./Mouse_gesture) recognition. This is computer interaction through the drawing of symbols with a pointing device cursor.[[10]](./Gesture_recognition#cite_note-10)[[11]](./Gesture_recognition#cite_note-11)[[12]](./Gesture_recognition#cite_note-12) [Pen computing](./Pen_computing) expands digital gesture recognition beyond traditional input devices such as keyboards and mice, and reduces the hardware impact of a system.[*[how?](./Wikipedia:Please_clarify)*]

 

## Gesture types

 

In computer interfaces, two types of gestures are distinguished:[[13]](./Gesture_recognition#cite_note-13) We consider online gestures, which can also be regarded as direct manipulations like scaling and rotating, and in contrast, offline gestures are usually processed after the interaction is finished; e. g. a circle is drawn to activate a [context menu](./Context_menu).

 
- Offline gestures: Those gestures that are processed after the user's interaction with the object. An example is a gesture to activate a menu.
- Online gestures: Direct manipulation gestures. They are used to scale or rotate a tangible object.

 

## Touchless interface

 

A touchless user interface (TUI) is an emerging type of technology wherein a device is controlled via body motion and gestures without touching a keyboard, mouse, or screen.[[14]](./Gesture_recognition#cite_note-14)

 

### Types of touchless technology

 

There are several devices utilizing this type of interface such as smartphones, laptops, games, TVs, and music equipment.

 

One type of touchless interface uses the Bluetooth connectivity of a smartphone to activate a company's visitor management system. This eliminates having to touch an interface, for convenience or to avoid a potential source of contamination as during the [COVID-19 pandemic](./COVID-19_pandemic).[[15]](./Gesture_recognition#cite_note-15)

 

## Input devices

 

The ability to track a person's movements and determine what gestures they may be performing can be achieved through various tools. Kinetic user interfaces (KUIs) are an emerging type of [user interfaces](./User_interfaces) that allow users to interact with computing devices through the motion of objects and bodies.[*[citation needed](./Wikipedia:Citation_needed)*] Examples of KUIs include [tangible user interfaces](./Tangible_user_interface) and motion-aware games such as [Wii](./Wii) and Microsoft's [Kinect](./Kinect), and other interactive projects.[[16]](./Gesture_recognition#cite_note-16)

 

Although there is a large amount of research done in image/video-based gesture recognition, there is some variation in the tools and environments used between implementations.

 
- [Wired gloves](./Wired_glove). These can provide input to the computer about the position and rotation of the hands using magnetic or inertial tracking devices. Furthermore, some gloves can detect finger bending with a high degree of accuracy (5-10 degrees), or even provide haptic feedback to the user, which is a simulation of the sense of touch. The first commercially available hand-tracking glove-type device was the DataGlove,[[17]](./Gesture_recognition#cite_note-17) a glove-type device that could detect hand position, movement and finger bending. This uses fiber optic cables running down the back of the hand. Light pulses are created and when the fingers are bent, light leaks through small cracks and the loss is registered, giving an approximation of the hand pose.
- Depth-aware cameras. Using specialized cameras such as [structured light](./Structured_light) or [time-of-flight cameras](./Time-of-flight_camera), one can generate a [depth map](./Depth_map) of what is being seen through the camera at a short-range, and use this data to approximate a 3D representation of what is being seen. These can be effective for the detection of hand gestures due to their short-range capabilities.[[18]](./Gesture_recognition#cite_note-18)
- [Stereo cameras](./Stereo_cameras). Using two cameras whose relations to one another are known, a 3D representation can be approximated by the output of the cameras. To get the cameras' relations, one can use a positioning reference such as a [lexian-stripe](./Lexian-stripe?action=edit&redlink=1) or [infrared](./Infrared) emitter.[[19]](./Gesture_recognition#cite_note-19) In combination with direct motion measurement ([6D-Vision](./Stereoscopy#Stereoscopic_motion_measurement_(6D-Vision))) gestures can directly be detected.
- Gesture-based controllers. These controllers act as an extension of the body so that when gestures are performed, some of their motion can be conveniently captured by the software. An example of emerging gesture-based [motion capture](./Motion_capture) is skeletal [hand tracking](./Hand_tracking), which is being developed for [augmented reality](./Augmented_reality) and [virtual reality](./Virtual_reality) applications. An example of this technology is shown by tracking companies [uSens](./USens) and [Gestigon](./Gestigon), which allow users to interact with their surroundings without controllers.[[20]](./Gesture_recognition#cite_note-20)[[21]](./Gesture_recognition#cite_note-21)
- [Wi-Fi sensing](./Wi-Fi_sensing)[[22]](./Gesture_recognition#cite_note-22)
- [Mouse gesture](./Mouse_gesture) tracking, where the motion of the mouse is correlated to a symbol being drawn by a person's hand which can study changes in acceleration over time to represent gestures.[[23]](./Gesture_recognition#cite_note-23)[[24]](./Gesture_recognition#cite_note-24)[[25]](./Gesture_recognition#cite_note-25)  The software also compensates for human tremor and inadvertent movement.[[26]](./Gesture_recognition#cite_note-Wong-26)[[27]](./Gesture_recognition#cite_note-Cousins-27)[[28]](./Gesture_recognition#cite_note-TechJournal-28)  The sensors of these smart light-emitting cubes can be used to sense hands and fingers as well as other objects nearby, and can be used to process data. Most applications are in music and sound synthesis,[[29]](./Gesture_recognition#cite_note-29) but can be applied to other fields.
- **Single camera**. A standard 2D camera can be used for gesture recognition where the resources/environment would not be convenient for other forms of image-based recognition. Earlier it was thought that a single camera may not be as effective as stereo or depth-aware cameras, but some companies are challenging this theory. Software-based gesture recognition technology using a standard 2D camera that can detect robust hand gestures. [*[citation needed](./Wikipedia:Citation_needed)*]

 

## Algorithms

 [![](//upload.wikimedia.org/wikipedia/en/thumb/d/df/BigDiagram2.jpg/500px-BigDiagram2.jpg)](./File:BigDiagram2.jpg)Some alternative methods of tracking and analyzing gestures, and their respective relationships 

Depending on the type of input data, the approach for interpreting a gesture could be done in different ways. However, most of the techniques rely on key pointers represented in a 3D coordinate system. Based on the relative motion of these, the gesture can be detected with high accuracy, depending on the quality of the input and the algorithm's approach.[[30]](./Gesture_recognition#cite_note-30)

 

In order to interpret movements of the body, one has to classify them according to common properties and the message the movements may express. For example, in sign language, each gesture represents a word or phrase.

 

Some literature differentiates 2 different approaches in gesture recognition: a 3D model-based and an appearance-based.[[31]](./Gesture_recognition#cite_note-31) The foremost method makes use of 3D information on key elements of the body parts in order to obtain several important parameters, like palm position or joint angles. Approaches derived from it such as the volumetric models have proven to be very intensive in terms of computational power and require further technological developments in order to be implemented for real-time analysis. Alternately, appearance-based systems use images or videos for direct interpretation. Such models are easier to process, but usually lack the generality required for human-computer interaction.

 

### 3D model-based algorithms

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/9/99/Volumetric-hands.jpg/250px-Volumetric-hands.jpg)](./File:Volumetric-hands.jpg)A real hand (left) is interpreted as a collection of vertices and lines in the 3D mesh version (right), and the software uses their relative position and interaction in order to infer the gesture. 

The 3D model approach can use volumetric or skeletal models or even a combination of the two. Volumetric approaches have been heavily used in the computer animation industry and for computer vision purposes. The models are generally created from complicated 3D surfaces, like NURBS or polygon meshes.

 

The drawback of this method is that it is very computationally intensive, and systems for real-time analysis are still to be developed. For the moment, a more interesting approach would be to map simple primitive objects to the person's most important body parts (for example cylinders for the arms and neck, sphere for the head) and analyze the way these interact with each other. Furthermore, some abstract structures like [super-quadrics](./Superquadrics) and [ generalized cylinders](./Cylinder_(geometry)) maybe even more suitable for approximating the body parts.

  

### Skeletal-based algorithms

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/d/d8/Skeletal-hand.jpg/250px-Skeletal-hand.jpg)](./File:Skeletal-hand.jpg)The skeletal version (right) is effectively modeling the hand (left). This has fewer parameters than the volumetric version and it's easier to compute, making it suitable for real-time gesture analysis systems. 

Instead of using intensive processing of the 3D models and dealing with a lot of parameters, one can just use a simplified version of joint angle parameters along with segment lengths. This is known as a skeletal representation of the body, where a virtual skeleton of the person is computed and parts of the body are mapped to certain segments. The analysis here is done using the position and orientation of these segments and the relation between each one of them( for example the angle between the joints and the relative position or orientation)

 

Advantages of using skeletal models:

 
- Algorithms are faster because only key parameters are analyzed.
- Pattern matching against a template database is possible
- Using key points allows the detection program to focus on the significant parts of the body

  

### Appearance-based models

 [![](//upload.wikimedia.org/wikipedia/commons/thumb/7/7b/Appearance_hands.jpg/250px-Appearance_hands.jpg)](./File:Appearance_hands.jpg)These binary silhouette(left) or contour(right) images represent typical input for appearance-based algorithms. They are compared with different hand templates and if they match, the correspondent gesture is inferred. 

Appearance-based models no longer use a spatial representation of the body, instead deriving their parameters directly from the images or videos using a template database. Some are based on the deformable 2D templates of the human parts of the body, particularly the hands. Deformable templates are sets of points on the outline of an object, used as interpolation nodes for the object's outline approximation. One of the simplest interpolation functions is linear, which performs an average shape from point sets, point variability parameters, and external deformation. These template-based models are mostly used for hand-tracking, but could also be used for simple gesture classification.

 

The second approach in gesture detection using appearance-based models uses image sequences as gesture templates. Parameters for this method are either the images themselves, or certain features derived from these. Most of the time, only one (monoscopic) or two (stereoscopic) views are used.

  

### Electromyography-based models

 

[Electromyography](./Electromyography) (EMG) concerns the study of electrical signals produced by muscles in the body. Through classification of data received from the arm muscles, it is possible to classify the action and thus input the gesture to external software.[[1]](./Gesture_recognition#cite_note-Kobylarz-1) Consumer EMG devices allow for non-invasive approaches such as an arm or leg band and connect via Bluetooth. Due to this, EMG has an advantage over visual methods since the user does not need to face a camera to give input, enabling more freedom of movement.

 

## Challenges

 

There are many challenges associated with the accuracy and usefulness of gesture recognition and software designed to implement it. For image-based gesture recognition, there are limitations on the equipment used and [image noise](./Image_noise). Images or video may not be under consistent lighting, or in the same location. Items in the background or distinct features of the users may make recognition more difficult.

 

The variety of implementations for image-based gesture recognition may also cause issues with the viability of the technology for general usage. For example, an algorithm calibrated for one camera may not work for a different camera.  The amount of background noise also causes tracking and recognition difficulties, especially when occlusions (partial and full) occur.  Furthermore, the distance from the camera, and the camera's resolution and quality, also cause variations in recognition accuracy.

 

In order to capture human gestures by visual sensors robust computer vision methods are also required, for example for hand tracking and hand posture recognition[[32]](./Gesture_recognition#cite_note-32)[[33]](./Gesture_recognition#cite_note-33)[[34]](./Gesture_recognition#cite_note-34)[[35]](./Gesture_recognition#cite_note-35)[[36]](./Gesture_recognition#cite_note-36)[[37]](./Gesture_recognition#cite_note-37)[[38]](./Gesture_recognition#cite_note-38)[[39]](./Gesture_recognition#cite_note-39)[[40]](./Gesture_recognition#cite_note-40)[*[excessive citations](./Wikipedia:Citing_sources#Bundling_citations)*] or for capturing movements of the head, facial expressions or gaze direction.

 

### Social acceptability

 

One significant challenge to the adoption of gesture interfaces on consumer mobile devices such as smartphones and smartwatches stems from the social acceptability implications of gestural input. While gestures can facilitate fast and accurate input on many novel form-factor computers, their adoption and usefulness are often limited by social factors rather than technical ones. To this end, designers of gesture input methods may seek to balance both technical considerations and user willingness to perform gestures in different social contexts.[[41]](./Gesture_recognition#cite_note-:0-41) In addition, different device hardware and sensing mechanisms support different kinds of recognizable gestures.

 

#### Mobile device

 

Gesture interfaces on [mobile](./Mobile_device) and small [form-factor](./Form-factor) devices are often supported by the presence of motion sensors such as [inertial measurement units](./Inertial_measurement_unit) (IMUs). On these devices, gesture sensing relies on users performing movement-based gestures capable of being recognized by these motion sensors. This can potentially make capturing signals from subtle or low-motion gestures challenging, as they may become difficult to distinguish from natural movements or noise. Through a survey and study of gesture usability, researchers found that gestures that incorporate subtle movement, which appear similar to existing technology, look or feel similar to every action, and are enjoyable were more likely to be accepted by users, while gestures that look strange, are uncomfortable to perform, interfere with communication, or involve uncommon movement caused users more likely to reject their usage.[[41]](./Gesture_recognition#cite_note-:0-41) The social acceptability of mobile device gestures relies heavily on the naturalness of the gesture and social context.

 

#### On-body and wearable computers

 

[Wearable computers](./Wearable_computer) typically differ from traditional [mobile devices](./Mobile_device) in that their usage and interaction location takes place on the user's body. In these contexts, gesture interfaces may become preferred over traditional input methods, as their small size renders [touch-screens](./Touchscreen) or [keyboards](./Computer_keyboard) less appealing. Nevertheless, they share many of the same social acceptability obstacles as mobile devices when it comes to gestural interaction. However, the possibility of wearable computers being hidden from sight or integrated into other everyday objects, such as clothing, allow gesture input to mimic common clothing interactions, such as adjusting a shirt collar or rubbing one's front pant pocket.[[42]](./Gesture_recognition#cite_note-Walter_2013-42)[[43]](./Gesture_recognition#cite_note-:1-43) A major consideration for wearable computer interaction is the location for device placement and interaction. A study exploring third-party attitudes towards wearable device interaction conducted across the United States and South Korea found differences in the perception of wearable computing use of males and females, in part due to different areas of the body considered socially sensitive.[[43]](./Gesture_recognition#cite_note-:1-43) Another study investigating the social acceptability of on-body projected interfaces found similar results, with both studies labelling areas around the waist, groin, and upper body (for women) to be least acceptable while areas around the forearm and wrist to be most acceptable.[[44]](./Gesture_recognition#cite_note-44)

 

#### Public installations

 

[Public Installations](./Interactive_kiosk), such as interactive public displays, allow access to information and displays interactive media in public settings such as museums, galleries, and theaters.[[45]](./Gesture_recognition#cite_note-:2-45) While touch screens are a frequent form of input for public displays, gesture interfaces provide additional benefits such as improved hygiene, interaction from a distance, and improved discoverability, and may favor performative interaction.[[42]](./Gesture_recognition#cite_note-Walter_2013-42) An important consideration for gestural interaction with public displays is the high probability or expectation of a spectator audience.[[45]](./Gesture_recognition#cite_note-:2-45)

 

### Fatigue

 

Arm fatigue was a side-effect of vertically oriented touch-screen or light-pen use. In periods of prolonged use, users' arms began to feel fatigued and/or discomfort. This effect contributed to the decline of touch-screen input despite its initial popularity in the 1980s.[[46]](./Gesture_recognition#cite_note-46)[[47]](./Gesture_recognition#cite_note-47)

 

In order to measure arm fatigue side effect, researchers developed a technique called Consumed Endurance.[[48]](./Gesture_recognition#cite_note-48)[[49]](./Gesture_recognition#cite_note-49)

 

## See also

 
- [Activity recognition](./Activity_recognition)
- [Articulated body pose estimation](./Articulated_body_pose_estimation)
- [Automotive head unit](./Automotive_head_unit)
- [Computer processing of body language](./Computer_processing_of_body_language)
- [3D pose estimation](./3D_pose_estimation)
- [Pointing device gesture](./Pointing_device_gesture)

 

## References

 
1. [1](./Gesture_recognition#cite_ref-Kobylarz_1-0) [2](./Gesture_recognition#cite_ref-Kobylarz_1-1) Kobylarz, Jhonatan; Bird, Jordan J.; Faria, Diego R.; Ribeiro, Eduardo Parente; Ekárt, Anikó (2020-03-07). ["Thumbs up, thumbs down: non-verbal human-robot interaction through real-time EMG classification via inductive and supervised transductive transfer learning"](https://publications.aston.ac.uk/id/eprint/41366/1/Kobylarz2020_Article_ThumbsUpThumbsDownNon_verbalHu.pdf) (PDF). *Journal of Ambient Intelligence and Humanized Computing*. **11** (12). Springer Science and Business Media LLC: 6021–6031. [doi](./Doi_(identifier)):[10.1007/s12652-020-01852-z](https://doi.org/10.1007%2Fs12652-020-01852-z). [ISSN](./ISSN_(identifier)) [1868-5137](https://search.worldcat.org/issn/1868-5137).
2. [↑](./Gesture_recognition#cite_ref-2) Matthias Rehm, Nikolaus Bee, Elisabeth André, [Wave Like an Egyptian – Accelerometer Based Gesture Recognition for Culture Specific Interactions](http://mm-werkstatt.informatik.uni-augsburg.de/files/publications/199/wave_like_an_egyptian_final.pdf), British Computer Society, 2007
3. [↑](./Gesture_recognition#cite_ref-3) ["Patent Landscape Report Hand Gesture Recognition PatSeer Pro"](https://web.archive.org/web/20230324224629/https://patseer.com/case-study-auto-categorization-of-hand-gesture-recognition-patents-using-patseers-ai-classifier/). *PatSeer*. Archived from the original on 2023-03-24. Retrieved 2017-11-02.`{{cite news}}`:  CS1 maint: bot: original URL status unknown ([link](./Category:CS1_maint:_bot:_original_URL_status_unknown))
4. [↑](./Gesture_recognition#cite_ref-4) Chai, Xiujuan, et al. "[Sign language recognition and translation with kinect](http://iip.ict.ac.cn/sites/default/files/publication/2013_FG_xjchai_Sign%20Language%20Recognition%20and%20Translation%20with%20Kinect.pdf) [Archived](https://web.archive.org/web/20210110035036/http://iip.ict.ac.cn/sites/default/files/publication/2013_FG_xjchai_Sign%20Language%20Recognition%20and%20Translation%20with%20Kinect.pdf) 2021-01-10 at the [Wayback Machine](./Wayback_Machine)." IEEE Conf. on AFGR. Vol. 655. 2013.
5. [↑](./Gesture_recognition#cite_ref-5) Sultana A, Rajapuspha T (2012),
 ["Vision Based Gesture Recognition for Alphabetical Hand Gestures Using the SVM Classifier"](https://pdfs.semanticscholar.org/2c11/h.pdf)[*[permanent dead link](./Wikipedia:Link_rot)*], International Journal of Computer Science & Engineering Technology (IJCSET)., 2012
6. [↑](./Gesture_recognition#cite_ref-6) Pavlovic, V., Sharma, R. & Huang, T. (1997), ["Visual interpretation of hand gestures for human-computer interaction: A review"](https://www.cs.rutgers.edu/~vladimir/pub/pavlovic97pami.pdf), IEEE Transactions on Pattern Analysis and Machine Intelligence, July, 1997. Vol. 19(7), pp. 677 -695.
7. [↑](./Gesture_recognition#cite_ref-7) R. Cipolla and A. Pentland, [Computer Vision for Human-Machine Interaction](https://books.google.com/books?id=Pe7gG0LxEUIC&q=pentland+cipolla+computer+vision+human+interaction), Cambridge University Press, 1998, [ISBN](./ISBN_(identifier)) [978-0-521-62253-0](./Special:BookSources/978-0-521-62253-0)
8. [↑](./Gesture_recognition#cite_ref-8) Ying Wu and Thomas S. Huang,
["Vision-Based Gesture Recognition: A Review"](http://reference.kfupm.edu.sa/content/v/i/vision_based_gesture_recognition__a_revi_291732.pdf) [Archived](https://web.archive.org/web/20110825211203/http://reference.kfupm.edu.sa/content/v/i/vision_based_gesture_recognition__a_revi_291732.pdf) 2011-08-25 at the [Wayback Machine](./Wayback_Machine), In: Gesture-Based Communication in Human-Computer Interaction, Volume 1739 of Springer Lecture Notes in Computer Science, pages 103-115, 1999, [ISBN](./ISBN_(identifier)) [978-3-540-66935-7](./Special:BookSources/978-3-540-66935-7), [doi](./Doi_(identifier)):[10.1007/3-540-46616-9](https://doi.org/10.1007%2F3-540-46616-9)
9. [↑](./Gesture_recognition#cite_ref-9) Alejandro Jaimes and Nicu Sebe,
[Multimodal human–computer interaction: A survey](http://staff.science.uva.nl/~nicu/PUBS/PDF/2005/sebeHCI05.pdf) [Archived](https://web.archive.org/web/20110606063605/http://staff.science.uva.nl/~nicu/PUBS/PDF/2005/sebeHCI05.pdf) 2011-06-06 at the [Wayback Machine](./Wayback_Machine),
Computer Vision and Image Understanding
Volume 108, Issues 1-2, October–November 2007, Pages 116-134
Special Issue on Vision for Human-Computer Interaction, [doi](./Doi_(identifier)):[10.1016/j.cviu.2006.10.019](https://doi.org/10.1016%2Fj.cviu.2006.10.019)
10. [↑](./Gesture_recognition#cite_ref-10) Dopertchouk, Oleg; ["Recognition of Handwriting Gestures"](http://www.gamedev.net/page/resources/_/technical/game-programming/recognition-of-handwritten-gestures-r2039), *gamedev.net*, January 9, 2004
11. [↑](./Gesture_recognition#cite_ref-11) Chen, Shijie; ["Gesture Recognition Techniques in Handwriting Recognition Application"](https://ieeexplore.ieee.org/xpls/abs_all.jsp?arnumber=5693514&tag=1), *Frontiers in Handwriting Recognition* p 142-147 November 2010
12. [↑](./Gesture_recognition#cite_ref-12) Balaji, R; Deepu, V; Madhvanath, Sriganesh; Prabhakaran, Jayasree ["Handwritten Gesture Recognition for Gesture Keyboard"](http://www.hpl.hp.com/india/documents/papers/GKB_IWFHR10_Final.pdf) [Archived](https://web.archive.org/web/20080906122710/http://www.hpl.hp.com/india/documents/papers/GKB_IWFHR10_Final.pdf) 2008-09-06 at the [Wayback Machine](./Wayback_Machine), *Hewlett-Packard Laboratories*
13. [↑](./Gesture_recognition#cite_ref-13) Dietrich Kammer, Mandy Keck, Georg Freitag, Markus Wacker, [Taxonomy and Overview of Multi-touch Frameworks: Architecture, Scope, and Features](http://vi-c.de/vic/sites/default/files/Taxonomy_and_Overview_of_Multi-touch_Frameworks_Revised.pdf) [Archived](https://web.archive.org/web/20110125014444/http://vi-c.de/vic/sites/default/files/Taxonomy_and_Overview_of_Multi-touch_Frameworks_Revised.pdf) 2011-01-25 at the [Wayback Machine](./Wayback_Machine)
14. [↑](./Gesture_recognition#cite_ref-14) ["touchless user interface Definition from PC Magazine Encyclopedia"](https://www.pcmag.com/encyclopedia/term/62816/touchless-user-interface). *pcmag.com*. Retrieved 2017-07-28.
15. [↑](./Gesture_recognition#cite_ref-15) Iqbal, Muhammad Zahid; Campbell, Abraham G. (2020). ["The emerging need for touchless interaction technologies"](https://www.researchgate.net/publication/342134613). *ResearchGate*. Retrieved 2021-06-30.
16. [↑](./Gesture_recognition#cite_ref-16) S. Benford; H. Schnadelbach; B. Koleva; B. Gaver; A. Schmidt; A. Boucher; A. Steed; R. Anastasi; C. Greenhalgh; T. Rodden; H. Gellersen (2003). ["Sensible, sensable and desirable: a framework for designing physical interfaces"](https://web.archive.org/web/20060126085052/http://www.equator.ac.uk/var/uploads/benfordTech2003.pdf) (PDF). [CiteSeerX](./CiteSeerX_(identifier)) [10.1.1.190.2504](https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.190.2504). Archived from [the original](http://www.equator.ac.uk/var/uploads/benfordTech2003.pdf) (PDF) on January 26, 2006. `{{cite journal}}`: Cite journal requires `|journal=` ([help](./Help:CS1_errors#missing_periodical))
17. [↑](./Gesture_recognition#cite_ref-17) Thomas G. Zimmerman, Jaron Lanier, Chuck Blanchard, Steve Bryson, and Young Harvill. [http://portal.acm.org](http://portal.acm.org). "[A HAND GESTURE INTERFACE DEVICE](http://netzspannung.org/cat/servlet/CatServlet/$files/228648/DataGlove+CHI+1987.pdf) [Archived](https://web.archive.org/web/20111002031500/http://netzspannung.org/cat/servlet/CatServlet/$files/228648/DataGlove+CHI+1987.pdf) 2011-10-02 at the [Wayback Machine](./Wayback_Machine)." [http://portal.acm.org](http://portal.acm.org).
18. [↑](./Gesture_recognition#cite_ref-18) Yang Liu, Yunde Jia, [A Robust Hand Tracking and Gesture Recognition Method for Wearable Visual Interfaces and Its Applications](https://ieeexplore.ieee.org/abstract/document/1410485/), Proceedings of the Third International Conference on Image and Graphics (ICIG'04), 2004
19. [↑](./Gesture_recognition#cite_ref-19) Kue-Bum Lee, Jung-Hyun Kim, Kwang-Seok Hong, [An Implementation of Multi-Modal Game Interface Based on PDAs](https://ieeexplore.ieee.org/abstract/document/4297013/), Fifth International Conference on Software Engineering Research, Management and Applications, 2007
20. [↑](./Gesture_recognition#cite_ref-20) ["Gestigon Gesture Tracking - TechCrunch Disrupt"](https://techcrunch.com/video/gestigon-gesture-tracking/517762030/). *TechCrunch*. Retrieved 11 October 2016.
21. [↑](./Gesture_recognition#cite_ref-21) Matney, Lucas (29 August 2016). ["uSens shows off new tracking sensors that aim to deliver richer experiences for mobile VR"](https://techcrunch.com/2016/08/29/usens-unveils-vr-sensor-modules-with-hand-tracking-and-mobile-positional-tracking-tech-baked-in/). *TechCrunch*. Retrieved 29 August 2016.
22. [↑](./Gesture_recognition#cite_ref-22) Khalili, Abdullah; Soliman, Abdel-Hamid; Asaduzzaman, Md; Griffiths, Alison (March 2020). ["Wi-Fi sensing: applications and challenges"](https://doi.org/10.1049%2Fjoe.2019.0790). *The Journal of Engineering*. **2020** (3): 87–97. [arXiv](./ArXiv_(identifier)):[1901.00715](https://arxiv.org/abs/1901.00715). [doi](./Doi_(identifier)):[10.1049/joe.2019.0790](https://doi.org/10.1049%2Fjoe.2019.0790). [ISSN](./ISSN_(identifier)) [2051-3305](https://search.worldcat.org/issn/2051-3305).
23. [↑](./Gesture_recognition#cite_ref-23) Per Malmestig, Sofie Sundberg, [SignWiiver – implementation of sign language technology](http://www.tricomsolutions.com/academic_reports.html) [Archived](https://web.archive.org/web/20081225190059/http://www.tricomsolutions.com/academic_reports.html) 2008-12-25 at the [Wayback Machine](./Wayback_Machine)
24. [↑](./Gesture_recognition#cite_ref-24) Thomas Schlomer, Benjamin Poppinga, Niels Henze, Susanne Boll, [Gesture Recognition with a Wii Controller](http://www.wiigee.com/download_files/gesture_recognition_with_a_wii_controller-schloemer_poppinga_henze_boll.pdf) [Archived](https://web.archive.org/web/20130727175427/http://www.wiigee.com/download_files/gesture_recognition_with_a_wii_controller-schloemer_poppinga_henze_boll.pdf) 2013-07-27 at the [Wayback Machine](./Wayback_Machine), Proceedings of the 2nd international Conference on Tangible and Embedded interaction, 2008
25. [↑](./Gesture_recognition#cite_ref-25) AiLive Inc., [LiveMove White Paper](http://www.ailive.net/papers/LiveMoveWhitePaper_en.pdf) [Archived](https://web.archive.org/web/20070713013109/http://www.ailive.net/papers/LiveMoveWhitePaper_en.pdf) 2007-07-13 at the [Wayback Machine](./Wayback_Machine), 2006
26. [↑](./Gesture_recognition#cite_ref-Wong_26-0) *Electronic Design* September 8, 2011. William Wong. [Natural User Interface Employs Sensor Integration.](http://electronicdesign.com/article/embedded/Natural-User-Interface-Employs-Sensor-Integration.aspx)
27. [↑](./Gesture_recognition#cite_ref-Cousins_27-0) *Cable & Satellite International* September/October, 2011. Stephen Cousins. [A view to a thrill.](http://www.csimagazine.com/csi/A-view-to-a-thrill.php) [Archived](https://web.archive.org/web/20120119075325/http://www.csimagazine.com/csi/A-view-to-a-thrill.php) 2012-01-19 at the [Wayback Machine](./Wayback_Machine)
28. [↑](./Gesture_recognition#cite_ref-TechJournal_28-0) *TechJournal South* January 7, 2008. [Hillcrest Labs rings up $25M D round.](https://archive.today/20120401173137/http://www.techjournalsouth.com/2008/01/hillcrest-labs-rings-up-25m-d-round/)
29. [↑](./Gesture_recognition#cite_ref-29) *Percussa AudioCubes Blog* October 4, 2012. [Gestural Control in Sound Synthesis.](http://www.percussa.com/2012/10/04/gestural-control-of-sound-synthesis-featured-question/) [Archived](https://web.archive.org/web/20150910063754/https://www.percussa.com/2012/10/04/gestural-control-of-sound-synthesis-featured-question) 2015-09-10 at the [Wayback Machine](./Wayback_Machine)
30. [↑](./Gesture_recognition#cite_ref-30) Mamtaz Alam; Dileep Kumar Tiwari (2016). ["Gesture Recognization & its Applications"](https://rgdoi.net/10.13140/RG.2.2.28139.54563). [doi](./Doi_(identifier)):[10.13140/RG.2.2.28139.54563](https://doi.org/10.13140%2FRG.2.2.28139.54563). `{{cite journal}}`: Cite journal requires `|journal=` ([help](./Help:CS1_errors#missing_periodical))
31. [↑](./Gesture_recognition#cite_ref-31) Vladimir I. Pavlovic, Rajeev Sharma, Thomas S. Huang, [Visual Interpretation of Hand Gestures for Human-Computer Interaction](https://www.cs.rutgers.edu/~vladimir/pub/pavlovic97pami.pdf); A Review, IEEE Transactions on Pattern Analysis and Machine Intelligence, 1997
32. [↑](./Gesture_recognition#cite_ref-32) Ivan Laptev and Tony Lindeberg ["Tracking of Multi-state Hand Models Using Particle Filtering and a Hierarchy of Multi-scale Image Features"](http://kth.diva-portal.org/smash/record.jsf?pid=diva2%3A440686&dswid=-2803), Proceedings Scale-Space and Morphology in Computer Vision, Volume 2106 of Springer Lecture Notes in Computer Science, pages 63-74, Vancouver, BC, 1999. [ISBN](./ISBN_(identifier)) [978-3-540-42317-1](./Special:BookSources/978-3-540-42317-1), [doi](./Doi_(identifier)):[10.1007/3-540-47778-0](https://doi.org/10.1007%2F3-540-47778-0)
33. [↑](./Gesture_recognition#cite_ref-33) von Hardenberg, Christian; Bérard, François (2001). "Bare-hand human-computer interaction". *Proceedings of the 2001 workshop on Perceptive user interfaces*. ACM International Conference Proceeding Series. Vol. 15 archive. Orlando, Florida. pp. 1–8. [CiteSeerX](./CiteSeerX_(identifier)) [10.1.1.23.4541](https://citeseerx.ist.psu.edu/viewdoc/summary?doi=10.1.1.23.4541).
34. [↑](./Gesture_recognition#cite_ref-34) Lars Bretzner, Ivan Laptev, Tony Lindeberg ["Hand gesture recognition using multi-scale colour features, hierarchical models and particle filtering"](http://kth.diva-portal.org/smash/record.jsf?pid=diva2%3A462620&dswid=-4589), Proceedings of the Fifth IEEE International Conference on Automatic Face and Gesture Recognition, Washington, DC, USA, 21–21 May 2002, pages 423-428. [ISBN](./ISBN_(identifier)) [0-7695-1602-5](./Special:BookSources/0-7695-1602-5), [doi](./Doi_(identifier)):[10.1109/AFGR.2002.1004190](https://doi.org/10.1109%2FAFGR.2002.1004190)
35. [↑](./Gesture_recognition#cite_ref-35) [Domitilla Del Vecchio](./Domitilla_Del_Vecchio), Richard M. Murray Pietro Perona, ["Decomposition of human motion into dynamics-based primitives with application to drawing tasks"](http://www.cds.caltech.edu/~ddomitilla/reports/AutomaticaReport.pdf) [Archived](https://web.archive.org/web/20100202211735/http://www.cds.caltech.edu/~ddomitilla/reports/AutomaticaReport.pdf) 2010-02-02 at the [Wayback Machine](./Wayback_Machine), Automatica Volume 39, Issue 12, December 2003, Pages 2085–2098, [doi](./Doi_(identifier)):[10.1016/S0005-1098(03)00250-4](https://doi.org/10.1016%2FS0005-1098%2803%2900250-4).
36. [↑](./Gesture_recognition#cite_ref-36) Thomas B. Moeslund and Lau Nørgaard, ["A Brief Overview of Hand Gestures used in Wearable Human Computer Interfaces"](http://www.vision.auc.dk/~tbm/Publications/gesture-hci.pdf) [Archived](https://web.archive.org/web/20110719120644/http://www.vision.auc.dk/~tbm/Publications/gesture-hci.pdf) 2011-07-19 at the [Wayback Machine](./Wayback_Machine), Technical report: CVMT 03-02, [ISSN](./ISSN_(identifier)) [1601-3646](https://search.worldcat.org/issn/1601-3646), Laboratory of Computer Vision and Media Technology, Aalborg University, Denmark.
37. [↑](./Gesture_recognition#cite_ref-37) M. Kolsch and M. Turk ["Fast 2D Hand Tracking with Flocks of Features and Multi-Cue Integration"](http://ilab.cs.ucsb.edu/projects/mathias/KolschTurk2004Fast2DHandTrackingWithFlocksOfFeatures.pdf) [Archived](https://web.archive.org/web/20080821111627/http://ilab.cs.ucsb.edu/projects/mathias/KolschTurk2004Fast2DHandTrackingWithFlocksOfFeatures.pdf) 2008-08-21 at the [Wayback Machine](./Wayback_Machine), CVPRW '04. Proceedings Computer Vision and Pattern Recognition Workshop, May 27-June 2, 2004, [doi](./Doi_(identifier)):[10.1109/CVPR.2004.71](https://doi.org/10.1109%2FCVPR.2004.71)
38. [↑](./Gesture_recognition#cite_ref-38) Xia Liu   Fujimura, K., "Hand gesture recognition using depth data", Proceedings of the Sixth IEEE International Conference on Automatic Face and Gesture Recognition, May 17–19, 2004
pages 529- 534, [ISBN](./ISBN_(identifier)) [0-7695-2122-3](./Special:BookSources/0-7695-2122-3), [doi](./Doi_(identifier)):[10.1109/AFGR.2004.1301587](https://doi.org/10.1109%2FAFGR.2004.1301587).
39. [↑](./Gesture_recognition#cite_ref-39) Stenger B, Thayananthan A, Torr PH, Cipolla R: ["Model-based hand tracking using a hierarchical Bayesian filter"](https://wayback.archive-it.org/all/20080221223332/http://www.bmva.ac.uk/sullivan/prizethesis-2005.pdf), IEEE Transactions on  IEEE Transactions on Pattern Analysis and Machine Intelligence, 28(9):1372-84, Sep 2006.
40. [↑](./Gesture_recognition#cite_ref-40) A Erol, G Bebis, M Nicolescu, RD Boyle, X Twombly, ["Vision-based hand pose estimation: A review"](https://www.cse.unr.edu/~bebis/handposerev.pdf), Computer Vision and Image Understanding Volume 108, Issues 1-2, October–November 2007, Pages 52-73 Special Issue on Vision for Human-Computer Interaction, [doi](./Doi_(identifier)):[10.1016/j.cviu.2006.10.012](https://doi.org/10.1016%2Fj.cviu.2006.10.012).
41. [1](./Gesture_recognition#cite_ref-:0_41-0) [2](./Gesture_recognition#cite_ref-:0_41-1) Rico, Julie; Brewster, Stephen (2010). "Usable gestures for mobile interfaces". *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems*. CHI '10. New York, NY, USA: ACM. pp. 887–896. [doi](./Doi_(identifier)):[10.1145/1753326.1753458](https://doi.org/10.1145%2F1753326.1753458). [ISBN](./ISBN_(identifier)) [9781605589299](./Special:BookSources/9781605589299). [S2CID](./S2CID_(identifier)) [16118067](https://api.semanticscholar.org/CorpusID:16118067).
42. [1](./Gesture_recognition#cite_ref-Walter_2013_42-0) [2](./Gesture_recognition#cite_ref-Walter_2013_42-1) Walter, Robert; Bailly, Gilles; Müller, Jörg (2013). ["StrikeAPose"](https://eref.uni-bayreuth.de/42090/). *Proceedings of the SIGCHI Conference on Human Factors in Computing Systems*. New York, New York, USA: ACM Press. pp. 841–850. [doi](./Doi_(identifier)):[10.1145/2470654.2470774](https://doi.org/10.1145%2F2470654.2470774). [ISBN](./ISBN_(identifier)) [9781450318990](./Special:BookSources/9781450318990). [S2CID](./S2CID_(identifier)) [2041073](https://api.semanticscholar.org/CorpusID:2041073).
43. [1](./Gesture_recognition#cite_ref-:1_43-0) [2](./Gesture_recognition#cite_ref-:1_43-1) Profita, Halley P.; Clawson, James; Gilliland, Scott; Zeagler, Clint; Starner, Thad; Budd, Jim; Do, Ellen Yi-Luen (2013). "Don't mind me touching my wrist". *Proceedings of the 2013 International Symposium on Wearable Computers*. ISWC '13. New York, NY, USA: ACM. pp. 89–96. [doi](./Doi_(identifier)):[10.1145/2493988.2494331](https://doi.org/10.1145%2F2493988.2494331). [ISBN](./ISBN_(identifier)) [9781450321273](./Special:BookSources/9781450321273). [S2CID](./S2CID_(identifier)) [3236927](https://api.semanticscholar.org/CorpusID:3236927).
44. [↑](./Gesture_recognition#cite_ref-44) Harrison, Chris; Faste, Haakon (2014). "Implications of location and touch for on-body projected interfaces". *Proceedings of the 2014 conference on Designing interactive systems*. DIS '14. New York, NY, USA: ACM. pp. 543–552. [doi](./Doi_(identifier)):[10.1145/2598510.2598587](https://doi.org/10.1145%2F2598510.2598587). [ISBN](./ISBN_(identifier)) [9781450329026](./Special:BookSources/9781450329026). [S2CID](./S2CID_(identifier)) [1121501](https://api.semanticscholar.org/CorpusID:1121501).
45. [1](./Gesture_recognition#cite_ref-:2_45-0) [2](./Gesture_recognition#cite_ref-:2_45-1) Reeves, Stuart; Benford, Steve; O'Malley, Claire; Fraser, Mike (2005). ["Designing the spectator experience"](http://eprints.nottingham.ac.uk/252/1/p133-reeves.pdf) (PDF). [*Proceedings of the SIGCHI Conference on Human Factors in Computing Systems*](https://nottingham-repository.worktribe.com/file/1020600/1/p133-reeves.pdf) (PDF). New York, New York, USA: ACM Press. pp. 741–750. [doi](./Doi_(identifier)):[10.1145/1054972.1055074](https://doi.org/10.1145%2F1054972.1055074). [ISBN](./ISBN_(identifier)) [978-1581139983](./Special:BookSources/978-1581139983). [S2CID](./S2CID_(identifier)) [5739231](https://api.semanticscholar.org/CorpusID:5739231).
46. [↑](./Gesture_recognition#cite_ref-46) Rupert Goodwins. ["Windows 7? No arm in it"](https://www.zdnet.com/article/windows-7-no-arm-in-it/). *ZDNet*.
47. [↑](./Gesture_recognition#cite_ref-47) ["gorilla arm"](http://www.catb.org/jargon/html/G/gorilla-arm.html). *catb.org*.
48. [↑](./Gesture_recognition#cite_ref-48) Hincapié-Ramos, J.D., Guo, X., Moghadasian, P. and Irani. P. 2014. ["Consumed Endurance: A Metric to Quantify Arm Fatigue of Mid-Air Interactions"](https://hci.cs.umanitoba.ca/projects-and-research/details/ce). In Proceedings of the 32nd annual ACM conference on Human factors in computing systems (CHI '14). ACM, New York, NY, USA, 1063–1072. DOI=10.1145/2556288.2557130
49. [↑](./Gesture_recognition#cite_ref-49) Hincapié-Ramos, J.D., Guo, X., and Irani, P. 2014. ["The Consumed Endurance Workbench: A Tool to Assess Arm Fatigue During Mid-Air Interactions"](https://hci.cs.umanitoba.ca/projects-and-research/details/ce). In Proceedings of the 2014 companion publication on Designing interactive systems (DIS Companion '14). ACM, New York, NY, USA, 109-112. DOI=10.1145/2598784.2602795

 

## External links

 
- [Annotated bibliography of references to gesture and pen computing](https://ruetersward.com/biblio.html)
- [Notes on the History of Pen-based Computing (YouTube)](https://www.youtube.com/watch?v=4xnqKdWMa_8)
- [The future, it is all a Gesture](https://www.bruceongames.com/2007/10/02/the-future-it-is-all-a-gesture/)—Gesture interfaces and video gaming
- [Ford's Gesturally Interactive Advert](https://web.archive.org/web/20111006003521/http://inition.co.uk/case-study/ford-c-max-campaign-ar-gestural-interface)—Gestures used to interact with digital signage
- [3D Hand Tracking](https://www.completegate.com/2017030265/blog/3d-hand-tracking#.WNlR_pxDqeQ.link)—A Literature Survey

 Interwikies 
| vteNonverbal communication |
| --- |
| ModalitiesPhysicalBlushingBody language/KinesicsBody-to-body communicationFacial expressionFacial Action Coding SystemMicroexpressionGestureListSpeech-independent gesturesHaptic communicationImitationInterpersonal synchronyLaughterOculesicsEye contactPupil dilationOlfactionPostureProxemicsSpeechAffectEmotional prosodyParalanguageIntonationLoudnessProsodyRhythmStressToneVoice qualitySocial contextChronemicsConventionsDisplay rulesHabitusHigh-context and low-context culturesInterpersonal relationshipSocial normOtherEmoticon/SmileyOne-bit messageMissed callSilent service codeUnconsciousMicroexpressionNon-verbal leakageMulti-facetedAffect displayDeceptionEmotion recognitionFirst impressionIntimacy | Modalities | PhysicalBlushingBody language/KinesicsBody-to-body communicationFacial expressionFacial Action Coding SystemMicroexpressionGestureListSpeech-independent gesturesHaptic communicationImitationInterpersonal synchronyLaughterOculesicsEye contactPupil dilationOlfactionPostureProxemicsSpeechAffectEmotional prosodyParalanguageIntonationLoudnessProsodyRhythmStressToneVoice qualitySocial contextChronemicsConventionsDisplay rulesHabitusHigh-context and low-context culturesInterpersonal relationshipSocial normOtherEmoticon/SmileyOne-bit messageMissed callSilent service codeUnconsciousMicroexpressionNon-verbal leakageMulti-facetedAffect displayDeceptionEmotion recognitionFirst impressionIntimacy | Physical | BlushingBody language/KinesicsBody-to-body communicationFacial expressionFacial Action Coding SystemMicroexpressionGestureListSpeech-independent gesturesHaptic communicationImitationInterpersonal synchronyLaughterOculesicsEye contactPupil dilationOlfactionPostureProxemics | Speech | AffectEmotional prosodyParalanguageIntonationLoudnessProsodyRhythmStressToneVoice quality | Social context | ChronemicsConventionsDisplay rulesHabitusHigh-context and low-context culturesInterpersonal relationshipSocial norm | Other | Emoticon/SmileyOne-bit messageMissed callSilent service code | Unconscious | MicroexpressionNon-verbal leakage | Multi-faceted | Affect displayDeceptionEmotion recognitionFirst impressionIntimacy |
| Modalities |
| PhysicalBlushingBody language/KinesicsBody-to-body communicationFacial expressionFacial Action Coding SystemMicroexpressionGestureListSpeech-independent gesturesHaptic communicationImitationInterpersonal synchronyLaughterOculesicsEye contactPupil dilationOlfactionPostureProxemicsSpeechAffectEmotional prosodyParalanguageIntonationLoudnessProsodyRhythmStressToneVoice qualitySocial contextChronemicsConventionsDisplay rulesHabitusHigh-context and low-context culturesInterpersonal relationshipSocial normOtherEmoticon/SmileyOne-bit messageMissed callSilent service codeUnconsciousMicroexpressionNon-verbal leakageMulti-facetedAffect displayDeceptionEmotion recognitionFirst impressionIntimacy | Physical | BlushingBody language/KinesicsBody-to-body communicationFacial expressionFacial Action Coding SystemMicroexpressionGestureListSpeech-independent gesturesHaptic communicationImitationInterpersonal synchronyLaughterOculesicsEye contactPupil dilationOlfactionPostureProxemics | Speech | AffectEmotional prosodyParalanguageIntonationLoudnessProsodyRhythmStressToneVoice quality | Social context | ChronemicsConventionsDisplay rulesHabitusHigh-context and low-context culturesInterpersonal relationshipSocial norm | Other | Emoticon/SmileyOne-bit messageMissed callSilent service code | Unconscious | MicroexpressionNon-verbal leakage | Multi-faceted | Affect displayDeceptionEmotion recognitionFirst impressionIntimacy |
| Physical | BlushingBody language/KinesicsBody-to-body communicationFacial expressionFacial Action Coding SystemMicroexpressionGestureListSpeech-independent gesturesHaptic communicationImitationInterpersonal synchronyLaughterOculesicsEye contactPupil dilationOlfactionPostureProxemics |
| Speech | AffectEmotional prosodyParalanguageIntonationLoudnessProsodyRhythmStressToneVoice quality |
| Social context | ChronemicsConventionsDisplay rulesHabitusHigh-context and low-context culturesInterpersonal relationshipSocial norm |
| Other | Emoticon/SmileyOne-bit messageMissed callSilent service code |
| Unconscious | MicroexpressionNon-verbal leakage |
| Multi-faceted | Affect displayDeceptionEmotion recognitionFirst impressionIntimacy |
| Broader conceptsCognitive academic language proficiencyCommunicationEmotional intelligenceNunchiPeople skillsSemioticsSocial behaviorSocial competenceSocial cueSocial skillsUnsaid | Broader concepts | Cognitive academic language proficiencyCommunicationEmotional intelligenceNunchiPeople skillsSemioticsSocial behaviorSocial competenceSocial cueSocial skillsUnsaid |
| Broader concepts |
| Cognitive academic language proficiencyCommunicationEmotional intelligenceNunchiPeople skillsSemioticsSocial behaviorSocial competenceSocial cueSocial skillsUnsaid |
| Further informationDisordersAprosodiaAsperger syndromeAutismFragile XPervasive developmental disorder not otherwise specifiedChildhood disintegrative disorderRett syndromeDyssemiaNonverbal learning disorderSocial (pragmatic) communication disorderNeuroanatomyLimbic system/Limbic lobeMirror neuronApplicationsCold readingLie detectionFreudian slipPoker tellTargeted advertisingTechnologyComputer processing of body languageEmotion recognition in conversationGesture recognitionList of facial expression databasesSentiment analysisKey peopleRay BirdwhistellCharles DarwinPaul EkmanRelatedAnimal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communicationManual-tactile verbalSign languageTactile signingTadomaArt and literatureMimeMimoplastic artSubtext | Further information | DisordersAprosodiaAsperger syndromeAutismFragile XPervasive developmental disorder not otherwise specifiedChildhood disintegrative disorderRett syndromeDyssemiaNonverbal learning disorderSocial (pragmatic) communication disorderNeuroanatomyLimbic system/Limbic lobeMirror neuronApplicationsCold readingLie detectionFreudian slipPoker tellTargeted advertisingTechnologyComputer processing of body languageEmotion recognition in conversationGesture recognitionList of facial expression databasesSentiment analysisKey peopleRay BirdwhistellCharles DarwinPaul EkmanRelatedAnimal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communicationManual-tactile verbalSign languageTactile signingTadomaArt and literatureMimeMimoplastic artSubtext | Disorders | AprosodiaAsperger syndromeAutismFragile XPervasive developmental disorder not otherwise specifiedChildhood disintegrative disorderRett syndromeDyssemiaNonverbal learning disorderSocial (pragmatic) communication disorder | Neuroanatomy | Limbic system/Limbic lobeMirror neuron | Applications | Cold readingLie detectionFreudian slipPoker tellTargeted advertising | Technology | Computer processing of body languageEmotion recognition in conversationGesture recognitionList of facial expression databasesSentiment analysis | Key people | Ray BirdwhistellCharles DarwinPaul Ekman | Related | Animal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communicationManual-tactile verbalSign languageTactile signingTadomaArt and literatureMimeMimoplastic artSubtext | Animal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communication | Manual-tactile verbal | Sign languageTactile signingTadoma | Art and literature | MimeMimoplastic artSubtext |
| Further information |
| DisordersAprosodiaAsperger syndromeAutismFragile XPervasive developmental disorder not otherwise specifiedChildhood disintegrative disorderRett syndromeDyssemiaNonverbal learning disorderSocial (pragmatic) communication disorderNeuroanatomyLimbic system/Limbic lobeMirror neuronApplicationsCold readingLie detectionFreudian slipPoker tellTargeted advertisingTechnologyComputer processing of body languageEmotion recognition in conversationGesture recognitionList of facial expression databasesSentiment analysisKey peopleRay BirdwhistellCharles DarwinPaul EkmanRelatedAnimal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communicationManual-tactile verbalSign languageTactile signingTadomaArt and literatureMimeMimoplastic artSubtext | Disorders | AprosodiaAsperger syndromeAutismFragile XPervasive developmental disorder not otherwise specifiedChildhood disintegrative disorderRett syndromeDyssemiaNonverbal learning disorderSocial (pragmatic) communication disorder | Neuroanatomy | Limbic system/Limbic lobeMirror neuron | Applications | Cold readingLie detectionFreudian slipPoker tellTargeted advertising | Technology | Computer processing of body languageEmotion recognition in conversationGesture recognitionList of facial expression databasesSentiment analysis | Key people | Ray BirdwhistellCharles DarwinPaul Ekman | Related | Animal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communicationManual-tactile verbalSign languageTactile signingTadomaArt and literatureMimeMimoplastic artSubtext | Animal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communication | Manual-tactile verbal | Sign languageTactile signingTadoma | Art and literature | MimeMimoplastic artSubtext |
| Disorders | AprosodiaAsperger syndromeAutismFragile XPervasive developmental disorder not otherwise specifiedChildhood disintegrative disorderRett syndromeDyssemiaNonverbal learning disorderSocial (pragmatic) communication disorder |
| Neuroanatomy | Limbic system/Limbic lobeMirror neuron |
| Applications | Cold readingLie detectionFreudian slipPoker tellTargeted advertising |
| Technology | Computer processing of body languageEmotion recognition in conversationGesture recognitionList of facial expression databasesSentiment analysis |
| Key people | Ray BirdwhistellCharles DarwinPaul Ekman |
| Related | Animal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communicationManual-tactile verbalSign languageTactile signingTadomaArt and literatureMimeMimoplastic artSubtext | Animal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communication | Manual-tactile verbal | Sign languageTactile signingTadoma | Art and literature | MimeMimoplastic artSubtext |
| Animal communicationBehavioral communicationAggressiveAssertivePassivePassive-aggressiveImpression managementMeta-communicationMonastic sign lexiconsVerbal communication |
| Manual-tactile verbal | Sign languageTactile signingTadoma |
| Art and literature | MimeMimoplastic artSubtext |

 Categories