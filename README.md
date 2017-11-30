# CSS Animations

### Transforms and Transitions

To add vendor prefixes, go to [Autoprefixer](http://autoprefixer.github.io/)

#### Popular Pseudo Classes
* hover: applies whenever you hover over a DOM element
```css
a:hover {
	...
}
```
* focus: applies whenever you select on a DOM element, persist as long as needed
```css
a:focus {
	...
}
```
* active: applies whenever you select on a DOM element, only persists through user interaction, i.e., when a button has been pressed down only, active state applies
```css
a:active {
	...
}
```

#### Popular Transforms
* translateX: moves a DOM element right or left
```css
button {
	transform: translateX(100px);
}
```
* translateY: moves a DOM elment up or down 
```css
button {
	transform: translateY(100px);
}
```
* scale: scales a DOM element
```css
button {
	transform: scale(1.5);
}
```
* transform-origin: sets where to transform a DOM element from
```css
button {
	transform-origin: left, right;
}
```
* rotate: rotates a DOM element
```css
div {
	transform: rotate(45deg);
}
```

#### Transitions
##### 4 transition properties:
* transition duration: duration of the transition
```css
div {
	transition-duration: 1s;
}
```
* transition property: specifies which css properties to transition
```css
div {
	transition-property: color, border-radius;
}
```
* transition-timing-function: controls aceleration of transition during the transition duration
```css
div {
	transition-timing-function: easeInSine;
}
```
Refer to [http://easings.net/](http://easings.net/) for more transition timing functions
* transition-delay: how long to delay before the transition starts
```css
div {
	transition-delay: 0.5s;
}
```

#### For performance reasons, only change the following CSS properties
* transform: translate
* transform: scale
* transform: rotate
* opacity


### Keyframes

Allows you to apply multi state animations

#### Defining Keyframes 
##### Keyframe Animation Properties
* animation-name: name of the keyframe animation to apply
* animation-duration: duration of the keyframe animation (i.e., 1s)
* animation-timing-function: animation function to apply for keyframe animation (i.e., ease-in) 
* animation-delay: the delay time for keyframe animation (i.e., 2s)
* animation-iteration-count: the number of times the keyframe animation should run (i.e., 2, 100, infinite)
* animation-direction: the direction to run the keyframe animations (i.e., forward, reverse, alternate)
* animation-fill-mode: if animation-delay is applied, it controls timing of different keyframe animations to apply of an element (i.e., none, forward, backward, both)
* animation-play-state: controls whether or not to run or pause the animation (i.e., paused, running)

[_**Quick Demo**_](https://codepen.io/npranto/pen/zPmVKm)
```css
	@keyframes rainbowtext {
		0% {
			color: red;
			font-size: 20px;
		}
		25% {
			color: orange;
		}
		50% {
			color: yellow;
			font-size: 40px;
		}
		75% {
			color: green;
		}
		100% {
			color: blue;
			font-size: 20px;
		}
	}
```

#### Applying keyframes
```css
	<!-- applying above keyframe to a <p> element -->
	p {
		animation-name: rainbowtext;
		animation-duration: 2s;
		animation-timing-function: ease-in;
		animation-delay: 0s;
		animation-iteration-count: infinite
	}
```



