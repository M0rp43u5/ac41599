<!DOCTYPE html>
<html>
    <head>
        <meta charset="utf-8"/>
        <title>Page Title</title>
        <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@500&display=swap" rel="stylesheet">
            <link rel = "stylesheet" href = "styles.css">
    </head>
    <body>
        <div class = "container">
            <div class="nav-wrapper">
                <div class="left-side">
                    <div class="nav-link-wrapper active-nav-link">
                    <a href="index.html">Home</a>
                    </div>
                    <div class="nav-link-wrapper">
                    <a href= "about.html">About</a>
                    </div>
                </div>
                <div class="right-side">
                    <div class="brand">
                        <div>ARCHIT CHAWLA</div> 
                    </div>
                </div>
            </div>
            
        <div class="content-wrapper">
            <div class="portfolio-items-wrapper">
                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style = "background-image:url(images/codingpic1.jpg)">
                    </div>  
                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="images/logos/devcamp.png">
                        </div>
                        <div class="subtitle">
                        I enjoy coding, specifically topis such as Inheritance and Polymorphism.
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style = "background-image:url(images/booksinlibraryshelf.jpg)">
                    </div>  
                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="images/logos/dailysmarty.png">
                        </div>
                        <div class="subtitle">
                        I am majoring in CIS at Georgia State University.
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style = "background-image:url(images/kotlinpic1.jpg)">
                    </div>  
                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="images/logos/crondose.png">
                        </div>
                        <div class="subtitle">
                        I am currently learning the Kotlin programming language from LinkedIn Learning to help in Android app. development.
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style = "background-image:url(images/codingpic2.jpg)">
                    </div>  
                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="images/logos/shop-hacker.png">
                        </div>
                        <div class="subtitle">
                        I am planning to minor in CS, & to that end, I am taking Data Structures in the summer & Computer org. & Programming in the fall.
                        </div>
                    </div>
                </div>

                <div class="portfolio-item-wrapper">
                    <div class="portfolio-img-background" style = "background-image:url(images/cispic1.jpg)">
                    </div>  
                    <div class="img-text-wrapper">
                        <div class="logo-wrapper">
                            <img src="images/logos/devtrunk.png">
                        </div>
                        <div class="subtitle">
                        With my major in CIS in mind, I am proficient at programming in Java as well as in Microsoft Office, specifically Msft. Excel.
                        </div>
                    </div>
                </div>

                
    </body>
<script>
    /* This comes from JavaScript. It means to tell us to find all elements on the page that use this selector. */
    const portfolioItems = document.querySelectorAll('.portfolio-item-wrapper')

    portfolioItems.forEach(portfolioItem => {
        portfolioItem.addEventListener('mouseover', () => {
            /* We are now taking the HTML object of the div and the classes and using JavaScript to manipulate it. */
            console.log(portfolioItem.childNodes[1].classList);
            portfolioItem.childNodes[1].classList.add('img-darken');
        })
        portfolioItem.addEventListener('mouseout', () => {
            portfolioItem.childNodes[1].classList.remove('img-darken');
        })
    })
</script>
</html>
