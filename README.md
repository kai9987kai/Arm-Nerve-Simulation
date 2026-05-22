# Advanced Arm Nervous System Simulation

A single-file, browser-based educational simulation for exploring the **major nerves of the upper limb**, the **brachial plexus**, nerve signal conduction, dermatomes, myotomes, cross-sections, and common clinical nerve-compression patterns.

The app keeps the original interactive canvas anatomy experience and expands it into a more advanced learning lab with research-informed teaching tools, lesion overlays, a conduction timing calculator, search, quiz mode, accessibility options, and exportable session notes.

> **Education only:** this project is a visual learning tool, not a diagnostic or treatment tool. Persistent numbness, weakness, trauma-related symptoms, spreading pain, loss of grip, or worsening sensory change should be assessed by a qualified clinician.

---

## Demo

Open the HTML file directly in a browser:

```text
advanced_arm_nerve_simulation.html
```

No build step, backend, install process, or external package manager is required.

---

## Core Features Preserved

- Interactive canvas-based arm anatomy simulation
- Major upper-limb nerve paths:
  - Musculocutaneous nerve
  - Median nerve
  - Ulnar nerve
  - Radial nerve
  - Axillary nerve
  - Medial cutaneous nerves
- Brachial plexus root display from **C5-T1**
- Anatomical view
- Dermatome view
- Myotome view
- Cross-section view
- Toggleable layers for:
  - Muscles
  - Bones
  - Vessels
  - Labels
- Click-to-stimulate nerve signalling
- Motor signal animation from brain to peripheral nerves
- Sensory signal animation from fingertips toward the brain
- Reflex arc simulation
- Signal speed and intensity controls
- Clinical information panel for selected nerves
- Hover/click interaction for nerve details

---

## New Advanced Features

### 1. Smart Nerve Finder

Search by nerve, root, symptom, test, or clinical clue.

Example searches:

```text
median
C8
wrist drop
Froment
carpal tunnel
deltoid
```

The finder highlights likely structures and helps connect symptoms to anatomical pathways.

### 2. Clinical Pattern Lens

Selecting a nerve now shows extra learning information:

- Mnemonic
- Examination-style tests
- Red flags
- Common lesion patterns
- Rehab/ergonomic concepts

This makes the app more useful for anatomy revision, physiotherapy-style teaching, clinical reasoning practice, and patient-friendly education.

### 3. Compression / Lesion Simulator

The app can model common nerve compression or lesion patterns with visual overlays and altered signal behaviour.

Included presets:

- **Carpal tunnel** — median nerve at the wrist
- **Cubital tunnel** — ulnar nerve at the elbow
- **Spiral groove lesion** — radial nerve near the humerus
- **Axillary nerve trauma** — shoulder dislocation/fracture-style pattern
- **Upper trunk C5-C6 pattern**
- **Lower trunk C8-T1 pattern**

Each preset includes:

- Affected nerve
- Anatomical level
- Sensory pattern
- Motor pattern
- Severity slider
- Affected signal animation
- Educational explanation

### 4. Conduction Timing Lab

A teaching calculator estimates latency using:

```text
latency = distance / conduction velocity
```

Fiber profiles included:

| Fiber type | Approximate role | Typical speed profile |
|---|---|---|
| Aα | Proprioception / motor alpha fibers | Fastest, heavily myelinated |
| Aβ | Touch and pressure | Fast, myelinated |
| Aδ | Fast pain and temperature | Slower, thinly myelinated |
| C | Slow pain, warmth, itch | Slowest, unmyelinated |

This helps learners understand why different sensory experiences can feel immediate or delayed.

### 5. Quiz Mode

Built-in questions test key anatomy and clinical pattern knowledge, including:

- Carpal tunnel nerve involvement
- Wrist drop
- Brachial plexus roots
- Deltoid/axillary nerve relationship
- Fastest fiber types
- Froment sign

### 6. Session Tools

The upgraded app includes a basic session workflow:

- Copy case note
- Download session note as JSON
- Session timeline log
- Reset function for signals and lesion overlays

These tools make it easier to use the simulation for teaching, revision notes, or documenting learning scenarios.

### 7. Accessibility and UX Improvements

- High-contrast mode
- Reduced-motion mode
- Responsive layout for smaller screens
- Keyboard shortcuts
- Floating help label
- Search chips for quick exploration
- Improved panels and educational cards

Keyboard shortcuts:

| Key | Action |
|---|---|
| `F` | Focus the nerve finder |
| `R` | Trigger reflex arc |
| `S` | Trigger sensory signal |
| `H` | Toggle high contrast |

