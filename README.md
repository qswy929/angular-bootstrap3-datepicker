# angular-bootstrap3-datepicker
An [AngularJS](http://angularjs.org/) datetimepicker based on [benzen's bootstrap3-datetimepicker](https://github.com/benzen/angular-bootstrap3-datepicker)

## Installation

Installation is easy, jQuery, momentjs, font-awesome, AngularJS and Bootstrap's JS/CSS are required.
You can download ethan-angular-bootstrap3-datepicker via bower:
`bower install ng-bootstrap3-datepicker --save`

When you are done downloading all the dependencies and project files the only remaining part is to add dependencies as an AngularJS module:

```javascript
angular.module('myApp', ['ng-bs3-datepicker']);
```

You also need to include these files:
```html
<link rel="stylesheet" href="bootstrap/css/bootstrap.css" />
<link rel="stylesheet" href="font-awesome.css" />
<link rel="stylesheet" href="ng-bs3-datepicker.css" />


<script src="jquery.js"></script>
<script src="bootstrap/js/bootstrap.js"></script>
<script src="angular.js"></script>
<script src="moment.js"></script>
<script src="moment-your-locale.js"></script>
<script src="ng-bs3-datepicker.js" charset="utf-8"></script>
```

Make sure you use `charset="utf-8"` in your script tag if your browser (or those of your users) is displaying characters wrong when using another language.

## Settings

To use the directive, use the following code :

```html
<ng-bs3-datepicker ng-model="date" language="zh-cn" date-format="YYYY-MM" min-viewmode="months" max-date="moment().format()" min-date="moment({y: 2000})" pick-date="true" pick-time="false"/>
```

`datepicker` : Indicates you want a date picker

`ng-model` : Variable of the controller scope to store the date. The date is currently store as a string, formatted according to date format.

`language` : The locale you want to use for this date picker. To work, this require adding the corresponding momentjs locale file.

`date-format`: Format to use to format the date. The correct definition can be found [here](http://momentjs.com/docs/#/displaying/format/)

Optional properties are as follows:

`min-viewmode` : "minViewMode" of BootStrap datetimepicker.

`max-date` : "maxDate" of BootStrap datetimepicker.

`min-date` : "minDate" of BootStrap datetimepicker.

`pick-date` : "pickDate" of BootStrap datetimepicker.

`pick-time` : "pickTime" of BootStrap datetimepicker.


# Thanks to
 * benzen: https://github.com/benzen/angular-bootstrap3-datepicker
 * cletourneau: https://github.com/cletourneau
 * Eonasdan: https://github.com/Eonasdan/bootstrap-datetimepicker
