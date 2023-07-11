# [4.0.0]

In this version, the page manager introduces the use of the `laravel-nova-publishable` and `laravel-nova-translatable` libraries.

## Breaking Change

* Run migrations
* The Model Page now has automatic binding on the slug and automatically detects whether it should include unpublished pages or not based on the preview settings.
* You can set the parameter of the route defined in the `front_route_name` configuration with the `front_route_parameter` configuration (`page` by default).
* The fields `publication_date` and `end_publication_date` have been removed. Utilisez à la place les champs de la librairie `laravel-nova-publishable`
  * `publication_status`
  * `published_first_at`
  * `published_at`
  * `expired_at`
