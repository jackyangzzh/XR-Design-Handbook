---
layout: default
title: Consolidated XR Design Guide
nav_order: 2
---

# Consolidated XR Design Guide
{: .no_toc }

A comprehensive synthesis of XR design principles from Apple, Meta, Microsoft, Google, Magic Leap, and Qualcomm.
{: .fs-6 .fw-300 }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Introduction

This guide consolidates design principles and best practices from major technology companies working in Extended Reality (XR), including Virtual Reality (VR), Augmented Reality (AR), and Mixed Reality (MR). Rather than navigating multiple company-specific guidelines, this document provides a unified framework organized by key design areas.

**Sources:** Apple visionOS, Meta Quest, Microsoft HoloLens, Google ARCore, Magic Leap, and Qualcomm Spaces.

---

## 1. Spatial Design Fundamentals

### 1.1 Human-Centered Design

**Core Principle:** Design with ergonomics and natural human behavior at the forefront.

- **Field of View (FOV):** Place critical content within the user's comfortable viewing area (typically 30°x30° from center)
- **Ergonomic Positioning:** Design interfaces relative to the user's natural head position and arm reach
- **Neutral Body Positions:** Promote comfortable postures and avoid requiring strenuous, repetitive, or extended arm movements
- **Content Distance:** Keep most content between 0.37m (minimum) and 5m from the user to prevent vergence-accommodation conflict and ensure comfort

**Company-Specific Insights:**
- *Apple:* Points system ensures scalable interface elements at different distances
- *Microsoft:* HoloLens displays are optimized at 2.0m optical distance
- *Magic Leap:* OCPA (Optimal Content Placement Area) is 30°x30° for always-visible content

### 1.2 Dimensionality and Scale

**Core Principle:** Leverage depth, scale, and spatial relationships to create hierarchy and immersive experiences.

- **Depth Hierarchy:** Use distance and layering to establish visual importance
- **Scale Appropriately:** Size objects based on their real-world counterparts and functional purpose
- **Spatial Audio:** Position audio to match visual elements, enhancing realism and spatial awareness
- **Soft Edges:** Blend virtual content with physical surroundings for seamless integration

**Key Techniques:**
- Use binocular and monocular depth cues (occlusion, shadows, parallax)
- Implement proper occlusion to make virtual objects feel grounded in physical space
- Apply consistent lighting that responds to the environment

---

## 2. User Interaction

### 2.1 Hand and Gesture Interaction

**Core Principle:** Design intuitive, natural hand interactions that minimize fatigue and false activations.

**Standard Gestures:**
- **Pinch:** Primary selection mechanism
- **Drag:** Move objects or scroll content
- **Zoom/Rotate:** Two-finger pinch-spread and twist motions
- **Pointing:** Ray-casting for distant object selection

**Best Practices:**
- Limit the number of gestures and make them distinct from one another
- Teach gestures gradually through tutorials, not all at once
- Provide continuous visual and audio feedback during interactions
- Design for both distal (distant) and proximal (close-range) interactions
- Avoid requiring overlapping hands to prevent tracking occlusion
- Support one-handed interactions when possible

**Button Design:**
- Near-field buttons: Large enough for accurate finger interaction
- Far-field buttons: Consider angular size for distant interactions
- Multiple states: default, focus, hover, pressed
- Clear visual feedback for each state transition

### 2.2 Eye Tracking and Gaze

**Core Principle:** Use eye direction as a signal of intent, not just as a pointer.

- **Indirect Interaction:** Combine gaze with hand gestures (look + pinch pattern)
- **Target Selection:** Eye focus determines which object will be affected by hand gestures
- **Precision:** Eye tracking enables more accurate interactions than head tracking alone
- **Privacy:** Be mindful of gaze data privacy and use it ethically

**Implementation Tips:**
- Pair voice commands with gaze for targeting specific objects
- Use gaze as the origin point for zooming or other transformations
- Don't require sustained gaze to avoid eye fatigue

### 2.3 Voice Input

**Core Principle:** Voice should complement, not replace, other interaction methods.

