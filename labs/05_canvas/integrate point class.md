In the integration in the lessons, you didn't make use of the `add()` method. Try to us it in the sketches, for instance, in this section:

```js
for (let i = 0; i != 20; i++) {
	draw.triangle( p1, p2, p3, `rgb(${r}, ${g}, ${b})`);
	p1.x -= 5;
	p1.y += 3;
	p2.x -= 6;
	p2.y += 3;
	p3.x -= 7;
	p3.y -= 1;
	r -= 1;
	g -= 2;
	b -= 3;
}
```