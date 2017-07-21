# grav-html-migration
A set of commands for migrating any html templates to grav

```
/img src="([^"]*)"/g
```

```
img src="{{ url('theme://$1')}}"
```