**Effective Voice Design:**
- **"See It, Say It":** Label voice commands directly in the interface
- **Universal Commands:** Support common commands like "Select," "Back," "Home"
- **Context-Aware:** Combine voice with gaze to determine target objects
- **Natural Language:** Allow conversational commands where appropriate

**Considerations:**
- Social acceptability varies by context (public vs. private)
- Provide visual feedback for voice recognition
- Support dictation for text input as alternative to virtual keyboards
- Account for ambient noise and reliability challenges

### 2.4 Direct Touch Interaction

**Core Principle:** Allow users to physically reach and touch virtual elements when appropriate.

- **Ergonomic Reach:** Place interactive elements within comfortable arm's reach (0.4-0.6m)
- **Touch Feedback:** Use audio and visual cues to compensate for lack of haptic feedback
- **Appropriate Use Cases:** Virtual keyboards, drawing interfaces, close object manipulation
- **Fatigue Prevention:** Don't require extended periods of arm elevation

---

## 3. Object Manipulation

### 3.1 Selection and Highlighting

**Techniques for Clear Selection:**
- Color changes or glowing outlines
- Scale changes or hover effects
- Audio cues on focus
- Distinct visual states (default, focused, selected)

### 3.2 Translation (Movement)

**Best Practices:**
- **Intuitive Controls:** On-screen dragging or physical device movement
- **Surface Transitions:** Allow smooth movement between different surfaces
- **Clear Boundaries:** Use visual cues (grids, shadows, opacity changes) to show movement limits
- **Multiple Surfaces:** Encourage exploration across the environment while maintaining smooth transitions

### 3.3 Rotation and Scaling

**Rotation:**
- Support free rotation in any direction
- Provide both manual (gesture) and automatic (animation) rotation
- Enable single-finger and multi-finger rotation gestures

**Scaling:**
- Pinch-to-zoom gesture pattern
- Set minimum and maximum size limits
- Maintain object proportions unless design specifically requires distortion
- Consider the viewing distance when setting scale limits

### 3.4 Advanced Interactions

**Pinch-and-Pull:**
- Provides tactile sense in virtual space
- Enables 1D, 2D, and 3D picker components
- Useful for color selection, sliders, and dimensional controls

**Proximity Handling:**
- Use two-finger gestures to disambiguate close objects
- Implement smart selection based on context and size
- Provide visual feedback when multiple objects are in range

---

## 4. Comfort and Motion

### 4.1 Preventing Motion Sickness

**Critical Factors:**
- **Frame Rate:** Maintain consistent, high frame rates (90+ FPS)
- **Head Tracking:** Ensure precise, low-latency head tracking
- **IPD Calibration:** Allow users to calibrate interpupillary distance
- **Minimize Judder:** Use Asynchronous Time Warp (ATW) or similar techniques

### 4.2 Locomotion Design

**Comfort Hierarchy (Most to Least Comfortable):**
1. Teleportation
2. Forward movement on flat terrain
3. Lateral movement (strafing)
4. Backward movement
5. Vertical movement (stairs, elevators, slopes)

**Best Practices:**
- Design primarily for forward movement
- Keep walls and large structures at a distance to reduce optic flow
- Provide teleportation options for stairs and slopes
- For continuous movement, use Independent Visual Backgrounds (IVB)
- Implement simulated physical activities (walking in place) for better vestibular alignment

**Reducing Discomfort:**
- Minimize slopes and vertical accelerations
- Simplify stair and elevator designs to reduce visual complexity
- Use spatial sound effects during transitions
- Provide clear visual anchors (skybox, cockpit frame)

### 4.3 Content Movement

**Guidelines:**
- Avoid rapid or unexpected object movement in user's field of view
- Minimize Z-axis movement (toward/away from user)
- Provide clear animation curves for object transitions
- Allow users to control pacing of content changes
- Never move the ground plane unexpectedly

---

## 5. User Interface Design

### 5.1 Window and Layout Design

**Spatial Windows:**
- **Glass Material:** Use semi-transparent materials that adapt to different lighting
- **Flexible Sizing:** Allow windows to resize based on content needs
- **Multiple Windows:** Support multi-window workflows for complex tasks
- **Tabs and Toolbars:** Extend beyond window bounds for quick access

