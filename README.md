# translate-press-title

<p>header.php + plugin ASF</p>

```php
<?php 
$current_language = get_locale();

if( $current_language == 'en_US' ){
  echo do_shortcode( '[trp_language language = "en_US"]' . the_field("тайтл_на_английском") . '[/trp_language]' . ' - ProtonGSM' );
}
if( $current_language == 'ru_RU' ){
  echo do_shortcode( '[trp_language language = "ru_RU"]' . the_title() . '[/trp_language]' . ' - ProtonGSM' );
}
?>
```
