user: ryan
Opinion: user can select word in the navbar
Modification results：

.nav-container {
----original code----

    user-select:none   
}  
    **Prevent users from selecting the text in the navigation bar**
-------------------------------------------------------------------------------
user: ryan
opiniton: you should add link in image card in about page
Modification results：
        <div class="location-card">
            **<a href="https://en.wikipedia.org/wiki/Milford_Sound" target="_blank">**
                <div class="location-image milford-sound"></div> 
                    <div class="location-content">
                        <h3>Milford Sound</h3>       
                        <p class="location-region">Fiordland, South Island</p>
                        <p class="location-description">A stunning fjord surrounded by towering peaks, cascading waterfalls, and pristine rainforest. Known as the "eighth wonder of the world," this UNESCO World Heritage site exemplifies the raw beauty we must protect through Kaitiakitanga.</p>
                    </div>
            **</a>**
        </div>

**Add an <a> to the location-card container so that users can click the entire card to jump instead of clicking on a part of it.**

**The above code is just an example. There are five other codes that are not listed here, but they are modified in the same way.**
-----------------------------------------------------------------------------
user:eric
opition:  The navigation bar of the home and action pages is the same, but different from the about page, the text size will change when switching pages
Modification results：
about.css：
body{
    font-family: Arial, sans-serif; 
}
**Problem: about.css overwrites the default font in reset.css.**
---------------------------------------------------------------------------
user:ryan
opition: I think you could use a better looking font for your website
Modification results：

reset.css:
/* Import Oswald font family */
@font-face {
    font-family: 'Oswald';
    src: url('../font/static/Oswald-ExtraLight.ttf') format('truetype');
    font-weight: 200;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'Oswald';
    src: url('../font/static/Oswald-Light.ttf') format('truetype');
    font-weight: 300;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'Oswald';
    src: url('../font/static/Oswald-Regular.ttf') format('truetype');
    font-weight: 400;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'Oswald';
    src: url('../font/static/Oswald-Medium.ttf') format('truetype');
    font-weight: 500;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'Oswald';
    src: url('../font/static/Oswald-SemiBold.ttf') format('truetype');
    font-weight: 600;
    font-style: normal;
    font-display: swap;
}

@font-face {
    font-family: 'Oswald';
    src: url('../font/static/Oswald-Bold.ttf') format('truetype');
    font-weight: 700;
    font-style: normal;
    font-display: swap;
}
--------------------------------------------------------------------
user:eric
opition:i think your footer font is too small
Modification results:

.footer-section h3 {
    font-size: 2.2rem;
}
.footer-section h4 {
    font-size: 1.3rem;
}
.footer-section p {
    font-size: 1.4rem;
}
.footer-section ul li a {
    font-size: 1.4rem;
}
.footer-bottom p {
    font-size: 1.2rem;
}
-----------------------------------------------------------
user:eric
opition：The footer text is not centered on mobile devices
Modification results：

.footer-section p {
    text-align: center;
    margin: 0 auto;
}
------------------------------------------------------------