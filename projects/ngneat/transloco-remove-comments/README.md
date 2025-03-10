# Translators Comments

> Help the translator with a description and meaning

There are times where we need to help the translator with a description and meaning. To translate a text message accurately, the translator may need additional information or context.

For each translation key that requires a description, we can add a companion key post-fixed with `.comment`, as shown in the example below:

```json
{
  "hello": "",
  "hello.comment": "Write a comment for the translator"
}
```

We don't want these keys to get into our final bundle, so we can remove them using the [optimize](https://netbasal.gitbook.io/transloco/plugins/transloco-optimize) library when building the production environment.

The library will take care of removing these keys from the translation files specified in the path.
