## Actions

### make\_add\_formats

```php
do_action( 'make_add_formats', $formatting );
```

Action: Fires at the end of the Formatting object's add\_formats method.

##### Description

This action gives a developer the opportunity to add or remove formats.

##### Parameters:

* **$formatting**: _(MAKE\_Formatting\_Manager)_ The Formatting object.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/formatting/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/formatting/manager.php#L218)

### make\_after\_builder\_menu

```php
do_action( 'make_after_builder_menu' );
```

Execute code after the builder menu items are displayed.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/templates/menu.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/menu.php#L42)

### make\_after\_builder\_stage

```php
do_action( 'make_after_builder_stage' );
```

Execute code after the builder stage is displayed.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/templates/stage-footer.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/stage-footer.php#L11)

### make\_api\_loaded

```php
do_action( 'make_api_loaded', $Make );
```

Action: Fire when the Make API has finished loading.

##### Parameters:

* **$Make**: _(MAKE\_API)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [functions.php](https://github.com/thethemefoundry/make/blob/master/src/functions.php#L40)

### make\_before\_builder\_menu

```php
do_action( 'make_before_builder_menu' );
```

Execute code before the builder menu items are displayed.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/templates/menu.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/menu.php#L18)

### make\_before\_builder\_stage

```php
do_action( 'make_before_builder_stage' );
```

Execute code before the builder stage is displayed.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/templates/stage-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/stage-header.php#L16)

### make\_before\_section\_header

```php
do_action( 'make_before_section_header' );
```

Execute code before the section header is displayed.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/templates/section-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/section-header.php#L59)

### make\_builder\_data\_saved

```php
do_action( 'make_builder_data_saved', $sections, $post_id );
```

Execute code after the section data is saved.

##### Description

While it is possible to use a &quot;save\_post&quot; to hook into the save routine, this action is preferred as it is only called after all validation and sanitization is completed.

##### Parameters:

* **$sections**: _(array)_ The clean section data.
* **$post\_id**: _(int)_ The post ID for the saved data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L196)

### make\_builder\_{$data\['section-type'\]}\_css

```php
do_action( 'make_builder_{$data['section-type']}_css', $data, $id, $style );
```

Allow section-specific CSS rules to be added to the document head of a Builder page.

##### Parameters:

* **$data**: _(array)_ The Builder section's data.
* **$id**: _(int)_ The ID of the Builder section.
* **$style**: _(MAKE\_Style\_ManagerInterface)_ The style manager instance.

##### Changelog:

* **Since**: 1.4.5
* **Since**: 1.7.0.

##### Source:

* [inc/builder/setup.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/setup.php#L147)

### make\_choices\_loaded

```php
do_action( 'make_choices_loaded', $choices );
```

Action: Fires at the end of the choices object's load method.

##### Description

This action gives a developer the opportunity to add or modify choice sets and run additional load routines.

##### Parameters:

* **$choices**: _(MAKE\_Choices\_Manager)_ The choices object that has just finished loading.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/choices/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/choices/manager.php#L74)

### make\_deprecated\_function\_run

```php
do_action( 'make_deprecated_function_run', $function, $version, $replacement, $message );
```

Fires when a deprecated function is called.

##### Parameters:

* **$function**: _(string)_ The function that was called.
* **$version**: _(string)_ The version of Make that deprecated the function.
* **$replacement**: _(string)_ The function that should have been called.
* **$message**: _(string)_ Explanatory text if there is no direct replacement available.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L284)

### make\_deprecated\_hook\_run

```php
do_action( 'make_deprecated_hook_run', $hook, $version, $message );
```

Fires when a deprecated hook has an attached function/method.

##### Parameters:

* **$hook**: _(string)_ The hook that was called.
* **$version**: _(string)_ The version of Make that deprecated the hook.
* **$message**: _(string)_ Optional. A message regarding the change. Default null.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L337)

### make\_doing\_it\_wrong\_run

```php
do_action( 'make_doing_it_wrong_run', $function, $message, $version );
```

Fires when the given function is being used incorrectly.

##### Parameters:

* **$function**: _(string)_ The function that was called.
* **$message**: _(string)_ A message explaining what has been done incorrectly.
* **$version**: _(string)_ The version of Make where the message was added.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L380)

### make\_font\_loaded

```php
do_action( 'make_font_loaded', $font );
```

Action: Fires at the end of the font object's load method.

##### Description

This action gives a developer the opportunity to add font sources and run additional load routines.

##### Parameters:

* **$font**: _(MAKE\_Font\_Manager)_ The font object that has just finished loading.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/font/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/manager.php#L79)

### make\_notice\_loaded

```php
do_action( 'make_notice_loaded', $notice );
```

Action: Fires at the end of the Admin Notice object's load method.

##### Description

This action gives a developer the opportunity to add additional admin notices and run additional load routines.

##### Parameters:

* **$notice**: _(MAKE\_Admin\_Notice)_ The notice object that has just finished loading.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/admin/notice.php](https://github.com/thethemefoundry/make/blob/master/src/inc/admin/notice.php#L108)

### make\_section\_text\_after\_column

```php
do_action( 'make_section_text_after_column', $ttfmake_section_data );
```

Execute code after an individual text column is displayed.

##### Parameters:

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L130)

### make\_section\_text\_after\_columns

```php
do_action( 'make_section_text_after_columns', $ttfmake_section_data );
```

Execute code after all columns are displayed.

##### Parameters:

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L193)

### make\_section\_text\_after\_columns\_select

```php
do_action( 'make_section_text_after_columns_select', $ttfmake_section_data );
```

Execute code after the columns select input is displayed.

##### Parameters:

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L31)

### make\_section\_text\_after\_title

```php
do_action( 'make_section_text_after_title', $ttfmake_section_data );
```

Execute code after the section title is displayed.

##### Parameters:

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L40)

### make\_section\_text\_before\_column

```php
do_action( 'make_section_text_before_column', $ttfmake_section_data );
```

Execute code before an individual text column is displayed.

##### Parameters:

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L108)

### make\_section\_text\_before\_columns\_select

```php
do_action( 'make_section_text_before_columns_select', $ttfmake_section_data );
```

Execute code before the columns select input is displayed.

##### Parameters:

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L22)

### make\_section\_{$ttfmake\_section\_data\['section'\]\['id'\]}\_after

```php
do_action( 'make_section_{$ttfmake_section_data['section']['id']}_after', $ttfmake_section_data );
```

Allow for script execution in the footer of a builder section.

##### Description

This action is a variable action that allows a developer to hook into specific section types (e.g., 'text'). Do not confuse &quot;id&quot; in this context as the individual section id (e.g., 14092814910).

##### Parameters:

* **$ttfmake\_section\_data**: _(array)_ The array of data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L774)

### make\_section\_{$ttfmake\_section\_data\['section'\]\['id'\]}\_before

```php
do_action( 'make_section_{$ttfmake_section_data['section']['id']}_before', $ttfmake_section_data );
```

Allow for script execution in the header of a builder section.

##### Description

This action is a variable action that allows a developer to hook into specific section types (e.g., 'text'). Do not confuse &quot;id&quot; in this context as the individual section id (e.g., 14092814910).

