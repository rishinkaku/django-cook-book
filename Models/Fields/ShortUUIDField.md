# ShortUUIDField

## CharField

* Installation

  ```shell
  pip install shortuuid
  ```

* default=shortuuid.uuid

  ```python
  import shortuuid

  uid = models.CharField(_(u'uid'), max_length=255, default=shortuuid.uuid, help_text=u'User UUID', db_index=True)
  ```
  * Since Django 1.7, Core Django support Migrations
  * And above will be ``ValueError: Cannot serialize:``
  * Detail See [Migrations](../Databases/Migrations.md)

## UUIDField

_New In Django 1.8_

* https://docs.djangoproject.com/en/dev/ref/models/fields/#uuidfield

## ShortUUIDField

* Installation

  ```shell
  pip install django-shortuuidfield
  ```

* Usage

  ```python
  from shortuuidfield import ShortUUIDField

  uid = ShortUUIDField(_(u'uid'), max_length=255, help_text=u'User UUID', db_index=True)
  ```

## References

[1] skorokithakis@Github, [shortuuid — A generator library for concise, unambiguous and URL-safe UUIDs](https://github.com/stochastic-technologies/shortuuid)

[2] nebstrebor@Github, [django-shortuuidfield — Short UUID field for django](https://github.com/nebstrebor/django-shortuuidfield)