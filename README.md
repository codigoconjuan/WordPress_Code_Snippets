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

<h2>Add Lightbox to normal WP Gallery / Agregar Lightbox a la galeria de WordPress</h2>
<p>En el archivo script.js</p>

```
              
        jQuery('.gallery a').each(function(){
                var captionText = $(this).closest('.gallery-item').find('.wp-caption-text').html();
                jQuery(this).attr({'data-lightbox':'slideshow', 'title': captionText});
        });
```