##### Parameters:

* **$ttfmake\_section\_data**: _(array)_ The array of data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L745)

### make\_settings\_thememod\_loaded

```php
do_action( 'make_settings_thememod_loaded', $settings );
```

Action: Fires at the end of the ThemeMod settings object's load method.

##### Description

This action gives a developer the opportunity to add or modify setting definitions and run additional load routines.

##### Parameters:

* **$settings**: _(MAKE\_Settings\_ThemeMod)_ The settings object that has just finished loading.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/settings/thememod.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/thememod.php#L120)

### make\_socialicons\_loaded

```php
do_action( 'make_socialicons_loaded', $socialicons );
```

Action: Fires at the end of the Social Icons object's load method.

##### Description

This action gives a developer the opportunity to add or modify icon definitions and run additional load routines.

##### Parameters:

* **$socialicons**: _(MAKE\_SocialIcons\_Manager)_ The settings object that has just finished loading.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L130)

### make\_style\_before\_file

```php
do_action( 'make_style_before_file', $style );
```

Action: Fires before the CSS rules are rendered and output as a file.

##### Parameters:

* **$style**: _(MAKE\_Style\_ManagerInterface)_ The style object.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L295)

### make\_style\_before\_inline

```php
do_action( 'make_style_before_inline', $style );
```

Action: Fires before the inline CSS rules are rendered and output.

##### Parameters:

* **$style**: _(MAKE\_Style\_ManagerInterface)_ The style object.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L234)

### make\_style\_before\_load

```php
do_action( 'make_style_before_load', $style );
```

Action: Fires before the Style class loads data files.

##### Description

This allows, for example, for filters to be added to thememod settings to change the values before the style definitions are loaded.

##### Parameters:

* **$style**: _(MAKE\_Style\_ManagerInterface)_ The style object.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L147)

### make\_style\_loaded

```php
do_action( 'make_style_loaded', $style );
```

Action: Fires at the end of the Styles object's load method.

##### Description

This action gives a developer the opportunity to add or modify dynamic styles and run additional load routines.

##### Parameters:

* **$style**: _(MAKE\_Style\_Manager)_ The style object

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L201)

### make\_view\_loaded

```php
do_action( 'make_view_loaded', $view );
```

Action: Fires at the end of the view object's load method.

##### Description

This action gives a developer the opportunity to add or modify views and run additional load routines.

##### Parameters:

* **$view**: _(MAKE\_Layout\_View)_ The view object that has just finished loading.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/layout/view.php](https://github.com/thethemefoundry/make/blob/master/src/inc/layout/view.php#L105)

### makeplus\_api\_loaded

```php
do_action( 'makeplus_api_loaded', $MakePlus );
```

Action: Fire when the Make Plus API has finished loading.

##### Parameters:

* **$MakePlus**: _(MAKEPLUS\_API)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* make-plus.php, line 77

### makeplus\_components\_loaded

```php
do_action( 'makeplus_components_loaded', $api );
```

Action: Fire when all components have been loaded.

##### Parameters:

* **$api**: _(MAKEPLUS\_APIInterface)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/api.php, line 320

### makeplus\_deprecated\_function\_run

```php
do_action( 'makeplus_deprecated_function_run', $function, $version, $replacement, $message );
```

Fires when a deprecated function is called.

##### Parameters:

* **$function**: _(string)_ The function that was called.
* **$version**: _(string)_ The version of Make that deprecated the function.
* **$replacement**: _(string)_ The function that should have been called.
* **$message**: _(string)_ Explanatory text if there is no direct replacement available.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L195)

### makeplus\_deprecated\_hook\_run

```php
do_action( 'makeplus_deprecated_hook_run', $hook, $version, $message );
```

Fires when a deprecated hook has an attached function/method.

##### Parameters:

* **$hook**: _(string)_ The hook that was called.
* **$version**: _(string)_ The version of Make that deprecated the hook.
* **$message**: _(string)_ Optional. A message regarding the change. Default null.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L255)

### makeplus\_doing\_it\_wrong\_run

```php
do_action( 'makeplus_doing_it_wrong_run', $function, $message, $version );
```

Fires when the given function is being used incorrectly.

##### Parameters:

* **$function**: _(string)_ The function that was called.
* **$message**: _(string)_ A message explaining what has been done incorrectly.
* **$version**: _(string)_ The version of Make where the message was added.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L304)

### makeplus\_notice\_loaded

```php
do_action( 'makeplus_notice_loaded', $notice );
```

Action: Fires at the end of the Admin Notice object's load method.

##### Description

This action gives a developer the opportunity to add additional admin notices and run additional load routines.

##### Parameters:

* **$notice**: _(MAKEPLUS\_Admin\_Notice)_ The notice object that has just finished loading.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/admin/notice.php](https://github.com/thethemefoundry/make/blob/master/src/inc/admin/notice.php#L119)

### makeplus\_perpage\_render\_metabox\_{$current\_view}

```php
do_action( 'makeplus_perpage_render_metabox_{$current_view}', $metabox );
```

Action: Fires before the default metabox callback for the current view is called.

##### Description

This allows for a custom metabox callback to be used in place of the default one. The provided $metabox object has methods for rendering the standard controls used for the layout settings. If this action has an action hooked to it, the default callback will not be used.

##### Parameters:

* **$metabox**: _(MAKEPLUS\_Component\_PerPage\_Metabox)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/perpage/metabox.php, line 167

## Filters

### make\_add\_font\_source\_{$source\_id}

```php
apply_filters( 'make_add_font_source_{$source_id}', $add_source );
```

Filter: Prevent a font source from being added.

##### Returns:

* **$add\_source**: _(bool)_ True to allow the font source to be added.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/font/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/manager.php#L116)

### make\_add\_integration\_{$integration\_name}

```php
apply_filters( 'make_add_integration_{$integration_name}', $add_integration );
```

Filter: Prevent an integration from being added.

##### Returns:

* **$add\_integration**: _(bool)_ True to allow the integration to be added.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/integration/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/integration/manager.php#L59)

### make\_add\_section

```php
apply_filters( 'make_add_section', $section );
```

Allow the added sections to be filtered.

##### Description

This filters allows for dynamically altering sections as they get added. This can help enforce policies for sections by sanitizing the registered values.

##### Returns:

* **$section**: _(array)_ The section being added.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/api.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/api.php#L96)

### make\_banner\_slide\_configuration

```php
apply_filters( 'make_banner_slide_configuration', $inputs );
```

Filter the definitions of the Banner slide configuration inputs.

##### Returns:

* **$inputs**: _(array)_ The input definition array.

##### Changelog:

* **Since**: 1.4.0.

##### Source:

* [inc/builder/sections/builder-templates/banner-slide.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/banner-slide.php#L70)

### make\_builder\_banner\_class

```php
apply_filters( 'make_builder_banner_class', $banner_class, $ttfmake_section_data );
```

Filter the class for the banner section.

##### Returns:

* **$banner\_class**: _(string)_ The banner class.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L462)

### make\_builder\_banner\_slide\_class

```php
apply_filters( 'make_builder_banner_slide_class', $slide_class );
```

Allow developers to alter the class for the banner slide.

##### Returns:

* **$slide\_class**: _(string)_ The banner classes.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L587)

