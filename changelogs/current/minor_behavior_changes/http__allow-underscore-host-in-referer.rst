The ``referer`` header is no longer removed when the host of an absolute URL contains an
underscore, such as ``https://a_b.example.com/``, which RFC 3986 allows and browsers send. This
behavioral change can be temporarily reverted by setting runtime guard
``envoy.reloadable_features.http_allow_underscore_host_in_referer`` to ``false``.
