These settings can be used to add ellipses **(...)** at the end of line when we want to show only particular number lines 

```css
.ellipses{
	display: -webkit-box;
	-webkit-line-clamp: 2;
	-webkit-box-orient: vertical;
	overflow: hidden;
	text-overflow: ellipsis;
}
```
