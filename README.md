# Stage of Light - One Panoramic Video

![Stage of Light Scene Preview](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20101251cropped.png)

**Stage of Light - One Panoramic Video** is a Unity project designed for NTNU Art Museum. It enables the projection of a single panoramic video onto the walls and floors of the immersive projection space, "Stage of Light." This space utilizes a Windows-based dome projection system that integrates with **Resolume Arena** to display the Unity project's build folder seamlessly.

---

## Table of Contents
1. [Features](#features)
2. [Getting Started](#getting-started)
3. [Adding Your Video](#adding-your-video)
4. [Video Format and Recommendations](#video-format-and-recommendations)
5. [Building the Project](#building-the-project)
6. [Demo Video](#demo-video)
7. [Credits](#credits)

---

## Features

- **Seamless Playback:** The panoramic video format allows playback across the entire immersive space.
- **Platform Agnostic:** Compatible with VR systems, dome projection systems, and Unity environments.
- **Customizable Content:** Easily replace demo content with your own panoramic videos.

---

## Getting Started

### Prerequisites
- Unity Editor **2021.3.6f1** or later is required (2021.3.6f1 is recommended).

### Installation
1. Clone or download the project:
   ```bash
   git clone https://github.com/hsuehyt/StageOfLight.git
   ```
2. Extract the zip file (if downloaded) and add the project to Unity Hub.
3. Open the project in Unity.

### Opening the Scene
1. Navigate to `Assets/StageOfLight/`.
2. Open the scene named **`1PanoramicVideo`**.
3. Click **Play** to test the scene.

---

## Adding Your Video

1. Import your video asset into Unity.
2. In the **Hierarchy** panel, select `VideoPlayer`.
3. In the **Inspector** panel, under `VideoPlayer > Video Clip`, replace the demo video by dragging your video into the slot.
4. Test the video by playing the scene.

---

## Video Format and Recommendations

### Suggested Format
- **Resolution:** 4K (4096x2048). For immersive/VR experiences, use **8K**, but note that Unity's Video Player currently supports up to **4K**.
- **Aspect Ratio:** Maintain a **2:1 aspect ratio** (width to height) for panoramic videos.

### Encoding with Adobe Media Encoder
- **Preset:** `H.264 > Match Source - Adaptive Low Bitrate`
- For better quality, use `Match Source - Adaptive High Bitrate`.

⚠ **Note:** High bitrate can cause playback issues for longer videos due to increased file sizes.

![Adobe Encoder Settings](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20134307highlighted.png)

### Projection Mapping
Panoramic videos should use the **equirectangular format**, commonly used for VR 360 content:
- **Sources:**  
  - 360 cameras (for live-action footage)  
  - Rendering from 3D tools like **Maya**, **Blender**, or **Unity**  
  - AI-generated content (e.g., text-to-360, image-to-360, image-to-video)

### Room Shape Considerations
- Due to the **eccentric shape of "Stage of Light"**, which deviates from an ideal straight cube or dome shape, parts of the image may be **cut or distorted during projection**.  
- To minimize image loss, ensure **careful alignment and testing**.

---

## Building the Project

1. Open **File > Build Settings** in Unity.
2. Check **StageOfLight/PanoramicVideo** in **Scenes in Build**.
3. Click **Build**, and follow the prompts to create the build folder.

---

## Demo Video

[![Watch the Demo Video](https://img.youtube.com/vi/dlJjMRLl21g/0.jpg)](https://youtu.be/dlJjMRLl21g)

---

## Credits

- **Original Unity Project Design:** [李綠恩 Lu-En Li](https://github.com/LeeMegumi)
- **Project Revision and Tutorial Demonstration:** [薛佑廷 Yuting Hsueh](https://github.com/hsuehyt)

### Supervising Institutions
- **Advanced Display Technology & Interdisciplinary Talent Cultivation Project Office**, Ministry of Education  
- **NTNU Advanced Display Technology Integration & Promotion in Art Venues**  
- **NTNU Art Museum**