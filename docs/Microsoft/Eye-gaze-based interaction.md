---
layout: default
title: Eye-gaze-based interaction
parent: Microsoft
---

# Eye-gaze-based interaction 
Original article: [Eye-gaze-based interaction](https://learn.microsoft.com/en-us/windows/mixed-reality/design/eye-gaze-interaction)

## TL;DR

HoloLens 2 integrates eye tracking as a new user input, enhancing the immersive experience. While eye-gaze offers rapid interactions, it comes with challenges like unintentional actions. Design recommendations include differentiating eye-gaze from head-gaze and combining it with other inputs for a seamless experience.

## Bullet points
1. 🕶️ **HoloLens 2 Eye Tracking**: HoloLens 2 introduces a revolutionary feature: eye tracking. This technology allows the device to understand where a user is looking, creating a more intuitive and immersive user experience. Before users can fully utilize this feature, they need to undergo a calibration process, ensuring the device accurately captures their unique eye movements.

2. 🎮 **Holographic Shell Experience**: The Holographic Shell is the main user interface users encounter when starting up their HoloLens 2. In this interface, eye-gaze input is subtly integrated, enhancing the overall experience by adding a layer of intuitiveness without being the primary mode of interaction.

3. 🌟 **Benefits of Eye-gaze Input**: The human eye's speed makes it an excellent tool for high-speed pointing. Combined with the minimal physical effort required to move one's eyes, this offers a seamless interaction method. The system can predict user intentions due to the implicit nature of eye movements. Furthermore, eye-gaze complements other input methods, capitalizing on years of hand-eye coordination experience. Lastly, the system can determine user attention, which has vast implications for UI design and remote communication.

4. 🚫 **Challenges of Eye-gaze Input**: Eye movements come with challenges when used as an input method. The risk of unintentional actions, the balance between observation and control, potential misalignments with slower manual inputs, discomfort from targeting small objects, and the rapid nature of eye movements can be challenging to track accurately. Changing light conditions can affect tracking reliability.

5. 📌 **Differentiating Eye-gaze and Head-gaze**: Designers need to understand the distinction between where a user is looking (eye-gaze) and where they are pointing their head (head-gaze). Tasks requiring smooth trajectories, like drawing, are better suited for hand or head pointing.

6. 🚀 **Eye-gaze's Power**: Eye-gaze stands out as a powerful input method because of its speed and the minimal effort it requires. When combined with other inputs like voice or hand gestures, it provides a rich contextual signal that can confirm a user's intent.

7. 🎯 **Target Size and Comfort**: For optimal user experience, designers should ensure that targets or interactive elements are of a comfortable size. A reference point is that these targets should be at least 2° in visual angle, which is roughly the size of your thumbnail when you stretch out your arm.

8. 🤝 **Combining Eye-gaze with Other Inputs**: It's beneficial to combine eye-gaze with other inputs like voice or hand gestures to prevent unintentional actions and to provide a richer interaction context. This combination allows for a more immersive and intuitive user experience.

9. 🎨 **Subtle Feedback for Eye Tracking**: Feedback for eye-gaze should be subtle to avoid overwhelming users. Slowly blending in and out, visual highlights, or other subtle target behaviors can indicate that the system correctly detected the user's gaze without interrupting their workflow.

10. 🚫 **Avoiding Specific Eye Movements**: Enforcing specific eye movements as inputs can be counterintuitive and should be avoided. Instead, designers should focus on natural and intuitive interactions that align with the user's expectations and behaviors.

## Keywords
- **HoloLens 2**: Microsoft's mixed reality smart glasses that overlay holograms on the real world.
  
- **Eye Tracking**: A technology that determines where a user is looking, used as an input method in HoloLens 2.
  
- **Calibration**: The process of adjusting the eye tracking system to work accurately for an individual user.
  
- **Holographic Shell**: The main user interface of the HoloLens 2.
  
- **Implicitness**: The quality of being implied or understood without being directly expressed.
  
- **Visual Attention**: The process by which a user focuses on specific visual information.
  
- **Eye-gaze**: The direction in which a person's eyes are looking.
  
- **Head-gaze**: The direction in which a person's head is pointing.
  
- **DirectX**: A collection of APIs for handling tasks related to multimedia, especially game programming and video, on Microsoft platforms.