### 5.2 UI Behavior Modes

Choose the appropriate UI anchoring based on use case:

- **Head-Relative:** UI follows head movement (use sparingly, can cause fatigue)
- **Body-Relative:** UI follows body orientation, reorients after significant head rotation
- **World-Relative:** UI fixed to physical space location
- **Input-Relative:** UI position determined by controller or hand position

**HUD Design:**
- Avoid head-locked HUDs that follow every head movement
- Use body-relative positioning for status information
- Provide clear visual separation from scene content
- Don't obstruct critical view areas

### 5.3 Visual Clarity

**Text and Typography:**
- **Minimum Font Size:** Consider viewing distance and display resolution
- **High Contrast:** Ensure readability against all background types
- **Dynamic Type:** Support adjustable text sizes for accessibility
- **Anti-Aliasing:** Use appropriate anti-aliasing for sharp text rendering

**Visual Effects:**
- Use lens distortion, chromatic aberration, and depth of field sparingly
- Avoid full-screen effects that disorient users
- Minimize persistent 2D overlays that break immersion
- Use animation to enhance, not distract from, core experience

### 5.4 UI Organization

**Content Structure:**
- Group similar objects following Gestalt principles
- Place objects within reach and sight
- Size elements appropriately for viewing distance
- Avoid obstructing the user's natural field of view
- Use contextual UI that adapts based on user focus and actions

---

## 6. Immersion Spectrum

### 6.1 Levels of Immersion

**Windowed Mode:**
- Apps share space with physical environment
- Multiple apps can coexist
- Good for productivity and multitasking

**Partial Immersion:**
- App content extends into 3D space
- Physical environment partially visible
- Balances immersion with real-world awareness

**Full Immersion:**
- Complete virtual environment
- Physical world replaced or heavily occluded
- Maximum presence and focus

### 6.2 Transition Design

**Best Practices:**
- **Clear Entry/Exit:** Provide obvious ways to enter and exit immersive modes
- **Gradual Transitions:** Use fade, blur, or scaling effects to ease transitions
- **User Control:** Let users initiate transition timing
- **Visual Continuity:** Maintain orientation and object relationships during transitions

### 6.3 Passthrough and Mixed Reality

**Passthrough Techniques:**
- **Background Passthrough:** Real-world view with virtual overlays
- **Selective Windows:** Portal views into physical environment
- **Stylization:** Apply artistic effects to camera passthrough
- **Blending:** Combine virtual and real with proper occlusion and shadows

**MR-Specific Considerations:**
- Use spatial anchors to align virtual content with physical objects
- Implement proper occlusion for realistic object placement
- Add shadows to ground virtual objects
- Avoid mixing realities without clear 1:1 correspondence

---

## 7. Accessibility

### 7.1 Vision Accessibility

**Core Practices:**
- **VoiceOver Support:** Provide accurate labels, traits, and descriptions for all interactive elements
- **High Contrast:** Ensure 4.5:1 contrast ratio for text
- **Large Touch Targets:** Minimum 44x44 points for interactive elements
- **Camera Anchors:** Use sparingly; prefer world anchors for content users may need to examine closely
- **Alternative Formats:** Provide non-visual alternatives for visual-only information

### 7.2 Motor Accessibility

**Alternative Inputs:**
- **Dwell Control:** Selection without hand gestures
- **Pointer Control:** Head or finger-based focus control
- **Voice Commands:** Complete voice-based navigation option
- **Switch Control:** Support for external adaptive devices

**Design Considerations:**
- Don't require precise timing
- Provide large, easy-to-hit targets
- Avoid requiring simultaneous multi-button presses
- Support one-handed operation

### 7.3 Cognitive Accessibility

**Simplification Strategies:**
- **Guided Access:** Lock to single app to minimize distractions
- **Clear Navigation:** Obvious paths through experiences
- **Consistent Patterns:** Use familiar interaction models
- **Undo/Redo:** All actions should be reversible
- **Clear Feedback:** Confirm actions with visual and audio cues

**Content Guidelines:**
- Provide visual and audio cues for navigation in full 360° space
- Minimize cognitive load through contextual UI
- Use clear, simple language
- Avoid time-limited interactions when possible