### make\_builder\_banner\_slide\_style

```php
apply_filters( 'make_builder_banner_slide_style', $slide_style, $slide, $ttfmake_section_data );
```

Allow developers to change the CSS for a Banner section.

##### Returns:

* **$slide\_style**: _(string)_ The CSS for the banner.

##### Other parameters:

* **$slide**: _(array)_ The slide data.
* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L624)

### make\_builder\_get\_banner\_array

```php
apply_filters( 'make_builder_get_banner_array', $banner_array, $ttfmake_section_data );
```

Filter the data array for a banner section.

##### Returns:

* **$banner\_array**: _(array)_ The ordered banner data.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ All of the data for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L428)

### make\_builder\_get\_banner\_slider\_atts

```php
apply_filters( 'make_builder_get_banner_slider_atts', $data_attributes, $ttfmake_section_data );
```

Allow for altering the banner slider attributes.

##### Returns:

* **$data\_attributes**: _(string)_ The data attributes in string form.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L561)

### make\_builder\_get\_gallery\_array

```php
apply_filters( 'make_builder_get_gallery_array', $gallery_array, $ttfmake_section_data );
```

Filter the gallery item data.

##### Returns:

* **$gallery\_array**: _(array)_ The array of gallery item data.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L68)

### make\_builder\_get\_gallery\_item\_class

```php
apply_filters( 'make_builder_get_gallery_item_class', $gallery_class, $item, $ttfmake_section_data, $i );
```

Filter the class used for a gallery item.

##### Returns:

* **$gallery\_class**: _(string)_ The computed gallery class.

##### Other parameters:

* **$item**: _(array)_ The item's data.
* **$ttfmake\_section\_data**: _(array)_ The section data.
* **$i**: _(int)_ The current gallery item number.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L217)

### make\_builder\_get\_gallery\_item\_image

```php
apply_filters( 'make_builder_get_gallery_item_image', $image, $item, $aspect );
```

Alter the generated gallery image.

##### Returns:

* **$image**: _(string)_ The image HTML.

##### Other parameters:

* **$item**: _(array)_ The item's data.
* **$aspect**: _(string)_ The aspect ratio for the section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L260)

### make\_builder\_get\_gallery\_style

```php
apply_filters( 'make_builder_get_gallery_style', $gallery_style, $ttfmake_section_data );
```

Filter the style added to a gallery section.

##### Returns:

* **$gallery\_style**: _(string)_ The style applied to the gallery.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L171)

### make\_builder\_get\_text\_array

```php
apply_filters( 'make_builder_get_text_array', $columns_array, $ttfmake_section_data );
```

Filter the array of builder data for the text section.

##### Returns:

* **$columns\_array**: _(array)_ The ordered data for the text section.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ The raw section data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L308)

### make\_builder\_get\_text\_class

```php
apply_filters( 'make_builder_get_text_class', $text_class, $ttfmake_section_data, $sections );
```

Filter the text section class.

##### Returns:

* **$text\_class**: _(string)_ The computed class string.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ The section data.
* **$sections**: _(array)_ The list of sections.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L350)

### make\_builder\_is\_default

```php
apply_filters( 'make_builder_is_default', $is_default );
```

Filter: Modify whether new pages default to the Builder template.

##### Returns:

* **$is\_default**: _(bool)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L363)

### make\_builder\_is\_section\_type

```php
apply_filters( 'make_builder_is_section_type', $is_section_type, $type, $data );
```

Allow developers to alter if a set of data is a specified section type.

##### Returns:

* **$is\_section\_type**: _(bool)_ Whether or not the data represents a specific section.

##### Other parameters:

* **$type**: _(string)_ The section type to check.
* **$data**: _(array)_ The section data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L27)

### make\_builder\_js\_dependencies

```php
apply_filters( 'make_builder_js_dependencies', $dependencies );
```

Filter the dependencies for the Make builder JS.

##### Returns:

* **$dependencies**: _(array)_ The list of dependencies.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L305)

### make\_builder\_js\_templates

```php
apply_filters( 'make_builder_js_templates', $templates );
```

Array of items to print as JS templates in the footer of the Builder screen.

##### Description

Each item is represented as an associative array and includes the following items:  id                  The ID of the template builder\_template    The relative path to the PHP template path                The path to the base directory 

##### Returns:

* **$templates**: _(array)_ The

##### Changelog:

* **Since**: 1.6.0.

##### Source:

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L719)

### make\_builder\_section\_links

```php
apply_filters( 'make_builder_section_links', $links );
```

Filter the definitions for the buttons that appear in each Builder section's header.

##### Returns:

* **$links**: _(array)_ The button definition array.

##### Changelog:

* **Since**: 1.4.0.

##### Source:

* [inc/builder/core/templates/section-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/section-header.php#L46)

### make\_column\_buttons

```php
apply_filters( 'make_column_buttons', $column_buttons, $ttfmake_section_data );
```

Filter the buttons added to a text column.

##### Returns:

* **$column\_buttons**: _(array)_ The current list of buttons.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ All data for the section.

##### Changelog:

* **Since**: 1.4.0.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L81)

### make\_column\_configuration

```php
apply_filters( 'make_column_configuration', $inputs );
```

Filter the definitions of the Columns section's column configuration inputs.

##### Returns:

* **$inputs**: _(array)_ The input definition array.

##### Changelog:

* **Since**: 1.4.0.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L148)

### make\_compatibility\_mode

```php
apply_filters( 'make_compatibility_mode', $mode );
```

Filter: Set the mode for compatibility.

##### Description

 'full' will load all the files to enable back compatibility with deprecated code. (Default) 'current' will not load any deprecated code. Use with caution! Could result in a fatal PHP error. A minor release value, such as '1.5', will load files necessary for back compatibility with version 1.5.x. Note that there are no separate modes for releases prior to 1.5.  Example: If a site was originally customized with a child theme and Make 1.6.x, setting the mode to 1.6 will load files necessary to enable compatibility with changes made in 1.7.x, but will skip files for 1.5 and 1.6.

##### Returns:

* **$mode**: _(string)_ The compatibility mode to run the theme in.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L168)

### make\_configuration\_overlay\_input

```php
apply_filters( 'make_configuration_overlay_input', $this_output, $args, $section_data );
```

Filter the HTML for the input.

##### Returns:

* **$this\_output**: _(string)_ The HTML for the input.

##### Other parameters:

* **$args**: _(string)_ The input data.
* **$section\_data**: _(string)_ The data for the section.

##### Changelog:

* **Since**: 1.4.0.

##### Source:

