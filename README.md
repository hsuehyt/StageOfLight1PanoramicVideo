# Stage of Light - One Panoramic Video

**Stage of Light - One Panoramic Video** is a Unity project designed for NTNU Art Museum. It enables the projection of a single panoramic video onto the walls and floors of the immersive projection space, "Stage of Light." This space utilizes a Windows-based dome projection system that integrates with **Resolume Arena** to display the Unity project's build folder seamlessly.

![Stage of Light Scene Preview](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20101251.png)

---

## About the Panoramic Video

The panoramic video format allows for **seamless playback across the entire room**, creating an immersive experience that spans walls and floors. 

### Versatility
- The video format is **universal**, meaning it can be played on various platforms, including VR systems and dome projection systems of different shapes.

### Room Shape Considerations
Due to the **eccentric shape of "Stage of Light"**, which deviates from an ideal straight cube or dome shape, parts of the image may be **cut or distorted during projection**. To minimize image loss or distortion in such non-standard spaces, **careful alignment and testing** are strongly recommended.

---

## Getting Started

### Prerequisites
Ensure you have **Unity Editor 2021.3.6f1** or later installed. The version 2021.3.6f1 is recommended.

### Installation
1. Download the latest release of the repository from [GitHub Releases](https://github.com/hsuehyt/StageOfLight1PanoramicVideo).
   - Extract the zip file.
   - Add the project folder to Unity Hub.
2. Alternatively, clone the repository:
   ```bash
   git clone https://github.com/hsuehyt/StageOfLight.git
   ```

### Opening the Project
1. Open the project in Unity.
2. Navigate to `Assets/StageOfLight/` and open the scene `1PanoramicVideo`.

### Testing the Scene
1. Click **Play** in the Unity Editor to test the scene. Verify everything works, then stop playback.

---

## Adding Your Video
1. Import your video asset into Unity.
2. In the **Hierarchy** panel, select `VideoPlayer`.
3. In the **Inspector** panel, under `VideoPlayer > Video Clip`, replace the demo video by dragging your video file into the slot.
4. Play the scene to ensure it works as expected, then stop playback.

---

## Video Format and Recommendations

### Suggested Video Format
- **Resolution**: 4K (4096x2048).  
  Unity’s Video Player currently supports up to 4K for panoramic videos. For immersive or VR experiences, **8K resolution** is recommended; however, Unity's built-in player does not yet support it.

### Aspect Ratio
- **Panoramic videos** typically use a **2:1 aspect ratio** (width to height), which should be maintained during encoding.

### Encoding with Adobe Media Encoder
- **Preset**: `H.264 > Match Source - Adaptive Low Bitrate`  
  - This preset ensures optimal compression and retains the source resolution and aspect ratio.
  - For higher quality, choose `Match Source - Adaptive High Bitrate`.  
    ⚠ **Note**: Be cautious when using high bitrate for longer videos, as it may cause playback issues due to increased file size and data load.

![Adobe Encoder Settings](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20134307highlighted.png)

### Projection Mapping
- Panoramic videos are often mapped in **equirectangular format**, a common format for VR 360 content. 
- Sources for equirectangular footage:
  - **360 cameras** (for live-action footage).
  - Rendering from **3D animation tools** like Maya, Blender, or Unity.
  - Generated by **AI tools** (e.g., ChatGPT for still images, followed by animation in video AI tools).

---

## Building the Project
1. Open **File > Build Settings**.
2. Ensure that only `StageOfLight/PanoramicVideo` is checked under **Scenes In Build**.
3. Click **Build**, and follow the prompts to generate the build folder.

---

## Demo Video
[![Watch the Demo Video](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20132004cropped.png)](https://youtu.be/3P2WE4laE2U)

---

## Credits

- **Original Unity Project Design**: [李綠恩 Lu-En Li](https://github.com/LeeMegumi)
- **Project Revision and Tutorial Demonstration**: [薛佑廷 Yuting Hsueh](https://github.com/hsuehyt)

### Supervising Institutions
- **Advanced Display Technology & Interdisciplinary Talent Cultivation Project Office**, Ministry of Education
- **NTNU Advanced Display Technology Integration & Promotion in Art Venues**
- **NTNU Art Museum**