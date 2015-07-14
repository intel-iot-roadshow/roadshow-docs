{% include base.html %}
{% if include.os %}
_Don't know how? Refer to [Shell Access]({{ site.baseurl }}{{ base }}/docs/shell_access/{{include.os}}/serial_connection.html)._
{% else %}
_Don't know how? Refer to [Shell Access]({{ site.baseurl }}{{ base }}/docs/shell_access/)._
{% endif %}