* [inc/builder/core/configuration-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/configuration-helpers.php#L200)

### make\_configuration\_overlay\_input\_wrap

```php
apply_filters( 'make_configuration_overlay_input_wrap', $wrapper, $args, $section_data );
```

Filter the wrapped used for the inputs.

##### Returns:

* **$wrapper**: _(string)_ The HTML to wrap around the input.

##### Other parameters:

* **$args**: _(string)_ The input data that is wrapped.
* **$section\_data**: _(string)_ The data for the section.

##### Changelog:

* **Since**: 1.4.0.

##### Source:

* [inc/builder/core/configuration-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/configuration-helpers.php#L189)

### make\_content\_width

```php
apply_filters( 'make_content_width', $new_width, $left, $right );
```

Filter to modify the $content\_width variable.

##### Returns:

* **$new\_width**: _(int)_ The new content width.

##### Other parameters:

* **$left**: _(bool)_ True if the current view has a left sidebar.
* **$right**: _(bool)_ True if the current view has a right sidebar.

##### Changelog:

* **Since**: 1.4.8

##### Source:

* [inc/setup/misc.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/misc.php#L195)

### make\_css\_add

```php
apply_filters( 'make_css_add', $data );
```

Filter: Modify CSS rules as they are registered.

##### Returns:

* **$data**: _(array)_ The selectors and properties to add to the CSS.

##### Changelog:

* **Since**: 1.2.3

##### Source:

* [inc/style/css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/css.php#L104)

### make\_css\_parse\_declarations

```php
apply_filters( 'make_css_parse_declarations', $output, $declarations, $tab );
```

Filter: Modify the full list of parsed declarations.

##### Returns:

* **$output**: _(string)_ The full CSS output.

##### Other parameters:

* **$declarations**: _(array)_ The list of CSS declarations.
* **$tab**: _(string)_ The tab character.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/style/css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/css.php#L283)

### make\_customizer\_key\_conversions

```php
apply_filters( 'make_customizer_key_conversions', $conversions );
```

Filter the array of Customizer option key conversions.

##### Description

The keys for some Customizer options have changed between versions. This array defines each change as $new\_key =&gt; $old key.

##### Returns:

* **$conversions**: _(array)_ The array of key conversions.

##### Changelog:

* **Since**: 1.3.0.

##### Source:

* [inc/compatibility/keyconverter.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/keyconverter.php#L104)

### make\_customizer\_panels

```php
apply_filters( 'make_customizer_panels', $panels );
```

Filter: Modify the array of panel definitions for the Customizer.

##### Returns:

* **$panels**: _(array)_ The array of panel definitions.

##### Changelog:

* **Since**: 1.3.0.

##### Source:

* [inc/customizer/controls.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/controls.php#L280)

### make\_customizer\_sections

```php
apply_filters( 'make_customizer_sections', $sections );
```

Filter: Modify the array of section/control definitions for the Customizer.

##### Returns:

* **$sections**: _(array)_ The array of section definitions.

##### Changelog:

* **Since**: 1.3.0.

##### Source:

* [inc/customizer/controls.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/controls.php#L355)

### make\_enqueue\_parent\_stylesheet

```php
apply_filters( 'make_enqueue_parent_stylesheet', $enqueue );
```

Filter: Toggle whether the parent stylesheet loads along with the child one.

##### Returns:

* **$enqueue**: _(bool)_ True enqueues the parent stylesheet.

##### Changelog:

* **Since**: 1.6.0.

##### Source:

* [inc/setup/scripts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/scripts.php#L283)

### make\_error\_backtrace\_limit

```php
apply_filters( 'make_error_backtrace_limit', $limit );
```

Filter: Change the number of steps shown in a Make Error backtrace.

##### Returns:

* **$limit**: _(int)_ The number of backtrace steps to show.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/error/collector.php](https://github.com/thethemefoundry/make/blob/master/src/inc/error/collector.php#L159)

### make\_exif\_aperture

```php
apply_filters( 'make_exif_aperture', $f_stop, $raw_aperture, $attachment_id );
```

Filter the aperture value.

##### Returns:

* **$f\_stop**: _(string)_ The aperture value.

##### Other parameters:

* **$raw\_aperture**: _(int)_ The raw aperture value.
* **$attachment\_id**: _(int)_ The ID of the attachment.

##### Changelog:

* **Since**: 1.2.3.
* **Since**: 1.7.0.

##### Source:

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L367)

### make\_exif\_shutter\_speed

```php
apply_filters( 'make_exif_shutter_speed', $converted_as, $raw_shutter_speed, $attachment_id );
```

Filter the shutter speed value.

##### Returns:

* **$converted\_as**: _(string)_ The shutter speed value.

##### Other parameters:

* **$raw\_shutter\_speed**: _(float)_ The raw shutter speed value.
* **$attachment\_id**: _(int)_ The ID of the attachment.

##### Changelog:

* **Since**: 1.2.3.
* **Since**: 1.7.0.

##### Source:

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L346)

### make\_fitvids\_custom\_selectors

```php
apply_filters( 'make_fitvids_custom_selectors', $selector_array );
```

Filter: Allow customization of the selectors that are used to apply FitVids.

##### Returns:

* **$selector\_array**: _(array)_ The selectors used by FitVids.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/setup/scripts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/scripts.php#L647)

### make\_font\_data\_{$this->id}

```php
apply_filters( 'make_font_data_{$this->id}', $font_data );
```

Filter: Modify the font data from a particular source.

##### Returns:

* **$font\_data**: _(array)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/font/source/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/base.php#L149)

### make\_font\_google\_stack

```php
apply_filters( 'make_font_google_stack', $stack, $category );
```

Filter: Modify the CSS font stack for a particular category of Google font.

##### Returns:

* **$stack**: _(string)_ The CSS font stack.

##### Other parameters:

* **$category**: _(string)_ The font category.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/font/source/google.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/google.php#L217)

### make\_font\_google\_variants

```php
apply_filters( 'make_font_google_variants', $variants, $font );
```

Allow developers to alter the Google font variant choice.

##### Returns:

* **$variants**: _(array)_ The variants for the font.

##### Other parameters:

* **$font**: _(string)_ The font to load variants for.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/font/source/google.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/google.php#L371)

### make\_font\_relative\_size

```php
apply_filters( 'make_font_relative_size', $sizes );
```

Filter the array of relative font sizes.

##### Description

Each array item defines a percentage by which to scale a font size compared to some other font size. Most of these were deprecated in version 1.3.0.

##### Returns:

* **$sizes**: _(array)_ The array of relative sizes.

##### Changelog:

* **Since**: 1.0.0.

##### Source:

* [inc/style/datahelper.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/datahelper.php#L211)

### make\_font\_stack

```php
apply_filters( 'make_font_stack', $stack, $font );
```

Allow developers to filter the full font stack.

##### Returns:

* **$stack**: _(string)_ The font stack.

##### Other parameters:

* **$font**: _(string)_ The font.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/font/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/manager.php#L295)

### make\_footer\_1

```php
apply_filters( 'make_footer_1', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Returns:

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [sidebar-footer-1.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-1.php#L13)

### make\_footer\_2

```php
apply_filters( 'make_footer_2', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Returns:

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [sidebar-footer-2.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-2.php#L13)

### make\_footer\_3

```php
apply_filters( 'make_footer_3', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Returns:

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [sidebar-footer-3.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-3.php#L13)

### make\_footer\_4

```php
apply_filters( 'make_footer_4', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Returns:

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [sidebar-footer-4.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-4.php#L13)

### make\_gallery\_class

```php
apply_filters( 'make_gallery_class', $gallery_class, $ttfmake_section_data, $sections );
```

Filter the class applied to a gallery.

##### Returns:

* **$gallery\_class**: _(string)_ The class applied to the gallery.

##### Other parameters:

* **$ttfmake\_section\_data**: _(array)_ The section data.
* **$sections**: _(array)_ The list of sections.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L125)

### make\_gallery\_item\_configuration

```php
apply_filters( 'make_gallery_item_configuration', $inputs );
```

Filter the definitions of the Gallery item configuration inputs.

##### Returns:

* **$inputs**: _(array)_ The input definition array.

##### Changelog:

* **Since**: 1.4.0.

##### Source:

* [inc/builder/sections/builder-templates/gallery-item.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/gallery-item.php#L68)

### make\_generate\_post\_content

```php
apply_filters( 'make_generate_post_content', $post_content, $data );
```

Filter the generated post content.

##### Description

This content is the full HTML version of the content that will be saved as &quot;post\_content&quot;.

##### Returns:

* **$post\_content**: _(string)_ The fully generated post content.

##### Other parameters:

* **$data**: _(array)_ The data used to generate the content.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L385)

### make\_get\_exif\_data

```php
apply_filters( 'make_get_exif_data', $output, $attachment_id );
```

Alter the exif data output.

##### Returns:

* **$output**: _(string)_ The EXIF data prepared as HTML.

##### Other parameters:

* **$attachment\_id**: _(int)_ The image being generated.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L439)

### make\_get\_google\_font\_uri

```php
apply_filters( 'make_get_google_font_uri', $url );
```

Filter the Google Fonts URL.

##### Returns:

* **$url**: _(string)_ The URL to retrieve the Google Fonts.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/font/source/google.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/google.php#L267)

### make\_get\_image

```php
apply_filters( 'make_get_image', $return, $image_id, $size );
```

Filter the image HTML.

##### Returns:

* **$return**: _(string)_ The image HTML.

##### Other parameters:

* **$image\_id**: _(int)_ The ID for the image.
* **$size**: _(bool)_ The requested image size.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L919)

### make\_get\_image\_src

```php
apply_filters( 'make_get_image_src', $src, $image_id, $size );
```

Filter the image source attributes.

##### Returns:

* **$src**: _(string)_ The image source attributes.

##### Other parameters:

* **$image\_id**: _(int)_ The ID for the image.
* **$size**: _(bool)_ The requested image size.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L964)

### make\_get\_next\_section\_data

```php
apply_filters( 'make_get_next_section_data', $next_data, $current_section, $sections );
```

Allow developers to alter the "next" section data.

##### Returns:

* **$next\_data**: _(array)_ The data for the next section.

##### Other parameters:

* **$current\_section**: _(array)_ The data for the current section.
* **$sections**: _(array)_ The list of all sections.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L518)

### make\_get\_placeholder\_image

```php
apply_filters( 'make_get_placeholder_image', $return, $image_id, $ttfmake_placeholder_images );
```

Filter the image source attributes.

##### Returns:

* **$return**: _(string)_ The image source attributes.

##### Other parameters:

* **$image\_id**: _(int)_ The ID for the image.
* **$ttfmake\_placeholder\_images**: _(bool)_ The list of placeholder images.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L996)

### make\_get\_prev\_section\_data

```php
apply_filters( 'make_get_prev_section_data', $prev_section, $current_section, $sections );
```

Allow developers to alter the "next" section data.

##### Returns:

* **$prev\_section**: _(array)_ The data for the next section.

##### Other parameters:

* **$current\_section**: _(array)_ The data for the current section.
* **$sections**: _(array)_ The list of all sections.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L550)

### make\_get\_section\_data

```php
apply_filters( 'make_get_section_data', $ordered_data, $post_id );
```

Filter the section data for a post.

##### Returns:

* **$ordered\_data**: _(array)_ The array of section data.

##### Other parameters:

* **$post\_id**: _(int)_ The post ID for the retrieved data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/setup.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/setup.php#L260)

### make\_get\_section\_default

```php
apply_filters( 'make_get_section_default', $value, $key, $section_type );
```

Filter the default section data that is received.

##### Returns:

* **$value**: _(mixed)_ The section value.

##### Other parameters:

* **$key**: _(string)_ The key to get data for.
* **$section\_type**: _(string)_ The type of section the data is for.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L831)

### make\_get\_section\_name

```php
apply_filters( 'make_get_section_name', $name, $data, $is_js_template );
```

Alter section name.

##### Returns:

* **$name**: _(string)_ The name of the section.

##### Other parameters:

* **$data**: _(array)_ The section data.
* **$is\_js\_template**: _(bool)_ Whether or not this is in the context of a JS template.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L880)

### make\_get\_wp\_editor\_id

```php
apply_filters( 'make_get_wp_editor_id', $id, $data, $is_js_template );
```

Alter the wp\_editor ID.

##### Returns:

* **$id**: _(string)_ The ID for the editor.

##### Other parameters:

* **$data**: _(array)_ The section data.
* **$is\_js\_template**: _(bool)_ Whether or not this is in the context of a JS template.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L848)

### make\_has\_sidebar

```php
apply_filters( 'make_has_sidebar', $has_sidebar, $location, $view );
```

Filter: Dynamically change the result of the "has sidebar" check.

##### Returns:

* **$has\_sidebar**: _(bool)_ Whether or not to show the sidebar.

##### Other parameters:

* **$location**: _(string)_ The location of the sidebar being evaluated.
* **$view**: _(string)_ The view name.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/setup/widgets.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/widgets.php#L236)

### make\_insert\_post\_data\_sections

```php
apply_filters( 'make_insert_post_data_sections', $data );
```

Filter the section data.

##### Returns:

* **$data**: _(array)_ The sanitized data.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L308)

