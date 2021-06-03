
--- question ---

---
legend: Question 3 of 3
---

In this project you've used two classes on the same element to apply CSS rules. If you had the following CSS and HTML, how would you expect the output to look in your browser?

```CSS
.dark_bg{
  background-color: black;
}

.alert_text{
  color: red;
}
```

```HTML
<div class="dark_bg alert_text">Important message!</div>
```

--- choices ---

- ( ) <div style="background-color: black">Important message!</div>


  --- feedback ---
    The background colour is correct, but the rules from `alert_text` aren't being applied.
  --- /feedback ---

- ( ) <div style="color: red">Important message!</div>


  --- feedback ---
  The text colour is correct, but the rules from `dark_bg` aren't being applied.
  --- /feedback ---

- (x) <div style="background-color: black; color: red">Important message!</div>


  --- feedback ---
  Correct! The two classes apply their rules, setting the background to black and making the text red.
  --- /feedback ---

- ( ) <div style="background-color: black; color: white">Important message!</div>


  --- feedback ---
  Two CSS rules are being applied here but, while the background is the right colour, the text isn't.
  --- /feedback ---

--- /choices ---

--- /question ---
