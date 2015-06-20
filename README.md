# WordPress_Code_Snippets
Useful Code Snippets for my Daily Workflow in WordPress
<h2>Print all Custom Fields Data / Imprimir toda la información de un Custom Field</h2>
```
<?php printf( '<pre>%s</pre>', var_export( get_post_custom( get_the_ID() ), true ) ); ?>
```