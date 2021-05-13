## Make a photo gallery 

Now you need to create a gallery of photographs to show off the product in action. Five photographs have been provided for you to use.

[[Gallery preview]]

--- task ---

Select all the code in `template.html` and copy it (Edit > Copy), then paste it into `product.html` (Edit > Paste).

--- /task ---

Once you've pasted the template, you need to add the photos.

--- task ---

Add five `img` tags inside the `main` div in `product.html`. Use the images:

  + `product_1.png`
  + `product_2.png`
  + `product_3.png`
  + `product_4.png`
  + `product_5.png`

```html
<div class="main">
    <img src="product_1.png">
    <img src="product_2.png">
    <img src="product_3.png">
    <img src="product_4.png">
    <img src="product_5.png">
</div>
```

--- /task ---

--- save ---

--- task ---

Open or preview `product.html`. Notice that the images don't really form a nice gallery, because they're different sizes and they don't evenly fill the container.

--- /task ---

[Messy gallery]

Of course, as you might expect by now, you can use CSS to fix all of this. The first step is creating a class to work with. You can't just use the `main` class, because it's used on every page and you need to create rules that only apply to this gallery page.

--- task ---

Add the `gallery` class to the `main` div in `product.html`, like so:

```html
<div class="main gallery">
```

One element can have lots of classes. The rules from each class get combined together.

--- /task ---

Now you can use the same sort of combined selector you used to select the links in the menu to select all the images in the gallery and make them the same size. Because `container` is 1200px wide, you're going to use 400px for your image width, so you'll fit three images across. You'll also need to add the `float: left` rule, which will push all the images to the left, so they fit in without gaps or moving on to new lines. Finally, it might be nice to make all the images the same height too. Though, if you are going to set both the width and the height of images, you need to make sure the values you pick are proportional to the original size of the image: if the original file is twice as high as it is wide, then you will need to set a height that's twice the width or it will end up looking wrong. If you only set either the width or the height of an image, the computer will figure out the other one to keep the image proportional. Of course, since these images are being given to you as a set, they've been checked to make sure they are proportional to the numbers you'll be using.

--- task ---

Add CSS to set the `width`, `height`, and `float` of all images in the gallery. Set the `width` and `height` to `400px`, and the `float` to `left`:

```css
.gallery img{
    width: 400px;
    height: 400px;
    float: left;
}
```

--- /task ---

--- save ---

Congratulations, you've completed the marketing website. You can show it off to your friends and family as an example of your website building skill, but don't let them think the product is actually real!