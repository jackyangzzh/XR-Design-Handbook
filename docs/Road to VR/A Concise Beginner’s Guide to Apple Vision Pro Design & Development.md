---
layout: default
title: A Concise Beginner’s Guide to Apple Vision Pro Design & Development
parent: Road to VR
---

# A Concise Beginner’s Guide to Apple Vision Pro Design & Development
Original article: [A Concise Beginner’s Guide to Apple Vision Pro Design & Development](https://www.roadtovr.com/apple-vision-pro-design-development-beginner-guide-sterling-crispin/)

## TL;DR
The document introduces visionOS, Apple's XR headset, with features like spatial audio and tool compatibility. It provides guidelines for spatial computing, including VR and AR, focusing on user sensory considerations and design principles. The text also highlights spatial computing weaknesses and emphasizes rapid development strategies, offering insights for developers in immersive technologies.

## Bullet points
1. 🖼️ **Scenes in visionOS (Windows, Volumes, and Spaces)**: visionOS organizes applications into three types of spatial contexts: Windows, Volumes, and Spaces. Windows are rectangular displays akin to traditional computer screens, while Volumes represent 3D or interactive objects, and Spaces are immersive environments that provide full control. Immersion styles within Spaces may vary from mixed to full, defining the extent of the real world to be seen.
2. 🎮 **User Input and Interaction Methods**: Users can interact with visionOS using various methods, from traditional gestures like pinching and tapping on floating windows to using Bluetooth trackpads or game controllers. Voice input and Dwell Control are also available. Developers need not worry about the origin of these events, focusing on handling them through elements like TapGesture.
3. 🎧 **Spatial Audio in Vision Pro**: Vision Pro's advanced spatial audio system gives a realistic sound experience by considering the room's physical attributes. Developers must prioritize using sound design for UI interaction and creating immersive experiences, acknowledging the importance of spatial audio in enhancing the user experience.
4. 🛠️ **Development Tools and Platforms**: Depending on the target platforms, developers can choose between Apple's development ecosystem (using tools like XCode, SwiftUI, RealityKit, ARKit, and Reality Composer Pro) or Unity for building fully immersive VR experiences that are compatible with various headsets. Apple's tools enable quick development with built-in assets, while Unity offers more extensive control and compatibility with non-Apple VR systems.
5. 📲 **Transitioning iOS Apps and Product Design Considerations**: Existing iOS apps can transition to visionOS as floating Windows, with the Ornament API allowing customization. Understanding spatial apps requires experiencing them firsthand (e.g., through Quest 2 or 3), and keeping a learning diary can be invaluable. Thoughtful design, understanding user needs, and avoiding overly complex or physically demanding interactions are paramount.
6. 📐 **Prototyping and Spatial Formats**: The design process for spatial apps may involve physical prototyping with paper or cardboard, or digital tools like ShapesXR. The app's purpose should be reflected in its spatial arrangements, with consideration for user comfort and familiarity. High-end tools like the Varjo XR-3 might be considered for those with substantial budgets. The prototyping phase emphasizes user-centric design, ensuring the application's spatial components align with user needs and expectations while exploring various interaction models.
7. 1. 🧠 **Visual and Perceptual Comfort:** The design of spatial computing interfaces should prioritize the sensory experience of the user. Ergonomics and cognitive impacts must be considered to minimize discomfort and motion sickness. Users may attribute discomfort to hardware, but it's the app's responsibility to ensure comfort.
8. 🎨 **UI and Web Design:** A blend of standard practices and innovation is key for intuitive interaction. Using tools like WebXR, designers can turn websites into immersive VR experiences. A balance between subtlety in space and motion and avoiding excessive 3D effects is essential.
9. 🎮 **Games and Media Development:** Choices of tools like Unity or Apple's ecosystem can significantly impact the development process. Varied contexts for gameplay mechanics, mixed inputs, and asymmetry should be explored. Existing tools like Apple's Game Porting Toolkit could facilitate the integration of high-end PC games.
10. 🏢 **Strengths, Weaknesses, and Strategies for Spatial Computing in Business and Products:** Spatial computing's strength lies in teaching spatial tasks, viewing things at scale, expressive applications, and immersive media. Limitations exist in activities involving quick movements and long-term use. A lean approach to development that encourages fast failure, pivots, and focuses on solving real problems can lead to success. For existing products, the focus should be on identifying specific spatial moments that enhance the experience while avoiding unnecessary complexity.


## Keywords
- **Volumes**: These are 3D objects or small interactive scenes in visionOS. They can be things like a 3D map or a small game that floats in front of the user.
- **Spaces**: In visionOS, these are fully immersive experiences where only one app is visible. Spaces can be mixed, progressive, or fully immersive, defining how much of the real world the user can see.
- **TapGesture**: A user input method where actions are triggered by tapping.
- **Dwell Control**: An accessibility feature in visionOS that allows eyes-only input.
- **SwiftUI**: A user interface toolkit that allows developers to design apps in a declarative way for Apple devices.
- **RealityKit**: A framework used for rendering 3D objects, materials, and light simulations in Apple's ecosystem.
- **ARKit**: Apple's framework for augmented reality (AR) development, allowing for advanced scene understanding and interaction with real-world objects.
- **Reality Composer Pro**: A 3D content editor specific to Apple's development stack, allowing developers to drag objects around a 3D scene.
- **PlayStation VR**: Sony's virtual reality system used with PlayStation gaming consoles.
- **PolySpatial tool**: A tool in Unity for converting materials, shaders, and other features.
- **Ornament API**: An API used to create floating islands of UI for spatial effect in existing iOS apps.
- **IDEO Design Thinking**: A methodology used for creative problem solving, emphasizing empathy with users, defining problems, ideation, prototyping, and testing.
- **ShapesXR**: An app used for sketching ideas in space and creating storyboards for spatial apps.
- **Passthrough AR**: A feature that allows users to see the real world through cameras on a VR headset, creating augmented reality experiences.
- **Varjo XR-3**: A high-end virtual and augmented reality headset known for its quality and high price.
- **Cognitive Impacts:** Relating to the mental processes of perception, memory, judgment, and reasoning. In this context, it refers to how design choices can affect these mental processes.
- **Fitts' Law:** A principle that predicts the time required to rapidly move to a target area, as a function of the ratio of the distance to the target and the width of the target. It's used in human-computer interaction and ergonomics.
- **WebXR:** A web framework that enables the creation of Virtual Reality (VR) and Augmented Reality (AR) experiences on web browsers.
- **2.5D:** A term describing the visual depth and perspective in a project that is otherwise two-dimensional. It represents a structure that has a 3D look but doesn’t fully exist in three-dimensional space.
- **Game Porting Toolkit:** A tool for adapting or porting games from one platform to another, mentioned in the context of bringing PC games to Mac.
- **Lean Startup:** A methodology for developing businesses and products that aim to shorten product development cycles and rapidly discover if a proposed business model is viable.