### make\_is\_builder\_page

```php
apply_filters( 'make_is_builder_page', $is_builder_page, $post_id );
```

Allow a developer to dynamically change whether the post uses the builder or not.

##### Returns:

* **$is\_builder\_page**: _(bool)_ Whether or not the post uses the builder.

##### Other parameters:

* **$post\_id**: _(int)_ The ID of post being evaluated.

##### Changelog:

* **Since**: 1.2.3

##### Source:

* [inc/builder/setup.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/setup.php#L350)

### make\_jetpack\_infinite\_scroll\_footer\_callback

```php
apply_filters( 'make_jetpack_infinite_scroll_footer_callback', $callback );
```

Filter: Change the callback used to render the Infinite Scroll footer.

##### Returns:

* **$callback**: _(array|string)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/integration/jetpack.php](https://github.com/thethemefoundry/make/blob/master/src/inc/integration/jetpack.php#L109)

### make\_jetpack\_infinite\_scroll\_render\_callback

```php
apply_filters( 'make_jetpack_infinite_scroll_render_callback', $callback );
```

Filter: Change the callback used to render posts retrieved by Infinite Scroll.

##### Returns:

* **$callback**: _(array|string)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/integration/jetpack.php](https://github.com/thethemefoundry/make/blob/master/src/inc/integration/jetpack.php#L127)

### make\_load\_section\_template

```php
apply_filters( 'make_load_section_template', $templates, $slug, $path );
```

Filter the templates to try and load.

##### Returns:

* **$templates**: _(array)_ The list of template to try and load.

##### Other parameters:

* **$slug**: _(string)_ The template slug.
* **$path**: _(string)_ The path to the template.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L807)

