Today I learned:

<header> → defines the top section of a webpage.

<img> → displays an image.

src → tells HTML where the image is located.

alt → alternative text for accessibility.

# Lesson 1 - HTML Structure
## New Tags

- <!DOCTYPE html> → Declares an HTML5 document.
- <html> → Root element of the webpage.
- <head> → Contains page information (title, CSS, metadata).
- <body> → Contains everything visible on the webpage.
- <meta charset="UTF-8"> → Supports international characters.
- <meta name="viewport"> → Makes the page responsive.
- <title> → Text shown in the browser tab.
- <link> → Connects the HTML page to a CSS stylesheet.

Step2 adding information inside the header 
# Session 3 – Hero Section (HTML & CSS)

## Goal
Continue building the hero section of the portfolio website using HTML and CSS.

---

## HTML Structure

Current HTML:

```html
<header>

    <div>
        <img src="assets/images/profile.jpg" alt="Profile photo">
    </div>

    <div>
        <h2>Hello, I'm</h2>

        <h1>Dr. Robabeh Bashiri</h1>

        <p>
            Applying machine learning to solve real-world challenges
            in materials and energy.
        </p>

        <h3>Materials Scientist | Data Scientist</h3>

        <p>Python • Machine Learning • SQL</p>
    </div>

</header>
2. Background Image
background-image: url("../images/background.jpg");

Adds the hero background image.

3. Background Size
background-size: cover;

Makes the image cover the entire hero section.

4. Background Position
background-position: center;

Keeps the image centered.

5. Background Repeat
background-repeat: no-repeat;

Prevents the image from repeating.

6. Flexbox
display: flex;

Places the two <div> elements next to each other.

7. Vertical Alignment
align-items: center;

Centers the content vertically.

8. Horizontal Spacing
justify-content: space-between;

Creates space between the profile photo and the text.

9. Padding
padding: 0 8%;

Adds left and right spacing inside the hero section.

10. Image Size
header img{
    width:380px;
    height:auto;
}

Controls the size of the profile photo while keeping the correct proportions.

11. Text Styling

Learned how to style:

h2
h1
h3
p

using

font-size
font-weight
margin
line-height
Bug Fixed

Missing closing brace:

Incorrect:

header > div:last-child{
    width:55%;
    margin-right:8%;

header img{

Correct:

header > div:last-child{
    width:55%;
    margin-right:8%;
}

header img{

A missing } prevented the remaining CSS rules from being applied.