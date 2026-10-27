## 1. Aim

To create an attractive, auto-responsive photo gallery using HTML5, CSS3, and CSS Grid.

## 2. Objectives

- Collect and display at least eight images.
- Place each image inside a separate gallery item.
- Use `grid-template-columns: repeat(auto-fit, minmax(...))`.
- Apply `width: 100%` and `object-fit: cover` to images.
- Maintain consistent spacing using the `gap` property.
- Make the gallery responsive for desktop, tablet, and mobile devices.
- Test the gallery by changing the browser width.
- Capture desktop and mobile screenshots of the completed webpage.

## 3. Technologies Used

- HTML5
- CSS3
- CSS Grid
- Responsive Media Queries
- Unsplash Images
- Google Fonts

## 4. Project Structure

Create a folder named `assignment-8.2` with the following files:

```text
assignment-8.2/
├── index.html
└── style.css
```

## 5. Complete HTML Code

Create a file named `index.html` and paste the following code.

### index.html

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">

    <meta
        name="description"
        content="An auto-responsive photo gallery showcasing beautiful places and nature."
    >

    <title>FrameSpace | Photo Gallery</title>

    <link rel="preconnect" href="https://fonts.googleapis.com">
    <link rel="preconnect" href="https://fonts.gstatic.com" crossorigin>

    <link
        href="https://fonts.googleapis.com/css2?family=Poppins:wght@400;500;600;700;800&display=swap"
        rel="stylesheet"
    >

    <link rel="stylesheet" href="style.css">
</head>

