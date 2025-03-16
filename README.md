# GSAP Text Animation

A simple and elegant text animation demo using GSAP (GreenSock Animation Platform). This project demonstrates smooth letter-by-letter animations with blurring, scaling, and position effects.

## Demo

View the live demo: [GSAP Text Animation](https://gsap-text-animation-two.vercel.app/)


## How It Works

The animation uses GSAP's timeline to animate individual letters with these effects:
- Starting state: Letters are invisible, blurred, scaled up, and positioned below
- Animated state: Letters become visible, clear, properly sized, and correctly positioned
- Staggered timing: Each letter animates slightly after the previous one (30ms delay)

## Implementation

The project consists of a single HTML file that includes:
- HTML structure with each letter in its own span
- CSS for styling and initial letter states
- GSAP import from CDN
- JavaScript for the animation logic


## GSAP Animation Parameters

```javascript
tl.to(".letter", {
    opacity: 1,
    y: 0,
    scale: 1,
    filter: "blur(0px)",
    duration: 1.2,
    stagger: 0.03,
    ease: "expo.out"
});
```

- `duration`: Length of each letter's animation (in seconds)
- `stagger`: Delay between each letter starting its animation (in seconds)
- `ease`: The easing function (expo.out provides a smooth deceleration)

## License

MIT