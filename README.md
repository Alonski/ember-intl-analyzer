ember-intl-analyzer
==============================================================================

Find unused translations in your Ember.js projects


Usage
------------------------------------------------------------------------------

```bash
npx ember-intl-analyzer
```


Configuration
------------------------------------------------------------------------------

ember-intl-analyzer can be configured by creating a `config/ember-intl-analyzer.js`
file in your app:

```js
export default {
  whitelist: [
    /^countries\./,
    /^currency\./,
    /^validations\.errors\./,
    /^[^.]+\.warnings\.[^.]+$/,
  ],
};
```

The only configuration option at the moment is `whitelist`, which accepts an
array of regular expressions that will be checked when looking for unused
translations.


Related
------------------------------------------------------------------------------

- [ember-intl](https://github.com/ember-intl/ember-intl) – Internationalization
  addon for Ember.js


License
------------------------------------------------------------------------------

This projects is developed by and &copy; [simplabs GmbH](http://simplabs.com)
and contributors. It is released under the [MIT License](LICENSE.md).
