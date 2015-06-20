# WordPress_Code_Snippets
Useful Code Snippets for my Daily Workflow in WordPress
<h2>Print all Custom Fields Data / Imprimir toda la información de todos los Custom Fields</h2>
```
<?php printf( '<pre>%s</pre>', var_export( get_post_custom( get_the_ID() ), true ) ); ?>
```



<h2>Print the value of specific Custom Field / Imprimir el valor de un Custom Field en Especifico</h2>

```
<?php echo get_post_meta( get_the_ID(), 'my-field', true ); ?>
```