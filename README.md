# Pdf Markdown Generator
```
Write the following content using the following Markdown PDF Exporter syntax. 
• All Standard markdown 
• LaTeX Math


Now Custom Feature 

Color Supported for all block 
teal,green,blue,red,yellow,pink,navy,maroon ( use small case for color name)


1. Inline Highlight ( this can be used anywhere /in any block)
==text==  ( default teal color)

For other color 
==ColorName:text== 

You can use `ColorName:text` for colorful less hilighted hilight


2. Chapter Banner

```chapter
color: teal
number: 01
title: Chapter Title
subtitle: 
\`\`\`


3. Timeline (for chronological content)

```timeline ColorName
1947 | India gains independence
1950 | Constitution comes into effect
1991 | Economic liberalisation begins
\`\`\`


4. Cards (comparison columns)

```cards
### Column Title (teal)
- Point one
- Point two
Plain paragraph text also works
---
### Second Column (purple)
- Another point
- More details
\`\`\`



5. Callout (for important notes)

```callout
type: info ( Types: info warning danger success tip)
title: Did You Know?
Body text goes here. Can be multiple sentences.
\`\`\`



6. Quote

```quote
The quote text goes here, as long as needed.
by: Author Name
\`\`\`


6. Stats / Metrics

```stats
1,240 | Total Users | +18% | blue
94% | Satisfaction | +3% | green
₹4.2L | Revenue | +22% | teal
12 | Open Issues | -5 | orange
\`\`\`

Format: value | label | delta | color
Delta prefix + = green arrow, - = red arrow



7. Highlighted Banner

```highlight
color: purple
icon: 🚀
title: Key Takeaway
Description text goes here. This is the main point of this section.
\`\`\`



8. Article Cards (numbered with colored left panel use for structured items with numbers)

```article maroon
14 | Article Title Here
- Bullet point one
- Bullet point two
Plain text body also works
---
15 | Second Article Title
- Another point
- Another point
\`\`\`

Format: N | Title then body, articles separated by ---


9. Numbered Feature Cards (for lists of key points)

```numbered teal
1 | First Point Title
Description body text for this numbered item goes here.
---
2 | Second Point Title
Description body text for this numbered item.
---
3 | Third Point Title
More body text here.
\`\`\`

Format: N | Title then body, items separated by ---



10. Important Notes Grid

```note
Label One | Fact or note text goes here.
Label Two | Another important point.
| Item with no label — just text.
\`\`\`

Format: Label | content — label is optional.


11. Section ( use for colorful headings)
```section
color: maroon
number: 4
title: Right to Freedom of Religion
subtitle: Art. 25-28
\`\`\`

12. You can use any other block inside any block

Tip — use :: for inline blocks
No need for triple backticks when writing inside another block.
Use ::grid, ::cards, ::pyq, ::callout, ::note — anything.
Close with :: on its own line.

::note
Article 32 | Right to move Supreme Court — heart & soul of the Constitution
Article 226 | Right to move High Court for enforcement of any legal right
::
```
<br>
<br>


# Replit Html web app artifact

```
I uploaded a standalone HTML file to attached asset

Create a react-vite web artifact at / and replace its index.html with the full content of my uploaded file by copying it directly. No other changes needed.

need to copy it directly. The simplest approach is to use a shell command to copy the file content directly to artifacts/html-app/index.html.

Since this is a standalone HTML file with no React/Vite dependencies needed, I just need to replace the index.html content. But wait - the Vite dev server expects index.html to be the entry point, and it currently loads src/main.tsx. The user's file is a complete standalone HTML with all CSS and JS inline.

The simplest approach: just copy the uploaded HTML file directly to artifacts/html-app/index.html.

Vite will serve the static HTML as-is since it contains all the necessary scripts and styles embedded, so I don't need any React rendering setup.
```



---



<br>
<br>
<br>


# Notebook lm prompt for handwritten notes

```
I am uploading a PDF file that contains handwritten notes created by a student (HandNotes).

Your task is to convert this PDF into a slide deck, following these rules very strictly:

🔒 Content Rules (Very Important)
 1. Do NOT remove, skip, summarize, or miss any content from the original PDF.
 2. Every point, line, example, formula, and explanation must be included.
 3. The sequence and structure must remain exactly the same as the original notes.
 4. The number of slides should match the content naturally (no forced reduction).

✍️ Handwritten Style (Mandatory)
 • All text must look handwritten (handwritten font style).
 • All diagrams, flowcharts, tables, and drawings must be recreated in handwritten style.
 • Use handwritten highlights, underlines, circles, arrows, boxes, and side notes.
 • Use soft, joyful colors (like student notes): blue, black, red, green, yellow highlights.
 • The slides should look like neatly written classroom notes, not typed PPT slides.

🧠 Grammar & Clarity
 • Correct grammar and spelling mistakes, if any.
 • Do NOT change the meaning of the original content.
 • Keep the language simple and student-friendly.

🎓 Expert Enhancement (Allowed but Limited)

You MAY add small expert support only, such as:
 • Clear headings (if missing)
 • Short clarification words
 • Tiny side notes for better understanding

⚠️ Do NOT remove, replace, or rewrite original content.
Your expertise should support, not dominate.

📄 Output Quality
 • Slides should feel like high-quality handwritten A4 notebook pages.
 • Clean spacing, readable handwriting, and visual clarity.
 • Final output must feel like professional handwritten study notes, not a presentation.

```



