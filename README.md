# spinning-balls
Page: https://hironsiuk.github.io/spinning-balls/

I just made this page to learn how to use @keyframes, but it ended up creating a nice effect so I'm saving it here.

That's also a good example to show to myself that transform should be used sometimes 
```css
/* Works as expected */
@keyframes spinning {
  0% {
    transform: rotate(0deg) translateX(100%);
    opacity: 1;
  }
  100% {
    transform: rotate(360deg) translateX(100%);
    opacity: 1;
  }
}
```
```css
/* Doesn't work, The ball will first move to the right, then spin infinitely on itself */
@keyframes spinning {
  0% {
    rotate: 0deg;
    translate: 100%;
    opacity: 1;
  }
  100% {
    rotate: 360deg;
    translate: 100%;
    opacity: 1;
  }
}
```
