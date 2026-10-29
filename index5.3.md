File 1: index.html
HTML
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Assignment 5.3 - Typography Showcase Page</title>

  <!-- Google Fonts: Playfair Display (Headings) and Montserrat (Body) -->
  <link rel="preconnect" href="https://fonts.googleapis.com">
  <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>
  <link href="https://fonts.googleapis.com/css2?family=Montserrat:ital,wght@0,300;0,400;0,600;0,700;1,400&family=Playfair+Display:ital,wght@0,600;0,700;0,900;1,400&display=swap" rel="stylesheet">

  <link rel="stylesheet" href="styles.css">
</head>
<body>

  <header class="hero">
    <h1 class="page-title">Typography Showcase</h1>
    <p class="subtitle">Exploring Font Pairings, Weights, Alignments, and Styling Techniques</p>
  </header>

  <main class="container">

    <!-- Section 1: Heading Styles -->
    <section class="showcase-section">
      <h2 class="section-title">1. Heading Styles</h2>
      <div class="card">
        <h1 class="heading-large">Display Heading (H1)</h1>
        <h2 class="heading-medium">Subheading Style (H2)</h2>
        <h3 class="heading-small">Section Subhead Style (H3)</h3>
      </div>
    </section>

    <!-- Section 2: Paragraph Styles -->
    <section class="showcase-section">
      <h2 class="section-title">2. Paragraph Styles</h2>
      <div class="card">
        <p class="intro-paragraph">
          This is an introductory paragraph styled with a larger font size, increased line height, and a bold font-weight to catch the reader's immediate attention.
        </p>
        <p class="body-paragraph">
          This standard body paragraph showcases tight, comfortable reading line-height and balanced letter spacing. Typography is the art and technique of arranging type to make written language legible, readable, and appealing when displayed.
        </p>
        <p class="caption-paragraph">
          Caption text: Styled with lighter weight, smaller font size, and subtle letter spacing.
        </p>
      </div>
    </section>

    <!-- Section 3: Text Emphasis -->
    <section class="showcase-section">
      <h2 class="section-title">3. Text Emphasis</h2>
      <div class="card">
        <p class="decorated-text">
          This text demonstrates <span class="underline-style">text-decoration: underline</span> and <span class="line-through-style">text-decoration: line-through</span>.
        </p>
        <p class="italic-text">
          This sentence uses font-style: italic to convey a classic quote or emphasis effect.
        </p>
        <p class="spaced-text">
          EXPANDED LETTER SPACING DEMONSTRATION
        </p>
        <p class="aligned-right">
          This paragraph is right-aligned using the text-align property.
        </p>
        <p class="aligned-center">
          This paragraph is center-aligned using the text-align property.
        </p>
      </div>
    </section>

  </main>

  <footer>
    <p>&copy; 2026 Web Development Typography Assignment</p>
  </footer>

</body>
</html>
File 2: styles.css
CSS
/* Universal Reset */
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
}

/* 
  1. Google Fonts setup:
     - Headings: 'Playfair Display', serif
     - Body: 'Montserrat', sans-serif
*/

body {
  font-family: 'Montserrat', sans-serif;
  font-size: 16px;
  line-height: 1.6;
  color: #2c3e50;
  background-color: #f8f9fa;
  padding: 20px;
}

/* Layout Container */
.container {
  max-width: 900px;
  margin: 0 auto;
}

/* Header Styles */
.hero {
  text-align: center;
  margin-bottom: 40px;
  padding: 30px 10px;
  background-color: #1e293b;
  color: #ffffff;
  border-radius: 12px;
}

.page-title {
  font-family: 'Playfair Display', serif;
  font-size: 2.8rem;
  font-weight: 900;
  letter-spacing: 2px;
  margin-bottom: 10px;
}

.subtitle {
  font-size: 1.1rem;
  font-weight: 300;
  letter-spacing: 1px;
  color: #cbd5e1;
}

/* Section & Card Layouts */
.showcase-section {
  margin-bottom: 35px;
}

.section-title {
  font-family: 'Playfair Display', serif;
  font-size: 1.8rem;
  font-weight: 700;
  color: #0f172a;
  border-bottom: 3px solid #3b82f6;
  display: inline-block;
  margin-bottom: 15px;
  padding-bottom: 5px;
}

.card {
  background-color: #ffffff;
  padding: 25px;
  border-radius: 8px;
  border: 1px solid #e2e8f0;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.05);
}

/* Section 1: Heading Styles */
.heading-large {
  font-family: 'Playfair Display', serif;
  font-size: 2.4rem;
  font-weight: 700;
  color: #1e293b;
  margin-bottom: 12px;
}

.heading-medium {
  font-family: 'Playfair Display', serif;
  font-size: 1.8rem;
  font-weight: 600;
  color: #334155;
  margin-bottom: 10px;
}

.heading-small {
  font-family: 'Playfair Display', serif;
  font-size: 1.3rem;
  font-weight: 600;
  font-style: italic;
  color: #475569;
}

/* Section 2: Paragraph Styles */
.intro-paragraph {
  font-size: 1.2rem;
  font-weight: 600;
  line-height: 1.8;
  color: #0f172a;
  margin-bottom: 15px;
}

.body-paragraph {
  font-size: 1rem;
  font-weight: 400;
  line-height: 1.6;
  letter-spacing: 0.3px;
  margin-bottom: 15px;
}

.caption-paragraph {
  font-size: 0.85rem;
  font-weight: 300;
  line-height: 1.4;
  letter-spacing: 0.5px;
  color: #64748b;
}

/* Section 3: Text Emphasis */
.decorated-text {
  margin-bottom: 12px;
}

.underline-style {
  text-decoration: underline;
  text-decoration-color: #3b82f6;
  font-weight: 600;
}

.line-through-style {
  text-decoration: line-through;
  color: #ef4444;
}

.italic-text {
  font-style: italic;
  color: #475569;
  margin-bottom: 12px;
}

.spaced-text {
  font-weight: 700;
  letter-spacing: 4px;
  color: #1e293b;
  margin-bottom: 12px;
}

.aligned-right {
  text-align: right;
  font-size: 0.95rem;
  color: #334155;
  margin-bottom: 12px;
}

.aligned-center {
  text-align: center;
  font-size: 0.95rem;
  font-weight: 600;
  color: #2563eb;
}

/* Footer */
footer {
  text-align: center;
  padding: 20px 0;
  color: #64748b;
  font-size: 0.9rem;
}
Features Implemented Checklist
2 Complementary Fonts from Google Fonts:

Playfair Display (serif) used for Headings and Section Titles.

Montserrat (sans-serif) used for Body text and Paragraphs.

Font Sizes & Weights: Applied weights ranging from light (300), normal (400), semi-bold (600), bold (700), to black (900), with font sizes spanning from 0.85rem to 2.8rem.

Text Formatting Attributes:

text-align: Used left (default), center, and right.

text-decoration: Applied underline and line-through.

font-style: Applied italic.

Spacing & Heights:

letter-spacing: Controlled subtle letter spacing on body copy (0.3px, 0.5px, 1px) and expanded spacing (4px).

line-height: Tuned for optimal reading flow (1.4, 1.6, 1.8).

3 Required Sections:

Section 1: Heading Styles

Section 2: Paragraph Styles

Section 3: Text Emphasis