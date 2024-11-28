# Stage of Light - One Panoramic Video

![Stage of Light Scene Preview](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20101251cropped.png)

**Stage of Light - One Panoramic Video** is a Unity project developed for 臺師大美術館 NTNU Art Museum. It enables the seamless projection of a single panoramic video onto the walls and floors of the immersive exhibition space, "光影走廊 Stage of Light." This project integrates with a Windows-based dome projection system and **Resolume Arena**, ensuring a streamlined visual experience by running the Unity project's build folder effortlessly.

This project also incorporates multimedia tools such as **Keijiro.Klak.SPOUT** for Spout-based video output and **iam1337.extOSC** for Open Sound Control (OSC) functionality, providing a versatile framework for interactive and immersive installations.

For a solution using six flat videos, please refer to [Stage of Light - Six Customized Videos](https://github.com/hsuehyt/StageOfLight6CustomizedVideos).

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

- **Simplified Projection Setup:** A single panoramic video eliminates the need for aligning multiple videos across surfaces.  
- **High Immersion Potential:** Best suited for VR or dome-like environments where seamless panoramic playback is prioritized.  
- **Universal Playback Compatibility:** Supports multiple platforms, including VR systems and dome projection environments.  

---

## Getting Started

### Prerequisites
- Unity Editor **2021.3.6f1** or later (2021.3.6f1 is recommended).

### Installation
1. Clone or download the project:
   ```bash
   git clone https://github.com/hsuehyt/StageOfLight1PanoramicVideo
   ```
2. Extract the zip file (if downloaded) and add the project to Unity Hub.
3. Open the project in Unity.

### Opening the Scene
1. Navigate to `Assets/StageOfLight/`.
2. Open the scene named **`1PanoramicVideo`**.
3. Click **Play** to test the scene.

---

## Adding Your Video

![Adding Your Video Preview](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-21%20142845.png)

1. Import your video into `Assets/StageOfLight/`.
2. In the **Hierarchy** panel, select `VideoPlayer`.
3. In the **Inspector** panel, under `VideoPlayer > Video Clip`, drag and drop your panoramic video to replace the demo content.
4. Test the video by playing the scene.

---

## Video Format and Recommendations

### Format Specifications

![Equirectangular Projection Example](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/01_cubeGrid_Equirectangular360_7680x4320.png)

- **Resolution:** 4K (4096x2048) or higher. For immersive experiences, 8K is ideal, but Unity's Video Player currently supports up to **4K**.  
- **Aspect Ratio:** 2:1 (width to height).  
- **Format:** Equirectangular projection, commonly used for 360° panoramic content.

### Encoding with Adobe Media Encoder

![Adobe Media Encoder Settings](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/Screenshot%202024-11-18%20134307highlighted.png)

- **Preset:** `H.264 > Match Source - Adaptive Low Bitrate`  
- For better quality, use `Match Source - Adaptive High Bitrate`.

### Room Shape Considerations

![Room Shape Diagram](https://github.com/hsuehyt/StageOfLight1PanoramicVideo/blob/main/README/image_011_0000%207680x4320.png)

- The black area represents the ceiling, which is **not** a projection area.
- The green area represents the walls and floors, which are the **projection areas**.
- The irregular shape of the "Stage of Light" may lead to image cropping or distortion.
- Ensure thorough alignment and testing for optimal results.

---

## Building the Project

1. Open **File > Build Settings** in Unity.
2. Ensure **StageOfLight/PanoramicVideo** is checked in **Scenes in Build**.
3. Click **Build**, and follow the prompts to create the build folder.

---

## Demo Video

[![Watch the Demo Video](https://img.youtube.com/vi/dlJjMRLl21g/0.jpg)](https://youtu.be/dlJjMRLl21g)

---

## Credits

- **The Original Unity Project Developer:** [李綠恩 Lu-En Li](https://github.com/LeeMegumi)  
- **The Project Maintainer and Developer:** [薛佑廷 Yuting Hsueh](https://github.com/hsuehyt)  
- **Integrated Tools:**  
  - **Keijiro.Klak.SPOUT** from [Keijiro's Scoped Registry](https://github.com/keijiro)  
  - **iam1337.extOSC** from [OpenUPM](https://package.openupm.com)  

### Supervising Institutions
- **教育部 前瞻顯示科技與跨領域人才培育計畫 總計畫辦公室 Advanced Display Technology & Interdisciplinary Talent Cultivation Project Office, Ministry of Education**  
- **臺師大 前瞻顯示科技導入藝術場域建置與推廣計畫 NTNU Advanced Display Technology Integration & Promotion in Art Venues**
- **臺師大 美術館 NTNU Art Museum**