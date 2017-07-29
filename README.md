# grav-html-migration
A set of commands for migrating any html templates to grav

```
/img src="([^"]*)"/g
```

```
img src="{{ url('theme://$1')}}"
```

```
<title>([^"]*)<\/title>
```

```
<title>{% if header.title %}{{ header.title|e('html') }} | {% endif %}{{ site.title|e('html') }}<\/title>
```

```
<script src="([^"]*)"><\/script>
```

```
{% do assets.addCss('theme://$1') %}
```
