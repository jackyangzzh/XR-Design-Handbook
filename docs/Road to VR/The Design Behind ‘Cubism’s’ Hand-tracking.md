---
layout: default
title: The Design Behind ‘Cubism’s’ Hand-tracking
parent: Road to VR
---

# Case Study: The Design Behind ‘Cubism’s’ Hand-tracking
Original article: [The Design Behind ‘Cubism’s’ Hand-tracking](https://www.roadtovr.com/cubism-hand-tracking-case-study/)

## TL;DR
Cubism mploys Ghost Hands for natural interactions and Contact Grabbing for precise object manipulation. Dynamic Hand Smoothing reduces jitter, while Raycast mechanisms detect objects and redundancies enhance usability. Debugging Visualizations aid developers, and careful design minimizes false positives, creating a seamless and immersive user experience.

## Bullet points
1. **🎯 Optimizing for Precise Interactions**: Cubism focuses on precision when it comes to hand tracking input. The interactions are centered around placing small irregular puzzle pieces precisely in a grid. This design principle has guided most of the decision-making around hand input, including grabbing and placing puzzle pieces with exactitude.

2. **👻 Ghost Hands Approach**: The developers decided against using physics-based hands, allowing them to pass through pieces until actively grabbed. This design choice avoids pushing away floating puzzle pieces when trying to grab them and facilitates plucking pieces from a full puzzle.

3. **🤏 Contact Grabbing Method**: The most effective approach for Cubism's intricate interactions was contact-based grabbing. This involves thumb and index finger intersection over a small distance rather than a full pinch. The fingers are locked in place when a grab starts, providing stability, and multiple safeguards are implemented to avoid unintentional releases.

4. **🎮 Midpoint Check for Grabbing**: To further fine-tune grabbing, a midpoint check is performed between the thumb and index fingertip. This helps prioritize the correct piece when multiple options are present, aiding in precise grabbing in densely filled areas of the puzzle grid.

5. **🧩 Grabbing the Puzzle & Dynamic Hand Smoothing**: Grabbing the puzzle employs a full pinch within a special zone around the puzzle. Dynamic hand smoothing is also introduced to mitigate the jitter from the Oculus Quest's hand tracking data, providing a more stable grip without a “laggy” feeling.

6. **🔘 Pressing Buttons with Interaction Cues**: Buttons in Cubism can be pressed and interacted with. The system utilizes raycasts, colliders, and various cues (such as highlight and drop shadow) to guide the user in interacting with buttons accurately.

7. **🔀 Interaction Redundancy and Cues**: Since different players may approach interactions in unintended ways, redundancy is implemented, such as allowing full-finger grabbing or pinching buttons. Multiple cues, like color highlighting and audio feedback, guide users in the intended direction.

8. **🏫 Teaching Limitations**: The article acknowledges the limitations of Quest’s hand tracking and stresses the importance of making players aware of these limitations. Guidance includes a modal explaining best practices and in-game indicators when tracking is lost.

9. **🖐️ Customizable Tracking Feedback**: Cubism allows players to customize the feedback they receive when tracking is lost. They can choose between the default red hands with warning messages or a more subtle fading of hands, depending on personal preference.

10. **🔧 Debugging and Tuning Options**: Throughout the article, the emphasis on fine-tuning and optimizing is evident. There are debug visualizations and settings available within the game for players and developers to understand and customize interactions, ensuring that the user experience is as intuitive and responsive as possible.

## Keywords
- **Ghost Hands**: Virtual hands in the application that can pass through objects unless actively grabbing them.
- **Contact Grabbing**: Interaction where an object is grabbed when specific parts of the virtual hand intersect with the object.
- **Dynamic Hand Smoothing**: Technique to counteract jitter in hand tracking data, providing natural and stable hand movement.
- **Raycast**: Method to detect objects along a path or in line of sight, used to detect hovering or pressing of buttons.
- **Redundancies**: Provision of multiple means to achieve the same interaction goal, enhancing usability and flexibility.
- **Debugging Visualizations**: Visual tools to help developers identify and fix problems in the software.
- **Grab Zone**: Designated area where specific grabbing actions can be performed to interact with the puzzle grid.
- **Jitter**: Erratic or shaky movement in hand tracking, countered by dynamic hand smoothing.
- **Pressable**: Buttons or interactive elements that can be pressed or activated by the user.
- **Raycast Mechanisms**: Techniques involving raycasting to detect position and state of objects in 3D space.
- **False Positives**: Unintentional activations or triggers of certain actions or responses in interaction.
