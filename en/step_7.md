## Make a photo gallery 

<div style="display: flex; flex-wrap: wrap">
<div style="flex-basis: 200px; flex-grow: 1; margin-right: 15px;">
You're going to use your finished template to make a product gallery.
</div>

--- task ---

Select all the code in `template.html` and copy it (Edit > Copy), then paste it into `product.html` (Edit > Paste).

--- /task ---

--- task ---

Now add the photos. Add five `img` tags inside the `main` div in `product.html`. Use the images:

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

--- save ---

--- /task ---

--- task ---
**Test:** view `product.html`. Notice that the images are different sizes and don't evenly fill the container. 

[Messy gallery]

As you might expect by now, you can use CSS to fix all of this.
--- /task ---

--- task ---

You can't just use the `main` class for your gallery rules. The `main` class is used on every page and you need to create rules that only apply to this gallery page. Add the `gallery` class to the `main` div in `product.html`:

```html
<div class="main gallery">
```

One element can have lots of classes. The rules from each class get combined together.

--- /task ---

Now you can use a child selector — like you used to select the links in the menu — to select all the `img` tags in the gallery.

--- task ---

Set the `width` and `height` of all images in the gallery to `400px`, and the `float` to `left`:

```css
.gallery img{
    width: 400px;
    height: 400px;
    /* use float to push all 
    the images left, so they
    fit without gaps */
    float: left;
    
}
```

--- save ---

**Test:** view `product.html`. Admire your nice neat gallery.

--- /task ---

When you're setting both the width and height of an image like this, it may look a little wrong if you don't match the **aspect ratio** of the image to the measurements you use in your CSS.

<p style="border-left: solid; border-width:10px; border-color: #0faeb0; background-color: aliceblue; padding: 10px;">
<span style="color: #0faeb0">**Aspect ratio**</span> is the relationship between the width and height of an image. An image that is 200px wide and 100px high has an aspect ratio of 2:1. So does an image that is 500px wide and 250px high. When using CSS to set width and height on the same image you need to maintain this relationship, or the image will look stretched, or squashed. If you only set either the width or the height, the browser will choose the other one to keep the image proportional.
</p>