<body>

    <!-- Header Section -->

    <header class="header">
        <div class="container navbar">

            <a href="#home" class="logo">
                <span class="logo-icon">F</span>
                FrameSpace
            </a>

            <nav aria-label="Main navigation">
                <ul class="nav-links">
                    <li><a href="#home">Home</a></li>
                    <li><a href="#gallery">Gallery</a></li>
                    <li><a href="#about">About</a></li>
                </ul>
            </nav>

            <a href="#gallery" class="header-button">
                Explore Photos ↗
            </a>

        </div>
    </header>

    <main id="home">

        <!-- Hero Section -->

        <section class="hero">
            <div class="container hero-content">

                <span class="eyebrow">A COLLECTION OF BEAUTIFUL MOMENTS</span>

                <h1>
                    Discover the Beauty
                    <span>of Our World.</span>
                </h1>

                <p>
                    Explore a collection of beautiful landscapes, peaceful
                    nature, amazing architecture, and unforgettable places
                    through photography.
                </p>

                <a href="#gallery" class="hero-button">
                    Explore the Gallery ↓
                </a>

            </div>
        </section>

        <!-- Gallery Section -->

        <section class="gallery-section" id="gallery">
            <div class="container">

                <div class="section-heading">
                    <div>
                        <span class="eyebrow">VISUAL INSPIRATION</span>
                        <h2>Our Photo Gallery</h2>
                        <p>
                            A little inspiration from around the world.
                        </p>
                    </div>

                    <span class="photo-count">12 Beautiful Photos</span>
                </div>

                <!-- Responsive CSS Grid -->

                <div class="gallery-grid">

                    <!-- Image 1 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1500530855697-b586d89ba3ee?auto=format&fit=crop&w=800&q=85"
                            alt="Beautiful green landscape under an open sky"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>01</span>
                            <div>
                                <h3>Open Landscapes</h3>
                                <p>Nature Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 2 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1470770841072-f978cf4d019e?auto=format&fit=crop&w=800&q=85"
                            alt="Mountain lake surrounded by green hills"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>02</span>
                            <div>
                                <h3>Mountain Escape</h3>
                                <p>Travel Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 3 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1441974231531-c6227db76b6e?auto=format&fit=crop&w=800&q=85"
                            alt="Sunlight passing through a green forest"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>03</span>
                            <div>
                                <h3>Forest Trails</h3>
                                <p>Nature Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 4 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1518837695005-2083093ee35b?auto=format&fit=crop&w=800&q=85"
                            alt="Blue ocean waves moving toward the shore"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>04</span>
                            <div>
                                <h3>Ocean Waves</h3>
                                <p>Coastal Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 5 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1501785888041-af3ef285b470?auto=format&fit=crop&w=800&q=85"
                            alt="Scenic mountain range and a peaceful lake"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>05</span>
                            <div>
                                <h3>Mountain Views</h3>
                                <p>Travel Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 6 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1470252649378-9c29740c9fa8?auto=format&fit=crop&w=800&q=85"
                            alt="Golden sunlight across a peaceful landscape"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>06</span>
                            <div>
                                <h3>Golden Sunrise</h3>
                                <p>Nature Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 7 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1464822759023-fed622ff2c3b?auto=format&fit=crop&w=800&q=85"
                            alt="Tall dramatic mountain peaks"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>07</span>
                            <div>
                                <h3>Mountain Peaks</h3>
                                <p>Adventure Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 8 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1507525428034-b723cf961d3e?auto=format&fit=crop&w=800&q=85"
                            alt="Beautiful tropical beach with blue water"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>08</span>
                            <div>
                                <h3>Tropical Beach</h3>
                                <p>Coastal Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 9 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1511497584788-876760111969?auto=format&fit=crop&w=800&q=85"
                            alt="Green trees and peaceful natural scenery"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>09</span>
                            <div>
                                <h3>Green Wilderness</h3>
                                <p>Nature Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 10 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1469474968028-56623f02e42e?auto=format&fit=crop&w=800&q=85"
                            alt="Sunlight illuminating a scenic mountain landscape"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>10</span>
                            <div>
                                <h3>Natural Wonders</h3>
                                <p>Travel Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 11 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1490750967868-88aa4486c946?auto=format&fit=crop&w=800&q=85"
                            alt="Colorful flowers in a beautiful garden"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>11</span>
                            <div>
                                <h3>Floral Dreams</h3>
                                <p>Garden Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                    <!-- Image 12 -->

                    <figure class="gallery-item">
                        <img
                            src="https://images.unsplash.com/photo-1519681393784-d120267933ba?auto=format&fit=crop&w=800&q=85"
                            alt="Mountain scenery beneath a starry night sky"
                            loading="lazy"
                        >
                        <figcaption>
                            <span>12</span>
                            <div>
                                <h3>Starry Night</h3>
                                <p>Night Sky Collection</p>
                            </div>
                        </figcaption>
                    </figure>

                </div>
            </div>
        </section>

        <!-- About Section -->

        <section class="about-section" id="about">
            <div class="container about-content">

                <div class="about-icon">✦</div>

                <div>
                    <h2>Every Picture Tells a Story</h2>
                    <p>
                        FrameSpace celebrates the beauty of the world
                        through photography. Discover new places,
                        appreciate little details, and find inspiration
                        in every frame.
                    </p>
                </div>

                <a href="#home" class="back-button">
                    Back to Top ↑
                </a>

            </div>
        </section>

    </main>

    <!-- Footer Section -->

    <footer class="footer">
        <div class="container footer-content">

            <a href="#home" class="footer-logo">
                FrameSpace
            </a>

            <p>
                &copy; 2026 FrameSpace. All rights reserved.
            </p>

            <a href="#gallery">Explore Gallery</a>

        </div>
    </footer>

</body>
</html>
```

## 6. Complete CSS Code

Create a file named `style.css` in the same folder and paste this code.

### style.css

```css
/* ===================================
   1. Global Styles
=================================== */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

html {
    scroll-behavior: smooth;
    scroll-padding-top: 100px;
}

body {
    font-family: "Poppins", sans-serif;
    color: #172554;
    background-color: #ffffff;
    line-height: 1.7;
}

a {
    text-decoration: none;
    color: inherit;
}

img {
    display: block;
    max-width: 100%;
}

.container {
    width: 90%;
    max-width: 1200px;
    margin: 0 auto;
}

/* ===================================
   2. Header and Navigation
=================================== */

.header {
    position: sticky;
    top: 0;
    z-index: 100;
    background-color: #ffffff;
    border-bottom: 1px solid #e5eaf2;
}

.navbar {
    min-height: 78px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 24px;
}

.logo {
    display: flex;
    align-items: center;
    gap: 10px;
    color: #172554;
    font-size: 23px;
    font-weight: 800;
    white-space: nowrap;
}

