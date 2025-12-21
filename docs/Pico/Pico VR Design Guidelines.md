---
layout: default
title: Pico VR Design Guidelines
parent: Pico
---

# Pico VR Design Guidelines
Original sources: [PICO Developer Documentation](https://developer-cn.picoxr.com/en/document/), [PICO Developer Platform](https://developer.picoxr.com/), [OpenXR Compliance](https://www.picoxr.com/global/about/newsroom/openxr)

## TL;DR
Pico VR emphasizes natural spatial interactions over traditional desktop metaphors, OpenXR standard compliance for cross-platform compatibility, comfort-first design with high frame rates and low latency, comprehensive hand tracking and controller support, and device-agnostic accessibility. Developers should embrace 3D spatial layouts, optimize performance rigorously, provide continuous feedback, and design for both hand tracking and controller inputs to create comfortable, accessible VR experiences.

## Bullet points

1. 🏗️ **Spatial-First Design Philosophy**: Avoid directly adapting 2D desktop paradigms like flat windows, buttons, and menus. Instead, embrace 3D spatial layouts that feel natural in VR. Organize UI with clear hierarchy and spatial context, placing elements at comfortable distances and angles. Spatial containers and behaviors should leverage depth and dimensionality rather than forcing flat interfaces into 3D space.

2. 🤲 **Natural Interaction Methods**: Gesture and hand-based controls significantly outperform traditional desktop metaphors in immersion and intuitiveness. Design for direct manipulation where users reach out and interact with objects naturally. Support both hand tracking and controller inputs, allowing users to choose their preferred interaction method based on comfort and context.

3. 🎯 **Continuous Feedback Systems**: Provide immediate visual, haptic, and audio feedback for every user action. This reinforces engagement and makes interfaces feel responsive and alive. Clear feedback helps users understand the results of their actions, builds confidence in interactions, and enhances the sense of presence in the virtual environment.

4. 📊 **Performance Optimization**: Maintain high frame rates (90Hz minimum, 120Hz preferred) and minimize latency to prevent motion sickness and discomfort. Optimize rendering through adaptive techniques, reduce mesh complexity, and implement level-of-detail systems. Performance directly impacts user comfort and immersion—it's non-negotiable for quality VR experiences.

5. 🎨 **Minimal UI Clutter**: Only show relevant information when needed, avoiding overwhelming users with persistent displays. Use contextual menus and adaptive interfaces that appear based on user focus and actions. Clean, focused interfaces reduce cognitive load and maintain immersion by not constantly reminding users they're in a virtual environment.

6. ♿ **Device-Agnostic Accessibility**: Design for inclusivity with legible text at various distances, high contrast modes, adjustable UI scaling, and multiple input methods. Support voice control, large text options, contrast adjustments, and adaptive environments for users with impairments. Accessibility should be built in from the start, not added as an afterthought.

7. 🌐 **OpenXR Standard Compliance**: Pico fully supports OpenXR, enabling cross-platform development. Build apps that run on Pico and other OpenXR-compliant hardware with minimal code changes. Leverage OpenXR-specific features to optimize performance and user experience while maintaining broad hardware compatibility and future-proofing applications.

8. 📐 **Ergonomic Placement**: Position interactive elements at comfortable locations and distances to reduce arm, hand, and neck fatigue. Consider reach envelopes and natural arm positions. Place frequently accessed controls between waist and shoulder height within 40-60cm reach. Avoid requiring extended periods of arm elevation or repetitive strenuous movements.

9. 🔧 **Platform Integration**: Utilize device-specific capabilities appropriately—hand tracking quality, spatial audio support, passthrough MR features, and input options vary by Pico model (Pico 4, Neo 3, etc.). Consult hardware-specific guides and test on target devices to ensure consistent experiences across the Pico ecosystem.

10. 🧪 **Rigorous User Testing**: Test comfort, performance, and accessibility with diverse user groups. Pain points like unintuitive gestures, small text, slow responsiveness, and accessibility barriers are often only revealed through real user testing. Iterate based on feedback to continuously improve usability, comfort, and inclusiveness of VR experiences.

## Keywords

- **OpenXR**: Open, royalty-free standard for VR and AR applications that provides cross-platform API access, enabling developers to build once and deploy across multiple XR devices.

- **Hand Tracking**: Computer vision technology that detects and tracks hand positions and gestures without requiring controllers, enabling natural interaction in VR.

- **Spatial Audio**: 3D audio positioning that creates realistic sound environments where audio sources have directional and distance properties matching visual elements.

- **Passthrough MR (Mixed Reality)**: Camera-based feature that allows users to see their real-world environment while wearing a VR headset, enabling mixed reality experiences.

- **Frame Rate**: Number of images displayed per second (measured in Hz), critical for VR comfort with 90Hz minimum and 120Hz preferred for optimal experiences.

- **Latency**: Time delay between user action and system response; low latency (under 20ms) is essential for preventing motion sickness and maintaining immersion.

- **Level of Detail (LOD)**: Optimization technique that renders objects at different quality levels based on distance from viewer, improving performance without noticeable quality loss.

- **Adaptive Rendering**: Dynamic adjustment of graphics quality based on performance metrics to maintain consistent frame rates.

- **Contextual UI**: Interface elements that appear or change based on user actions, focus, or environmental context rather than being persistently visible.

- **Ergonomic Design**: Interface and interaction design that considers human physical capabilities and limitations to minimize fatigue and maximize comfort.

- **Reach Envelope**: The 3D volume of comfortable arm reach without straining, typically 40-60cm from body at waist to shoulder height.

- **Device Manifest**: Android configuration file specifying app requirements, permissions, and device compatibility for Pico hardware.

- **6DoF (Six Degrees of Freedom)**: Tracking that monitors both rotational and positional movement in 3D space for natural interaction.