### 7.4 Hearing Accessibility

**Essential Features:**
- **Comprehensive Captions:** Caption all audio content, including sound effects
- **Customizable Captions:** Size, color, background options
- **Visual Alerts:** Alternative to audio-only notifications
- **Spatial Visual Cues:** Direction indicators for sound sources

---

## 8. Multiplayer and Shared Experiences

### 8.1 Shared Space Design

**Synchronization:**
- Coordinate surface detection across devices
- Maintain consistent spatial anchors
- Handle network latency gracefully
- Provide clear indicators of other users' presence and actions

### 8.2 Social Interaction

**Best Practices:**
- Show other users' gaze direction and gestures
- Provide personal space boundaries
- Support voice communication with spatial audio
- Allow users to control their visibility and participation level

### 8.3 Onboarding for Multiplayer

**Smooth Entry:**
- Visual/audio cues to guide users to shared space
- Simple, intuitive connection process
- Clear status indicators for connection state
- Graceful handling of disconnections

---

## 9. Performance and Technical Considerations

### 9.1 Rendering Performance

**Critical Metrics:**
- **Frame Rate:** Target 90 FPS minimum, 120 FPS preferred
- **Latency:** Motion-to-photon latency under 20ms
- **Draw Calls:** Minimize to maintain performance
- **Polygon Count:** Optimize mesh complexity

**Optimization Strategies:**
- Use level-of-detail (LOD) systems
- Implement occlusion culling
- Optimize texture sizes and formats
- Use instancing for repeated objects

### 9.2 Visual Stability

**Maintaining Stability:**
- Accurate environment tracking
- Persistent spatial anchors
- Smooth transitions between tracking states
- Fallback behaviors for tracking loss

### 9.3 Privacy and Security

**Data Handling:**
- Minimize collection of gaze data
- Store spatial mesh data locally when possible
- Provide clear privacy policies
- Request permissions with clear explanations
- Secure multiplayer communications

---

## 10. Onboarding and Error States

### 10.1 Effective Onboarding

**Progressive Disclosure:**
- Introduce features gradually
- Use interactive tutorials
- Provide contextual help
- Allow users to skip tutorials on repeat visits

**First Launch Experience:**
- Clear value proposition
- Smooth transition from 2D to spatial
- Visual cues for initialization
- User control over when to begin

### 10.2 Error Handling

**Clear Error States:**
- Specific, actionable error messages
- Visual indicators of what went wrong
- Suggestions for resolution
- Easy way to retry or recover

**Common Error Scenarios:**
- Tracking loss: Provide clear guidance to re-establish tracking
- Poor lighting: Indicate need for better lighting conditions
- Limited space: Suggest alternative play area or scaled experience
- Occlusion issues: Guide hand positioning for better tracking

---

## 11. Audio Design

### 11.1 Spatial Audio

**Immersive Sound:**
- Position audio sources to match visual elements
- Use Head-Related Transfer Functions (HRTF) for realistic positioning
- Implement proper distance attenuation
- Add environmental reverb and occlusion

### 11.2 Feedback Audio

**Interaction Sounds:**
- Confirm selections with distinct audio cues
- Provide directional feedback for off-screen events
- Use audio to enhance physical realism (footsteps, object impacts)
- Don't overuse audio to avoid fatigue

### 11.3 Voice and Dialogue

**Clear Communication:**
- Spatial positioning for dialogue sources
- Clear separation from background audio
- Support for multiple languages
- Volume controls independent of effects

---

## 12. Content Strategy

### 12.1 Contextual Design

**Adaptive Experiences:**
- Track user focus and adapt available elements
- Minimize visual clutter through contextual menus
- Show relevant information at relevant times
- Respect user attention and flow state

### 12.2 Content Placement Hierarchy

**Priority Zones:**
1. **Primary Zone (0-2m):** Interactive elements, text, primary content
2. **Secondary Zone (2-5m):** Contextual information, environmental elements
3. **Tertiary Zone (5m+):** Background, atmosphere, distant landmarks

### 12.3 Stylization and Aesthetics

