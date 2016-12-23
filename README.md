# angular-hex-luminance
### Angular filter to calculate lighter or darker hex colors

Easy way to make hex color lighter or darker using Angular filter. Takes a value between -1 and 1, where 0 - original color.

## How to use
js:
```js

$scope.color = '#FF69B4';

$scope.lighter = $filter('hexLuminance')($scope.color, 0.5) // #FF69B4 
$scope.darker = $filter('hexLuminance')($scope.color, -0.5) // #80355a

```
html:
```html
<p>{{ color | hexLuminance:0.5 }}</p>
```
