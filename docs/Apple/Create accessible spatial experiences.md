---
layout: default
title: Create accessible spatial experiences
parent: Apple
---

# Create accessible spatial experiences
Original video: [Create accessible spatial experiences](https://developer.apple.com/videos/play/wwdc2023/10034/)


## TL;DR
This video discusses accessibility in spatial computing, emphasizing inclusive design for people with disabilities. It covers VoiceOver support, gesture controls, RealityKit's accessibility component, vision accessibility considerations, camera anchors, alternate inputs like Dwell Control and Pointer Control, cognitive accessibility, hearing accessibility with captions, and the importance of creating inclusive spatial experiences.


## Bullet points
1. 💡 Accessibility is crucial in spatial computing to ensure that individuals with disabilities can fully engage with immersive experiences. It's important to consider the diverse needs of users, including those with visual, motor, cognitive, and hearing impairments.

2. 🗣️ VoiceOver support is available on this platform, allowing people who are blind or have low vision to interact with apps using finger pinches on their hands. VoiceOver provides spoken descriptions of on-screen elements, enabling users to navigate and interact with the app.

3. 🤝 VoiceOver's Direct Gesture Mode enables individuals to directly process hand input, providing a choice between default interaction mode and direct gestures. This allows users to interact with apps using hand gestures without VoiceOver interfering.

4. 👁️ Vision accessibility can be enhanced by adopting SwiftUI's accessibility modifiers and using the accessibility component in RealityKit. These tools enable developers to provide accurate accessibility information, such as labels and traits, to ensure that visually impaired users can understand and interact with app elements.

5. 📷 Camera anchors should be used sparingly, as individuals with low vision may need to get closer to content. Providing alternatives, such as world anchors instead of head anchors, allows users to view and interact with objects more effectively.

6. ⌨️ Dwell Control and Pointer Control offer alternate input methods for individuals with physical disabilities affecting their use of eyes and hands. Dwell Control allows users to select and interact with UI elements without using their hands, while Pointer Control changes the system focus based on head or finger movements.

7. 🧠 Cognitive accessibility can be improved by using Guided Access to minimize distractions and provide a focused experience. Guided Access restricts the system to a single app, preventing users from switching between apps and maintaining focus on the current task.

8. 🔊 Captions play a vital role in hearing accessibility, and they should be comprehensive, customizable, and easy to read. Providing accurate captions for audio content ensures that individuals with hearing impairments can access and understand the information being conveyed.

9. 🌍 Inclusive spatial experiences require setting accessibility properties on entities and providing options for interaction to accommodate different needs. Developers can use features like the accessibility component in RealityKit to specify accessibility labels, values, and traits, as well as custom actions and content.

10. 📚 Developers should familiarize themselves with accessibility features, such as Dynamic Type (adjustable text size), high contrast ratios, and API frameworks like AVKit and AVFoundation, to create accessible apps. Understanding and implementing these features will help ensure that individuals with disabilities can fully enjoy and benefit from spatial computing experiences.



## Keywords:
- **Spatial computing**: The use of digital technologies to create immersive experiences that integrate the physical and virtual worlds.
- **Accessibility**: The design of products, devices, services, or environments that can be used by people with disabilities.
- **VoiceOver**: A built-in screen reader available on Apple platforms that provides spoken feedback to assist users who are blind or have low vision.
- **RealityKit**: A framework by Apple for creating augmented reality (AR) and virtual reality (VR) experiences.
- **Dynamic Type**: A feature that allows users to adjust the text size in apps to make it more readable.
- **SwiftUI**: A user interface toolkit by Apple for building apps across all Apple platforms.
- **Dwell Control**: An accessibility feature that allows users to interact with UI elements without using their hands.
- **Cognitive accessibility**: The design of products and experiences to accommodate individuals with cognitive disabilities or impairments.
- **AVKit and AVFoundation**: Frameworks by Apple for working with audio and video content in apps.
- **Captioning**: The process of displaying text on screen that corresponds to the audio in a video or other media.