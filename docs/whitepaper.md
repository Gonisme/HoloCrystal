# Photon Matrix Technical Whitepaper

## 1. Abstract
Photon Matrix (public-facing name: HoloCrystal) is a novel volumetric display architecture that combines multi-layer dynamic optical modules with high-speed projection to create spatial images that closely resemble real 3D objects. The technology is currently in the prototype validation phase and is developed under an open-source model to encourage global collaboration.

## 2. Technical Background
### 2.1 Challenges
- **High Data Throughput**: Simulating light interference and multiple viewpoints is computationally heavy.
- **Hardware Cost/Complexity**: Optical modules and high-speed controllers remain expensive.
- **Limited Applications**: Most systems are demos or research prototypes; commercialization is slow.

### 2.2 Positioning
Photon Matrix aims to offer a scalable spatial display platform with a reasonable balance between performance, complexity, and cost, supporting various content sources and interactive modes.

## 3. System Architecture
1. **High-Speed Projection Module**: DLP/LCoS, >240 Hz
2. **Multi-Layer Optical Module**: Diffusion layers, optional fast-switching LC
3. **Synchronization Control**: FPGA/high-speed MCU, frame-to-layer sync
4. **Content Processing & Rendering**: Pre-sliced depth layers, high-speed streaming

(Diagram) System overview: /media/diagrams/system_overview.png

## 4. Key Modules
### 4.1 Projection & Optical Switching
- Single projector + multiple optical layers
- Precise synchronization required

### 4.2 Layered Rendering
- Slice 3D scene into N depth layers
- Render each layer and stream at high speed

### 4.3 Optical Materials
- Micro-structured diffusion films
- Variable-focus liquid crystal layers

## 5. Prototype & Experiments
Ref: Experimental Process Log (實驗歷程記錄.pdf)
- Assembly and alignment
- Optical layer switching tests
- Projection synchronization verification

#### Prototype Videos (example links)
- Prototype Test 1: media/videos/test1.mp4
- Prototype Test 2: media/videos/test2.mp4
- Prototype Test 3: media/videos/test3.mp4

## 6. Performance & Limitations
- **Brightness**: Depends on layer count and diffusion properties
- **Viewing Angle**: Determined by optics and diffusion
- **Refresh**: >60 Hz per layer to avoid flicker

Limitations:
- Layer count limited by frame rate and switching speed
- Costly high-speed optical panels
- High-precision alignment required

## 7. Future Work
- Increase layer count & parallax fidelity
- Reduce cost via optical process optimization
- Integrate interaction (gesture/position tracking)
- Real-time rendering & compression strategies

## 8. Appendix
- Patents: US20050062684A1, US6806849, WO2016092464A1
- Literature: Nayar et al., Tomographic Displays (SIGGRAPH 2016)
- Resources: GitHub yourrepo (replace with actual link)
