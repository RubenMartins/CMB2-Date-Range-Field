# WDS CMB2 Date Range Field #
- **Contributors:**      WebDevStudios
- **Donate link:**       http://webdevstudios.com
- **Tags:**
- **Requires at least:** 3.6.0
- **Tested up to:**      3.6.0
- **Stable tag:**        0.1.0
- **License:**           GPLv2
- **License URI:**       http://www.gnu.org/licenses/gpl-2.0.html

## Description ##

Adds a date range field to CMB2

![CMB 2 Date Range Field Demo](https://cldup.com/bdK41R22yW.gif)

## Installation ##

### Manual Installation ###

1. Upload the entire `/wds-cmb2-date-range-field` directory to the `/wp-content/plugins/` directory.
2. Activate WDS CMB2 Date Range Field through the 'Plugins' menu in WordPress.

## Frequently Asked Questions ##

### How do I use the field? ###
Use the field type of `date_range` when initializing your CMB2 Field.

```
$prefix = '_yourprefix_';
$cmb_demo = new_cmb2_box( array(
 		'id'           => $prefix . 'metabox',
 		'title'        => __( 'Test Metabox', 'cmb2' ),
 		'object_types' => array( 'post', ), // Post type
 		'context'      => 'normal',
 		'priority'     => 'high',
 		'show_names'   => true,
 
 	) );
 
 	$cmb_demo->add_field( array(
 		'name'       => __( 'Test Date Range', 'cmb2' ),
 		'desc'       => __( 'field description (optional)', 'cmb2' ),
 		'id'         => $prefix . 'date_range',
 		'type'       => 'date_range',
 	) );
 ```

## Screenshots ##


## Changelog ##

### 0.1.0 ###
* First release
