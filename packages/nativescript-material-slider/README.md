[![npm](https://img.shields.io/npm/v/nativescript-material-slider.svg)](https://www.npmjs.com/package/nativescript-material-slider)
[![npm](https://img.shields.io/npm/dt/nativescript-material-slider.svg?label=npm%20downloads)](https://www.npmjs.com/package/nativescript-material-slider)
[![GitHub forks](https://img.shields.io/github/forks/Akylas/nativescript-material-components.svg)](https://github.com/Akylas/nativescript-material-components/network)
[![GitHub stars](https://img.shields.io/github/stars/Akylas/nativescript-material-components.svg)](https://github.com/Akylas/nativescript-material-components/stargazers)

## Installation

* `tns plugin add nativescript-material-slider`

Be sure to run a new build after adding plugins to avoid any issues.

---

##### [Material Design Spec](https://material.io/design/components/sliders.html)

### Usage


## Plain NativeScript

<span style="color:red">IMPORTANT: </span>_Make sure you include `xmlns:mds="nativescript-material-slider"` on the Page element_

### XML

```XML
<Page xmlns:mds="nativescript-material-slider">
    <StackLayout horizontalAlignment="center">
        <mds:Slider value="50" minValue="0" maxValue="100" />
   </StackLayout>
</Page>
```

### CSS

```CSS
mdcslider {
    ripple-color: blue;
    elevation: 4;
}
```

## NativeScript + Angular

```typescript
import { registerElement } from 'nativescript-angular/element-registry';
import { Slider } from 'nativescript-material-slider';
registerElement('MDSlider', () => Slider);
```

```html
<MDSlider value="50" minValue="0" maxValue="100"></MDSlider>
```

## NativeScript + Vue

```javascript
import Vue from 'nativescript-vue';
Vue.registerElement('MDSlider', () => require('nativescript-material-slider').Slider);
```

```html
<MDSlider value="50" minValue="0" maxValue="100"/>
```

## Attributes

Inherite from Nativescript [Activity Indicator](https://docs.nativescript.org/ui/ns-ui-widgets/slider) so it already has all the same attributes

## Attributes

* **elevation** _optional_

An attribute to set the elevation of the slider. This will increase the 'drop-shadow' of the slider.

* **rippleColor** _optional_

An attribute to set the ripple color of the slider.