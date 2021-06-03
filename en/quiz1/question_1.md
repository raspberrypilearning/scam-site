## Reflection

Well done, you have learned a lot! Now it's time to reflect — reflecting is an important part of learning because it helps make new connections in your brain.

Answer the three questions below to reflect on what you've learned.

After each question, press submit. You will be guided towards the correct answer. You can do this activity as many times as you want to.

Have fun!

--- question ---

---
legend: Question 1 of 3
---

Which of these is the correct code for linking from `index.html` to `product.html` in the site you have just built?

--- choices ---

- ( ) `<a>product.html</a>`

  --- feedback ---
  This will display a broken link, where the text of the link is "product.html". The URL for the target of a link needs to be in the `href` atribute of the tag, with the text of the link appearing between the opening and closing tags, like this:

  ```html
  <a href="https://raspberrypi.org"> the Raspberry Pi website </a>
  ```

  --- /feedback ---

- ( ) `<a href="https://oursite.com/product.html"> our product gallery </a>`

  --- feedback ---
  This is an absolute link, and will work if, and only if, the website exists at `oursite.com`. If it doesn't, or if the site moves to any other domain (e.g. `newsite.com`), then this link will break. There is a way to avoid this.
  --- /feedback ---

- (x) `<a href="product.html"> our product gallery </a>`

  --- feedback ---
  You're right! The relative link `product.html` will point from `index.html` to the product gallery as long as those two pages remain in the same directory, no matter where on the internet the website is located.
  --- /feedback ---

--- /choices ---

--- /question ---
