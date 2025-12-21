---
layout: default
title: PlayStation VR2 Design Guidelines
parent: Sony
---

# PlayStation VR2 Design Guidelines
Original sources: [Sony Developer Portal](https://sonyinteractive.com), [PlayStation Blog](https://blog.playstation.com/2023/02/06/playstation-vr2-the-ultimate-faq/)

## TL;DR
PlayStation VR2 emphasizes ergonomic comfort, eye tracking for enhanced interaction and performance, foveated rendering for optimal graphics, integrated haptic feedback for immersion, and comprehensive accessibility features. Developers should leverage PS VR2's unique hardware capabilities including 6DoF tracking, see-through view, and spatial awareness to create comfortable, immersive experiences with natural break points to prevent fatigue.

## Bullet points

1. 👓 **Ergonomic Design and Comfort**: PS VR2 underwent extensive user testing across diverse head shapes, sizes, and with users wearing glasses. The headset features adjustable lens-eye distance, reduced weight distribution, and improved ventilation. Developers should design experiences that accommodate various physical attributes and provide natural break points for extended sessions to maintain user comfort throughout gameplay.

2. 👁️ **Eye Tracking Integration**: Eye tracking enables both innovative gameplay mechanics and performance optimizations. Games can use eye movement for menu navigation, object selection via gaze, and context-sensitive interactions. Eye tracking data should be used ethically, respecting user privacy, and developers should ensure diverse testing across different eye colors and physical characteristics to maintain consistent tracking accuracy.

3. 🎨 **Foveated Rendering**: The hardware natively supports foveated rendering, which renders high-resolution graphics only where the user is focused while reducing quality in peripheral vision. This is recommended through Unity's Universal Render Pipeline (URP) and significantly improves GPU performance. Developers should design interfaces that guide attention appropriately and avoid requiring high detail in peripheral areas.

4. 📍 **6DoF Positional Tracking and Reprojection**: PS VR2 provides six-degrees-of-freedom tracking with high-frequency positional reprojection, ensuring minimal latency and natural perspective changes. UI elements must remain stable and readable during fast head movements. Design for smooth transitions and maintain consistent frame rates (90Hz/120Hz optimal) to prevent judder and discomfort.

5. 🎮 **Sense Controllers with Haptic Feedback**: The Sense Controllers feature adaptive triggers, balanced haptic feedback, and ergonomic design for natural finger movements. Headset vibration can reinforce in-game events. Developers should use haptic feedback purposefully to enhance immersion without overwhelming or distracting users, creating a multimodal sensory experience across both controllers and headset.

6. 🌍 **Play Area Customization and Safety**: The system includes play area scanning that allows users to define safe zones. Games should utilize this feature to provide in-game warnings when boundaries are approached. Design experiences that don't require excessive player movement beyond what the system can reliably track, respecting the defined safe space and user comfort.

7. 👀 **See-Through View Feature**: Users can check their real-world surroundings without removing the headset via the see-through camera view. Developers should consider implementing auto-pause or pause prompts when this feature is activated, enhancing both safety and usability by allowing users to remain aware of their physical environment.

8. 🎬 **Cinematic Mode Support**: PS VR2 supports both VR and non-VR content through Cinematic Mode, which displays content on a virtual screen. Provide clear UI transitions between VR and non-VR modes with intuitive cues, ensuring users understand which mode they're in and can easily switch between immersive and traditional viewing experiences.

9. ♿ **Accessibility Features**: Built-in accessibility includes adjustments for users with glasses, UI scaling options, customizable controller mapping, and various comfort settings. Developers should support these system-level features and consider additional accessibility options such as adjustable difficulty, subtitle customization, and alternative input methods to ensure inclusive experiences.

10. 🎯 **Graphics Pipeline Optimization**: Use the Universal Render Pipeline (URP) in Unity for full exploitation of PS VR2's capabilities including foveated rendering and eye tracking. Target 90Hz minimum (120Hz preferred) frame rates for optimal comfort. Avoid overengineering graphics at the expense of performance—consistent frame rate is critical for user comfort and immersion.

## Keywords

- **Eye Tracking**: Technology that monitors where and how users move their eyes, enabling gaze-based interaction and performance optimization through foveated rendering.

- **Foveated Rendering**: Rendering technique that displays high-resolution graphics only in the user's focal area while reducing quality in peripheral vision, improving performance without perceived quality loss.

- **6DoF (Six Degrees of Freedom)**: Tracking that monitors both rotational movement (pitch, yaw, roll) and positional movement (forward/back, left/right, up/down) in 3D space.

- **Positional Reprojection**: Technique that adjusts rendered frames based on updated head position to reduce perceived latency and maintain visual stability.

- **Adaptive Triggers**: Controller triggers that can dynamically change resistance, providing tactile feedback that simulates different actions or materials.

- **Haptic Feedback**: Physical vibrations and sensations that provide tactile responses to user actions and in-game events.

- **URP (Universal Render Pipeline)**: Unity's modern rendering pipeline optimized for performance across various platforms, recommended for PS VR2 development.

- **See-Through View**: Camera-based passthrough feature allowing users to see their physical environment without removing the headset.

- **Cinematic Mode**: Display mode that shows non-VR content on a virtual screen within the VR environment.

- **Play Area**: User-defined physical space boundaries for safe VR movement and interaction.

- **Judder**: Visual artifacting from inconsistent frame rates that causes discomfort and breaks immersion.

- **Vergence-Accommodation Conflict**: Mismatch between where eyes focus and converge in VR, which PS VR2 minimizes through optical design.