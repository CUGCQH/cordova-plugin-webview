


To open a new webview, just call in your app's js:
```javascript
    webview.Show(URL);
```

Where `URL` is the path to the page to be opened. In Android, the plugin automatically adds the prefix `file:///android_asset/www/`
But only if no `*://` or `javascript:` is present at the front of the URL.

Then, to close the second webview and return to the main view, call in your second webview (the opened webview, not the main webview):
```javascript
    webview.Close();
```

This will close and destroy the second webview.

