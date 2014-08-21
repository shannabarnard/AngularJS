AngularJS rating with CSS3 labels
=========

This snippet is based on [Angular Ratings](http://angular-ratings.thomporter.com) directive.

The additional code is the CSS3 labels and the clear button.


## Angular Ratings

A diretive to help out with rating systems on your Angular powered website.  This directive automatically notifies
the server of the rating change, you just have to tell it a few things and follow a pattern.


## Usage

HTML
```
<angular-ratings ng-model="user_rating" notify-url="notify.json" notify-id="id">
```

JavaScript
```
angular.module('myApp', ['ratings']).controller('testCtrl', function($scope){
	$scope.user_rating = 3;
	$scope.id = 1;

});
```

## Server Communication

The directive will use the "notify-url" and "notify-id" attributes, along with the user's chosen rating to send
a post request to the server.  It will look like this:

{notify-url}?id={notify-id}&rating=2


## Demo

To follow soon!