### make\_located\_file\_url

```php
apply_filters( 'make_located_file_url', $url, $file_names );
```

Filter: Modify the URL the theme will use to attempt to access a particular file.

##### Description

This can be used to set the URL for a file if the get\_located\_file\_url() method is not determining the correct URL.

##### Returns:

* **$url**: _(string)_ 

##### Other parameters:

* **$file\_names**: _(string|array)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/setup/scripts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/scripts.php#L437)

### make\_logo\_information

```php
apply_filters( 'make_logo_information', $logo_information );
```

Filter the URL and dimensions of the custom logo.

##### Description

This filter may be useful if you encounter problems getting your custom logo to appear. Note, however, that using this filter will hard-code the logo information and settings in the Logo interface in the Customizer won't be reflected.

##### Returns:

* **$logo\_information**: _(array)_ The array of information.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/logo/legacy.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/legacy.php#L384)

### make\_logo\_load\_legacy

```php
apply_filters( 'make_logo_load_legacy', $load_legacy );
```

Filter: Switch to prevent legacy logo functionality from loading.

##### Returns:

* **$load\_legacy**: _(bool)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/logo/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/methods.php#L67)

### make\_logo\_max\_width

```php
apply_filters( 'make_logo_max_width', $width );
```

Filter the maximum allowable width for a custom logo.

##### Returns:

* **$width**: _(int)_ The maximum width, in pixels.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/logo/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/methods.php#L199)

### make\_parse\_declaration

```php
apply_filters( 'make_parse_declaration', $parsed_value, $property, $value, $t, $n );
```

Filter: Modify the final CSS declaration after being parsed.

##### Returns:

* **$parsed\_value**: _(string)_ The full CSS declaration.

##### Other parameters:

* **$property**: _(string)_ The property being parsed.
* **$value**: _(string)_ The value for the property.
* **$t**: _(string)_ The tab character.
* **$n**: _(string)_ The newline character.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/style/css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/css.php#L271)

### make\_prepare\_data

```php
apply_filters( 'make_prepare_data', $clean_sections, $sections, $order );
```

Filter the full set of data for a post.

##### Returns:

* **$clean\_sections**: _(array)_ The clean sections.

##### Other parameters:

* **$sections**: _(array)_ The raw sections.
* **$order**: _(array)_ The order for the sections.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L157)

### make\_prepare\_data\_section

```php
apply_filters( 'make_prepare_data_section', $data, $section_type );
```

Filter the prepared data for an individual section.

##### Description

The result of the call\_user\_func\_array() call is an array of data representing the data for the section. This filter allows a developer to alter that data after it is handled.

##### Returns:

* **$data**: _(array)_ The raw section data.

##### Other parameters:

* **$section\_type**: _(string)_ The type of section being handled.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L141)

### make\_preview\_font\_data

```php
apply_filters( 'make_preview_font_data', $response, $fonts );
```

Filter: Modify the preview font data array before it is converted to JSON and sent as an Ajax response.

##### Returns:

* **$response**: _(array)_ The array of font data.

##### Other parameters:

* **$fonts**: _(array)_ The font values to preview.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/customizer/preview.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/preview.php#L217)

### make\_sanitize\_section\_choice

```php
apply_filters( 'make_sanitize_section_choice', $value, $key, $section_type );
```

Allow developers to alter a section choice during the sanitization process.

##### Returns:

* **$value**: _(mixed)_ The value for the section choice.

##### Other parameters:

* **$key**: _(string)_ The key for the section choice.
* **$section\_type**: _(string)_ The section type.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L878)

### make\_sanitize\_text\_allowed\_tags

```php
apply_filters( 'make_sanitize_text_allowed_tags', $expandedtags, $string );
```

Customize the tags and attributes that are allowed during text sanitization.

##### Returns:

* **$expandedtags**: _(array)_ The list of allowed tags and attributes.

##### Other parameters:

* **$string**: _(string)_ The text string being sanitized.

##### Changelog:

* **Since**: 1.4.3

##### Source:

* [inc/settings/sanitize.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/sanitize.php#L120)

### make\_section\_choices

```php
apply_filters( 'make_section_choices', $choices, $key, $section_type );
```

Filter the section choices.

##### Returns:

* **$choices**: _(array)_ The default section choices.

##### Other parameters:

* **$key**: _(string)_ The key for the data.
* **$section\_type**: _(string)_ The type of section this relates to.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L802)

### make\_section\_classes

```php
apply_filters( 'make_section_classes', $classes, $current_section );
```

Filter the section classes.

##### Returns:

* **$classes**: _(string)_ The sting of classes.

##### Other parameters:

* **$current\_section**: _(array)_ The array of data for the current section.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L611)

### make\_section\_defaults

```php
apply_filters( 'make_section_defaults', $defaults );
```

Filter the section defaults.

##### Returns:

* **$defaults**: _(array)_ The default section data

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L773)

### make\_section\_html\_id

```php
apply_filters( 'make_section_html_id', $section_id, $current_section );
```

Filter the section wrapper's HTML id attribute.

##### Returns:

* **$section\_id**: _(string)_ The string used in the section's HTML id attribute.

##### Other parameters:

* **$current\_section**: _(array)_ The data for the section.

##### Changelog:

* **Since**: 1.6.0.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L574)

### make\_settings\_{$this->type}\_current\_value

```php
apply_filters( 'make_settings_{$this->type}_current_value', $value, $setting_id, $context );
```

Filter: Modify the current value for a particular setting.

##### Returns:

* **$value**: _(mixed)_ The current value of the setting.

##### Other parameters:

* **$setting\_id**: _(string)_ The id of the setting.
* **$context**: _(string)_ Optional. The context in which a setting needs to be sanitized.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/settings/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/base.php#L341)

### make\_settings\_{$this->type}\_default\_value

```php
apply_filters( 'make_settings_{$this->type}_default_value', $default_value, $setting_id );
```

Filter: Modify the default value for a particular setting.

##### Returns:

* **$default\_value**: _(string|array)_ The default value of the setting.

##### Other parameters:

* **$setting\_id**: _(string)_ The id of the setting.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/settings/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/base.php#L369)

### make\_settings\_{$this->type}\_sanitize\_callback

```php
apply_filters( 'make_settings_{$this->type}_sanitize_callback', $callback, $setting_id, $context );
```

Filter: Modify the name of the sanitize callback function for a particular setting.

##### Returns:

* **$callback**: _(string|array)_ The name of the callback function.

##### Other parameters:

* **$setting\_id**: _(string)_ The id of the setting.
* **$context**: _(string)_ The context in which the setting needs to be sanitized.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/settings/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/base.php#L425)

### make\_settings\_{$this->type}\_sanitize\_callback\_parameters

```php
apply_filters( 'make_settings_{$this->type}_sanitize_callback_parameters', $value, $setting_id, $callback );
```

Filter: Prepare the array of parameters to feed into the sanitize callback function.

##### Description

Some callbacks may require more than one parameter. This filter provides an opportunity to add additional items to the array that will become the callback's parameters.

