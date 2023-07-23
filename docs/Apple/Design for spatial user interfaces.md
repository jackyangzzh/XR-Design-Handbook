---
layout: default
title: Design for spatial user interfaces
parent: Apple
---

# Design for spatial user interfaces
Original video: [Design for spatial user interfaces](https://developer.apple.com/videos/play/wwdc2023/10076/)

## TL;DR
The video discusses designing iOS applications, outlining core structures like a window for content, a tab bar for main navigation, and sidebars for sub-navigation. It introduces a new feature, "ornaments", that can expand or disappear based on user interaction. It also covers additional interactive elements like menus, popovers, and sheets (modals) that can extend interactions beyond the window. The video emphasizes the use of the platform's spatial capabilities to create immersive experiences.

## Bullet Points
1. 🪟 **Window:** The iOS app structure is built around a core element known as a window. It's not just a display frame, but a canvas that holds all interactive elements. It's made of an opaque material, providing a stage for all app components. The design ensures a fluid movement in the user's space.

2. 🎚 **Tab Bar Controller:** On iPhone, it traditionally sits at the bottom, enabling primary navigation within the app. In this new platform, it's vertically oriented and is positioned on the left, floating in a fixed position.

3. 📌 **Sidebar:** A sidebar co-exists with the tab bar providing an additional layer of navigation. It's particularly useful where users need to navigate between multiple sections or subsections within a tab.

4. 🎈 **Ornaments:** A new presentation style called "ornaments" are floating accessories placed in various locations on the interface. They serve as persistent control tools, enabling quick actions related to the content. They leverage depth to create a hierarchy within the interface.

5. 🎧 **Music App Ornaments:** The Now Playing controls are presented as a floating ornament that persists no matter where a user navigates within the app. It allows users to control their music playback while exploring other parts of the app.

6. 🍥 **Menus and Popovers:** They have been designed to expand outside the app window. They appear centered by default, and the button that invokes them changes to its selected state, featuring black labels on a white background.

7. 📑 **Sheets:** They are designed to present modal views and they appear at the center of the app. They maintain the same Z position as the parent window, which is pushed back and dimmed.

8. 🎀 **Secondary Modals:** If another sheet needs to be presented while one is already open, a secondary modal appears with an additional layer of dimming, pushing everything else back.

9. 🗺 **Push Navigation:** It's recommended for nested views. Instead of a close button, a back button is presented in the top-left corner, enabling users to navigate back to the previous view.

10. 📸 **Leverage Spatial Capabilities:** Developers are urged to leverage the unique spatial capabilities of the platform, creating immersive experiences using the depth and spatiality that the platform provides.

## Keywords
- **iOS**: iOS is the operating system for Apple devices like the iPhone and iPad. It's the software that enables users to interact with their devices.
- **Window**: In the context of iOS app development, a window is a fundamental part of the user interface that provides the canvas for all other elements to sit on.
- **Tab bar controller**: This is a special type of view controller in iOS that lets users switch between different views (or tabs) at the same level of hierarchy in an app.
- **Sidebar**: In the context of app interfaces, a sidebar is a vertical panel that provides additional navigation or control options. It can be used for sub-navigation within a particular tab.
- **Ornaments**: A term used in the video to refer to floating accessory elements or controls in an app interface that provide additional functionality and are persistent, meaning they are always available.
- **Popover**: A popover is a transient view that shows up on the screen when a user taps a button or performs a certain action. It appears on top of your content and usually provides additional information or includes a list of actions.
- **Modal**: In the context of user interface design, a modal is a type of window that demands user interaction before they can return to the parent interface. It is used to focus the user's attention and is often used for alerts, data entry and other tasks that require user input before proceeding.
- **Sheet**: In the context of iOS development, a sheet refers to a specific style of modal window that presents content in a distinct layer over the parent view.
- **Spatial Captures**: It seems to be a term used within this specific platform to refer to a feature in the Photos app that provides an immersive way to view photos. The exact nature of the feature would likely be explained in more depth in the video or other related resources.
- **Z Position**: In 3D design or interface design involving depth, the Z position refers to the depth of an element or how far it appears to be from the user (away or closer to the screen).
- **Push Navigation**: In the context of user interface design, push navigation is a navigation style where new content is "pushed" onto the screen, typically from the right, replacing the current content.
