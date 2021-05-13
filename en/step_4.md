## Make a header

Still working in `template.html` and `style.css`, it's time to start on making the header for the website. This will appear at the top of every page to remind people which site they're on. Creating this header will require two tags you've seen before: `h1` and `img`.

--- task ---

Add an image inside `header`. Use the `logo.png` file provided, or create your own if you like! Give it the class `logo` and the alt-text 'Our logo'.

```html
<img src="logo.png" alt="Our logo" class="logo">
```

--- /task ---

--- task ---

Below the image, add a level 1 heading inside `header` that reads 'Translucent Technologies: a vision of the future'. Give it the class `title`.

```html
<h1 class="title">Translucent Technologies: a vision of the future</h1>
```

Now check how it looks in your browser or preview.

--- /task ---

That's a little squashed together, and might look better if it had some colour. Time for CSS!

--- task ---

In `style.css`, create a style rule for the `title` class that gives the heading a nice colour.

```css
.title{
    color: deeppink;
}
```

--- /task ---

Now, to create a space between the logo and the heading, you need to tell one or the other to create that gap. To do this, you can set the `margin` on one of them. A future project will show you lots of ways to use `margin`, but for now just use the code below to create a gap to the right of the logo.

--- task ---

In `style.css`, create a style rule for the `logo` class that creates a gap to the right of the image.

```css
.logo{
    margin-right: 20px;
}
```

You can try different numbers of pixels, until you find one you like.

Now refresh the page in your browser and check out your improved site header!

--- /task ---

Of course, you could also try setting a different `background-color` property on the `header` div, but that's up to you!