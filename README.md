**nuget maintainer repo**

This repo tracks the upstream repo at https://github.com/aidanlister/jquery-stickytabs and adds nuget package info for https://www.nuget.org/packages/jquery.stickytabs/

Please only report packaging bugs and requests for new releases to this repo's issue tracker, for all functionality requests please use the upstream issue tracker instead.

Please don't report nuget package issues to upstream as they aren't planning on maintaining the nuget package (ref https://github.com/aidanlister/jquery-stickytabs/issues/2 )

jquery-stickytabs
=================

Provides pushState (back and forward button support) to Bootstrap tabs


Usage
=====

Run this in document ready or some equivalent initializer on your page:

    $('.nav-tabs').stickyTabs();

Where `nav-tabs` is the default class for the bootstrap tabs feature.

Options
=======

The following options are available to pass to jquery-stickytabs on instantiation

**Example**

````javascript
$(function() {
	var options = { 
		selectorAttribute: "data-target",
		backToTop: true
	};
	$('.nav-tabs').stickyTabs( options );
});
````

|option|default|description|
|------|-------|-----------|
| selectorAttribute | false | Override the default `href` attribute used as selector when you need to activate multiple TabPanels at once with a single Tab using the `data-target` attribute. |
| backToTop |false | Prevent the page from jumping down to the tab content by setting the backToTop setting to true. |

NuGet package
=============

Tim Abell maintains a [nuget package of stickytabs](https://www.nuget.org/packages/jquery.stickytabs/) for easier installation in .NET projects. Report any packaging issues here: https://github.com/timabell/jquery-stickytabs/issues
