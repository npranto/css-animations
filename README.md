#CSS Animations

Transforms and Transitions

To add vendor prefixes, go to [Autoprefixer](http://autoprefixer.github.io/)


####Popular Pseudo Classes
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

####Popular Transforms
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