**Visual Style:**
- Authentic spatial experiences that utilize platform capabilities
- Consistent art direction
- Purposeful use of color for attention and emotion
- Balance between realism and stylization based on experience goals

---

## Quick Reference Checklist

Use this checklist to ensure your XR experience follows core principles:

### Core Design
- ☐ Content placed between 0.37m - 5m from user
- ☐ Critical UI within 30°x30° field of view
- ☐ Consistent 90+ FPS frame rate
- ☐ Proper depth cues (occlusion, shadows, parallax)
- ☐ Smooth transitions between interaction modes

### Interaction
- ☐ Standard gestures work as expected (pinch, drag, zoom, rotate)
- ☐ Clear visual feedback for all interactive elements
- ☐ Support for both direct and indirect interaction
- ☐ Voice commands labeled when available
- ☐ Minimal required arm movement

### Comfort
- ☐ Primarily forward movement for locomotion
- ☐ Teleportation option for vertical navigation
- ☐ No sudden unexpected movements
- ☐ Walls kept at comfortable distance
- ☐ Head-locked UI avoided or minimized

### Accessibility
- ☐ VoiceOver labels for all interactive elements
- ☐ High contrast text (4.5:1 minimum)
- ☐ Alternative to gesture-only interactions
- ☐ Captions for all audio content
- ☐ Large touch targets (44x44 points minimum)

### Polish
- ☐ Clear onboarding experience
- ☐ Helpful error messages
- ☐ Spatial audio matches visuals
- ☐ Smooth enter/exit from immersion
- ☐ Tested on target devices

---

## Company-Specific Deep Dives

For detailed, platform-specific guidelines:

- **[Apple visionOS](/docs/Apple)** - Spatial computing, window design, SwiftUI integration
- **[Meta Quest](/docs/Meta)** - Hand tracking, MR passthrough, locomotion
- **[Microsoft HoloLens](/docs/Microsoft)** - Enterprise MR, spatial mapping, voice input
- **[Google ARCore](/docs/Google)** - Mobile AR, surface detection, lighting
- **[Magic Leap](/docs/Magic%20Leap)** - Spatial computing, controller interaction, enterprise applications
- **[Qualcomm Spaces](/docs/Qualcomm)** - Hand tracking, cross-platform XR

---

## Glossary

**Accommodation:** The eye's ability to change focus for different distances.

**Affordance:** Design characteristic that suggests how an object should be used.

**Binocular Disparity:** The difference between images seen by left and right eyes, enabling depth perception.

**Dwell Control:** Interaction method that selects elements by gazing at them for a set duration.

**Field of View (FOV):** The extent of the observable world visible at any moment.

**Haptic Feedback:** Tactile sensations used to communicate information to users.

**IPD (Interpupillary Distance):** Distance between the centers of the pupils of the two eyes.

**Occlusion:** When one object blocks another from view, providing depth information.

**Optic Flow:** Pattern of apparent motion in the visual field caused by movement.

**Passthrough:** Technology allowing users to see the real world through VR headset cameras.

**Spatial Anchor:** Reference point that maintains virtual object position in physical space.

**Vection:** Sensation of self-motion induced by visual stimuli.

**Vergence:** Simultaneous rotation of eyes to focus on an object.

**Vergence-Accommodation Conflict:** Mismatch between focus distance and eye convergence in VR displays.

---

## Conclusion

This consolidated guide synthesizes best practices from leading XR platforms. While each platform has unique capabilities and constraints, these core principles provide a foundation for creating comfortable, intuitive, and accessible XR experiences.

**Key Takeaways:**
1. **Human-Centered:** Always prioritize user comfort and natural interaction patterns
2. **Accessible:** Design for diverse abilities from the start
3. **Performant:** Maintain high frame rates and low latency
4. **Intuitive:** Leverage familiar patterns while embracing spatial capabilities
5. **Tested:** Validate designs with real users on target hardware

For the latest updates and platform-specific details, always refer to the original design guidelines from each company.

---

*Last Updated: 2024*
*This guide synthesizes information from official design guidelines from Apple, Meta, Microsoft, Google, Magic Leap, and Qualcomm. For platform-specific implementation details, please refer to the individual company documentation.*
