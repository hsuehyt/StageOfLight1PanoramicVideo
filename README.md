# Stage of Light - One Panoramic Video

**Stage of Light - One Panoramic Video** is a Unity project designed for NTNU Art Museum. It enables the projection of a single panoramic video onto the walls and floors of the immersive projection space, "Stage of Light." This space utilizes a Windows-based dome projection system that integrates with **Resolume Arena** to display the Unity project's build folder seamlessly.

![Stage of Light Scene Preview](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20101251.png)

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

## Building the Project
1. Open **File > Build Settings**.
2. Ensure that only `StageOfLight/PanoramicVideo` is checked under **Scenes In Build**.
3. Click **Build**, and follow the prompts to generate the build folder.

---

## Demo Video
[![Watch the Demo Video](https://img.youtube.com/vi/3P2WE4laE2U/maxresdefault.jpg)](https://youtu.be/3P2WE4laE2U)

---

## Credits

- **Original Unity Project Design**: [李綠恩 Lu-En Li](https://github.com/LeeMegumi)
- **Project Revision and Tutorial Demonstration**: [薛佑廷 Yuting Hsueh](https://github.com/hsuehyt)

### Supervising Institutions
- **Advanced Display Technology & Interdisciplinary Talent Cultivation Project Office**, Ministry of Education
- **NTNU Advanced Display Technology Integration & Promotion in Art Venues**
- **NTNU Art Museum**