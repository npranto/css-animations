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


