# Welcome to [Slidev](https://github.com/slidevjs/slidev)!

A Slidev presentation template for creating professional slide decks with Markdown.

## Getting Started

Install dependencies:
```bash
npm install
# or
pnpm install
```

Start the development server:
```bash
npm run dev
# or
pnpm dev
```

Visit <http://localhost:3030> to view your presentation.

Edit [slides.md](./slides.md) to see live changes.

## CLI Commands

### Development
```bash
npm run dev              # Start dev server (default port 3030)
npm run dev -- --port 3031  # Start on custom port
npm run dev -- --open    # Auto-open in browser
npm run dev -- --remote  # Allow remote access
```

### Build & Export
```bash
npm run build            # Build for production (SPA)
npm run export           # Export to PDF
npm run export -- --output slides.pdf  # Custom output name
npm run export -- --format pptx        # Export to PowerPoint
npm run export -- --format png         # Export as images
npm run export -- --with-clicks        # Include each click animation as separate slide
```

### Other Commands
```bash
npx slidev --help        # Show all available options
npx slidev format        # Format slides.md
npx slidev theme         # Manage themes
```

## Project Structure

```
.
├── slides.md           # Main presentation file
├── components/         # Custom Vue components
├── public/            # Static assets (images, etc.)
├── pages/             # Additional slide pages
└── style.css          # Custom styles
```

## Exporting

**PDF Export:**
```bash
npm run export
```

**PowerPoint Export:**
```bash
npm run export -- --format pptx
```

**PNG Export (per slide):**
```bash
npm run export -- --format png
```

**With custom output:**
```bash
npm run export -- --output my-presentation.pdf
```

**With click animations (each animation as separate page):**
```bash
npm run export -- --with-clicks
npm run export -- --with-clicks --format pptx
```

## Presenter Mode

Press `?` during presentation to see all keyboard shortcuts.

Key shortcuts:
- `Space` / `→` - Next slide/animation
- `←` - Previous slide
- `O` - Toggle slides overview
- `F` - Toggle fullscreen
- `D` - Toggle dark mode
- `C` - Toggle camera
- `R` - Start/stop recording

## Learn More

- [Slidev Documentation](https://sli.dev/)
- [Themes Gallery](https://sli.dev/resources/theme-gallery)
- [Awesome Slidev](https://github.com/slidevjs/awesome-slidev)
