---
layout: default
title: Create accessible spatial experiences
parent: Apple
---

# Augmented reality
Original article: [Augmented reality](https://developer.apple.com/design/human-interface-guidelines/augmented-reality)

## TL;DR
In Augmented Reality (AR) experiences, prioritize clear, non-technical instructions and favor 3D hints over 2D text overlays. Handle interruptions, like app switches or calls, with user guidance to maintain AR tracking. Consistently use unaltered AR icons and badges to indicate AR functionalities.

## Bullet points

1. 📱 **Approachable Terminology**:
    - Instead of technical jargon like "ARKit" or "tracking," use friendlier alternatives. For example, say "Unable to find a surface" instead of "Unable to find a plane." This ensures users who might be unfamiliar with AR concepts still understand instructions and prompts.

2. 🌍 **World Mapping**:
    - ARKit utilizes world mapping to overlay virtual objects accurately. It understands the user's environment in detail, allowing for a more immersive AR experience. This is why suggestions like "moving your phone more slowly" or "turning on more lights" might improve the AR experience by assisting with world detection.

3. 🔄 **Relocalization**:
    - When interruptions occur, like phone calls, AR might misplace virtual objects. Relocalization is the process where ARKit tries to reposition these objects correctly. Providing a reset option or guidance on returning the device to its original position can help in such scenarios.

4. 🌀 **3D Hints vs. 2D**:
    - Visual feedback is essential in AR. When hinting at possible actions, such as rotating an object, 3D visual hints (like a rotation indicator) are more intuitive than 2D text prompts. It aligns better with the immersive nature of AR.

5. 🔡 **Text Readability**:
    - When text is indispensable in AR, ensure it is large enough to read and always faces the viewer, even in 3D space. It's about guaranteeing that the user gets the message, no matter their orientation or the text's position.

6. 🔍 **More Information**:
    - Sometimes, users might need additional information about AR objects. Using visual indicators, like labels with a ">" sign, shows users that they can tap to learn more, enhancing the interactive nature of AR.

7. 🛑 **Handling Interruptions**:
    - If the user switches apps or accepts a call, ARKit loses tracking. On returning, it's crucial to guide the user to either relocalize or consider hiding misplaced virtual objects to avoid confusion or visual glitches.

8. 🔄 **Minimizing Interruptions**:
    - For an uninterrupted AR experience, blend non-AR elements within AR. For instance, changing object properties, like furniture upholstery, shouldn't require exiting the AR mode. It promotes sustained engagement.

9. 🔖 **Icons and Badges**:
    - ARKit provides specific icons for AR experiences. They are meant for specific uses, such as initiating an AR experience. Use these icons uniformly and don't alter their appearance. These consistent visuals help users identify AR-specific interactions quickly.

10. 💡 **Problem Solving**:
    - AR can sometimes face challenges like insufficient lighting or problems in detecting surfaces. Address these proactively by suggesting fixes. This not only educates the user about potential issues but also empowers them to rectify and enjoy a seamless AR experience.

## Keywords
- **ARKit**: Apple's framework for creating augmented reality experiences on iOS devices.
  
- **World Detection**: The ability of AR systems to identify and track the user's environment in real-time, allowing virtual objects to be placed with accuracy.

- **Tracking**: The process by which AR systems follow the movement and orientation of the user's device to align virtual objects with the real world.

- **Relocalization**: An ARKit feature that attempts to realign virtual objects to their original real-world positions after an interruption.

- **3D Hints**: Visual indicators in three-dimensional space used to guide users in AR experiences.

- **System-provided coaching view**: A built-in view provided by ARKit to help users with tasks such as relocalization.

- **Glyph**: A specific icon or symbol used to represent a function or feature, such as the AR icon in ARKit.

- **Badging**: Using specific icons or markers to indicate certain capabilities or features, like viewing an object in AR.
