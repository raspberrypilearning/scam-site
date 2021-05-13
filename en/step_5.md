## Make a menu
Now that you've got a beautiful header in place, it's time to add a menu so visitors to the website can find their way around. Menus are usually made by using unordered lists (`ul`) of hyperlinks (`a`) and adding some special CSS rules. So the first thing you'll need to do is make that list.

### Relative links
When making the menu you'll be linking to pages inside your own site. To do that, you'll have to use links that might be a little different to what you might have seen before. Links to other websites on the internet look like this:

```html
<a href="https://example.com/about.html">About us</a>
```

If your website isn't directly related to another one, you have to give the full URL (web address) like this — the `https://`, the domain name (example.com), etc. This is called an **absolute** link and is like giving the full street address of a house — anyone can use that information to find it. But links to other pages in your site don't include most of what's in the `href` attribute for an absolute link. If you were making the webiste that lives at `example.com` and you wanted to link to the about page, you'd make a link like this instead:

```html
<a href="about.html">About us</a>
```
This is called a **relative** link, because it is relative to where the link is starting from. A relative link is like giving someone directions to a house — 'take the second left, then the thrid right', or the like — the directions only work for someone starting from that spot. For files in the same directory as the one you're starting from, which all of the files in this project are, you only need to give their name. It's like pointing to a house on the same street and saying 'that one'! This is the same way you usually include images with the `src` attribute of the `img` element, or stylesheets with the `href` attribute of the `link` element. You can also use absolute URLs for images and stylesheets too, but you don't usually need to.

--- task ---

Create a list of hyperlinks to the pages your site will have: the home page (`index.html`) and the product gallery (`product.html`), inside the `nav` div. Give that `ul` the `menu` class.

```html
<ul class="menu">
    <li>
        <a href="index.html">Home</a>
    </li>
    <li>
        <a href="product.html">Our product</a>
    </li>
</ul>
```

Now refresh the page and check that your links work properly. If they don't, check that the files exist, and that you have spelt their names correctly.
--- /task ---

### Style your menu

Now you have a working list of links and, thanks to some code in `company_style.css` that will be covered in a later project, they're going across rather than down the page. 

[[Image of same]]

But they still look like hyperlinks in text, not the shiny menu the company wants on their website. So it's time for some more CSS!

--- task ---

In `style.css` create a `menu` class and use it to set a nice background colour and turn off the bullet points on the list.

```css
.menu{
    background-color: violet;
    list-style-type: none;
}
```

--- /task ---

Now you need to change the colour of the text on the links, and get rid of the underlines. You could create a class for the `a` tags, but there's another way to do this: you only want to change links that are inside the `menu` div. You can write a CSS rule that only effects them by writing a rule with a selector that only targets `a` tags that are **children** of an element with the `menu` class. An element's children are those tags that are between its opening and closing tags. That selector would look like this:

```css
.menu a{
    /** Rules go here **/
}
```

The space between them means 'child of'. There are a lot of ways to combine selectors, but this is one of the most useful.

--- task ---

Create a rule that targets hyperlinks in the menu and gives them a distinctive colour. Also, use the `text-decoration` property to turn off the underline.

```css
.menu a{
    color: white;
    text-decoration: none;
}
```
--- /task ---

--- save ---

--- task ---
Now refresh your page and look at your finished menu!
--- /task ---

[[Image of same]]

That's the template finished! Now you can move on to using it to create a website.