##### Returns:

* **$value**: _(array)_ The array of parameters, initially containing only the value to be sanitized.

##### Other parameters:

* **$setting\_id**: _(string)_ The id of the setting being sanitized.
* **$callback**: _(string)_ The callable that will accept parameters.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/settings/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/base.php#L482)

### make\_show\_errors

```php
apply_filters( 'make_show_errors', $show_errors );
```

Filter: Toggle for showing Make errors.

##### Returns:

* **$show\_errors**: _(bool)_ True to show errors.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/error/collector.php](https://github.com/thethemefoundry/make/blob/master/src/inc/error/collector.php#L51)

### make\_show\_footer\_credit

```php
apply_filters( 'make_show_footer_credit', $show );
```

Allow toggling of the footer credit.

##### Returns:

* **$show**: _(bool)_ Whether or not to show the footer credit.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [partials/footer-credit.php](https://github.com/thethemefoundry/make/blob/master/src/partials/footer-credit.php#L13)

### make\_sidebar\_left

```php
apply_filters( 'make_sidebar_left', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Returns:

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [sidebar-left.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-left.php#L13)

### make\_sidebar\_right

```php
apply_filters( 'make_sidebar_right', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Returns:

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [sidebar-right.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-right.php#L13)

### make\_site\_header\_class

```php
apply_filters( 'make_site_header_class', $classes );
```

Filter: Modify the classes applied to the site header element.

##### Returns:

* **$classes**: _(array)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L249)

### make\_socialicons\_default

```php
apply_filters( 'make_socialicons_default', $icon );
```

Filter: Modify the icon definition for a URL that doesn't match any icon URL pattern.

##### Returns:

* **$icon**: _(array)_ The icon definition.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L357)

### make\_socialicons\_email

```php
apply_filters( 'make_socialicons_email', $icon );
```

Filter: Modify the icon definition for an email address.

##### Returns:

* **$icon**: _(array)_ The icon definition.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L315)

### make\_socialicons\_render\_override

```php
apply_filters( 'make_socialicons_render_override', $override, $icon_data );
```

Filter: Override the default social icons rendered output.

##### Returns:

* **$override**: _(string|null)_ This value will be returned if it is not null.

##### Other parameters:

* **$icon\_data**: _(array)_ The array of icon data to use for rendering.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L647)

### make\_socialicons\_rss

```php
apply_filters( 'make_socialicons_rss', $icon );
```

Filter: Modify the icon definition for an RSS feed.

##### Returns:

* **$icon**: _(array)_ The icon definition.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L336)

### make\_style\_formats

```php
apply_filters( 'make_style_formats', $style_formats );
```

Filter the styles that are added to the TinyMCE Formats dropdown.

##### Returns:

* **$style\_formats**: _(array)_ The format items being added to TinyMCE.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/formatting/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/formatting/manager.php#L443)

### make\_template\_content\_archive

```php
apply_filters( 'make_template_content_archive', $type, $post );
```

Allow for changing the template partial.

##### Returns:

* **$type**: _(string)_ The default template type to use.

