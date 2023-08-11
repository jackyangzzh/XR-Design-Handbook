---
layout: default
title: Hand Tracking Best practices
parent: Qualcomm
---

# Hand Tracking Best practices
Original article: [Hand Tracking Best practices](https://docs.spaces.qualcomm.com/unity/handtracking/design/BestPractices.html)

## TL;DR
Extended Reality (XR) design emphasizes intuitive hand gestures and interactions. Usability and accessibility are key to comfortable virtual experiences. Technological constraints must be acknowledged for robust and engaging XR applications.

## Bullet points
1. **🤲 Virtual Interactions**: Interactions with virtual content are made possible through Hand Tracking technology. This includes hand gestures, specific poses to trigger actions, and physical interactions with virtual objects. Distal interactions allow actions at a distance, while proximal interactions require closer physical engagement.

2. **✋ Hand Gestures**: Hand gestures need to be taught gradually in a tutorial, rather than all at once. It's essential to limit the number of gestures and ensure they are distinct, consistent throughout the application, and always accessible via tutorials. This approach ensures intuitive and user-friendly experiences.

3. **🖥️ Usability**: To create an engaging and immersive user experience, the design must prioritize spatial environments, interactions, object placement, and user journeys. The ergonomic considerations need to be in sync with user interactions and the overall journey to make the virtual environment feel natural.

4. **🚶 User Posture**: Promoting neutral body positions and natural arm placements helps avoid fatigue. Designing interactions that avoid large, strenuous, and repetitive movements aids in maintaining user comfort and enhancing the overall experience.

5. **🎗️ Accessibility**: Accessibility in XR is about creating a user interface that everyone can interact with. This includes designing cues that guide users through a full 360° and 3D space, enabling actions at a natural arm's reach, and considering font, color, and interaction methods that are inclusive.

6. **🗺️ User Journey**: Guiding users with visual or audio cues, and providing clear feedback helps in building an intuitive experience. Ensuring actions are reversible and offering clear exits from unwanted states allow users to feel in control, enhancing their engagement.

7. **🧠 Context**: Contextual design helps in streamlining content delivery and relevant interactions. By tracking user focus and adapting available elements, the visual clutter is minimized. Context makes the experience more intuitive, as seen in the example of a drawing demo, where the menu changes based on user selections.

8. **📦 Object Placement**: Following the Gestalt Principles, similar objects are grouped for easier discovery. Objects are placed within reach and sight, appropriately sized, and positioned not to obstruct the user's vision. These considerations improve navigation and interaction within the virtual space.

9. **📐 Field of View (FOV)**: FOV is vital in AR/VR. Understanding how Camera FOV (captured by the device's cameras) and Display FOV (what the user actually sees) work ensures that the design aligns with the device's limitations, providing an optimal viewing experience.

10. **🚫 Limitations**: Limitations in XR design include occlusion, where one hand may block the other, impacting Hand Tracking. This can be minimized by avoiding overlapping hand gestures and using one-handed patterns. Outdoor environment limitations due to hardware restrictions must also be considered to ensure the application behaves as expected.
    
## Keywords
- **Distal Interaction**: Interaction with objects from a distance.
- **Proximal Interaction**: Physical interaction with virtual objects at close range.
- **Ergonomics**: The study of designing equipment and devices that fit the human body and its movements.
- **Gestalt Principles**: Psychological principles that describe how humans naturally perceive objects as organized patterns and objects.
- **Field of View (FOV)**: The extent of the observable environment seen at any given moment. In AR/VR, it includes Camera FOV (captured by cameras) and Display FOV (what the user sees).
- **Occlusion**: In 3D space, when one object blocks another object from view, often impacting hand tracking in XR experiences.