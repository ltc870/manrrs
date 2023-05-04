# Ways to use CSS in your HTML.

## Inline CSS

<p>You can write your CSS inline with your HTML. It's the least preferred way because it can bloat your HTML file, making it easily unreadable. Only use this when you want to make very small changes to the styling of a particular element or if your HTML file isn't very very big (but normally your HTML file will get bigger as time go). Keep in mind, this form of CSS takes precedence over any other method of CSS you add. This is what it would look like:</p>

```html
<h1 style="color: red; text-align: center;">Inline CSS</h1>
<p style="color: blue;">
  Notice the style attributes, with your styling in double quotations. You end a
  style property with a ";" semicolon. Intellisense will show you where to put
  the semicolon if you forget.
</p>
```

## Internal CSS

<p>The next way to add CSS in your HTML is internally in you HTML file (don't confuse this with inline CSS). This is what it will look like:</p>

```html
<head>
  <meta charset="UTF-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="stylesheet" types="text/css" href="styles.css" />
  <style>
    h1 {
      color: red;
      background-color: #000000;
    }

    p {
      font-size: 25px;
    }

    a {
      font-weight: bold;
    }
  </style>
  <title>...</title>
</head>

<body>
  <h1>Talk About Internal CSS</h1>
  <p>
    Notice that the styling rules(the code within the style tag are called
    "rules") match up with the specific tags you're targeting. There's other
    ways you can target specific elements, but you can look those us. Go to
    <a href="https://www.w3schools.com">W3Schools</a> to find out.
  </p>
</body>
```

## Linking your External CSS file

<p>In your HTML file, you want to nest this link tag within the head tag of your HTML file. For example:</p>

```html
<head>
  <meta charset="UTF-8" />
  <meta http-equiv="X-UA-Compatible" content="IE=edge" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <link rel="stylesheet" types="text/css" href="styles.css" />
  <title>...</title>
</head>
```

<p style="font-weight: bold;">In the link tag, you have an href attribute. You will link your external CSS file within this property.</p>

<p>Then within the body tag, you'll add your HTML like normal:</p>

<p>You can name your css file index.css or styles.css (there' multiple conventions when naming your CSS files but when putting your styles in one style sheet, you'll either name them index.css or styles.css)</p>

```html
<body>
  <h1>Using External CSS</h1>
  <p>We're talking about linking your External CSS file.</p>
  <a href="https://www.w3schools.com">Click here to learn more on W3Schools.</a>
</body>
```

<p>Then your external css file will look like this:</p>

```css
h1 {
  font-family: Georgia, sans-serif;
}

p {
  font-size: 2rem;
  font-family: "Gill Sans Extrabold", sans-serif;
}

a {
  font-weight: bold;
}
```
