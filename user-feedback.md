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