---


<br>
<br>
<br>

# Notebook lm Prompt
```
I am uploading a PDF containing handwritten student notes.

Your task is to convert every page into a slide deck while preserving the feeling of premium handwritten classroom notes.


1. Content Preservation (Highest Priority)

• Do NOT remove, skip, summarize, shorten, or rewrite any original content.
• Every sentence, point, formula, example, definition, diagram, table, and explanation must appear.
• Maintain exactly the same order as the original PDF.
• Split content naturally across slides only when necessary.
• Never compress multiple pages just to reduce slide count.


2. Handwritten Study Notes Style (Mandatory)
• The output must look like premium aesthetic handwritten notes (Studygram / Sketchnote style), NOT a normal PowerPoint presentation.
• Every slide should resemble a neat A4 notebook page.


Use:
• realistic handwritten font
• slightly varied handwriting size
• blue and black ink for normal writing
• red ink for important rules
• green ink for keywords
• yellow marker highlights
• hand-drawn arrows
• rounded boxes
• circles
• brackets
• curly braces
• underlines
• callouts
• handwritten numbering
• sticky-note style remarks where appropriate
• Everything should feel naturally handwritten.


3. Visual Layout
Use the same visual organization as excellent classroom notes.

Include:

• Large handwritten title
• Colorful subheadings
• Flow diagrams
• Step-by-step blocks
• Highlight boxes
• Exception boxes
• Warning symbols
• Comparison tables
• Hand-drawn connectors
• Mind-map branches
• Side notes
• Margin comments
• Small doodles only when they improve understanding

The page should never look empty.


4. Color Palette
Use soft educational colors only.
Primary colors:
• Blue
• Black
• Red
• Green

Yellow Highlighter
Avoid dark presentation themes.

Use a clean white notebook background.


5. Grammar
Correct spelling and grammar mistakes only.
Never change the meaning.
Never simplify the actual concepts.


6. Expert Enhancement (Limited)
You may only add:
• better headings
• tiny clarification notes
• cleaner formatting
• visual grouping

Do NOT replace or rewrite the student's notes.


7. Slide Appearance
Each slide should resemble a premium handwritten notebook page rather than a presentation.

Maintain:
• balanced spacing
• neat alignment
• generous white space
• readable handwriting
• visually pleasing hierarchy


8. Style Reference
Match the aesthetic of high-quality Studygram notes.

Characteristics include:
• colorful handwritten headings
• highlighted keywords
• hand-drawn arrows
• rounded boxes
• flowchart layouts
• handwritten diagrams
• classroom revision-sheet appearance
• infographic-style note organization


The final result should look as though an expert student spent hours creating beautiful handwritten revision notes.

Never produce slides that resemble a standard PowerPoint with typed text.
```



<br>
<br>
<br>

# Image Creation Prompt

```
I want my image to convert in this design


This design style is primarily:

Neumorphism (Soft UI)
A modern UI trend that combines:

• Soft extruded shadows
• Subtle highlights
• Rounded surfaces
• Embossed/debossed effects
• Minimal depth with realistic lighting


Your infographic specifically uses:

Core Characteristics
• Soft pastel background
• Floating rounded cards
• Inner + outer shadows
• Low-contrast depth
• Smooth gradients
• Soft glowing elements
• Tactile button-like sections
• It’s Actually a Hybrid Style


Your final version mixes multiple premium aesthetics:

1. Neumorphism
Main card surfaces and panels.

2. Glassmorphism Elements
Some translucent glowing areas and gradient highlights still remain from the previous iteration.

3. Gradient UI Design
Modern gradient typography and colored UI accents.

4. 3D Soft Illustration Style
Icons like:
• bulb
• plant
• check/cross
• tape
• speaker
• have soft 3D clay-like rendering.


Professional Name for This Style
If you want to search inspiration or tell a designer:

“Premium Neumorphic Educational Infographic with Soft Gradient UI”

Or:

“Soft UI + Neumorphism + Pastel Gradient Infographic Design”


Why It Looks Premium

The design succeeds because of:
• excellent spacing
• low visual noise
• controlled shadows
• hierarchy through gradients
• soft depth instead of hard borders
• modern typography contrast
• balanced pastel palette


This is very close to modern:

• Dribbble-style UI
• Apple-inspired soft depth
• premium edtech branding
• Behance infographic trends
```


<br>
<br>
<br>

<div align="center">
  
# ❤️ 

