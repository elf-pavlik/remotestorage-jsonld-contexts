# remoteStorage JSON-LD contexts

[@context](http://www.w3.org/TR/json-ld/#the-context) files for proper support of
[JSON-LD](http://json-ld.org) in
[remoteStorage](http://remotestorage.io)

## curent state of things


* http://slides.kip.pe/remotestorage-intro/#slide-81
* https://github.com/remotestorage/remotestorage.io/issues/68

## proposed design

### remotestorage.jsonld

context common for all data in remote storage

```js
{
  "@context": "http://remotestorage.io/spec/remotestorage.jsonld"
}
```

### per module context

contexts specific to each module

```js
{
  "@context": [
    "http://remotestorage.io/spec/remotestorage.jsonld",
    "http://remotestorage.io/spec/modules/bookmarks.jsonld"
  ]
}
```

* bookmarks