##### Other parameters:

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [archive.php](https://github.com/thethemefoundry/make/blob/master/src/archive.php#L31)

### make\_template\_content\_page

```php
apply_filters( 'make_template_content_page', $type, $post );
```

Allow for changing the template partial.

##### Returns:

* **$type**: _(string)_ The default template type to use.

##### Other parameters:

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [page.php](https://github.com/thethemefoundry/make/blob/master/src/page.php#L25)

### make\_template\_content\_search

```php
apply_filters( 'make_template_content_search', $type, $post );
```

Allow for changing the template partial.

##### Returns:

* **$type**: _(string)_ The default template type to use.

##### Other parameters:

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [search.php](https://github.com/thethemefoundry/make/blob/master/src/search.php#L30)

### make\_template\_content\_single

```php
apply_filters( 'make_template_content_single', $type, $post );
```

Allow for changing the template partial.

##### Returns:

* **$type**: _(string)_ The default template type to use.

##### Other parameters:

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [single.php](https://github.com/thethemefoundry/make/blob/master/src/single.php#L25)

### make\_the\_builder\_content

```php
apply_filters( 'make_the_builder_content', $content );
```

Filter the content used for "post\_content" when the builder is used to generate content.

##### Returns:

* **$content**: _(string)_ The post content.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L630)

### make\_widget\_display\_args

```php
apply_filters( 'make_widget_display_args', $widget_args, $sidebar_id );
```

Filter: Modify the wrapper markup parameters for the widgets in a particular sidebar.

##### Returns:

* **$widget\_args**: _(array)_ The default widget markup for sidebars.

##### Other parameters:

* **$sidebar\_id**: _(string)_ The ID of the sidebar that the widget markup will apply to.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/setup/widgets.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/widgets.php#L95)

### make\_will\_be\_builder\_page

```php
apply_filters( 'make_will_be_builder_page', $will_be_builder_page, $template, $use_builder );
```

Allow developers to dynamically change the builder page status.

##### Returns:

* **$will\_be\_builder\_page**: _(bool)_ Whether or not this page will be a builder page.

##### Other parameters:

* **$template**: _(string)_ The template name.
* **$use\_builder**: _(int)_ Value of the &quot;use-builder&quot; input. 1 === use builder. 0 === do not use builder.

##### Changelog:

* **Since**: 1.2.3.

##### Source:

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L719)

### makeplus\_admin\_view\_is\_product

```php
apply_filters( 'makeplus_admin_view_is_product', $is_product );
```

Filter: Modify the result of the check to see if the current admin view is "product".

##### Returns:

* **$is\_product**: _(bool)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/ecommerce/enhancement/layoutproduct.php, line 142

### makeplus\_compatibility\_mode

```php
apply_filters( 'makeplus_compatibility_mode', $mode );
```

Filter: Set the mode for compatibility.

##### Description

 'full' will load all the files to enable back compatibility with deprecated code. (Default) 'current' will not load any deprecated code. Use with caution! Could result in a fatal PHP error. A minor release value, such as '1.6', will load files necessary for back compatibility with version 1.6.x. Note that there are no separate modes for releases prior to 1.6.  Example: If a site was originally customized with a child theme and Make Plus 1.6.x, setting the mode to 1.6 will load files necessary to enable compatibility with changes made in 1.7.x, but will skip files for 1.6.

##### Returns:

* **$mode**: _(string)_ The compatibility mode to run the theme in.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* [inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L138)

### makeplus\_ecommerce\_colorhighlight\_description

```php
apply_filters( 'makeplus_ecommerce_colorhighlight_description', $description );
```

Filter: Change the description of the Highlight Color control in the Customizer.

##### Description

Useful for specifying which site elements are affected by the color choice.

##### Returns:

* **$description**: _(string)_ The control description.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/ecommerce/enhancement/colorhighlight.php, line 166

### makeplus\_ecommerce\_layoutproduct\_description

```php
apply_filters( 'makeplus_ecommerce_layoutproduct_description', $description );
```

Filter: Change the description of the Layout: Product section in the Customizer.

##### Description

Useful for specifying what constitutes the &quot;Product&quot; view.

##### Returns:

* **$description**: _(string)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/ecommerce/enhancement/layoutproduct.php, line 265

### makeplus\_ecommerce\_layoutshop\_description

```php
apply_filters( 'makeplus_ecommerce_layoutshop_description', $description );
```

Filter: Change the description of the Layout: Shop section in the Customizer.

##### Description

Useful for specifying what constitutes the &quot;Shop&quot; view.

##### Returns:

* **$description**: _(string)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/ecommerce/enhancement/layoutshop.php, line 227

### makeplus\_font\_weights

```php
apply_filters( 'makeplus_font_weights', $weights, $family );
```

Filter: Modify the available font weights for a given font family.

##### Returns:

* **$weights**: _(array)_ The array of available font weights.

##### Other parameters:

* **$family**: _(string)_ The option value of the font family.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/fontweight/setup.php, line 258

### makeplus\_get\_sidebars

```php
apply_filters( 'makeplus_get_sidebars', $sidebars );
```

Filter: Modify sidebar data before use without modifying values stored in the database.

##### Returns:

* **$sidebars**: _(array)_ The array of sidebar data.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/sidebars/manager.php, line 94

### makeplus\_postslist\_filter\_choices

```php
apply_filters( 'makeplus_postslist_filter_choices', $choice_list, $post_type );
```

Returns the choices available in the "From" dropdown that filters the posts returned in the query.

##### Returns:

* **$choice\_list**: _(array)_ The $value =&gt; $label array of choices.

##### Other parameters:

* **$post\_type**: _(string)_ The ID of the post type to retrieve filter choices for.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/postslist/filter.php, line 139

### makeplus\_postslist\_output

```php
apply_filters( 'makeplus_postslist_output', $output, $query, $display );
```

Filter: Modify the HTML output for a Posts List.

##### Returns:

* **$output**: _(string)_ 

##### Other parameters:

* **$query**: _(WP\_Query)_ 
* **$display**: _(array)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/postslist/setup.php, line 848

### makeplus\_postslist\_query\_args

```php
apply_filters( 'makeplus_postslist_query_args', $args, $options );
```

Filter the arguments that are used to create the Posts List query object.

##### Returns:

* **$args**: _(array)_ The query arguments.

##### Other parameters:

* **$options**: _(array)_ The section/widget options used to determine the arguments.

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/postslist/setup.php, line 692

### makeplus\_postslist\_template\_paths

```php
apply_filters( 'makeplus_postslist_template_paths', $paths );
```

Filter: Modify the array of paths used when locating the post-list-item.php template file.

##### Returns:

* **$paths**: _(array)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/postslist/setup.php, line 766

### makeplus\_typekit\_async

```php
apply_filters( 'makeplus_typekit_async', $async );
```

Filter: Modify the async property of the Typekit font loading script.

##### Returns:

* **$async**: _(bool)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/typekit/setup.php, line 428

### makeplus\_view\_is\_product

```php
apply_filters( 'makeplus_view_is_product', $is_product );
```

Filter: Modify the result of the check to see if the current view is "product".

##### Returns:

* **$is\_product**: _(bool)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/ecommerce/enhancement/layoutproduct.php, line 120

### makeplus\_view\_is\_shop

```php
apply_filters( 'makeplus_view_is_shop', $is_shop );
```

Filter: Modify the result of the check to see if the current view is "shop".

##### Returns:

* **$is\_shop**: _(bool)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/ecommerce/enhancement/layoutshop.php, line 109

### makeplus\_woocommerce\_product\_grid\_output

```php
apply_filters( 'makeplus_woocommerce_product_grid_output', $output );
```

Filter: Modify the output for the Product Grid.

##### Returns:

* **$output**: _(string)_ 

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/woocommerce/shortcode.php, line 439

### makeplus\_woocommerce\_product\_grid\_query\_args

```php
apply_filters( 'makeplus_woocommerce_product_grid_query_args', $args, $atts );
```

Filter: Modify the query arguments for the Product Grid.

##### Returns:

* **$args**: _(array)_ Query args

##### Other parameters:

* **$atts**: _(array)_ Shortcode attributes

##### Changelog:

* **Since**: 1.7.0.

##### Source:

* inc/component/woocommerce/shortcode.php, line 262

### ttfmake-text-column-classes

```php
apply_filters( 'ttfmake-text-column-classes', $column_classes, $i, $ttfmake_section_data );
```

Filter the classes applied to each column in a Columns section.

##### Returns:

* **$column\_classes**: _(string)_ The classes for the column.

##### Other parameters:

* **$i**: _(int)_ The column number.
* **$ttfmake\_section\_data**: _(array)_ The array of data for the section.

##### Changelog:

* **Since**: 1.2.0.

##### Source:

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L93)

### ttfmp\_panels\_item\_configuration

```php
apply_filters( 'ttfmp_panels_item_configuration', $inputs );
```

Filter the definitions of the panel configuration inputs.

##### Returns:

* **$inputs**: _(array)_ The input definition array.

##### Changelog:

* **Since**: 1.6.0.

##### Source:

* inc/component/panels/sections/builder-templates/section-item.php, line 254

### ttfmp\_parallax\_js\_config

```php
apply_filters( 'ttfmp_parallax_js_config', $config );
```

Filter: Modify the frontend JS configuration for the Parallax feature.

##### Description

See: https://github.com/markdalgleish/stellar.js/blob/master/README.md#configuring-everything

##### Returns:

* **$config**: _(array)_ The array of configuration options.

##### Changelog:

* **Since**: 1.6.1

##### Source:

* inc/component/parallax/setup.php, line 183

### ttfmp\_perpage\_post\_types

```php
apply_filters( 'ttfmp_perpage_post_types', $post_types );
```

Filter: Modify the array of post types that qualify as the "Post" view in the admin.

##### Description

This helps to determine whether the Layout Settings metabox should appear on the Edit screen for a particular post type.

##### Returns:

* **$post\_types**: _(array)_ 

##### Changelog:

* **Since**: 1.0.0.

##### Source:

* inc/component/perpage/setup.php, line 196

### ttfmp\_post\_list\_post\_title\_element

```php
apply_filters( 'ttfmp_post_list_post_title_element', $t_wrap, $ttfmp_data );
```

Filter: Modify the element used to wrap post titles in a Posts List instance.

##### Returns:

* **$t\_wrap**: _(string)_ The element name. E.g. h3, strong, div

##### Other parameters:

* **$ttfmp\_data**: _(array)_ The array of data specific to the Posts List instance.

##### Changelog:

* **Since**: 1.6.6.

##### Source:

* inc/component/postslist/templates/post-list-item.php, line 56

### ttfmp\_posts\_list\_thumbnail\_size

```php
apply_filters( 'ttfmp_posts_list_thumbnail_size', $thumbnail_size, $ttfmp_data );
```

Filter: Modify the image size used for featured images in a Posts List instance.

##### Returns:

* **$thumbnail\_size**: _(string)_ The image size to use. E.g. thumbnail, medium, large, full.

##### Other parameters:

* **$ttfmp\_data**: _(array)_ The array of data specific to the Posts List instance.

##### Changelog:

* **Since**: 1.3.0.

##### Source:

* inc/component/postslist/templates/post-list-item.php, line 22

