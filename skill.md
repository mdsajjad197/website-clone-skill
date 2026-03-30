# Skill Profile – Website Cloning (Exact Replica)

## Overview
This skill enables cloning a website from a given URL with high fidelity.  
The output replicates the original website’s visual appearance, structure, media assets, 3D elements, animations, and interactive components as closely as technically possible.

The goal is **pixel-perfect reproduction**, not redesign.

---

## Input
- Website URL (publicly accessible)
- Optional:
  - Target framework (HTML/CSS/JS, React, Next.js, etc.)
  - Desktop / Mobile / Both
  - Performance or SEO optimization requirements

---

## Core Capabilities

### 1. Visual Replication
- Pixel-perfect layout recreation
- Exact color schemes, gradients, shadows
- Font matching (Google Fonts / custom fonts)
- Spacing, alignment, and responsive breakpoints

### 2. Media Cloning
- Image extraction and optimization
- Video embedding or recreation
- Background videos
- SVG and canvas-based graphics

### 3. 3D Elements
- WebGL / Three.js scene replication
- Model loading (GLTF / GLB)
- Camera movement and lighting recreation
- Scroll-based 3D animations
- Performance-optimized rendering

### 4. UI Components
- Buttons, cards, modals, sliders
- Navigation menus and mega-menus
- Forms and input components
- Custom cursor effects
- Hover, focus, and active states

### 5. Animations & Interactions
- Scroll-triggered animations
- Micro-interactions
- Page transitions
- Parallax effects
- GSAP / Framer Motion replication

---

## Asset Acquisition & Download (Implemented)

### Supported Asset Types
- Images: JPG, PNG, WebP, SVG
- Videos: MP4, WebM (non-DRM)
- Fonts: WOFF, WOFF2, TTF (publicly accessible)
- 3D Models: GLTF, GLB
- Animations: Lottie JSON, SVG animations

### Download Scope
- Assets must be publicly accessible
- No authentication, paywall, or DRM-protected assets
- No private API asset fetching
- Dynamic assets captured only if technically feasible

### Download Behavior
- Extract asset URLs from:
  - HTML
  - CSS (`url()`)
  - JS (static references)
- Preserve original filenames where possible
- Deduplicate identical assets
- Normalize paths for local usage
- Replace remote URLs with local asset paths

### Output Asset Structure
public/
├── assets/
│   ├── images/
│   ├── videos/
│   ├── fonts/
│   ├── models/
│   └── animations/

### Post-Download Integration
- Update HTML, CSS, and JS references to local assets
- Ensure compatibility with bundlers (Vite, Webpack, Next.js)
- Validate loading performance and fallback behavior

---

## Technical Stack

### Frontend
- HTML5
- CSS3 / SCSS / Tailwind CSS
- JavaScript (ES6+)
- React / Next.js (if required)

### Animation & 3D
- Three.js
- GSAP
- Framer Motion
- Lottie
- WebGL

### Media Handling
- Image compression & lazy loading
- Video optimization
- Responsive media delivery

---

## Cloning Process

1. Analyze target URL structure
2. Identify layout grid and breakpoints
3. Extract visual and interactive patterns
4. Download and organize public assets
5. Rebuild components from scratch
6. Match animations and transitions
7. Optimize performance and responsiveness
8. Cross-browser testing

---

## Accuracy Level
- Visual accuracy: **95–100%**
- Interaction accuracy: **90–100%**
- Responsive behavior: **Fully matched**
- Asset fidelity: **Original-quality or optimized equivalent**
- Performance: Optimized without altering visuals

---

## Limitations
- Cannot bypass authentication, paywalls, or DRM
- Backend logic not cloned unless specified
- Third-party APIs may require replacements
- Streaming media (HLS/DASH) not downloaded
- Proprietary assets recreated visually if required

---

## Ethical & Legal Compliance
- No direct copying of copyrighted source code
- Asset downloads limited to publicly accessible files
- Assets recreated or replaced when licensing requires
- Intended for learning, auditing, or licensed replication

---

## Output
- Clean, readable source code
- Modular component structure
- Local asset storage with organized hierarchy
- Responsive layouts
- Ready-to-deploy build

---

## Version
v1.1.0