---

## Research-Informed Design Ideas

The upgrade is designed around several modern educational and clinical-teaching concepts:

- **Brachial plexus organisation:** roots → trunks → divisions → cords → terminal branches
- **Pattern-based nerve learning:** combine anatomy, sensory territory, motor role, and lesion signs
- **Electrodiagnostic reasoning:** slowed conduction can suggest demyelinating/compression effects, while reduced response amplitude can suggest axonal involvement
- **Entrapment education:** compression syndromes are easier to understand when symptoms are mapped onto anatomical tunnels and nerve territories
- **Multimodal learning:** visual anatomy, animation, search, quiz questions, and exportable notes support different learning styles
- **Accessible simulation:** high-contrast and reduced-motion modes make the tool more usable for a wider range of learners

---

## How to Use

1. Open `advanced_arm_nerve_simulation.html` in a modern browser.
2. Click or hover over nerves to inspect their roots, motor function, sensory field, and clinical notes.
3. Use the view buttons to switch between:
   - Anatomical
   - Dermatomes
   - Myotomes
   - Cross-section
4. Toggle muscles, bones, vessels, and labels as needed.
5. Use signal buttons to simulate:
   - Full motor signal
   - Sensory signal
   - Reflex arc
6. Search for symptoms or nerves with the Smart Nerve Finder.
7. Apply a lesion preset and adjust severity.
8. Use the conduction timing lab to compare fiber types.
9. Try quiz mode for revision.
10. Export a case note if you want to save the session state.

---

## Suggested Use Cases

- Anatomy revision
- Brachial plexus learning
- Nerve lesion pattern teaching
- Clinical reasoning demonstrations
- Physiotherapy/occupational therapy education support
- Patient-friendly explanation of nerve compression concepts
- Browser-based educational prototypes
- Interactive medical visualization experiments

---

## File Structure

```text
.
├── advanced_arm_nerve_simulation.html   # Complete single-file app
└── README.md                            # Project documentation
```

Everything is contained inside the HTML file:

- HTML markup
- CSS styling
- Canvas rendering
- Nerve datasets
- Signal animation logic
- Lesion simulation logic
- Search and quiz logic
- Export tools

---

## Browser Support

Recommended:

- Chrome / Chromium
- Edge
- Firefox
- Safari

The app uses standard browser APIs:

- HTML5 Canvas
- JavaScript classes
- DOM events
- `requestAnimationFrame`
- Local file download via Blob
- Clipboard API where supported

---

## Limitations

This is a simplified educational simulation. It does not replace:

- Clinical examination
- Nerve conduction studies
- EMG
- Ultrasound
- MRI/CT imaging
- Professional diagnosis
- Medical treatment planning

Anatomical paths, conduction values, and lesion behaviour are approximate and intended for teaching rather than measurement.

---

## Future Feature Ideas

- Add neck and cervical root origin view
- Add full brachial plexus branching diagram mode
- Add EMG/NCS waveform simulator
- Add printable study cards
- Add labelled clinical case scenarios
- Add left/right arm switch
- Add pinch/grip strength simulation
- Add sensory mapping brush tool
- Add comparative normal vs lesion signal graphs
- Add multilingual labels
- Add mobile-first touch controls
- Add saved custom study sessions
- Add teacher mode with hidden answers
- Add export to PNG/SVG for diagrams

---

## Development Notes

The project is intentionally kept as a **single-file prototype** so it can be copied, hosted, edited, or shared easily.

To modify the app:

1. Open the HTML file in a code editor.
2. Edit the nerve data, clinical notes, lesion presets, or quiz bank directly in the JavaScript section.
3. Refresh the browser to test changes.

Useful areas to extend:

- `nerves` object — core nerve paths and descriptions
- `advancedNerveMeta` — mnemonics, tests, red flags, rehab concepts
- `lesionPresets` — compression/lesion scenarios
- `fiberProfiles` — conduction timing lab
- `quizBank` — revision questions
- Canvas draw functions — visual rendering layers

---

## Safety / Medical Disclaimer

This software is for education, simulation, and visualization only. It should not be used to diagnose, treat, or rule out medical conditions. Any real symptoms such as weakness, numbness, severe pain, trauma-related nerve signs, progressive loss of sensation, hand wasting, or loss of function should be assessed by a qualified healthcare professional.

---

## Credits

Created as an experimental browser-based anatomy and nerve-signal learning tool.

Built with:

- HTML
- CSS
- Vanilla JavaScript
- HTML5 Canvas

No external dependencies required.