.logo-icon {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 40px;
    height: 40px;
    border-radius: 11px;
    background: linear-gradient(135deg, #4f46e5, #8b5cf6);
    color: #ffffff;
    font-size: 22px;
}

.nav-links {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 28px;
    list-style: none;
}

.nav-links a {
    color: #64748b;
    font-size: 14px;
    font-weight: 500;
    transition: color 0.3s ease;
}

.nav-links a:hover {
    color: #4f46e5;
}

.header-button {
    display: inline-block;
    padding: 11px 18px;
    border-radius: 9px;
    background-color: #4f46e5;
    color: #ffffff;
    font-size: 13px;
    font-weight: 600;
    white-space: nowrap;
    transition: background-color 0.3s ease;
}

.header-button:hover {
    background-color: #3730a3;
}

/* ===================================
   3. Hero Section
=================================== */

.hero {
    padding: 85px 0 80px;
    text-align: center;
    background:
        radial-gradient(
            circle at 50% 0%,
            #ede9fe 0,
            transparent 55%
        ),
        #f8faff;
}

.hero-content {
    max-width: 800px;
}

.eyebrow {
    display: inline-block;
    color: #4f46e5;
    font-size: 11px;
    font-weight: 700;
    letter-spacing: 1.8px;
}

.hero h1 {
    margin: 18px 0;
    font-size: clamp(36px, 5.5vw, 62px);
    font-weight: 800;
    line-height: 1.2;
    letter-spacing: -1.5px;
}

.hero h1 span {
    display: block;
    color: #4f46e5;
}

.hero p {
    max-width: 650px;
    margin: 0 auto 28px;
    color: #64748b;
    font-size: 15px;
    line-height: 1.9;
}

.hero-button {
    display: inline-block;
    padding: 13px 23px;
    border-radius: 9px;
    background-color: #4f46e5;
    color: #ffffff;
    font-size: 14px;
    font-weight: 600;
    transition: transform 0.3s ease,
                background-color 0.3s ease;
}

.hero-button:hover {
    background-color: #3730a3;
    transform: translateY(-2px);
}

/* ===================================
   4. Gallery Section
=================================== */

.gallery-section {
    padding: 75px 0 90px;
}

.section-heading {
    display: flex;
    justify-content: space-between;
    align-items: flex-end;
    flex-wrap: wrap;
    gap: 20px;
    margin-bottom: 35px;
}

.section-heading h2 {
    margin: 8px 0;
    font-size: clamp(27px, 4vw, 38px);
    line-height: 1.3;
    letter-spacing: -0.7px;
}

.section-heading p {
    color: #64748b;
    font-size: 14px;
}

.photo-count {
    padding: 9px 14px;
    border: 1px solid #e0e7ff;
    border-radius: 30px;
    background-color: #f5f3ff;
    color: #4f46e5;
    font-size: 12px;
    font-weight: 600;
    white-space: nowrap;
}

/* Main Responsive Grid */

.gallery-grid {
    display: grid;
    grid-template-columns: repeat(
        auto-fit,
        minmax(min(100%, 260px), 1fr)
    );
    gap: 24px;
    align-items: stretch;
}

/* Individual Gallery Items */

.gallery-item {
    min-width: 0;
    overflow: hidden;
    border: 1px solid #e8edf5;
    border-radius: 16px;
    background-color: #ffffff;
    box-shadow: 0 5px 20px rgba(15, 23, 42, 0.04);
    transition: transform 0.3s ease,
                box-shadow 0.3s ease;
}

.gallery-item:hover {
    transform: translateY(-5px);
    box-shadow: 0 15px 35px rgba(15, 23, 42, 0.12);
}

.gallery-item img {
    width: 100%;
    height: 230px;
    object-fit: cover;
    object-position: center;
    background-color: #e2e8f0;
    transition: transform 0.5s ease;
}

.gallery-item:hover img {
    transform: scale(1.04);
}

.gallery-item figcaption {
    display: flex;
    align-items: center;
    gap: 13px;
    padding: 17px;
}

.gallery-item figcaption > span {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-shrink: 0;
    width: 36px;
    height: 36px;
    border-radius: 10px;
    background-color: #eef2ff;
    color: #4f46e5;
    font-size: 12px;
    font-weight: 700;
}

.gallery-item figcaption h3 {
    font-size: 14px;
    font-weight: 600;
}

.gallery-item figcaption p {
    color: #94a3b8;
    font-size: 11px;
}

/* ===================================
   5. About Section
=================================== */

.about-section {
    padding: 55px 0;
    background-color: #f8faff;
    border-top: 1px solid #e8edf5;
    border-bottom: 1px solid #e8edf5;
}

.about-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 25px;
}

