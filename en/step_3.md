## Make a page template

Now that you have the starter files, it's time to build a website that will convince people to buy our spectacular product! The first thing to do is make sure the different pages on the site look good to do this, you're going to create a template page without any real content — it will only have the things that will appear on every page, like the menu and the company logo. You will then copy this template and use it to create all the other pages on your site.

--- task ---

Open `template.html` in your editor and look at the code. Also, open the page in your web browser, or look at it in the preview.

--- /task ---

You'll notice that the only tag in the `body` of the page right now is a `div` tag with the class `container`. You'll also notice that you can't see it when you try to view the page. This is because the `div` tag is an invisible box. You'll use CSS to add some style rules to it and make it visible.

### Add CSS to your template
The first thing you'll need to do is add your stylesheet to your template. You may notice that there's already one stylesheet, called `company_style.css` linked to this page. This sheet contains some rules that you need to make the page look the way the company wants it, but which aren't what you're focusing on learning right now. You might have seen some of them before, and you'll learn others later. Pages can have lots of stylesheets, but you have to be careful that the rules don't contradict each other!

--- task ---

Add a link to `style.css` inside the `head` tag, like this:

```html
 <link rel="stylesheet" href="style.css">
```

--- /task ---

### Setup your content box

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

Look at how `template.html` has changed. Remember, you may need to refresh the page if you're viewing it in your browser.

--- /task ---

You still can't see the `container` div, but that's fine. You haven't given it any style rules yet, so it's still invisible. Time to fix that!

--- task ---

In `style.css` add a rule that sets a background colour for the `container` class. Again, you can pick a different colour if you like. Also, add a rule that sets the width of the `div` so it has those coloured borders either side of it.

```css
.container{
    background-color: white;
    width: 1200px;
}
```

Now refresh `template.html` in your browser and see what's happened.

--- /task ---

The `div` is still invisible! This is beacuse there's nothing in it. If a `div` has no elements with any width or height inside it, it will be invisible unless you give it both a `width` and `height` property with CSS rules. But to set an exact height, you would need to know how high everything that you will put into it will be, or the `div` will end beofre its contents, and that would look strange. Instead, if you don't set a height, the `div` will automatically grow to the correct height to contain whatever you put in it. Try that now: 

--- task ---

Type some text into the `container` `div` in `template.html`, like this:

```html
<div class="container">
    Hello!
</div>
```

Now refresh the page and you should see the text in a white box. That's the `div`!
--- /task ---

## Add sections to your template
Now that you have the content box the company wants, you'll need to add the sections you're going to use in the rest of the template, and in making the pages based on it. These will also be `div` tags.

--- task ---

First, delete the text you added to test the `div` in the last step.

Then, create three new `div` tags inside of the `container` `div`. Each should have its own class:

  + Give the first `div` the `header` class. It will contain your logo and page heading.
  + Give the second `div` the `nav` (short for navigation) class. It will contain the menu your visitors will use to get around the site.
  + Give the last `div` the `main` class. It's where the main content of the page will go. This is the part that will change from page to page.

The finished code should look like this:

```html
<div class="container">
    <div class="header">
    </div>
    <div class="nav">
    </div>
    <div class="main">
    </div>
</div>
```

--- /task ---

[[Save]]

Now you're ready to start filling in those sections!