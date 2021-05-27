## Make a page template

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
Add an introductory sentence. What will learners achieve by the end of this step?
</div>
<div>
Image, gif or video showing what they will achieve by the end of the step. ![](images/image.png){:width="300px"}
</div>
</div>

--- task ---

Open `template.html` in your editor and look at the code. Also, open the page in your web browser, or look at it in the preview.

Notice that the only tag in the `body` of the page right now is a `div` tag with the class `container`. This `div` tag is an invisible box. Next, you'll use CSS to add some style rules to it and make it visible.

--- /task ---

To add your CSS, you first need to add your stylesheet to `template.html`.

--- task ---

Add a link to `style.css` inside the `head` tag, like this:

```html
 <link rel="stylesheet" href="style.css">
```

--- /task ---

--- collapse ---
---
title: What about the stylesheet that's already there?
---
You may notice that there's already one stylesheet, called `company_style.css` linked to this page. This sheet contains some rules that you need to make the page look the way the company wants it, but which aren't what you're focusing on learning right now. You might have seen some of them before, and you'll learn others later. Pages can have lots of stylesheets, but you have to be careful that the rules don't contradict each other!

--- /collapse ---

The design the company wants is the content box over a coloured backgreound that you've probably seen on other websites. At its most basic, it looks like this.

![A webpage with a white box in the middle of a blue background.](images/content_box.png)

To start making this, use the CSS file you just linked to add some colour to the page.

--- task ---

In `style.css` add a rule that sets a background colour for the `body` tag, which will set that colour as the background for the whole page.

```css
body{
    background-color: lightblue;
}
```

If you don't like this colour, you can choose your own. You can find a list on [this page](https://www.w3schools.com/colors/colors_names.asp).

--- save ---

Look at how `template.html` has changed. Remember, you may need to refresh the page if you're viewing it in your browser.

--- /task ---

You still can't see the `container` div, but that's fine. You haven't given it any style rules yet, so it's still invisible. You'll fix that next.

--- task ---

In `style.css` add a rule that sets a background colour for the `container` class. Again, you can pick a different colour if you like. Also, add a rule that sets the width of the `div` so it has those coloured borders either side of it.

```css
.container{
    background-color: white;
    width: 1200px;
}
```

Type some text into the `container` `div` in `template.html`, like this:

```html
<div class="container">
    Hello!
</div>
```
--- save ---

Now refresh `template.html` in your browser and see what's happened.

--- /task ---

You should see something like this:

![A webpage with a white box in the middle of a blue background. The box contains the word 'Hello!'](images/filled_container.png)

Now that you have the content box the company wants, you'll need to add the sections you're going to use in the rest of the template, and in making the pages based on it. These will also be `div` tags.

--- task ---

First, delete the text you added to test the `div` in the last step. Then, create three new `div` tags inside of the `container` `div`. Each should have its own class. For now, you'll also type the name of the `div` into the `div`, so you can see it. A `div` tag with nothing in it is invisible!

  + Give the first `div` the `header` class.
  + Give the second `div` the `nav` (short for navigation) class.
  + Give the last `div` the `main` class.

The finished code should look like this:

```html
<div class="container">
    <div class="header">
        <!-- Page titles and the company logo go here -->
        Header
    </div>
    <div class="nav">
        <!-- The navigation menu goes here -->
        Nav
    </div>
    <div class="main">
        <!-- The main content of the page goes here -->
        Main
    </div>
</div>
```

--- save ---

--- /task ---
