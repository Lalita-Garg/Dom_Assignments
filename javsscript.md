# Dom Manipulation Assignment

1. Webiste Name: [Dev To](https://dev.to/)

### Topics

    - Query Selctory, Inner HTML

### Sample Image

![Sample One](./Pic1.png)

### Tasks

        Target the Top description div and change the DEV Community to <Your_Name> and description to your passion

### Output

![Output](./Pic2.png)

## Solution 1

![Output](./solution1.PNG)

2. Website Name: [Apple](https://support.apple.com/en-in)

### Task

![Store](./Picture_3.png)

### Fetch all the product name and store in an array

### Output

['iPhone', 'Mac', 'iPad', 'Watch', 'AirPods', 'Music', 'TV']
***
## Solution 2

     - const list = document.querySelectorAll(".main .as-imagegrid .as-imagegrid--7up .row .as-imagegrid-item")

     const products = [];
     for (let element of list) {
     products.push(element.innerText);
     }
     const product = products.map(element => {
     return element.replace("\nSupport"," ");
     });
     product
     ['iPhone ', 'Mac ', 'iPad ', 'Watch ', 'AirPods ', 'Music ', 'TV ']
***
3. Webiste Name: [Youtube Support](https://support.google.com/youtube/)

### Topics

    - Get Element By Id, Create Element, Create Text Node, Append Child

### Sample Image

![Sample One](./Pic4.png)

### Tasks

     Add another FAQ 'My New FAQ' to the list

### Output

![Output](./Pic5.png)

---
***
## Solution3

     - const section = document.createElement("section")

       section.setAttribute("id","mySection")

       document.body.querySelector("#hcfe-content .primary-container .page-width-container
       .main-content .article .accordion-homepage").appendChild(section)

      const heading = document.createElement("h3")

      heading.innerHTML = "My New FAQ"

      document.getElementById('mySection').appendChild(heading)

      document.getElementById("mySection").style.borderTop = "1px solid #c9cbca";

      document.querySelector("#mySection").style.padding ="0px"
      '0px'

### SOlution 3 Image
 ![Solution3](./solution3.PNG)
***
---

4. Webiste Name: [OnePlus](https://www.oneplus.in/support)

### Topics

     Query Selector, InnerText

### Sample Image

![Sample One](./Pic6.png)

### Tasks

      Change the contact number

### Output

![Output](./Pic7.png)

---

## Solution4

     - document.querySelector("#footer
      .container-infinite .container-text .contact-us
      .one-tel-number").innerText = "+91 6366256689"
      '+91 6366256689'

### Solution Image ![Solution Image](./solution4.PNG)

---

5. Webiste Name: [Samsung](https://www.samsung.com/in/offer/online/samsung-fest/)

### Topics

       getElementById, createElement, InnerText, append, setAttribute

### Sample Image

![Sample One](./Pic8.png)

### Tasks

     Target the main div of card and change the Button text to Check out

### Output

![Output](./Pic9.png)
***
## Solution 5

     const cards =document.querySelectorAll("#smartphone-deals .listing .mytabs .diwali-deals-product-sale-pro .diwali-deals-product-sale-btn")

     for (let element of cards) {
          element.innerHTML = "Check Now";
     }
      'Check Now'

### Solution 5 image ![Solution 5 image](./solution5.PNG)
***
6. Webiste Name: [Adidas](https://www.adidas.co.in/)

### Topics

    -   Query Selector, Event listeners, Changing Styles

### Sample Image

![Sample One](./Pic10.png)

### Tasks

     Target the search box and on hover change thebackground color to red.

### Output

![Output](./Pic11.png)
***
## Soluton 6

     let searchBox = document.body.querySelector("#app .gl-app .content-wrapper___1xMQS .sheet___2Zvfp .header___3wNCY .header-desktop___158Zl .glass-header-bottom-desktop-white___2AUaf .right-side-menu___2ykzq .glass-search___X4QNv .searchinput-wrapper___3YrvF .searchinput___19uW0")

      searchBox.addEventListener('mouseover', function(){
        searchBox.style.backgroundColor="red";
      });

### Solution Image ![Solution 6 image](./solution6.PNG)
***
7. Webiste Name: [MDN Web Docs](https://developer.mozilla.org/en-US/)

### Topics

       Form, Value, Submit

### Sample Image

![Sample One](./Pic12.png)

### Tasks

     To Search a topic in the MDN Search bar.
     First add a text to search in the search bar and then hit the submit search button to search the docs using DOM

### Output

![Output](./Pic13.png)

---

## Solution 7

     let element = document.getElementById("hp-search-input")
     let btn = document.querySelector("#hp-search-form .search-button");
     element.value = "DOM"
     if (btn) {
     btn.click();
     }

---

8. Webiste Name: [Google](https://www.google.com/)

### Topics

       Remove Elements

### Sample Image

![Sample One](./Pic14.png)

### Tasks

     Remove alternate languages from the home page languages listed

### Output

![Output](./Pic15.png)

---

## Solution 8

     let list = document.querySelectorAll("#SIvCob a");
     for (let i = 0; i < list.length; i++) {
     if (i % 2 == 0) {
     list[i].remove();

}
}

### solution Image ![Solution 8 Image](./solution8.PNG)

---

9. Webiste Name: [Code Wars](https://www.codewars.com/)

### Topics

       Change Font Family, Color of Text.

### Sample Image

![Sample One](./Pic16.png)

### Tasks

    Change the font family of the text to monospace and text color to the logo’s background color.

### Output

![Output](./Pic17.png)

***
## Soluton 9

    let heading = document.querySelector(".content-width-extra-large .display-heading-1");

    heading.style.color = "firebrick";

    heading.style.fontFamily = "monospace";

### Solution 9 Image 
![Solution 9 image](./solution9.PNG)
***

10. Webiste Name: [Freecodecamp](https://www.freecodecamp.org/)

### Topics

       querySelector, mouseover, click eventListener,  callback function, style,

### Sample Image

![Sample One](./Pic18.png)

### Tasks

    Target the button and change background colour on mouseover

### Output

![Output](./Pic19.png)

***
## Soluton 10

    let element = document.querySelector(".btn-cta-big .login-btn-text");
    element.addEventListener("mouseover",(event) => {event.target.style.backgroundColor = "red"});

### Solution 10 Image 
![Solution 10 image](./solution10.PNG)
***

11. Webiste Name: [realme](https://www.realme.com/in/)

### Topics

       querySelector,style,background-image

### Sample Image

![Sample One](./Pic20.png)

### Tasks

    change the realme logo to ineuron logo

### Output

![Output](./Pic21.png)

***
## Soluton 11

    let element = document.querySelector(".logo .icon ");
    element.style.backgroundImage = "url('https://ineuron.ai/images/ineuron-logo.png')"

### Solution 11 Image 
![Solution 11 image](./solution11.PNG)
***

12. Webiste Name: [Github](https://github.com/)

### Topics

       querySelector,style,background-Color

### Sample Image

![Sample One](./Pic22.png)

### Tasks

     change the background colour of the button to blue.

### Output

![Output](./Pic23.png)

***
## Soluton 12

    let btn = document.querySelector(".col-xl-4 .btn");
    btn.style.backgroundColor = "blue"

### Solution 12 Image 
![Solution 12 image](./solution12.PNG)
***

13. Webiste Name: [Hackerrank](https://www.hackerrank.com/)

### Topics

       querySelector,innerHtml

### Sample Image

![Sample One](./Pic24.png)

### Tasks

Target the top description and change “Matching developers with great companies” to ‘JSBOOTCAMP“.

### Output

![Output](./Pic25.png)

***
## Soluton 13

      document.querySelector(".fl-heading .fl-heading-text").innerHTML = "JSBOOTCAMP";

### Solution 13 Image 
![Solution 13 image](./solution13.PNG)
***

14. Webiste Name: [Asus](https://www.asus.com/in/)

### Topics

      querySelector,style,font-size

### Sample Image

![Sample One](./Pic26.png)

### Tasks

       change the fontsize of “Hot Deals” to 80px

### Output

![Output](./Pic27.png)

***
## Soluton 14

     document.querySelector(".HotDealsAll__Heading__2fIbe").style.fontSize = "80px";

### Solution 14 Image 
![Solution 14 image](./solution14.PNG)
***

15. Webiste Name: [Dell](https://www.dell.com/en-in/shop/deals/laptop-deals?gacd=10415953-9016-5761040-285981356-0&dgc=ST&gclid=Cj0KCQjwguGYBhDRARIsAHgRm4-XUDMhhVNyHXb3s1gY4ZBzORr_d9Se-buhJwy7asyUe7YdqEA11eEaAt6UEALw_wcB&gclsrc=aw.ds&nclid=BxjBlpBQsX6pjSHh-L8YYSU77EpfXRkG1AGMB5Wbeu386ykspfrPDnfx_DdFau20)

### Topics

      querySelector,style.textAlign

### Sample Image

![Sample One](./Pic28.png)

### Tasks

       Convert the text “G15 Gaming Laptop” from left to right

### Output

![Output](./Pic29.png)

***
## Soluton 15

        document.querySelector("#d560824win9b .ps-top .ps-title").style.textAlign = "right";

### Solution 15 Image 
![Solution 15 image](./solution15.PNG)
***

16. Webiste Name: [Vercel](https://vercel.com/)

### Topics

     querySelector,innerHTMl

### Sample Image

![Sample One](./Pic30.png)

### Tasks

      change the heading “Start with the developer” to “Start with Scratch”

### Output

![Output](./Pic31.png)
***
## Soluton 16

     document.querySelector(".section-title_title__VEDfK").innerHTML  = "Start with Scratch";

### Solution 16 Image 
![Solution 16 image](./solution16.PNG)
***

17. Webiste Name: [Sony](https://www.sony.co.in/)

### Topics

    querySelector,innerHTMl

### Sample Image

![Sample One](./Pic33.png)

### Tasks

     change the button text To current Date.

### Output

![Output](./Pic32.png)
***
## Soluton 17

       let element = document.querySelector(".buy-button .button-and-link-wrapper");

       let today=new Date();

       element.innerHTML = today; 

### Solution 17 Image 
![Solution 17 image](./solution17.PNG)
***

18. Webiste Name: [Philips](https://www.philips.co.in/)

### Topics

     querySelector,style,backgroundcolor

### Sample Image

![Sample One](./Pic34.png)

### Tasks

    change the background colour blue to orange

### Output

![Output](./Pic35.png)

## Solution 18

        document.querySelector(".footerpage .p-footer-content .globalfooter .p-f03-footer-container").style.background= "#ffc233";

### Solution Image ![Solution 18 image](./solution18.PNG)

19. Webiste Name: [Canon](https://in.canon/)

### Topics

          querySelector,src

### Sample Image

![Sample One](./Pic36.png)

### Tasks

    extract the canon logo

### Output

![Output](./Pic37.png)

## Solution 19

     document.querySelector(".navbar-header .logo").src
    'https://in.canon/assets/brandlogo-300-002e45a4aec98fd92899838da9d5560f. png'

20. Webiste Name: [Oppo](https://www.oppo.com/in/)

### Topics

          querySelector,style,color

### Sample Image

![Sample One](./Pic38.png)

### Tasks

      Change the description colour black to orange

### Output

![Output](./Pic39.png)

---

## Solution 20

     let desc = document.querySelector(".wide .desc");
     desc.style.color = "Orange";

### Solution Image ![Solution 20 image](./solution20.PNG)

---
