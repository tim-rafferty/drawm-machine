
# Drawm Machne is a work in progress and several things are currently not working.

### How to test:

- Download the HTML file and open it in your browser
- Draw patterns and press play
- Click effects to change different FX
- Clear all will clear all drawings

## 1. Key Features and Functionalities

### Drawing Mechanics
- Gesture capture system (recording form, motion, speed, and direction)
- Multitrack drawing canvas supporting independent paths
- Path animation with continuous looping
- Drawing manipulation tools (resize, copy/paste, straighten)
- Path intersection detection

### Audio Features
- Tone.js audio engine integration
- Custom sample import and management system
- Sound triggering along drawn paths
- X/Y coordinate parameter mapping to audio properties
- Flexible timing (gesture-accurate or quantized to tempo)
- Multiple trigger point placement
- Crossover trigger functionality
- Per-track and master effects processing

### User Interface Elements
- Minimalist main drawing canvas
- Sound/sample selection panel
- Parameter mapping controls
- Track management system
- Expandable panels for advanced features
- Transport controls (play, stop, tempo)
- Visual feedback for active paths and trigger points

### Additional Functionalities
- Project saving and loading
- Audio export capabilities
- Preset system for sounds and effects
- Tutorial/onboarding system
- Undo/redo functionality

## 2. User Interface Design

### Main Interface Layout
- Central drawing canvas (70-80% of screen real estate)
- Top toolbar with essential drawing tools and global controls
- Collapsible bottom panel for track management
- Side panel (expandable) for detailed parameters and effects
- Minimal color palette with high contrast for clarity

### Interaction Design
- Primary mode: drawing paths with cursor/touch
- Secondary mode: editing/manipulating existing paths
- Path selection via simple tap/click
- Long-press for context menu options
- Drag handles for path manipulation
- Double-tap to access track-specific settings

### Advanced Options Architecture
- Layered disclosure design (progressive revelation of complexity)
- Icon-based expandable panels that slide in from edges
- Parameter grouping with collapsible sections
- Contextual controls that appear based on current selection
- Tab-based organization for different categories of advanced options

### Visual Feedback System
- Color-coding for different tracks
- Animated "playheads" showing current position on paths
- Visual indicators for trigger points and crossovers
- Parameter value visualization through path properties (thickness, color)
- Real-time waveform/spectrum visualization options

## 3. Sound Engine and Audio Features

### Tone.js Implementation
- Core audio system built on Tone.js framework
- Transport system for synchronization and timing
- Players/samplers for sample playback
- Signal routing architecture for parameter modulation
- Effects chains for processing

### Sample Management
- Sample browser with categorization
- Custom sample import functionality (drag-and-drop)
- Basic sample editing (trimming, normalization)
- Sample preview functionality
- Included sample library organized by instrument type

### Trigger System
- Point-based trigger mechanism along paths
- Variable trigger types (one-shot, gate, toggle)
- Trigger visualization system
- Trigger point editing interface
- Trigger filtering options (velocity, probability)

### Parameter Mapping Engine
- Coordinate-to-parameter mapping system
- Configurable mapping destinations:
  - Pitch/playback rate
  - Filter parameters
  - Effect parameters
  - Volume/amplitude
- Mapping curve editors (linear, exponential, custom)
- Parameter range limiters

## 4. Drawing and Animation

### Path Creation System
- Vector-based path drawing using Canvas API
- High-resolution point capture with timestamps
- Velocity and pressure data capture (where available)
- Path smoothing algorithms
- Path analysis for musical features extraction

### Animation Engine
- Continuous loop animation system
- Variable speed playback based on tempo
- Visual playhead following path
- Interpolation between points for smooth movement
- Visual effects tied to sound parameters

### Gesture Analysis
- Real-time analysis of drawing characteristics:
  - Velocity detection
  - Direction changes
  - Shape recognition
  - Pattern detection
- Translation of gesture properties to musical qualities

### Performance Optimization
- Efficient path rendering techniques
- Canvas optimization for smooth animation
- Selective rendering based on view
- Hardware acceleration where available
- Balanced visual fidelity vs. performance

## 5. Parameter Control and Effects

### Parameter Control System
- Modulation matrix connecting coordinates to parameters
- Multi-point envelope generation from path shapes
- Parameter automation based on playhead position
- Global parameter scaling controls
- Parameter grouping and macro controls

### Per-Track Effects
- Filter section (lowpass, highpass, bandpass)
- Delay with tempo-sync options
- Reverb with size and damping controls
- Distortion/saturation effects
- Modulation effects (chorus, phaser, flanger)
- Dynamics processing (compression, limiting)

### Master Effects Chain
- Master EQ section
- Bus compression
- Spatial effects (stereo widening)
- Limiting for output protection
- Global reverb send

### Advanced Modulation
- LFO generation from path shapes
- Crossover modulation between paths
- Trigger-based envelope generators
- Randomization options for parameters
- Conditional modulation logic

## 6. Sequencer Functionality

### Timing Engine
- Grid-based timing system with variable resolution
- Tempo control (60-200 BPM)
- Time signature settings
- Swing/groove amount controls
- Global transport controls

### Quantization Options
- Real-time quantization during drawing
- Post-drawing quantization tools
- Variable quantization strengths (0-100%)
- Grid visualization options
- Quantization templates (straight, triplet, dotted)

### Multi-Trigger System
- Multiple trigger point placement along paths
- Trigger type configuration
- Trigger density controls
- Trigger point editing interface
- Probability controls for triggers

### Intersection and Crossover Logic
- Path intersection detection algorithm
- Special event triggering at crossover points
- Crossover behavior options:
  - Trigger both paths
  - Alternate between paths
  - Blend parameters of both paths
  - Create new combined sounds

## 7. Additional Features

### Drawing Tools
- Path selection and transformation
- Copy/paste/duplicate functionality
- Path editing (add/remove points, smooth)
- Path alignment tools
- Layer management for organizing paths

### Project Management
- Project saving and loading
- Autosave functionality
- Version history
- Project templates
- Export options (audio, MIDI, project file)

### Sample Management
- Sample browser with categories
- Custom sample import
- Basic sample editing
- Sample organization system
- Favorites and collections

### Performance Features
- CPU usage monitoring
- Performance mode (reduced visual feedback)
- Track freezing for CPU reduction
- Audio buffer size adjustment
- Background processing for intensive operations
