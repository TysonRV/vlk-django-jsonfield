VLK JSONField
=============

A model JSONField with an integrated form.

Installation
------------

Just copy this project to any folder in your computer.

Usage
-----

### Model

To create your JSONField just use the same notation as an usual model field:

    jsonfield = VLKJSONField(null=True, default=lambda: {'field1': False, 'field2': 'abc'})

[You must use lambda when using a dict as default] (https://docs.djangoproject.com/en/dev/ref/models/fields/#default)

### Form

To use this field in a form just use the form field with the same name of your model field and the subname separated by `__`:

    jsonfield__field1 = forms.CharField()
    jsonfield__field2 = forms.IntegerField(required=False)

The right side is the usual of a form field.

Contributing
------------

Do the usual github fork and pull request dance.

License
-------

Released under the MIT license. Read LICENSE.md for more information.