.about-icon {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-shrink: 0;
    width: 55px;
    height: 55px;
    border-radius: 15px;
    background-color: #ede9fe;
    color: #6d28d9;
    font-size: 28px;
}

.about-content > div:nth-child(2) {
    flex: 1;
    min-width: 0;
}

.about-content h2 {
    margin-bottom: 8px;
    font-size: 22px;
}

.about-content p {
    max-width: 700px;
    color: #64748b;
    font-size: 13px;
}

.back-button {
    flex-shrink: 0;
    padding: 11px 16px;
    border: 1px solid #dbe3f0;
    border-radius: 9px;
    background-color: #ffffff;
    color: #4f46e5;
    font-size: 12px;
    font-weight: 600;
}

/* ===================================
   6. Footer
=================================== */

.footer {
    padding: 25px 0;
    background-color: #172554;
    color: #cbd5e1;
}

.footer-content {
    display: flex;
    justify-content: space-between;
    align-items: center;
    flex-wrap: wrap;
    gap: 15px;
}

.footer-logo {
    color: #ffffff;
    font-size: 17px;
    font-weight: 700;
}

.footer-content p,
.footer-content > a:last-child {
    font-size: 12px;
}

.footer-content > a:last-child {
    color: #c4b5fd;
}

/* ===================================
   7. Tablet Responsive Design
=================================== */

@media (max-width: 850px) {
    .navbar {
        gap: 16px;
    }

    .nav-links {
        gap: 16px;
    }

    .gallery-grid {
        gap: 18px;
    }

    .gallery-item img {
        height: 210px;
    }

    .about-content {
        flex-wrap: wrap;
    }
}

/* ===================================
   8. Mobile Responsive Design
=================================== */

@media (max-width: 600px) {
    .container {
        width: 92%;
    }

    .navbar {
        justify-content: space-between;
        flex-wrap: wrap;
        padding: 14px 0;
        gap: 14px;
    }

    .logo {
        font-size: 20px;
    }

    .logo-icon {
        width: 35px;
        height: 35px;
        font-size: 19px;
    }

    .header-button {
        padding: 9px 12px;
        font-size: 11px;
    }

    .nav-links {
        order: 3;
        width: 100%;
        justify-content: center;
        gap: 12px 24px;
    }

    .nav-links a {
        font-size: 12px;
    }

    .hero {
        padding: 60px 0;
    }

    .hero h1 {
        font-size: clamp(34px, 9vw, 46px);
        letter-spacing: -1px;
    }

    .hero p {
        font-size: 13px;
    }

    .eyebrow {
        font-size: 10px;
        letter-spacing: 1.2px;
    }

    .gallery-section {
        padding: 55px 0 65px;
    }

    .section-heading {
        align-items: flex-start;
        flex-direction: column;
        gap: 14px;
        margin-bottom: 25px;
    }

    .gallery-grid {
        grid-template-columns: repeat(
            auto-fit,
            minmax(min(100%, 220px), 1fr)
        );
        gap: 16px;
    }

    .gallery-item img {
        height: 230px;
    }

    .about-content {
        align-items: flex-start;
        flex-direction: column;
        gap: 18px;
    }

    .about-content h2 {
        font-size: 20px;
    }

    .footer-content {
        flex-direction: column;
        align-items: center;
        text-align: center;
    }
}

/* ===================================
   9. Extra Small Screens
=================================== */

