
--- question ---

---
legend: Question 2 of 3
---

If you had this webpage, which CSS selector would target only the image in the `pop_out` `div`?

```HTML
<img src="example.jpg" />

<div class="pop_out">
  <img src="extra.jpg" />
</div>
```
--- choices ---

- (x) `.pop_out img`

  --- feedback ---
  This is the right answer. This selector targets only `img` tags that appear inside the `div` with the `pop_out` class.
  --- /feedback ---

- ( ) `img .pop_out`

  --- feedback ---
  This selector is backwards. It's trying to select elements with the `pop_out` class that appear inside an `img` tag. As an `img` tag cannot have children, it will never work.
  --- /feedback ---

- ( ) `img`

  --- feedback ---
This selector will choose every image on the page. So while it will target the image in `pop_out`, it will also target the image outside it.
  --- /feedback ---

- ( ) `.pop_out`

  --- feedback ---
  This selector will target anything with the `.pop_out` class. Since the image you want to target is inside a `div` with that class, the rules will apply to the `img` tag. However, those rules will also apply to the `pop_out` `div` itself, and any other children it has.
  --- /feedback ---

--- /choices ---

--- /question ---
