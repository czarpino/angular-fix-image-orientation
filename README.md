# Angular Fix Image Orientation Directive

Fix image orientation by reading image exif data and applying appropriate CSS transformations. This is, however, just a **visual** fix.

## Usage

    <img img-fix-orientation="imageUrl" ng-src="{{ imageUrl }}">

> Note: Currently, only URL and data-url (i.e. `data:image/jpeg...`) image sources are accepted. Feel free to send PRs to support more image sources.

## Installation

You can install via Bower, downloading the source, or outright copy-pasting. For the latter 2, you'll also have to manually install [EXIF-JS](https://github.com/jseidelin/exif-js). The preferred way to install, however, is with Bower:

    bower install czarpino/angular-fix-image-orientation --save

Include js file in your HTML below AngularJS and EXIF-JS (yes, also include `exif.js`):

    <script src="path/to/exif-js/exif.js"></script>
    <script src="path/to/angular/angular.js"></script>
    <script src="path/to/angular-fix-image-orientation/angular-fix-image-orientation.js"></script>

And don't forget to include as module dependency:

    angular.module("appModule", ['cp.ng.fix-image-orientation']);

