# README Cheat Sheet: CSS Animation Tricks

## Introduction
Welcome to the 20th day of our 100 Days of Web Development Challenge! Today, we're diving into the world of CSS animations to create exciting and dynamic web experiences.

### 1. Keyframes Magic
Define keyframes for smooth animations. Use percentages to control the animation progress.

```css
@keyframes slide-in {
  0% { opacity: 0; transform: translateX(-100%); }
  100% { opacity: 1; transform: translateX(0); }
}

.element {
  animation: slide-in 1s ease-in-out;
}
```

### 2. Infinite Looping
Keep the party going by looping your animations endlessly.

```css
@keyframes spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}

.element {
  animation: spin 2s infinite linear;
}
```

### 3. Bounce Effect
Add some bounce to your elements for a playful touch.

```css
@keyframes bounce {
  0%, 20%, 50%, 80%, 100% { transform: translateY(0); }
  40% { transform: translateY(-20px); }
  60% { transform: translateY(-10px); }
}

.element {
  animation: bounce 1s infinite ease-in-out;
}
```

### 4. Delayed Start
Control when your animations kick in for a more orchestrated effect.

```css
.element {
  animation: slide-in 1s ease-in-out 0.5s forwards;
}
```

## Example Project: Animated Landing Page

### HTML
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <link rel="stylesheet" href="styles.css">
  <title>Animated Landing Page</title>
</head>
<body>
  <div class="header">
    <h1 class="title">Welcome!</h1>
  </div>
  <div class="content">
    <p class="description">Explore the magic of CSS animations.</p>
    <a href="#" class="btn">Get Started</a>
  </div>
</body>
</html>
```

### CSS (styles.css)
```css
body {
  margin: 0;
  font-family: 'Arial', sans-serif;
  text-align: center;
}

.header {
  background-color: #3498db;
  padding: 20px;
  color: #fff;
}

.title {
  font-size: 2em;
  animation: slide-in 1s ease-in-out;
}

.content {
  padding: 40px;
}

.description {
  font-size: 1.5em;
  animation: bounce 1s infinite ease-in-out;
}

.btn {
  display: inline-block;
  padding: 10px 20px;
  margin-top: 20px;
  text-decoration: none;
  color: #fff;
  background-color: #e74c3c;
  border-radius: 5px;
  font-size: 1.2em;
  animation: pulse 1s infinite;
}

@keyframes pulse {
  0%, 100% { transform: scale(1); }
  50% { transform: scale(1.2); }
}
```

## Day 20 Challenge: CSS Animations
Celebrate the 20th day of our 100 Days of Web Development Challenge by mastering CSS animations! Create visually stunning web elements and enhance your web design skills, you'd need it for next week's projects.

## Reference Materials
Explore these resources to keep yourself engaged over the weekend:

- [YouTuber 1: CSSAnimationsMasters](#)
- [YouTuber 2: WebDesignWonders](#)
- [Tutor 1: CodeCraftingGenius](#)
- [Tutor 2: AnimationMagic101](#)

Happy coding! 🚀
