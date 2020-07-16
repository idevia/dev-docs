# Guide for writing SCSS (and CSS) code

We almost always use SCSS (instead of CSS) in our projects, but some of these rules apply to general CSS too.

## Spacing

We expect you to have a space between the colon following the property name and the value. Also, there must at least be a new line between two code blocks. Now this may very well sound like nitpicking, but this will be important in improving the readability of the code you write.

```scss
  .card {
    .card__body {
      font-size: 15px;
      color: white;
    }
  }

  .navbar {
    background-color: turquoise;
    padding: 20px;
  }
```

## Class naming using BEM (Block, Element, Modifier) syntax

To be consistent with the CSS our team writes, we have decided to use the popular naming convention for classes in HTML and CSS. Look at the following code block:

```html
<div class="card card--border">
  <div class="card__body">
    <h2 class="card__body__title">This is a new card</h2>
  </div>
  <div class="card__footer">
    <p>This is the card footer</p>
  </div>
</div>
```

Here, **.card** is the block component, **.card__body, .card__body__title, .card__footer etc** are elements that depend upon the block element and **.card--border** is a modifier that changes the style of the block component. The SCSS (or CSS) you will write for this markup will look like this:

```scss
  .card {
    &--border {
      border: 2px solid crimson;
    }

    &__body {
      font-size: 15px;
      color: white;

      &__title {
        font-weight: bolder;
      }
    }
  }
```
_Note: **&** symbol here is SCSS specific, it just means the parent base class._

This may look like a lot of work, but with repeated practice, you'll get the hang of it (*cough* treat *cough*). For further reading, you can read [this](https://css-tricks.com/bem-101/) article.