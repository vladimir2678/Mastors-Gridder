# Mastors-Gridder v1.2

**Comprehensive CSS Grid Utility Library** - Professional-grade grid classes for modern web layouts.

A powerful, flexible, and production-ready CSS utility library that provides everything you need to build responsive, complex layouts with ease. No build tools required—just pure CSS classes ready to use.

---

<p align="center">
  <a href="/">
    <img src="https://img.shields.io/badge/SASS-DOCUMENTATION-cc6699?style=for-the-badge&logo=sass&logoColor=white">
  </a>
  &nbsp;
  <a href="https://kehem-it.github.io/Mastors-Gridder/">
    <img src="https://img.shields.io/badge/FULL-DOCUMENTATION-2ea44f?style=for-the-badge&logo=readthedocs&logoColor=white">
  </a>
  &nbsp;
  <a href="#whats-new-in-v12">
    <img src="https://img.shields.io/badge/VERSION-1.2-blue?style=for-the-badge">
  </a>
</p>

---

## 📋 Table of Contents

- [What's New in v1.2](#-whats-new-in-v12)
- [Installation](#-installation)
- [Quick Start](#-quick-start)
- [Grid Classes Overview](#-grid-classes-overview)
- [Quick Reference Table](#-quick-reference-table)
- [Detailed Documentation](#-detailed-documentation)
  - [Responsive Grid Classes](#responsive-grid-classes)
  - [Fixed Grid Classes](#fixed-grid-classes)
  - [Layout Pattern Classes](#layout-pattern-classes)
  - [Grid Item Classes](#grid-item-classes)
  - [Alignment & Utility Classes](#alignment--utility-classes)
  - [Advanced Grid Controls (New v1.2)](#advanced-grid-controls-new-v12)
  - [Grid Layering & Overlays (New v1.2)](#grid-layering--overlays-new-v12)
  - [Container Queries (New v1.2)](#container-queries-new-v12)
  - [Responsive Modifiers](#responsive-modifiers)
- [Usage Examples](#-usage-examples)
- [Best Practices](#-best-practices)
- [Browser Support](#-browser-support)

---

## 🎉 What's New in v1.2

Version 1.2 adds **20 powerful new utility classes** for advanced grid control:

### 🎯 Advanced Grid Controls
- **Auto-flow utilities** - Control item placement direction with `.grid-flow-row`, `.grid-flow-col`, `.grid-flow-dense`
- **Auto-sizing** - `.auto-rows-*` and `.auto-cols-*` for dynamic track sizing
- **Explicit layouts** - `.grid-explicit-*` for precise column/row definitions
- **FR unit grids** - Direct fractional unit control with `.grid-fr-*` classes

### 🔧 Enhanced Features
- **Grid layering** - `.grid-layer-full` for overlapping content (hero sections, overlays)
- **Intrinsic sizing** - `.grid-intrinsic-min/max` for content-based layouts
- **Fit-content grids** - `.grid-fit-content-*` for flexible responsive layouts
- **Pattern repeating** - Custom repeating patterns for unique designs
- **Content alignment** - `.grid-content-*` for aligning the entire grid

### 🚀 Modern Web Features
- **Container queries** - `.grid-container-aware` for component-based responsiveness
- **Improved masonry** - `.grid-masonry-modern` with better packing
- **Place shortcuts** - `.grid-place-*` for concise alignment
- **Full-span utilities** - Quick `.grid-full-width` and `.grid-full-height` classes

### 📱 Better Responsive Control
- **Responsive grid areas** - Mobile-first template area switching
- **Enhanced minmax** - More control over min/max column sizing
- **Auto-track control** - Flexible auto-fit/fill with custom constraints

**Total classes: 43 mixins → 100+ utility classes**

---

## 🚀 Installation

### Via CDN (Recommended for Quick Start)

Add this link in your HTML `<head>`:

```html
<link
  rel="stylesheet"
  href="https://cdn.jsdelivr.net/gh/KEHEM-IT/Mastors-Gridder@v1.2/mastors-gridder.css"
/>
```

### Via NPM

Install the package:

```bash
npm i mastors-gridder@latest
```

Then import in your CSS or HTML:

```css
@import "mastors-gridder";
```

Or link in HTML:

```html
<link
  rel="stylesheet"
  href="node_modules/mastors-gridder/mastors-gridder.css"
/>
```

### Manual Installation

Download `mastors-gridder.css` and link it in your HTML:

```html
<link rel="stylesheet" href="path/to/mastors-gridder.css" />
```

---

## ⚡ Quick Start

```html
<!-- Auto-fit responsive grid -->
<div class="grid-auto gap-lg">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>

<!-- Fixed 4-column grid -->
<div class="grid-cols-4 gap-md">
  <div>Column 1</div>
  <div>Column 2</div>
  <div>Column 3</div>
  <div>Column 4</div>
</div>

<!-- Sidebar layout -->
<div class="grid-sidebar gap-lg">
  <aside>Sidebar</aside>
  <main>Main Content</main>
</div>

<!-- Centered content -->
<div class="grid-center" style="min-height: 400px;">
  <h1>Centered Content</h1>
</div>

<!-- NEW v1.2: Layered hero section -->
<div class="grid-cols-1">
  <img class="grid-layer-full" src="hero.jpg" alt="Background" />
  <div class="grid-layer-full grid-center">
    <h1>Overlaid Content</h1>
  </div>
</div>

<!-- NEW v1.2: Container-aware responsive grid -->
<div class="grid-container-aware gap-md">
  <div>Responds to container size</div>
  <div>Not viewport size</div>
</div>
```

---

## 🎯 Grid Classes Overview

| Category              | Classes                                                    | Use Case                      |
| --------------------- | ---------------------------------------------------------- | ----------------------------- |
| **Responsive**        | `grid-auto`, `grid-fill`, `grid-cards`                     | Auto-responsive grids         |
| **Fixed**             | `grid-cols-*`, `grid-rows-*`                               | Fixed column/row grids        |
| **Layouts**           | `grid-sidebar`, `grid-holy-grail`, `grid-full-bleed`       | Common layout patterns        |
| **Items**             | `col-span-*`, `row-span-*`, `order-*`                      | Grid item positioning         |
| **Alignment**         | `grid-center`, `items-*`, `self-*`, `grid-content-*` (NEW) | Content alignment             |
| **Spacing**           | `gap-*`, `gap-x-*`, `gap-y-*`                              | Grid spacing                  |
| **Flow Control** (NEW) | `grid-flow-*`, `auto-rows-*`, `auto-cols-*`               | Item placement & auto-sizing  |
| **Advanced** (NEW)    | `grid-layer-*`, `grid-intrinsic-*`, `grid-fit-content-*`  | Layering, intrinsic sizing    |
| **Modern** (NEW)      | `grid-container-aware`, `grid-place-*`, `grid-fr-*`        | Container queries, FR units   |
| **Responsive**        | `sm:*`, `md:*`, `lg:*`                                     | Breakpoint modifiers          |

---

## 📊 Quick Reference Table

Complete list of all utility classes with descriptions and usage examples.

### Responsive Grid Classes

| Class                      | Description                        | Usage Example                              |
| -------------------------- | ---------------------------------- | ------------------------------------------ |
| `grid-auto`                | Auto-fit grid, min 250px columns   | `<div class="grid-auto gap-lg">`           |
| `grid-auto-sm`             | Auto-fit grid, min 150px columns   | `<div class="grid-auto-sm">`               |
| `grid-auto-md`             | Auto-fit grid, min 250px columns   | `<div class="grid-auto-md">`               |
| `grid-auto-lg`             | Auto-fit grid, min 350px columns   | `<div class="grid-auto-lg">`               |
| `grid-fill`                | Auto-fill grid, keeps empty tracks | `<div class="grid-fill gap-md">`           |
| `grid-fill-sm`             | Auto-fill grid, min 150px          | `<div class="grid-fill-sm">`               |
| `grid-fill-lg`             | Auto-fill grid, min 350px          | `<div class="grid-fill-lg">`               |
| `grid-cards`               | Responsive card grid, 280px min    | `<div class="grid-cards">`                 |
| `grid-cards-sm`            | Card grid, 200px min               | `<div class="grid-cards-sm">`              |
| `grid-cards-lg`            | Card grid, 350px min               | `<div class="grid-cards-lg">`              |
| `grid-dense`               | Dense packing, fills gaps          | `<div class="grid-dense">`                 |
| `grid-stacked`             | Mobile stack → 2 cols at 640px     | `<div class="grid-stacked">`               |
| `grid-stacked-3`           | Mobile stack → 3 cols at 768px     | `<div class="grid-stacked-3">`             |
| `grid-container-aware` 🆕  | Container query responsive         | `<div class="grid-container-aware">`       |
| `grid-container-aware-sm` 🆕 | Container aware, 150px min        | `<div class="grid-container-aware-sm">`    |
| `grid-container-aware-lg` 🆕 | Container aware, 350px min        | `<div class="grid-container-aware-lg">`    |

### Fixed Grid Classes

| Class          | Description         | Usage Example                |
| -------------- | ------------------- | ---------------------------- |
| `grid-cols-1`  | 1 column grid       | `<div class="grid-cols-1">`  |
| `grid-cols-2`  | 2 column grid       | `<div class="grid-cols-2">`  |
| `grid-cols-3`  | 3 column grid       | `<div class="grid-cols-3">`  |
| `grid-cols-4`  | 4 column grid       | `<div class="grid-cols-4">`  |
| `grid-cols-5`  | 5 column grid       | `<div class="grid-cols-5">`  |
| `grid-cols-6`  | 6 column grid       | `<div class="grid-cols-6">`  |
| `grid-cols-7`  | 7 column grid       | `<div class="grid-cols-7">`  |
| `grid-cols-8`  | 8 column grid       | `<div class="grid-cols-8">`  |
| `grid-cols-9`  | 9 column grid       | `<div class="grid-cols-9">`  |
| `grid-cols-10` | 10 column grid      | `<div class="grid-cols-10">` |
| `grid-cols-11` | 11 column grid      | `<div class="grid-cols-11">` |
| `grid-cols-12` | 12 column grid      | `<div class="grid-cols-12">` |
| `grid-rows-1`  | 1 equal-height row  | `<div class="grid-rows-1">`  |
| `grid-rows-2`  | 2 equal-height rows | `<div class="grid-rows-2">`  |
| `grid-rows-3`  | 3 equal-height rows | `<div class="grid-rows-3">`  |
| `grid-rows-4`  | 4 equal-height rows | `<div class="grid-rows-4">`  |
| `grid-rows-5`  | 5 equal-height rows | `<div class="grid-rows-5">`  |
| `grid-rows-6`  | 6 equal-height rows | `<div class="grid-rows-6">`  |

### Layout Pattern Classes

| Class                     | Description                        | Usage Example                           |
| ------------------------- | ---------------------------------- | --------------------------------------- |
| `grid-sidebar`            | Sidebar (300px) + content          | `<div class="grid-sidebar">`            |
| `grid-sidebar-sm`         | Sidebar (200px) + content          | `<div class="grid-sidebar-sm">`         |
| `grid-sidebar-lg`         | Sidebar (400px) + content          | `<div class="grid-sidebar-lg">`         |
| `grid-sidebar-right`      | Content + sidebar (300px) on right | `<div class="grid-sidebar-right">`      |
| `grid-sidebar-responsive` | Responsive sidebar (stacks mobile) | `<div class="grid-sidebar-responsive">` |
| `grid-holy-grail`         | Header/sidebars/content/footer     | `<div class="grid-holy-grail">`         |
| `grid-holy-grail-sm`      | Holy grail with 200px sidebars     | `<div class="grid-holy-grail-sm">`      |
| `grid-holy-grail-lg`      | Holy grail with 300px sidebars     | `<div class="grid-holy-grail-lg">`      |
| `grid-full-bleed`         | Content with full-width breakouts  | `<div class="grid-full-bleed">`         |
| `grid-full-bleed-sm`      | Full bleed, 960px max              | `<div class="grid-full-bleed-sm">`      |
| `grid-full-bleed-lg`      | Full bleed, 1440px max             | `<div class="grid-full-bleed-lg">`      |
| `grid-asymmetric-2-1`     | 2:1 ratio two-column               | `<div class="grid-asymmetric-2-1">`     |
| `grid-asymmetric-1-2`     | 1:2 ratio two-column               | `<div class="grid-asymmetric-1-2">`     |
| `grid-asymmetric-3-1`     | 3:1 ratio two-column               | `<div class="grid-asymmetric-3-1">`     |
| `grid-asymmetric-1-3`     | 1:3 ratio two-column               | `<div class="grid-asymmetric-1-3">`     |
| `grid-asymmetric-3-2`     | 3:2 ratio two-column               | `<div class="grid-asymmetric-3-2">`     |
| `grid-masonry`            | 3-column masonry layout            | `<div class="grid-masonry">`            |
| `grid-masonry-2`          | 2-column masonry layout            | `<div class="grid-masonry-2">`          |
| `grid-masonry-4`          | 4-column masonry layout            | `<div class="grid-masonry-4">`          |
| `grid-masonry-modern` 🆕  | 3-col masonry with dense flow      | `<div class="grid-masonry-modern">`     |
| `grid-equal-rows`         | Equal-height auto rows             | `<div class="grid-equal-rows">`         |

### Grid Item Classes

| Class           | Description               | Usage Example                 |
| --------------- | ------------------------- | ----------------------------- |
| `col-span-1`    | Span 1 column             | `<div class="col-span-1">`    |
| `col-span-2`    | Span 2 columns            | `<div class="col-span-2">`    |
| `col-span-3`    | Span 3 columns            | `<div class="col-span-3">`    |
| `col-span-4`    | Span 4 columns            | `<div class="col-span-4">`    |
| `col-span-5`    | Span 5 columns            | `<div class="col-span-5">`    |
| `col-span-6`    | Span 6 columns            | `<div class="col-span-6">`    |
| `col-span-7`    | Span 7 columns            | `<div class="col-span-7">`    |
| `col-span-8`    | Span 8 columns            | `<div class="col-span-8">`    |
| `col-span-9`    | Span 9 columns            | `<div class="col-span-9">`    |
| `col-span-10`   | Span 10 columns           | `<div class="col-span-10">`   |
| `col-span-11`   | Span 11 columns           | `<div class="col-span-11">`   |
| `col-span-12`   | Span 12 columns           | `<div class="col-span-12">`   |
| `col-span-full` | Span all columns (1 / -1) | `<div class="col-span-full">` |
| `row-span-1`    | Span 1 row                | `<div class="row-span-1">`    |
| `row-span-2`    | Span 2 rows               | `<div class="row-span-2">`    |
| `row-span-3`    | Span 3 rows               | `<div class="row-span-3">`    |
| `row-span-4`    | Span 4 rows               | `<div class="row-span-4">`    |
| `row-span-5`    | Span 5 rows               | `<div class="row-span-5">`    |
| `row-span-6`    | Span 6 rows               | `<div class="row-span-6">`    |
| `row-span-full` | Span all rows (1 / -1)    | `<div class="row-span-full">` |
| `order-first`   | Display first (order: -1) | `<div class="order-first">`   |
| `order-last`    | Display last (order: 999) | `<div class="order-last">`    |
| `order-none`    | Reset order (order: 0)    | `<div class="order-none">`    |
| `order-1`       | Order: 1                  | `<div class="order-1">`       |
| `order-2`       | Order: 2                  | `<div class="order-2">`       |
| `order-3`       | Order: 3                  | `<div class="order-3">`       |
| `order-4`       | Order: 4                  | `<div class="order-4">`       |
| `order-5`       | Order: 5                  | `<div class="order-5">`       |
| `order-6`       | Order: 6                  | `<div class="order-6">`       |

### NEW v1.2: Grid Flow Control Classes

| Class                  | Description                    | Usage Example                        |
| ---------------------- | ------------------------------ | ------------------------------------ |
| `grid-flow-row` 🆕     | Flow items in rows (default)   | `<div class="grid-flow-row">`        |
| `grid-flow-col` 🆕     | Flow items in columns          | `<div class="grid-flow-col">`        |
| `grid-flow-dense` 🆕   | Pack items densely             | `<div class="grid-flow-dense">`      |
| `grid-flow-row-dense` 🆕 | Row flow with dense packing   | `<div class="grid-flow-row-dense">`  |
| `grid-flow-col-dense` 🆕 | Column flow with dense packing | `<div class="grid-flow-col-dense">` |

### NEW v1.2: Auto-Sizing Classes

| Class             | Description                 | Usage Example                   |
| ----------------- | --------------------------- | ------------------------------- |
| `auto-rows-auto` 🆕 | Auto-sized rows            | `<div class="auto-rows-auto">`  |
| `auto-rows-min` 🆕  | Min-content sized rows     | `<div class="auto-rows-min">`   |
| `auto-rows-max` 🆕  | Max-content sized rows     | `<div class="auto-rows-max">`   |
| `auto-rows-fr` 🆕   | Equal fractional rows      | `<div class="auto-rows-fr">`    |
| `auto-cols-auto` 🆕 | Auto-sized columns         | `<div class="auto-cols-auto">`  |
| `auto-cols-min` 🆕  | Min-content sized columns  | `<div class="auto-cols-min">`   |
| `auto-cols-max` 🆕  | Max-content sized columns  | `<div class="auto-cols-max">`   |
| `auto-cols-fr` 🆕   | Equal fractional columns   | `<div class="auto-cols-fr">`    |

### NEW v1.2: Grid Layering Classes

| Class                 | Description                  | Usage Example                       |
| --------------------- | ---------------------------- | ----------------------------------- |
| `grid-layer-full` 🆕  | Layer over entire grid       | `<div class="grid-layer-full">`     |
| `grid-full-width` 🆕  | Span all columns (shortcut)  | `<div class="grid-full-width">`     |
| `grid-full-height` 🆕 | Span all rows (shortcut)     | `<div class="grid-full-height">`    |

### NEW v1.2: Intrinsic Sizing Classes

| Class                  | Description                | Usage Example                        |
| ---------------------- | -------------------------- | ------------------------------------ |
| `grid-intrinsic-min` 🆕 | Min-content auto-fit grid | `<div class="grid-intrinsic-min">`   |
| `grid-intrinsic-max` 🆕 | Max-content auto-fit grid | `<div class="grid-intrinsic-max">`   |
| `grid-fit-content` 🆕   | Fit-content 300px max     | `<div class="grid-fit-content">`     |
| `grid-fit-content-sm` 🆕 | Fit-content 200px max    | `<div class="grid-fit-content-sm">`  |
| `grid-fit-content-lg` 🆕 | Fit-content 400px max    | `<div class="grid-fit-content-lg">`  |

### Gap/Spacing Classes

| Class      | Description           | Usage Example                      |
| ---------- | --------------------- | ---------------------------------- |
| `gap-0`    | No gap                | `<div class="grid-auto gap-0">`    |
| `gap-1`    | 0.25rem gap           | `<div class="grid-auto gap-1">`    |
| `gap-2`    | 0.5rem gap            | `<div class="grid-auto gap-2">`    |
| `gap-3`    | 0.75rem gap           | `<div class="grid-auto gap-3">`    |
| `gap-4`    | 1rem gap              | `<div class="grid-auto gap-4">`    |
| `gap-5`    | 1.25rem gap           | `<div class="grid-auto gap-5">`    |
| `gap-6`    | 1.5rem gap            | `<div class="grid-auto gap-6">`    |
| `gap-7`    | 1.75rem gap           | `<div class="grid-auto gap-7">`    |
| `gap-8`    | 2rem gap              | `<div class="grid-auto gap-8">`    |
| `gap-10`   | 2.5rem gap            | `<div class="grid-auto gap-10">`   |
| `gap-12`   | 3rem gap              | `<div class="grid-auto gap-12">`   |
| `gap-16`   | 4rem gap              | `<div class="grid-auto gap-16">`   |
| `gap-x-0`  | No horizontal gap     | `<div class="grid-auto gap-x-0">`  |
| `gap-x-1`  | 0.25rem horizontal    | `<div class="grid-auto gap-x-1">`  |
| `gap-x-2`  | 0.5rem horizontal     | `<div class="grid-auto gap-x-2">`  |
| `gap-x-3`  | 0.75rem horizontal    | `<div class="grid-auto gap-x-3">`  |
| `gap-x-4`  | 1rem horizontal gap   | `<div class="grid-auto gap-x-4">`  |
| `gap-x-5`  | 1.25rem horizontal    | `<div class="grid-auto gap-x-5">`  |
| `gap-x-6`  | 1.5rem horizontal gap | `<div class="grid-auto gap-x-6">`  |
| `gap-x-8`  | 2rem horizontal gap   | `<div class="grid-auto gap-x-8">`  |
| `gap-y-0`  | No vertical gap       | `<div class="grid-auto gap-y-0">`  |
| `gap-y-1`  | 0.25rem vertical      | `<div class="grid-auto gap-y-1">`  |
| `gap-y-2`  | 0.5rem vertical       | `<div class="grid-auto gap-y-2">`  |
| `gap-y-3`  | 0.75rem vertical      | `<div class="grid-auto gap-y-3">`  |
| `gap-y-4`  | 1rem vertical gap     | `<div class="grid-auto gap-y-4">`  |
| `gap-y-5`  | 1.25rem vertical      | `<div class="grid-auto gap-y-5">`  |
| `gap-y-6`  | 1.5rem vertical gap   | `<div class="grid-auto gap-y-6">`  |
| `gap-y-8`  | 2rem vertical gap     | `<div class="grid-auto gap-y-8">`  |

### Alignment Classes

| Class                      | Description                       | Usage Example                                      |
| -------------------------- | --------------------------------- | -------------------------------------------------- |
| `grid-center`              | Center items both axes            | `<div class="grid-center">`                        |
| `grid-place-center` 🆕     | Place-items center (shorthand)    | `<div class="grid-place-center">`                  |
| `grid-place-content-center` 🆕 | Place-content center         | `<div class="grid-place-content-center">`          |
| `justify-items-start`      | Justify items to start            | `<div class="grid-auto justify-items-start">`      |
| `justify-items-center`     | Justify items to center           | `<div class="grid-auto justify-items-center">`     |
| `justify-items-end`        | Justify items to end              | `<div class="grid-auto justify-items-end">`        |
| `justify-items-stretch`    | Stretch items horizontally        | `<div class="grid-auto justify-items-stretch">`    |
| `align-items-start`        | Align items to start              | `<div class="grid-auto align-items-start">`        |
| `align-items-center`       | Align items to center             | `<div class="grid-auto align-items-center">`       |
| `align-items-end`          | Align items to end                | `<div class="grid-auto align-items-end">`          |
| `align-items-stretch`      | Stretch items vertically          | `<div class="grid-auto align-items-stretch">`      |
| `justify-content-start` 🆕 | Justify grid content to start     | `<div class="grid-auto justify-content-start">`    |
| `justify-content-center` 🆕 | Justify grid content to center   | `<div class="grid-auto justify-content-center">`   |
| `justify-content-end` 🆕   | Justify grid content to end       | `<div class="grid-auto justify-content-end">`      |
| `justify-content-between` 🆕 | Space between grid tracks       | `<div class="grid-auto justify-content-between">`  |
| `justify-content-around` 🆕 | Space around grid tracks         | `<div class="grid-auto justify-content-around">`   |
| `justify-content-evenly` 🆕 | Space evenly between tracks      | `<div class="grid-auto justify-content-evenly">`   |
| `align-content-start` 🆕   | Align grid content to start       | `<div class="grid-auto align-content-start">`      |
| `align-content-center` 🆕  | Align grid content to center      | `<div class="grid-auto align-content-center">`     |
| `align-content-end` 🆕     | Align grid content to end         | `<div class="grid-auto align-content-end">`        |
| `align-content-between` 🆕 | Space between rows                | `<div class="grid-auto align-content-between">`    |
| `align-content-around` 🆕  | Space around rows                 | `<div class="grid-auto align-content-around">`     |
| `align-content-evenly` 🆕  | Space evenly between rows         | `<div class="grid-auto align-content-evenly">`     |
| `justify-self-start`       | Justify self to start             | `<div class="justify-self-start">`                 |
| `justify-self-center`      | Justify self to center            | `<div class="justify-self-center">`                |
| `justify-self-end`         | Justify self to end               | `<div class="justify-self-end">`                   |
| `justify-self-stretch`     | Stretch self horizontally         | `<div class="justify-self-stretch">`               |
| `align-self-start`         | Align self to start               | `<div class="align-self-start">`                   |
| `align-self-center`        | Align self to center              | `<div class="align-self-center">`                  |
| `align-self-end`           | Align self to end                 | `<div class="align-self-end">`                     |
| `align-self-stretch`       | Stretch self vertically           | `<div class="align-self-stretch">`                 |

### Responsive Modifiers

| Prefix | Breakpoint | Usage Example                                     |
| ------ | ---------- | ------------------------------------------------- |
| `sm:`  | 640px+     | `<div class="grid-cols-1 sm:grid-cols-2">`        |
| `md:`  | 768px+     | `<div class="grid-cols-1 md:grid-cols-3">`        |
| `lg:`  | 1024px+    | `<div class="grid-cols-1 lg:grid-cols-4">`        |
| `xl:`  | 1280px+    | `<div class="grid-cols-1 xl:grid-cols-5">`        |

**Available responsive classes:**

- `sm:grid-cols-1`, `sm:grid-cols-2`, `sm:col-span-full`
- `md:grid-cols-2`, `md:grid-cols-3`, `md:grid-cols-4`
- `lg:grid-cols-3`, `lg:grid-cols-4`, `lg:grid-cols-5`, `lg:grid-cols-6`
- `xl:grid-cols-4`, `xl:grid-cols-5`, `xl:grid-cols-6`

### Common Layout Patterns (Ready-to-Use)

| Class               | Description                      | Usage Example                     |
| ------------------- | -------------------------------- | --------------------------------- |
| `grid-dashboard` 🆕 | Sidebar + header + main layout   | `<div class="grid-dashboard">`    |
| `grid-hero-split` 🆕 | 50/50 hero split (responsive)   | `<div class="grid-hero-split">`   |
| `grid-gallery` 🆕   | Responsive image gallery         | `<div class="grid-gallery">`      |
| `grid-features` 🆕  | Feature section grid (300px min) | `<div class="grid-features">`     |
| `grid-pricing` 🆕   | Pricing cards grid               | `<div class="grid-pricing">`      |
| `grid-blog` 🆕      | Blog layout (2:1 with sidebar)   | `<div class="grid-blog">`         |
| `grid-team` 🆕      | Team members grid                | `<div class="grid-team">`         |
| `grid-stats` 🆕     | Statistics grid (200px min)      | `<div class="grid-stats">`        |
| `grid-testimonials` 🆕 | Testimonials grid (320px min) | `<div class="grid-testimonials">` |
| `grid-portfolio` 🆕 | Portfolio with featured items    | `<div class="grid-portfolio">`    |
| `grid-footer` 🆕    | Footer columns layout            | `<div class="grid-footer">`       |

---

## 📖 Detailed Documentation

### Responsive Grid Classes

#### `.grid-auto` / `.grid-auto-sm` / `.grid-auto-md` / `.grid-auto-lg`

Creates a **responsive grid** that automatically fits as many columns as possible based on minimum width.

**Variants:**

- `.grid-auto-sm`: 150px minimum
- `.grid-auto` / `.grid-auto-md`: 250px minimum (default)
- `.grid-auto-lg`: 400px minimum

**Use case:** Image galleries, product cards, any content that should flow naturally

```html
<div class="grid-auto gap-lg">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
</div>
```

---

#### `.grid-fill` / `.grid-fill-sm` / `.grid-fill-lg`

Similar to `.grid-auto`, but uses `auto-fill` instead of `auto-fit`. Creates **empty columns** if there's extra space.

**Difference from `.grid-auto`:**

- `auto-fit`: Collapses empty tracks, items stretch to fill space
- `auto-fill`: Keeps empty tracks, items maintain consistent size

```html
<div class="grid-fill gap-md">
  <div>Item 1</div>
  <div>Item 2</div>
</div>
```

---

#### `.grid-cards` / `.grid-cards-sm` / `.grid-cards-md` / `.grid-cards-lg`

Responsive card grid with **min/max constraints** for better control.

**Variants:**

- `.grid-cards-sm`: 200px minimum
- `.grid-cards`: 280px minimum (default)
- `.grid-cards-md`: 320px minimum
- `.grid-cards-lg`: 400px minimum

```html
<div class="grid-cards">
  <div class="card">Card 1</div>
  <div class="card">Card 2</div>
  <div class="card">Card 3</div>
</div>
```

---

#### `.grid-dense` / `.grid-dense-sm` / `.grid-dense-lg`

Fills gaps by placing items **densely** (useful for varying item sizes).

```html
<div class="grid-dense gap-md">
  <div class="col-span-2">Large item</div>
  <div>Normal</div>
  <div>Normal</div>
</div>
```

---

#### `.grid-stacked` / `.grid-stacked-2` / `.grid-stacked-3` / `.grid-stacked-4`

**Mobile-first stacked grid** that expands on larger screens.

- `.grid-stacked` / `.grid-stacked-2`: 1 column → 2 columns at 640px
- `.grid-stacked-3`: 1 column → 3 columns at 640px
- `.grid-stacked-4`: 1 column → 2 columns at 640px → 4 columns at 1024px

```html
<div class="grid-stacked gap-md">
  <div>Stacks on mobile</div>
  <div>2 columns on tablet+</div>
</div>
```

---

### Fixed Grid Classes

#### `.grid-cols-*` (1-12)

Creates a grid with a **fixed number of columns**.

Available: `grid-cols-1` through `grid-cols-12`

```html
<div class="grid-cols-4 gap-md">
  <div>Column 1</div>
  <div>Column 2</div>
  <div>Column 3</div>
  <div>Column 4</div>
</div>
```

---

#### `.grid-rows-*` (1-6)

Creates a grid with a **fixed number of rows** with equal height.

Available: `grid-rows-1` through `grid-rows-6`

```html
<div class="grid-rows-3 gap-md" style="height: 400px;">
  <div>Row 1</div>
  <div>Row 2</div>
  <div>Row 3</div>
</div>
```

---

### Layout Pattern Classes

#### `.grid-sidebar` / `.grid-sidebar-sm` / `.grid-sidebar-lg`

Creates a **sidebar + main content** layout.

**Variants:**

- `.grid-sidebar-sm-left`: 200px sidebar on left
- `.grid-sidebar-left`: 300px sidebar on left (default)
- `.grid-sidebar-lg-left`: 400px sidebar on left
- `.grid-sidebar-sm-right`: 200px sidebar on right
- `.grid-sidebar-right`: 300px sidebar on right
- `.grid-sidebar-lg-right`: 400px sidebar on right

```html
<div class="grid-sidebar-left gap-lg">
  <aside>Sidebar</aside>
  <main>Main Content</main>
</div>
```

---

#### `.grid-sidebar-responsive`

Sidebar that **stacks on mobile** and appears side-by-side on larger screens (768px+).

```html
<div class="grid-sidebar-responsive gap-lg">
  <aside>Sidebar (stacks on mobile)</aside>
  <main>Main Content</main>
</div>
```

---

#### `.grid-holy-grail` / `.grid-holy-grail-sm` / `.grid-holy-grail-lg`

Classic **Holy Grail layout** (header, sidebars, content, footer).

**Required child classes:**

- `.area-header`
- `.area-sidebar-left`
- `.area-content`
- `.area-sidebar-right`
- `.area-footer`

```html
<div class="grid-holy-grail">
  <header class="area-header">Header</header>
  <aside class="area-sidebar-left">Left Sidebar</aside>
  <main class="area-content">Main Content</main>
  <aside class="area-sidebar-right">Right Sidebar</aside>
  <footer class="area-footer">Footer</footer>
</div>
```

---

#### `.grid-full-bleed` / `.grid-full-bleed-sm` / `.grid-full-bleed-lg`

Grid that allows items to **break out** to full width while keeping content centered.

Child elements automatically constrained; override with inline grid-column style if needed.

```html
<div class="grid-full-bleed">
  <h1>Normal Content (constrained to 1200px)</h1>
  <p>Regular paragraph</p>
  <img style="grid-column: 1 / -1;" src="hero.jpg" alt="Full width image" />
  <p>Back to constrained width</p>
</div>
```

---

#### `.grid-asymmetric-*`

Creates an **asymmetric 2-column layout** with custom ratio.

Available:
- `.grid-asymmetric-2-1`: 2:1 ratio (main content larger)
- `.grid-asymmetric-1-2`: 1:2 ratio (sidebar larger)
- `.grid-asymmetric-3-1`: 3:1 ratio
- `.grid-asymmetric-1-3`: 1:3 ratio
- `.grid-asymmetric-3-2`: 3:2 ratio

```html
<div class="grid-asymmetric-2-1 gap-lg">
  <main>Main content (2/3 width)</main>
  <aside>Sidebar (1/3 width)</aside>
</div>
```

---

#### `.grid-masonry` / `.grid-masonry-2` / `.grid-masonry-4` / `.grid-masonry-modern` 🆕

Creates a **masonry-style layout** effect.

- `.grid-masonry`: 3 columns, traditional masonry
- `.grid-masonry-2`: 2 columns
- `.grid-masonry-4`: 4 columns
- `.grid-masonry-modern` 🆕: 3 columns with improved dense packing

**Note:** Items need inline `grid-row-end: span X` for varying heights.

```html
<div class="grid-masonry-modern">
  <div style="grid-row-end: span 20;">Tall item</div>
  <div style="grid-row-end: span 10;">Short item</div>
  <div style="grid-row-end: span 15;">Medium item</div>
</div>
```

---

### Grid Item Classes

#### `.col-span-*` (1-12, full)

Makes a grid item **span across multiple columns**.

```html
<div class="grid-cols-4">
  <div class="col-span-2">Spans 2 columns</div>
  <div>Normal</div>
  <div>Normal</div>
</div>
```

---

#### `.row-span-*` (1-6, full)

Makes a grid item **span across multiple rows**.

```html
<div class="grid-cols-3">
  <div class="row-span-2">Tall item (2 rows)</div>
  <div>Normal</div>
  <div>Normal</div>
  <div>Normal</div>
  <div>Normal</div>
</div>
```

---

#### `.order-*`

Changes the **visual order** of grid items without changing HTML.

Available: `.order-first`, `.order-last`, `.order-none`, `.order-1` through `.order-6`

```html
<div class="grid-cols-3">
  <div class="order-last">Appears last</div>
  <div>Middle</div>
  <div class="order-first">Appears first</div>
</div>
```

---

### Alignment & Utility Classes

#### `.grid-center` / `.grid-place-center` 🆕

Centers content **both horizontally and vertically** within a grid cell.

```html
<div class="grid-center" style="min-height: 400px;">
  <h1>Perfectly Centered</h1>
</div>
```

---

#### Alignment Classes

Control **how items align** within their grid cells.

**Container alignment (affects all items):**

- `.justify-items-start`, `.justify-items-center`, `.justify-items-end`, `.justify-items-stretch`
- `.align-items-start`, `.align-items-center`, `.align-items-end`, `.align-items-stretch`

**Grid content alignment (new v1.2):** 🆕

- `.justify-content-start`, `.justify-content-center`, `.justify-content-end`
- `.justify-content-between`, `.justify-content-around`, `.justify-content-evenly`
- `.align-content-start`, `.align-content-center`, `.align-content-end`
- `.align-content-between`, `.align-content-around`, `.align-content-evenly`

**Self alignment (affects single item):**

- `.justify-self-start`, `.justify-self-center`, `.justify-self-end`, `.justify-self-stretch`
- `.align-self-start`, `.align-self-center`, `.align-self-end`, `.align-self-stretch`

```html
<div class="grid-cols-3 align-items-center">
  <div>Centered vertically</div>
  <div class="align-self-start">Aligned to top</div>
  <div>Centered vertically</div>
</div>
```

---

#### Gap Classes

Control **spacing between grid items**.

**Uniform gaps:** `.gap-0` through `.gap-16`

**Directional gaps:** `.gap-x-*` (horizontal), `.gap-y-*` (vertical)

```html
<!-- Large uniform gap -->
<div class="grid-auto gap-8">
  <div>Item 1</div>
  <div>Item 2</div>
</div>

<!-- Different horizontal and vertical gaps -->
<div class="grid-auto gap-x-8 gap-y-2">
  <div>Wide horizontal space</div>
  <div>Narrow vertical space</div>
</div>
```

---

### Advanced Grid Controls (New v1.2)

#### Grid Flow Control 🆕

Control how grid items are **automatically placed** and whether gaps should be filled.

**Classes:**
- `.grid-flow-row`: Place items in rows (default)
- `.grid-flow-col`: Place items in columns
- `.grid-flow-dense`: Fill gaps with smaller items
- `.grid-flow-row-dense`: Row placement with dense packing
- `.grid-flow-col-dense`: Column placement with dense packing

```html
<!-- Dense packing for varying-size items -->
<div class="grid-cols-4 grid-flow-dense gap-4">
  <div class="col-span-2">Large item</div>
  <div>Small</div>
  <div class="col-span-2">Large item</div>
  <div>Small</div>
  <!-- Dense flow fills gaps automatically -->
</div>
```

---

#### Auto-Sizing Classes 🆕

Control the size of **automatically created** grid tracks.

**Auto Rows:**
- `.auto-rows-auto`: Auto-sized based on content
- `.auto-rows-min`: Minimum content size
- `.auto-rows-max`: Maximum content size
- `.auto-rows-fr`: Equal fractional units

**Auto Columns:**
- `.auto-cols-auto`: Auto-sized based on content
- `.auto-cols-min`: Minimum content size
- `.auto-cols-max`: Maximum content size
- `.auto-cols-fr`: Equal fractional units

```html
<!-- All rows sized to content -->
<div class="grid-cols-3 auto-rows-min gap-4">
  <div>Short content</div>
  <div>Longer content that spans multiple lines</div>
  <div>Medium</div>
</div>

<!-- Equal height rows -->
<div class="grid-cols-3 auto-rows-fr gap-4">
  <div>Row 1</div>
  <div>Row 2</div>
  <div>Row 3</div>
</div>
```

---

### Grid Layering & Overlays (New v1.2)

#### `.grid-layer-full` 🆕

Overlay elements across the **entire grid** (all columns and rows). Perfect for hero sections with overlaid content.

```html
<div class="grid-cols-1" style="min-height: 500px;">
  <!-- Background image spans full grid -->
  <img class="grid-layer-full" src="hero-bg.jpg" alt="Background" style="object-fit: cover;" />
  
  <!-- Overlay content also spans full grid -->
  <div class="grid-layer-full grid-center" style="background: rgba(0,0,0,0.5);">
    <div style="color: white; text-align: center;">
      <h1>Hero Title</h1>
      <p>Overlaid content</p>
    </div>
  </div>
</div>
```

---

#### `.grid-full-width` 🆕 / `.grid-full-height` 🆕

Quick shortcuts to span all columns or rows.

- `.grid-full-width`: Same as `grid-column: 1 / -1`
- `.grid-full-height`: Same as `grid-row: 1 / -1`

```html
<div class="grid-cols-3 gap-4">
  <div>Column 1</div>
  <div>Column 2</div>
  <div>Column 3</div>
  <div class="grid-full-width">Full width banner</div>
  <div>Column 1</div>
  <div>Column 2</div>
  <div>Column 3</div>
</div>
```

---

### Intrinsic Sizing (New v1.2)

#### `.grid-intrinsic-min` 🆕 / `.grid-intrinsic-max` 🆕

Create grids where columns size based on **content** rather than fixed widths.

- `.grid-intrinsic-min`: Columns shrink to minimum content width
- `.grid-intrinsic-max`: Columns expand to maximum content width

**Use case:** Tag lists, navigation menus, button groups

```html
<!-- Tags that size to their content -->
<div class="grid-intrinsic-max gap-2">
  <span class="tag">Short</span>
  <span class="tag">Medium Length</span>
  <span class="tag">Very Long Tag Name</span>
</div>
```

---

#### `.grid-fit-content` 🆕 / `.grid-fit-content-sm` 🆕 / `.grid-fit-content-lg` 🆕

Columns size to content but with a **maximum width** constraint.

- `.grid-fit-content-sm`: Max 200px per column
- `.grid-fit-content`: Max 300px per column (default)
- `.grid-fit-content-lg`: Max 400px per column

```html
<div class="grid-fit-content gap-4">
  <div>Sizes to content up to 300px</div>
  <div>Another item</div>
</div>
```

---

### Container Queries (New v1.2)

#### `.grid-container-aware` 🆕

Enable **container-based responsiveness** instead of viewport-based. Grid responds to its container width, not screen width.

**Variants:**
- `.grid-container-aware-sm`: 150px minimum columns
- `.grid-container-aware`: 250px minimum columns (default)
- `.grid-container-aware-lg`: 350px minimum columns

**Use case:** Reusable components that adapt to any container size

```html
<div style="width: 400px;"> <!-- Small container -->
  <div class="grid-container-aware gap-4">
    <!-- Adjusts based on 400px width, not viewport -->
    <div>Item 1</div>
    <div>Item 2</div>
  </div>
</div>

<div style="width: 1200px;"> <!-- Large container -->
  <div class="grid-container-aware gap-4">
    <!-- Shows more columns in this wider container -->
    <div>Item 1</div>
    <div>Item 2</div>
    <div>Item 3</div>
    <div>Item 4</div>
  </div>
</div>
```

---

### Responsive Modifiers

Use **breakpoint prefixes** to apply classes at specific screen sizes.

**Breakpoints:**

- `sm:` - 640px and up (tablets)
- `md:` - 768px and up (landscape tablets)
- `lg:` - 1024px and up (desktops)
- `xl:` - 1280px and up (large desktops)

```html
<!-- 1 column mobile, 2 tablet, 4 desktop -->
<div class="grid-cols-1 sm:grid-cols-2 lg:grid-cols-4 gap-md">
  <div>Item 1</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
</div>

<!-- Responsive spanning -->
<div class="grid-cols-2 md:grid-cols-4">
  <div class="col-span-2 md:col-span-1">Full width mobile, 1/4 desktop</div>
  <div>Item 2</div>
  <div>Item 3</div>
  <div>Item 4</div>
</div>
```

---

## 💡 Usage Examples

### Responsive Image Gallery with Featured Item

```html
<div class="grid-auto-lg gap-4 grid-flow-dense">
  <img src="1.jpg" alt="Photo 1" />
  <img src="2.jpg" alt="Photo 2" />
  <img class="col-span-2 row-span-2" src="3.jpg" alt="Featured" />
  <img src="4.jpg" alt="Photo 4" />
  <img src="5.jpg" alt="Photo 5" />
  <img src="6.jpg" alt="Photo 6" />
</div>
```

---

### Dashboard Layout with Auto-Sized Sidebar

```html
<div class="grid-dashboard">
  <aside class="area-sidebar">
    <nav>Navigation</nav>
  </aside>
  
  <header class="area-header">
    <h1>Dashboard</h1>
  </header>
  
  <main class="area-main grid-cards gap-6">
    <div class="card">Widget 1</div>
    <div class="card">Widget 2</div>
    <div class="card col-span-2">Large Widget</div>
    <div class="card">Widget 4</div>
  </main>
</div>
```

---

### Hero Section with Layered Content (NEW v1.2) 🆕

```html
<div class="grid-cols-1" style="min-height: 600px;">
  <!-- Background image -->
  <img 
    class="grid-layer-full" 
    src="hero-bg.jpg" 
    alt="Hero background"
    style="object-fit: cover; width: 100%; height: 100%;" 
  />
  
  <!-- Dark overlay -->
  <div class="grid-layer-full" style="background: rgba(0, 0, 0, 0.4);"></div>
  
  <!-- Content on top -->
  <div class="grid-layer-full grid-center">
    <div style="color: white; text-align: center; z-index: 1;">
      <h1 style="font-size: 3rem; margin-bottom: 1rem;">Welcome</h1>
      <p style="font-size: 1.25rem;">Discover amazing content</p>
      <button style="margin-top: 2rem;">Get Started</button>
    </div>
  </div>
</div>
```

---

### Container-Aware Component Grid (NEW v1.2) 🆕

```html
<!-- Sidebar with responsive widget grid -->
<div class="grid-sidebar-responsive gap-8">
  <aside style="background: #f5f5f5; padding: 2rem;">
    <!-- Grid adapts to sidebar width, not viewport -->
    <div class="grid-container-aware gap-4">
      <div class="widget">Widget 1</div>
      <div class="widget">Widget 2</div>
      <div class="widget">Widget 3</div>
    </div>
  </aside>
  
  <main>
    <h1>Main Content</h1>
    <p>Sidebar widgets adapt to sidebar width</p>
  </main>
</div>
```

---

### Product Grid with Dense Packing (NEW v1.2) 🆕

```html
<div class="grid-cols-4 grid-flow-dense gap-4">
  <div class="product col-span-2 row-span-2">Featured Product</div>
  <div class="product">Product 2</div>
  <div class="product">Product 3</div>
  <div class="product row-span-2">Tall Product</div>
  <div class="product">Product 5</div>
  <div class="product col-span-2">Wide Product</div>
  <!-- Dense flow automatically fills gaps -->
</div>
```

---

### Blog Layout with Content Alignment (NEW v1.2) 🆕

```html
<div class="grid-sidebar-responsive gap-8 align-content-start">
  <article class="grid-rows-3 gap-6 auto-rows-min">
    <header>
      <h1>Article Title</h1>
      <p class="meta">Published on Jan 1, 2024</p>
    </header>
    
    <div class="content">
      <p>Article content that can vary in length...</p>
    </div>
    
    <footer class="align-self-end">
      <div class="tags grid-intrinsic-max gap-2">
        <span class="tag">CSS</span>
        <span class="tag">Grid</span>
        <span class="tag">Web Design</span>
      </div>
    </footer>
  </article>

  <aside>
    <div class="widget">Recent Posts</div>
    <div class="widget">Categories</div>
  </aside>
</div>
```

---

### Pricing Table with Equal Heights (NEW v1.2) 🆕

```html
<div class="grid-cols-3 auto-rows-fr gap-6">
  <div class="pricing-card">
    <h3>Basic</h3>
    <p class="price">$9/mo</p>
    <ul class="features">
      <li>Feature 1</li>
      <li>Feature 2</li>
    </ul>
    <button class="align-self-end">Choose Plan</button>
  </div>
  
  <div class="pricing-card">
    <h3>Pro</h3>
    <p class="price">$29/mo</p>
    <ul class="features">
      <li>Everything in Basic</li>
      <li>Feature 3</li>
      <li>Feature 4</li>
    </ul>
    <button class="align-self-end">Choose Plan</button>
  </div>
  
  <div class="pricing-card">
    <h3>Enterprise</h3>
    <p class="price">Custom</p>
    <ul class="features">
      <li>Everything in Pro</li>
      <li>Feature 5</li>
      <li>Priority Support</li>
    </ul>
    <button class="align-self-end">Contact Sales</button>
  </div>
</div>
```

---

## 🎯 Best Practices

### 1. Choose the Right Grid Type

- **Auto-fit/Auto-fill** (`.grid-auto`, `.grid-fill`): Use for galleries, cards, or any content that should flow naturally
- **Fixed columns** (`.grid-cols-*`): Use when you need precise control over layout structure
- **Container-aware** 🆕 (`.grid-container-aware`): Use for reusable components that need to adapt to their container

### 2. Gap Sizing Guidelines

- `.gap-2` or `.gap-3`: Tight spacing (tags, small components)
- `.gap-4`: Default spacing (most layouts)
- `.gap-6` or `.gap-8`: Generous spacing (cards, sections)
- `.gap-12` or `.gap-16`: Large spacing (major sections)

### 3. Responsive Strategy

Start mobile-first, then add breakpoints:

```html
<!-- Mobile: 1 col, Tablet: 2 cols, Desktop: 4 cols -->
<div class="grid-cols-1 sm:grid-cols-2 lg:grid-cols-4">
  <!-- content -->
</div>
```

### 4. Using Grid Flow 🆕

- Use `.grid-flow-dense` when items have varying sizes to fill gaps efficiently
- Use `.grid-flow-col` for vertical layouts (navigation, sidebars)
- Combine with auto-rows/cols for dynamic layouts

### 5. Layering Content 🆕

For overlapping content (hero sections, overlays):

```html
<div class="grid-cols-1">
  <img class="grid-layer-full" src="bg.jpg" />
  <div class="grid-layer-full grid-center">
    <!-- Your overlaid content -->
  </div>
</div>
```

### 6. Content vs Items Alignment 🆕

- **Items alignment** (`.align-items-*`, `.justify-items-*`): Aligns content within each grid cell
- **Content alignment** (`.align-content-*`, `.justify-content-*`): Aligns the entire grid within its container (useful when grid doesn't fill container)

### 7. Combining Classes

Stack utilities for precise control:

```html
<div class="grid-auto-lg gap-6 grid-flow-dense align-items-start">
  <!-- Large auto-fit grid with dense packing and top-aligned items -->
</div>
```

---

## 🌐 Browser Support

- **Modern browsers**: Full support (Chrome, Firefox, Safari, Edge)
- **CSS Grid**: 96%+ global support
- **Container Queries** 🆕: 90%+ support (all modern browsers, IE11 excluded)
- **Subgrid**: 85%+ support (not IE11/old Safari)

### Fallbacks

For older browsers, consider:

```css
/* Fallback for container queries */
@supports not (container-type: inline-size) {
  .grid-container-aware {
    /* Regular responsive grid fallback */
  }
}
```
