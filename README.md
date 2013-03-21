MediaBrowser.ApiClient.Javascript
=================================

This library makes it very easy to harness the power of the Media Browser API from JavaScript.

This is available as a Nuget package:

[MediaBrowser.ApiClient.Javascript](https://www.nuget.org/packages/MediaBrowser.ApiClient.JavaScript/)

This library has a dependency on **jQuery**, which must be available prior to loading the script.

Usage is very simple:

```javascript
	var client = new MediaBrowser.ApiClient("http:", "localhost", 8096, "My app name");
	
	client.getAllUsers().done(function(users) {
	    
	    // Do something with the list of returned users
	
	});
```

All ajax methods return a deferred promise object.
