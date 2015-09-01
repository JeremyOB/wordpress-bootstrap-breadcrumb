# Bootstrap breadcrumb Wordpress plugin

> It's a plugin which display the website Bootstrap breadcrumb.

## Version
1.0

## Content

Bootstrap breadcrumb Wordpress plugin allow to :

* Automatic arborescence indexation (*Home > sub-page > sub-sub-page*)
* Custom post support
* Use icon to the home link

## Installation

This section describes how to install the plugin and get it working.

* Upload ```bootstrap-breadcrumb.php``` to the ```/wp-content/plugins/bootstrap-breadcrumb/``` directory.
* Activate the plugin through the *Plugins* menu in WordPress
* Place the next code in your page template :
```
<?php 
if( function_exists('bootstrap_breadcrumb') )
	bootstrap_breadcrumb();
?>
```

## Differents ways
### Custom home icon
```
<?php 
if( function_exists('bootstrap_breadcrumb') )
	bootstrap_breadcrumb('<i class="fa fa-home fa-lg"></i>');
?>
```

### Custom post support

```
<?php 
if( function_exists('bootstrap_breadcrumb') )
	bootstrap_breadcrumb( array( "custom_post_name" ) );
?>
```

### How to use in a template file

```
<?php if( function_exists('bootstrap_breadcrumb') ): ?>
	<section class="section-breadcrumb">
		<div class="container">
			<?php bootstrap_breadcrumb('<i class="fa fa-home fa-lg"></i>'); ?>
		</div>
	</section>
<?php endif; ?>
```
