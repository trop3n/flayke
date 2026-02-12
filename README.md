# FLAKE Tool

A parametric tool for creating complex symmetrical patterns and generative textures based on vector custom shapes. Built with p5.js and inspired by Antlii's FLAKE Tool.

![FLAKE Tool Preview](preview.png)

## Features

### Core Features
- **Grid-Based Pattern Generation**: Configurable rows/columns with flexible cell sizing
- **Distance-Based Transformations (SDF)**: Scale, rotation, and color controlled by distance from grid center
- **Symmetry Modes**: None, Horizontal, Vertical, Both (4-way), and Radial symmetry
- **Multiple Shape Types**: Circle, Square, Triangle, Hexagon, Star, Diamond, Cross, Heart, and Custom SVG

### Shape Controls
- **Scale Modes**: Linear, Ease In, Ease Out, Ease In-Out, Step, and Swirl
- **Fill Modes**: Solid, Distance Gradient, Palette Cycle, Random
- **Blend Modes**: Normal, Add, Multiply, Screen, Overlay, Difference, XOR
- **Auto-rotation** with configurable speed

### Pattern/Noise
- Simplex noise-based pattern generation
- Configurable scale, intensity, and seed
- Adds organic variation to patterns

### Animation
- Smooth looping animations
- Animate size, rotation, and color independently
- Configurable loop duration and speed
- Export as PNG sequence for video creation

### Color Palette
- 5-color palette system
- Distance-based color interpolation
- One-click randomization

### Import/Export
- **SVG Shape Import**: Drag and drop custom SVG files
- **Mask Image**: Use raster images to modulate pattern
- **Export Formats**:
  - PNG (up to 4x scale)
  - SVG (vector output)
  - PNG Sequence (for video)
  - WebM Video (direct video recording)
- **Preset System**: 12 built-in presets, save your own as JSON

## Keyboard Shortcuts

| Key | Action |
|-----|--------|
| `Space` | Play/Pause animation |
| `Shift + R` | Randomize all parameters |
| `Ctrl + S` | Export |

## Getting Started

### Installation

```bash
npm install
```

### Development

```bash
npm run dev
```

Open http://localhost:5173 in your browser.

### Build for Production

```bash
npm run build
```

The output will be in the `dist` folder.

## Usage Tips

1. **Start with Presets**: Use the built-in presets to explore different styles
2. **Try Symmetry**: Radial symmetry with 6-12 divisions creates mandala-like patterns
3. **Scale Modes**: 
   - Use "Ease Out" for patterns that are large in center, small at edges
   - Use "Swirl" for spiral-like effects
4. **SVG Import**: Simple, single-path SVGs work best. Icons and glyphs are ideal.
5. **Animation**: Enable "Animate Size" for subtle breathing effects
6. **Blend Modes**: "Add" mode creates glowing effects with overlapping shapes
7. **Video Export**: Use WebM export to record animations directly. Click Export to start, click again to stop.

## Built-in Presets

1. **Radial Gradient** - Classic radial pattern with smooth falloff
2. **Geometric Mandala** - Hexagonal symmetry pattern
3. **Organic Swirl** - Noise-based organic texture
4. **Star Burst** - Explosive radial star pattern
5. **Minimal Cross** - Clean geometric cross design
6. **Triangular Flow** - Vertical triangle symmetry
7. **Neon Circles** - Additive blend glowing circles
8. **Diamond Echo** - Horizontal mirrored diamonds
9. **Hearts Bloom** - Romantic radial heart pattern
10. **Noise Texture** - Dense noise-based texture
11. **Retro Grid** - Classic retro aesthetic
12. **Spiral Galaxy** - Swirling spiral pattern

## Technical Details

- Built with **p5.js** for rendering
- **Tweakpane** for the UI
- **Simplex Noise** for organic patterns
- Canvas-based rendering with SVG export

## License

MIT License - Feel free to use, modify, and distribute.

## Credits

Inspired by [Antlii's FLAKE Tool](https://antlii.work/FLAKE-Tool).

Created as a learning project for creative coding with p5.js, paper.js, and generative art techniques.
