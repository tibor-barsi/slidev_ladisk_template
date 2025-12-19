---
theme: default
title: Slidev Template
author: Your Name
duration: 15min
class: text-center
colorSchema: light
aspectRatio: 16/9
defaults:
  layout: default
  class: text-s
layout: cover
lineNumbers: true
fonts:
  sans: 'Open Sans'
---

# Your Presentation Title

**Subtitle or tagline goes here**

<br>

Additional information can go here.

---
layout: default
---

## Default Layout

This is the standard layout with content spanning the full width.

- Content flows naturally from top to bottom
- Great for text-heavy slides
- Can include images inline

<br>

<div style="display: flex; justify-content: center;">
  <img src="/toolchanger.jpg" style="width: 200px; height: auto;" />
</div>

---
layout: image-right
image: /toolchanger.jpg
backgroundSize: contain
---

## Image-Right Layout

The image automatically fills the right half.

- Set image in frontmatter
- Content goes on the left
- Control size with `backgroundSize`

**Options:**
- `contain` - fit entire image
- `cover` - fill the space
- `80%` - specific percentage

---
layout: two-cols
---

## Two Columns Layout

Content is split into two equal columns.

- Left column for text
- Right column for images
- Use `::right::` to define right column

**Perfect for:**
- Comparing concepts
- Text + visual combinations
- Side-by-side content

::right::

<div style="display: flex; justify-content: center; align-items: center; height: 100%;">
  <img src="/toolchanger.jpg" style="width: 350px; height: auto;" />
</div>

---
layout: two-cols-header
---

## Two Columns with Header

A centered header spans both columns.

::left::

### Left Column

- First point
- Second point
- Third point

Content in left section.

::right::

### Right Column

<div style="display: flex; justify-content: center;">
  <img src="/toolchanger.jpg" style="width: 250px; height: auto;" />
</div>

---
layout: center
class: text-center
---

## Centered Layout

Everything is vertically and horizontally centered.

<div style="display: flex; justify-content: center; margin-top: 2rem;">
  <img src="/toolchanger.jpg" style="width: 200px; height: auto;" />
</div>

Perfect for title slides, section breaks, or emphasis.

---

## Markdown: Headings

# Heading 1
## Heading 2
### Heading 3
#### Heading 4

Use headings to structure your content hierarchically.

---
layout: two-cols
---

## Markdown: Lists

### Unordered Lists
- First item
- Second item
  - Nested item
  - Another nested item
- Third item

### Ordered Lists
1. First step
2. Second step
3. Third step

::right::

### Task Lists
- [x] Completed task
- [x] Another done
- [ ] Pending task
- [ ] To be done

<br>

**Mix and match** as needed for your content structure.

---

## Markdown: Text Formatting

**Bold text** for emphasis

*Italic text* for subtle emphasis

~~Strikethrough~~ for removed content

`inline code` for technical terms

Combine **_bold and italic_** or **`bold code`**

<br>

> Blockquotes are great for highlighting important statements or quotes from sources.

---
layout: two-cols
---

## Markdown: Tables

Tables organize data clearly:

| Feature | Description | Status |
|---------|-------------|--------|
| Markdown | Write in plain text | ✅ |
| Themes | Multiple options | ✅ |
| Export | PDF, PPTX, PNG | ✅ |
| LaTeX | Math equations | ✅ |

::right::

<br>
<br>
<br>
<br>
<br>
<div class="text-s text-center">

**Alignment options:**<br>
Left: `|:---|`<br>
Center: `|:---:|`<br>
Right: `|---:|`

</div>
---

## Markdown: Links & More

**External links:**  
[Slidev Documentation](https://sli.dev)

**Internal navigation:**  
Go to [slide 3](#3) or [slide 1](#1)

---
layout: two-cols
---

## Click animation

Use bullet points to organize your content:

- 📝 **Markdown-based** - Write slides in Markdown
- 🎨 **Themable** - Multiple themes available
- 🧑‍💻 **Developer Friendly** - Syntax highlighting included

<br>

<div v-click=1>

#### Key Feature:
- single-process workflow,
- multiple output formats.

</div>

::right::

<div style="display: flex; justify-content: center;">

<img v-click=1 src="/toolchanger.jpg" style="width: 350px; height: auto;" />

</div>

---
layout: default
---

## Sequential Click Animations

<div v-click="1">

### 1. First item appears

</div>

<div v-click="2">

### 2. Then the second item

</div>

<div v-click="3">

### 3. Finally the third item

</div>

<br>
<div class="flex gap-4 justify-center items-center">
  <img v-click="1" src="/experiment_11.png" class="w-64" />
  <img v-click="2" src="/toolchanger.jpg" class="w-64" />
  <img v-click="3" src="/printing_direction_sketch.png" class="w-55" />
</div>

---
layout: two-cols-header
---

<div class="text-center">

## Math Equations with LaTeX

</div>

::left::
<br>
<br>
<div style="display: flex; justify-content: center;">
<img src="/intro_smart_structures.png" style="width: 270px; height: auto;" />
</div>

::right::
<div class="text-center">
<br>

Inline equation example:

</div>

$$\frac{\Delta\boldsymbol{\rho}}{\rho_0} = \boldsymbol{\pi} \cdot \boldsymbol{\sigma}$$

<div class="text-s text-center">

$\boldsymbol{\rho}$ ... resistivity, $\boldsymbol{\pi}$ ... coefficients, $\boldsymbol{\sigma}$ ... stress

</div>
<br>

<v-click>
<div class="text-center">

**Another Formula**

</div>

$$GF = \frac{\Delta R / R_\text{0}}{\Delta L / L_\text{0}}$$

<div class="text-s text-center">

$R$ ... resistance, $L$ ... length

</div>
</v-click>

---
layout: two-cols
---

## Tables Example

<br>

> Tables are useful for presenting data.

<br>

<ColorBox color='gray'>

| **Category** | **Value** | **Unit** |
|---|---|---|
| Parameter A | 0.86 | GPa⁻¹ |
| Parameter B | 1.09 | GPa⁻¹ |
| Parameter C | 2.51 | GPa⁻¹ |

</ColorBox>

::right::

<br>
<div style="display: flex; justify-content: center;">
  <img src="/toolchanger.jpg" style="width: 300px; height: auto;" />
</div>

---
layout: two-cols-header
---

## Custom ColorBox Components

::left::

<ColorBox color='green'>

#### Green Box
- Success message
- Positive information
- Confirmation

</ColorBox>

<ColorBox color='blue'>

#### Blue Box
- Information
- Research question
- Key point

</ColorBox>

::right::

<ColorBox color='red'>

#### Red Box
- Warning
- Important limitation
- Critical issue

</ColorBox>

<ColorBox color='gray'>

#### Gray Box
- Neutral content
- Data tables
- Reference info

</ColorBox>

---
layout: center
class: text-center
---

# Thank You!

Questions?

[Documentation](https://sli.dev) · [GitHub](https://github.com/slidevjs/slidev)
