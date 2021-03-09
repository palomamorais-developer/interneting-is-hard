# <a href="https://www.internetingishard.com/">Interneting Is Hard</a>
<hr/>

🚀 **My journey** on web development through this *awesome* Web Development Tutorial focused on **HTML & CSS**, authored and maintained by *Oliver James*.
 
 ><a href="https://www.internetingishard.com/" target="_blank">*Interneting is Hard*</a> is a **100% free** and friendly web development tutorials, made to help transform complete beginners into talented Interneting professionals. 
 
## Nº 01 <a href="https://www.internetingishard.com/html-and-css/introduction/">Introduction</a>
✳ A short but solid concept about **web development**, which helped me understand how HTML, CSS and JS are connected. Now I am able to implement good practices to develop a website.😎

## Nº 02 <a href="https://www.internetingishard.com/html-and-css/basic-web-pages/">Basic Web Pages</a>

✳ This chapter introduced me to raw HTML structure (*that I'm  already totally familiar with it, but extra knowledge never hurts* 😊 ).
```html
<!DOCTYPE html>
<html>
    <head>
        <title>Basic Web Page</title>
    </head>
    <body>
        <h1>Basics of HTML</h1>
        <p>How use tags, create lists, 
        inline elements and more.</p>
    </body>
</html>

```
## Nº 03 <a href="https://www.internetingishard.com/html-and-css/links-and-images/">Links and Images</a>

1. ✅How create and manipulate links:
```html
<a href="https://www.internetingishard.com/">Interneting Is Hard</a>
```
2. 💡 Most common image formats:
```html
    <h2>JPGs</h2>
    <p>JPG images are good for photos.</p>
    <img src="images/mochi.jpg"/>

     <h2>GIFs</h2>
     <p>GIFs are good for animations.</p>
     <img src="images/mochi.gif"/>

     <h2>PNGs</h2>
     <p>PNGs are good for diagrams and icons.</p>
     <img src="images/mochi.png"/>

     <h2>SVGs</h2>
     <p>SVGs are <em>amazing</em>. Use them wherever you can.</p>
     <img src="images/mochi.svg"/>
```

## Nº 04 <a href="https://www.internetingishard.com/html-and-css/hello-css/">Hello,CSS</a>
✳ **Introduction to CSS** basics, styling headings and lists.( *Again, just learning some extras here.*)
>On my own, I went further and started playing with **pseudo-classes** (like: root) and also tried give some *minimalist* effect to links.😅


## Nº 05 <a href="https://www.internetingishard.com/html-and-css/css-box-model/">Box Model</a>
✳ In this chapter, i dove deep to box model concepts.
* ***Everything is a box.*** 📦
* Boxes can be **inline** or **block-level**.
* Boxes have content, **padding**, **borders**, and **margins**.
* They also have seemingly arbitrary rules about how they interact.


## Nº 06 <a href="https://www.internetingishard.com/html-and-css/css-selectors/">Selectors</a>
✅I  learned how to properly use **classes**, **pseudo-classes** and **ids** and implement in many ways. 


## Nº 07 <a href="https://www.internetingishard.com/html-and-css/floats/">Floats</a>
✅  Learned how deal with horizontal alignment and had fun creating a magazine layout. I released that ***floats are good but also limited***  😅. 


## Nº 08 <a href="https://www.internetingishard.com/html-and-css/flexbox/">Flexbox</a>
✳ Yay! Finally, Flexbox Chapter. One of the best tutorials I've ever seen on Internet, easy and very detailed. Now I feel confident to create layouts. ;) 

💡 **Quick Tips:** 
* Use `display: flex;` to create a flex container.
* Use `justify-content` to define the horizontal alignment of items.
* Use `align-items` to define the vertical alignment of items.
* Use `flex-direction` if you need columns instead of rows.
* Use the `row-reverse` or column-reverse values to flip item order.
* Use `order` to customize the order of individual elements.
* Use `align-self` to vertically align individual items.
* Use `flex` to create flexible boxes that can stretch and shrink.


## Nº 09 <a href="https://www.internetingishard.com/html-and-css/advanced-positioning/" >Advanced Positioning</a>
✳ Change a element without mess the layout is really powerfull. This chapter introduced me to **relative** ,**absolute**, ***relatively absolute*** and **fixed** and as exercise we made a drop-down menu(*not responsive yet!*) wrapping all this techniques learned.

💡 **Quick Tips:** 
* `position:relative` - tweak the position of an element without affecting its surrounding boxes.
* `position:absolute` - take elements out of the static flow of the page and place them relative to the browser window.

* `position:fixed` - let us make elements that don't scroll with the rest of the page.

* *Relatively Absolute* (`position:relative` on parent -> `position:absolute` on child) - allow us to hook back into the static flow of the page. 

## Nº 10 <a href="https://www.internetingishard.com/html-and-css/responsive-design/">Responsive Design</a>
✳During this chapter, I learned about *important* concepts of **responsive design**, such as:
* Difference between **fluid layouts** and **fixed-width layouts**.
* How use **media queries** to create layouts for mobile, tablet and desktop.
* How create a ***mobile first*** stylesheet.

>**Design pattern used:** <a href="https://developers.google.com/web/fundamentals/design-and-ux/responsive/patterns?hl=en#layout_shifter">Layout Shifter</a>

##  Nº 11 <a href="https://www.internetingishard.com/html-and-css/responsive-images/">Responsive Images</a>

✳ Making a image responsive is way more complicated than just making a responsive design,  but using the right methods, the results can be very good. 

💡 **Quick Tips:**

1. **Retina Optimization**:

    Using `srcset` to optimize for screen resolution.

  >💠 *Great for images **less than 600 pixels** wide because they aren’t big enough to benefit from the second scenario.* 
```html

        <img src='illustration-small.png'
             srcset='images/illustration-small.png 1x,
                     images/illustration-big.png 2x'
             style='max-width: 500px' />

```

2. **Screen Width Optimization**:

    Using `srcset` plus `sizes` to optimize for device width.

>💠 *This method gives a very important optimization for **larger images**, especially full-bleed photos.* 

```html

        <img src='images/photo-small.jpg'
             srcset='images/photo-big.jpg 2000w,
                     images/photo-small.jpg 1000w'
             sizes='(min-width: 960px) 960px, 100vw' />

```
3. **Art Direction** using `<picture>`:

    Using the `<picture>` element for manual control over which image file is displayed.
  >💠 *Think of art direction as **responsive image optimization for designers**.*
    


 ```html

        <picture>
            <source media='(min-width: 401px)'
                    srcset='images/photo-big.jpg'/>
            <source media='(max-width: 400px)'
                    srcset='images/photo-tall.jpg'/>
            <img src='images/photo-small.jpg'/>
        </picture>
           
 ```
## Nº 12 <a href="https://www.internetingishard.com/html-and-css/semantic-html/">Semantic HTML</a>

✳ “**Semantic HTML**” refers to the idea that all your *HTML markup* should convey the underlying meaning of your content—not its appearance.

💡 **Quick Tips:**

 ▪ `<article>` -> Represents an *independent article* in a web page.
    
   >👍  *It should only wrap content that can be plucked out of your page and distributed in a completely different context.*

 ▪ `<section>` -> This is sort of like an article, except it *doesn’t* need to make sense outside the context of the document.
 
  ▪  `<nav>` -> Lets you mark up the various navigation sections of your website.

   >👍  *This goes for the main site navigation, links to related pages in a sidebar, tables of content, and pretty much any group of links.* 
     
  ▪`<header>` -> It denotes introductory content for a section, article, or entire web page.

  >👍  *Not to be confused with headings (the `<h1>-<h6>` elements).*
  
 ▪ `<footer>` -> Conceptually, footers are basically the same as headers, except they generally come at end of an article/website opposed to the beginning.

 ▪ `<aside>` -> If the content looks different than the rest of the article, chances are it’s an *aside*.

## Nº 13 <a href="https://www.internetingishard.com/html-and-css/forms/">HTML Forms</a>
✳ Through this chapter, I learned about...
* ✅ best **CSS** and **HTML** practices for forms. 
* ✅ differences between **post** and **get** methods.
* ✅ how works forms elements(inputs, labels...).
* ✅ how create a **responsive form**. 


## Nº 14 <a href="https://www.internetingishard.com/html-and-css/web-typography/">Web Typography</a>
Where to find web fonts, hosting locally versus externally, dealing with multiple font faces, and basic typographic principles like text alignment, leading, and measure.

✳The goal of this chapter was twofold:
1. Learn the mechanics of **web fonts** and **basic CSS typography properties**.
2. Understand *how designers think about **typography***.


## 🏆 Tutorial Completed ✔ 
<hr/>