@media (max-width: 360px) {
    .logo {
        gap: 6px;
        font-size: 18px;
    }

    .header-button {
        padding: 8px;
        font-size: 10px;
    }

    .nav-links {
        gap: 10px 18px;
    }

    .hero h1 {
        font-size: 32px;
    }

    .gallery-grid {
        grid-template-columns: minmax(0, 1fr);
        gap: 18px;
    }

    .gallery-item img {
        height: 220px;
    }

    .gallery-item figcaption {
        padding: 14px;
    }

    .photo-count {
        font-size: 11px;
    }
}
```

## 7. Explanation of Important CSS Properties

| CSS Property | Purpose |
|---|---|
| `display: grid` | Creates a grid layout for gallery items. |
| `grid-template-columns` | Defines the columns of the gallery. |
| `repeat()` | Repeats the column definition automatically. |
| `auto-fit` | Fits as many columns as possible into the available space. |
| `minmax()` | Sets a minimum and maximum size for each column. |
| `width: 100%` | Makes each image fill the width of its container. |
| `object-fit: cover` | Fills the image area without distorting the image proportions. |
| `gap` | Adds consistent spacing between gallery items. |
| `flex-wrap: wrap` | Allows navigation and other Flexbox content to wrap when necessary. |
| `@media` | Adjusts the design for different screen widths. |

### Main Responsive Grid Code

```css
.gallery-grid {
    display: grid;
    grid-template-columns: repeat(
        auto-fit,
        minmax(min(100%, 260px), 1fr)
    );
    gap: 24px;
}
```

This code automatically adjusts the number of columns according to the available width. On a wide screen, several images appear in one row; on a narrow screen, fewer columns fit, and the images move to additional rows.

## 8. How to Run the Project

1. Open Visual Studio Code.
2. Create a folder named `assignment-8.2`.
3. Create `index.html` and `style.css` inside that folder.
4. Paste the complete HTML and CSS code into the respective files.
5. Save both files.
6. Right-click `index.html` and select **Open with Live Server**.
7. If Live Server is unavailable, open `index.html` directly in your browser.
8. Keep the internet connected so the external images and Google Fonts can load.

## 9. Responsive Testing

Test the gallery at these viewport widths:

- **1440px — Desktop:** Multiple columns should appear in each row.
- **768px — Tablet:** The number of columns should decrease automatically.
- **390px — Mobile:** The gallery should display fewer columns, with readable captions.
- **320px — Small mobile:** The gallery should use a single column without horizontal overflow.

### Browser Inspection Steps

1. Open the webpage in Google Chrome.
2. Right-click anywhere on the page and choose **Inspect**.
3. Open the **Elements** panel.
4. Select the element with the class `gallery-grid`.
5. Inspect the `display: grid` and `grid-template-columns` properties.
6. Click the **Toggle Device Toolbar** icon to simulate a mobile device.
7. Change the viewport width and observe how the columns adjust.

## 10. Desktop and Mobile Screenshots

The assignment requires screenshots of the completed gallery on desktop and mobile.

### Desktop Screenshot

1. Open the webpage in Chrome on your computer.
2. Maximize the browser window.
3. Make sure the gallery images have loaded.
4. Capture the webpage using `Windows + Shift + S`.
5. Save the screenshot as `desktop-screenshot.png`.

### Mobile Screenshot

1. Open Chrome DevTools using `F12`.
2. Click the **Toggle Device Toolbar** icon.
3. Select a mobile device or set the viewport width to approximately `390px`.
4. Refresh the page if needed and wait for the images to load.
5. Capture the page using `Windows + Shift + S`.
6. Save the screenshot as `mobile-screenshot.png`.

Place the screenshots in the project folder if they are required for submission.

Final project structure with screenshots:

```text
assignment-8.2/
├── index.html
├── style.css
├── desktop-screenshot.png
└── mobile-screenshot.png
```

## 11. Expected Output

The completed webpage contains:

- A navigation bar with the FrameSpace logo and links.
- A centered hero section with a heading and description.
- A responsive photo gallery containing 12 images.
- Captions for every gallery image.
- An About section describing the gallery.
- A footer with copyright information.
- A responsive layout that automatically adjusts columns according to screen width.

## 12. Result

Successfully created an auto-responsive image gallery using HTML5, CSS3, and CSS Grid. The gallery displays 12 images in individual gallery items, uses `repeat(auto-fit, minmax(...))` to adjust columns automatically, maintains consistent spacing with `gap`, and adapts to desktop, tablet, and mobile screen sizes.
