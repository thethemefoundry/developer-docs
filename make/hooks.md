
## Actions

### make\_api\_loaded

```php
do_action( 'make_api_loaded', $Make );
```

##### Description

Action: Fire when the Make API has finished loading.

##### Parameters:


* **$Make**: _(MAKE\_API)_ 

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/functions.php](https://github.com/thethemefoundry/make/blob/master/src/functions.php#L40)

### make\_notice\_loaded

```php
do_action( 'make_notice_loaded', $notice );
```

##### Description

Action: Fires at the end of the Admin Notice object's load method.
This action gives a developer the opportunity to add additional admin notices
and run additional load routines.

##### Parameters:


* **$notice**: _(MAKE\_Admin\_Notice)_ The notice object that has just finished loading.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/admin/notice.php](https://github.com/thethemefoundry/make/blob/master/src/inc/admin/notice.php#L108)

### make\_section\_'.$ttfmake\_section\_data['section']['id'].'\_before

```php
do_action( 'make_section_' . $ttfmake_section_data['section']['id'] . '_before', $ttfmake_section_data );
```

##### Description

Allow for script execution in the header of a builder section.
This action is a variable action that allows a developer to hook into specific section types (e.g., 'text'). Do
not confuse "id" in this context as the individual section id (e.g., 14092814910).

##### Parameters:


* **$ttfmake\_section\_data**: _(array)_ The array of data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L792)

### make\_section\_'.$ttfmake\_section\_data['section']['id'].'\_after

```php
do_action( 'make_section_' . $ttfmake_section_data['section']['id'] . '_after', $ttfmake_section_data );
```

##### Description

Allow for script execution in the footer of a builder section.
This action is a variable action that allows a developer to hook into specific section types (e.g., 'text'). Do
not confuse "id" in this context as the individual section id (e.g., 14092814910).

##### Parameters:


* **$ttfmake\_section\_data**: _(array)_ The array of data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L821)

### make\_builder\_data\_saved

```php
do_action( 'make_builder_data_saved', $sections, $post_id );
```

##### Description

Execute code after the section data is saved.
While it is possible to use a "save_post" to hook into the save routine, this action is preferred as it is
only called after all validation and sanitization is completed.

##### Parameters:


* **$sections**: _(array)_ The clean section data.

* **$post\_id**: _(int)_ The post ID for the saved data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L184)

### make\_before\_builder\_menu

```php
do_action( 'make_before_builder_menu' );
```

##### Description

Execute code before the builder menu items are displayed.

##### Parameters:


##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/templates/menu.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/menu.php#L18)

### make\_after\_builder\_menu

```php
do_action( 'make_after_builder_menu' );
```

##### Description

Execute code after the builder menu items are displayed.

##### Parameters:


##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/templates/menu.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/menu.php#L42)

### make\_before\_section\_header

```php
do_action( 'make_before_section_header' );
```

##### Description

Execute code before the section header is displayed.

##### Parameters:


##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/templates/section-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/section-header.php#L56)

### make\_after\_builder\_stage

```php
do_action( 'make_after_builder_stage' );
```

##### Description

Execute code after the builder stage is displayed.

##### Parameters:


##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/templates/stage-footer.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/stage-footer.php#L11)

### make\_section\_text\_before\_column

```php
do_action( 'make_section_text_before_column', $ttfmake_section_data );
```

##### Description

Execute code before an individual text column is displayed.

##### Parameters:


* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/columns/builder-template-column.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/columns/builder-template-column.php#L72)

### make\_section\_text\_after\_column

```php
do_action( 'make_section_text_after_column', $ttfmake_section_data );
```

##### Description

Execute code after an individual text column is displayed.

##### Parameters:


* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/columns/builder-template-column.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/columns/builder-template-column.php#L95)

### make\_section\_text\_before\_columns\_select

```php
do_action( 'make_section_text_before_columns_select', $ttfmake_section_data );
```

##### Description

Execute code before the columns select input is displayed.

##### Parameters:


* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/columns/builder-template.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/columns/builder-template.php#L17)

### make\_section\_text\_after\_columns\_select

```php
do_action( 'make_section_text_after_columns_select', $ttfmake_section_data );
```

##### Description

Execute code after the columns select input is displayed.

##### Parameters:


* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/columns/builder-template.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/columns/builder-template.php#L26)

### make\_section\_text\_after\_title

```php
do_action( 'make_section_text_after_title', $ttfmake_section_data );
```

##### Description

Execute code after the section title is displayed.

##### Parameters:


* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/columns/builder-template.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/columns/builder-template.php#L35)

### make\_section\_text\_after\_columns

```php
do_action( 'make_section_text_after_columns', $ttfmake_section_data );
```

##### Description

Execute code after all columns are displayed.

##### Parameters:


* **$ttfmake\_section\_data**: _(array)_ The data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/columns/builder-template.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/columns/builder-template.php#L46)

### make\_builder\_'.$data['section-type'].'\_css

```php
do_action( 'make_builder_' . $data['section-type'] . '_css', $data, $id, $style );
```

##### Description

Allow section-specific CSS rules to be added to the document head of a Builder page.

##### Parameters:


* **$data**: _(array)_ The Builder section's data.

* **$id**: _(int)_ The ID of the Builder section.

* **$style**: _(MAKE\_Style\_ManagerInterface)_ The style manager instance.

##### Changelog:


* **Since**: 1.4.5

* **Since**: 1.7.0.

##### Source:

* [src/inc/builder/setup.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/setup.php#L149)

### make\_choices\_loaded

```php
do_action( 'make_choices_loaded', $choices );
```

##### Description

Action: Fires at the end of the choices object's load method.
This action gives a developer the opportunity to add or modify choice sets
and run additional load routines.

##### Parameters:


* **$choices**: _(MAKE\_Choices\_Manager)_ The choices object that has just finished loading.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/choices/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/choices/manager.php#L74)

### make\_deprecated\_function\_run

```php
do_action( 'make_deprecated_function_run', $function, $version, $replacement, $message );
```

##### Description

Fires when a deprecated function is called.

##### Parameters:


* **$function**: _(string)_ The function that was called.

* **$version**: _(string)_ The version of Make that deprecated the function.

* **$replacement**: _(string)_ The function that should have been called.

* **$message**: _(string)_ Explanatory text if there is no direct replacement available.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L284)

### make\_deprecated\_hook\_run

```php
do_action( 'make_deprecated_hook_run', $hook, $version, $message );
```

##### Description

Fires when a deprecated hook has an attached functionmethod.

##### Parameters:


* **$hook**: _(string)_ The hook that was called.

* **$version**: _(string)_ The version of Make that deprecated the hook.

* **$message**: _(string)_ Optional. A message regarding the change. Default null.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L337)

### make\_doing\_it\_wrong\_run

```php
do_action( 'make_doing_it_wrong_run', $function, $message, $version );
```

##### Description

Fires when the given function is being used incorrectly.

##### Parameters:


* **$function**: _(string)_ The function that was called.

* **$message**: _(string)_ A message explaining what has been done incorrectly.

* **$version**: _(string)_ The version of Make where the message was added.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L380)

### make\_font\_loaded

```php
do_action( 'make_font_loaded', $font );
```

##### Description

Action: Fires at the end of the font object's load method.
This action gives a developer the opportunity to add font sources
and run additional load routines.

##### Parameters:


* **$font**: _(MAKE\_Font\_Manager)_ The font object that has just finished loading.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/font/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/manager.php#L79)

### make\_add\_formats

```php
do_action( 'make_add_formats', $formatting );
```

##### Description

Action: Fires at the end of the Formatting object's add_formats method.
This action gives a developer the opportunity to add or remove formats.

##### Parameters:


* **$formatting**: _(MAKE\_Formatting\_Manager)_ The Formatting object.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/formatting/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/formatting/manager.php#L218)

### make\_view\_loaded

```php
do_action( 'make_view_loaded', $view );
```

##### Description

Action: Fires at the end of the view object's load method.
This action gives a developer the opportunity to add or modify views
and run additional load routines.

##### Parameters:


* **$view**: _(MAKE\_Layout\_View)_ The view object that has just finished loading.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/layout/view.php](https://github.com/thethemefoundry/make/blob/master/src/inc/layout/view.php#L105)

### make\_settings\_thememod\_loaded

```php
do_action( 'make_settings_thememod_loaded', $settings );
```

##### Description

Action: Fires at the end of the ThemeMod settings object's load method.
This action gives a developer the opportunity to add or modify setting definitions
and run additional load routines.

##### Parameters:


* **$settings**: _(MAKE\_Settings\_ThemeMod)_ The settings object that has just finished loading.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/settings/thememod.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/thememod.php#L120)

### make\_socialicons\_loaded

```php
do_action( "make_socialicons_loaded", $socialicons );
```

##### Description

Action: Fires at the end of the Social Icons object's load method.
This action gives a developer the opportunity to add or modify icon definitions
and run additional load routines.

##### Parameters:


* **$socialicons**: _(MAKE\_SocialIcons\_Manager)_ The settings object that has just finished loading.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L130)

### make\_style\_before\_load

```php
do_action( 'make_style_before_load', $style );
```

##### Description

Action: Fires before the Style class loads data files.
This allows, for example, for filters to be added to thememod settings to change the values
before the style definitions are loaded.

##### Parameters:


* **$style**: _(MAKE\_Style\_ManagerInterface)_ The style object.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L147)

### make\_css

```php
do_action( 'make_css' );
```

##### Description

The hook used to add CSS rules for the generated inline CSS.
This hook is the correct hook to use for adding CSS styles to the group of selectors and properties that will be
added to inline CSS that is printed in the head. Hooking elsewhere may lead to rules not being registered
correctly for the CSS generation. Most Customizer options will use this hook to register additional CSS rules.

##### Parameters:


##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L188)

### make\_style\_loaded

```php
do_action( 'make_style_loaded', $style );
```

##### Description

Action: Fires at the end of the Styles object's load method.
This action gives a developer the opportunity to add or modify dynamic styles
and run additional load routines.

##### Parameters:


* **$style**: _(MAKE\_Style\_Manager)_ The style object

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L201)

### make\_style\_before\_inline

```php
do_action( 'make_style_before_inline', $style );
```

##### Description

Action: Fires before the inline CSS rules are rendered and output.

##### Parameters:


* **$style**: _(MAKE\_Style\_ManagerInterface)_ The style object.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L234)

### make\_style\_before\_file

```php
do_action( 'make_style_before_file', $style );
```

##### Description

Action: Fires before the CSS rules are rendered and output as a file.

##### Parameters:


* **$style**: _(MAKE\_Style\_ManagerInterface)_ The style object.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/style/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/manager.php#L295)


## Filters

### make\_template\_content\_archive

```php
apply_filters( 'make_template_content_archive', $type, $post );
```

##### Description

Allow for changing the template partial.

##### Parameters:


* **$type**: _(string)_ The default template type to use.

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/archive.php](https://github.com/thethemefoundry/make/blob/master/src/archive.php#L31)

### make\_add\_section

```php
apply_filters( 'make_add_section', $section );
```

##### Description

Allow the added sections to be filtered.
This filters allows for dynamically altering sections as they get added. This can help enforce policies for
sections by sanitizing the registered values.

##### Parameters:


* **$section**: _(array)_ The section being added.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/api.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/api.php#L113)

### make\_builder\_js\_dependencies

```php
apply_filters( 'make_builder_js_dependencies', $dependencies );
```

##### Description

Filter the dependencies for the Make builder JS.

##### Parameters:


* **$dependencies**: _(array)_ The list of dependencies.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L333)

### make\_builder\_is\_default

```php
apply_filters( 'make_builder_is_default', $is_default );
```

##### Description

Filter: Modify whether new pages default to the Builder template.

##### Parameters:


* **$is\_default**: _(bool)_ 

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L400)

### make\_will\_be\_builder\_page

```php
apply_filters( 'make_will_be_builder_page', $will_be_builder_page, $template, $use_builder );
```

##### Description

Allow developers to dynamically change the builder page status.

##### Parameters:


* **$will\_be\_builder\_page**: _(bool)_ Whether or not this page will be a builder page.

* **$template**: _(string)_ The template name.

* **$use\_builder**: _(int)_ Value of the "use-builder" input. 1 === use builder. 0 === do not use builder.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L766)

### make\_load\_section\_template

```php
apply_filters( 'make_load_section_template', $templates, $slug, $path );
```

##### Description

Filter the templates to try and load.

##### Parameters:


* **$templates**: _(array)_ The list of template to try and load.

* **$slug**: _(string)_ The template slug.

* **$path**: _(string)_ The path to the template.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L855)

### make\_get\_wp\_editor\_id

```php
apply_filters( 'make_get_wp_editor_id', $id, $data, $is_js_template );
```

##### Description

Alter the wp_editor ID.

##### Parameters:


* **$id**: _(string)_ The ID for the editor.

* **$data**: _(array)_ The section data.

* **$is\_js\_template**: _(bool)_ Whether or not this is in the context of a JS template.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L904)

### make\_get\_section\_name

```php
apply_filters( 'make_get_section_name', $name, $data, $is_js_template );
```

##### Description

Alter section name.

##### Parameters:


* **$name**: _(string)_ The name of the section.

* **$data**: _(array)_ The section data.

* **$is\_js\_template**: _(bool)_ Whether or not this is in the context of a JS template.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L930)

### make\_get\_image

```php
apply_filters( 'make_get_image', $return, $image_id, $size );
```

##### Description

Filter the image HTML.

##### Parameters:


* **$return**: _(string)_ The image HTML.

* **$image\_id**: _(int)_ The ID for the image.

* **$size**: _(bool)_ The requested image size.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L969)

### make\_get\_image\_src

```php
apply_filters( 'make_get_image_src', $src, $image_id, $size );
```

##### Description

Filter the image source attributes.

##### Parameters:


* **$src**: _(string)_ The image source attributes.

* **$image\_id**: _(int)_ The ID for the image.

* **$size**: _(bool)_ The requested image size.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L1014)

### make\_get\_placeholder\_image

```php
apply_filters( 'make_get_placeholder_image', $return, $image_id, $ttfmake_placeholder_images );
```

##### Description

Filter the image source attributes.

##### Parameters:


* **$return**: _(string)_ The image source attributes.

* **$image\_id**: _(int)_ The ID for the image.

* **$ttfmake\_placeholder\_images**: _(bool)_ The list of placeholder images.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L1046)

### make\_get\_section\_json

```php
apply_filters( 'make_get_section_json', $section );
```

##### Description

Filters the json representation of a single section.
This filters allows for dynamically altering this section
json representation.

##### Parameters:


* **$section**: _(array)_ The section being jsonified.

##### Changelog:


* **Since**: 1.8.0

##### Source:

* [src/inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L1089)

### make\_configuration\_overlay\_input\_wrap

```php
apply_filters( 'make_configuration_overlay_input_wrap', $wrapper, $args, $section_data );
```

##### Description

Filter the wrapped used for the inputs.

##### Parameters:


* **$wrapper**: _(string)_ The HTML to wrap around the input.

* **$args**: _(string)_ The input data that is wrapped.

* **$section\_data**: _(string)_ The data for the section.

##### Changelog:


* **Since**: 1.4.0.

##### Source:

* [src/inc/builder/core/configuration-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/configuration-helpers.php#L238)

### make\_configuration\_overlay\_input

```php
apply_filters( 'make_configuration_overlay_input', $this_output, $args, $section_data );
```

##### Description

Filter the HTML for the input.

##### Parameters:


* **$this\_output**: _(string)_ The HTML for the input.

* **$args**: _(string)_ The input data.

* **$section\_data**: _(string)_ The data for the section.

##### Changelog:


* **Since**: 1.4.0.

##### Source:

* [src/inc/builder/core/configuration-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/configuration-helpers.php#L249)

### make\_prepare\_data

```php
apply_filters( 'make_prepare_data', $clean_sections, $sections );
```

##### Description

Filter the full set of data for a post.

##### Parameters:


* **$clean\_sections**: _(array)_ The clean sections.

* **$sections**: _(array)_ The raw sections.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L145)

### make\_insert\_post\_data\_sections

```php
apply_filters( 'make_insert_post_data_sections', $data );
```

##### Description

Filter the section data.

##### Parameters:


* **$data**: _(array)_ The sanitized data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L296)

### make\_generate\_post\_content

```php
apply_filters( 'make_generate_post_content', $post_content, $data );
```

##### Description

Filter the generated post content.
This content is the full HTML version of the content that will be saved as "post_content".

##### Parameters:


* **$post\_content**: _(string)_ The fully generated post content.

* **$data**: _(array)_ The data used to generate the content.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L375)

### make\_get\_next\_section\_data

```php
apply_filters( 'make_get_next_section_data', $next_data, $current_section, $sections );
```

##### Description

Allow developers to alter the "next" section data.

##### Parameters:


* **$next\_data**: _(array)_ The data for the next section.

* **$current\_section**: _(array)_ The data for the current section.

* **$sections**: _(array)_ The list of all sections.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L508)

### make\_get\_prev\_section\_data

```php
apply_filters( 'make_get_prev_section_data', $prev_section, $current_section, $sections );
```

##### Description

Allow developers to alter the "next" section data.

##### Parameters:


* **$prev\_section**: _(array)_ The data for the next section.

* **$current\_section**: _(array)_ The data for the current section.

* **$sections**: _(array)_ The list of all sections.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L540)

### make\_section\_html\_id

```php
apply_filters( 'make_section_html_id', $section_id, $current_section );
```

##### Description

Filter the section wrapper's HTML id attribute.

##### Parameters:


* **$section\_id**: _(string)_ The string used in the section's HTML id attribute.

* **$current\_section**: _(array)_ The data for the section.

##### Changelog:


* **Since**: 1.6.0.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L564)

### make\_section\_classes

```php
apply_filters( 'make_section_classes', $classes, $current_section );
```

##### Description

Filter the section classes.

##### Parameters:


* **$classes**: _(string)_ The sting of classes.

* **$current\_section**: _(array)_ The array of data for the current section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L601)

### ttfmake\_the\_builder\_content

```php
apply_filters( 'ttfmake_the_builder_content', $content );
```

##### Description

Filter the content used for "post_content" when the builder is used to generate content.

##### Parameters:


* **$content**: _(string)_ The post content.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L621)

### make\_the\_builder\_content

```php
apply_filters( 'make_the_builder_content', $content );
```

##### Description

Filter the content used for "post_content" when the builder is used to generate content.

##### Parameters:


* **$content**: _(string)_ The post content.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L630)

### ttfmake\_builder\_section\_footer\_links

```php
apply_filters( 'ttfmake_builder_section_footer_links', $links );
```

##### Description

Deprecated: Filter the definitions for the links that appear in each Builder section's footer.
This filter is deprecated. Use make_builder_section_links instead.

##### Parameters:


* **$links**: _(array)_ The link definition array.

##### Changelog:


* **Since**: 1.0.7.

##### Source:

* [src/inc/builder/core/templates/section-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/section-header.php#L37)

### make\_builder\_section\_links

```php
apply_filters( 'make_builder_section_links', $links );
```

##### Description

Filter the definitions for the buttons that appear in each Builder section's header.

##### Parameters:


* **$links**: _(array)_ The button definition array.

##### Changelog:


* **Since**: 1.4.0.

##### Source:

* [src/inc/builder/core/templates/section-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/section-header.php#L45)

### make\_banner\_slide\_configuration

```php
apply_filters( 'make_banner_slide_configuration', $inputs );
```

##### Description

Filter the definitions of the Banner slide configuration inputs.

##### Parameters:


* **$inputs**: _(array)_ The input definition array.

##### Changelog:


* **Since**: 1.4.0.

##### Source:

* [src/inc/builder/sections/banner/definition.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/banner/definition.php#L208)

### make\_column\_buttons

```php
apply_filters( 'make_column_buttons', $column_buttons, $item_type );
```

##### Description

Filter the buttons added to a text column.

##### Parameters:


* **$column\_buttons**: _(array)_ The current list of buttons.

* **$item\_type**: _(string)_ Item type, in this case 'column'.

##### Changelog:


* **Since**: 1.4.0.

* **Since**: 1.8.8.

##### Source:

* [src/inc/builder/sections/columns/builder-template-column.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/columns/builder-template-column.php#L40)

### ttfmake-text-column-classes

```php
apply_filters( 'ttfmake-text-column-classes', $column_classes, $i, $ttfmake_section_data );
```

##### Description

Filter the classes applied to each column in a Columns section.

##### Parameters:


* **$column\_classes**: _(string)_ The classes for the column.

* **$i**: _(int)_ The column number.

* **$ttfmake\_section\_data**: _(array)_ The array of data for the section.

##### Changelog:


* **Since**: 1.2.0.

##### Source:

* [src/inc/builder/sections/columns/builder-template-column.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/columns/builder-template-column.php#L52)

### make\_gallery\_item\_configuration

```php
apply_filters( 'make_gallery_item_configuration', $inputs );
```

##### Description

Filter the definitions of the Gallery item configuration inputs.

##### Parameters:


* **$inputs**: _(array)_ The input definition array.

##### Changelog:


* **Since**: 1.4.0.

##### Source:

* [src/inc/builder/sections/gallery/definition.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/gallery/definition.php#L164)

### make\_section\_defaults

```php
apply_filters( 'make_section_defaults', $defaults );
```

##### Description

Filter the section defaults.

##### Parameters:


* **$defaults**: _(array)_ The default section data

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L120)

### make\_section\_choices

```php
apply_filters( 'make_section_choices', $choices, $key, $section_type );
```

##### Description

Filter the section choices.

##### Parameters:


* **$choices**: _(array)_ The default section choices.

* **$key**: _(string)_ The key for the data.

* **$section\_type**: _(string)_ The type of section this relates to.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L144)

### make\_get\_section\_default

```php
apply_filters( 'make_get_section_default', $value, $key, $section_type );
```

##### Description

Filter the default section data that is received.

##### Parameters:


* **$value**: _(mixed)_ The section value.

* **$key**: _(string)_ The key to get data for.

* **$section\_type**: _(string)_ The type of section the data is for.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L176)

### make\_sanitize\_section\_choice

```php
apply_filters( 'make_sanitize_section_choice', $value, $key, $section_type );
```

##### Description

Allow developers to alter a section choice during the sanitization process.

##### Parameters:


* **$value**: _(mixed)_ The value for the section choice.

* **$key**: _(string)_ The key for the section choice.

* **$section\_type**: _(string)_ The section type.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L223)

### make\_builder\_is\_section\_type

```php
apply_filters( 'make_builder_is_section_type', $is_section_type, $type, $data );
```

##### Description

Allow developers to alter if a set of data is a specified section type.

##### Parameters:


* **$is\_section\_type**: _(bool)_ Whether or not the data represents a specific section.

* **$type**: _(string)_ The section type to check.

* **$data**: _(array)_ The section data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L27)

### make\_builder\_get\_gallery\_array

```php
apply_filters( 'make_builder_get_gallery_array', $gallery_array, $ttfmake_section_data );
```

##### Description

Filter the gallery item data.

##### Parameters:


* **$gallery\_array**: _(array)_ The array of gallery item data.

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L68)

### make\_gallery\_class

```php
apply_filters( 'make_gallery_class', $gallery_class, $ttfmake_section_data, $sections );
```

##### Description

Filter the class applied to a gallery.

##### Parameters:


* **$gallery\_class**: _(string)_ The class applied to the gallery.

* **$ttfmake\_section\_data**: _(array)_ The section data.

* **$sections**: _(array)_ The list of sections.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L132)

### make\_builder\_get\_gallery\_style

```php
apply_filters( 'make_builder_get_gallery_style', $gallery_style, $ttfmake_section_data );
```

##### Description

Filter the style added to a gallery section.

##### Parameters:


* **$gallery\_style**: _(string)_ The style applied to the gallery.

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L184)

### make\_builder\_get\_gallery\_item\_class

```php
apply_filters( 'make_builder_get_gallery_item_class', $gallery_class, $item, $ttfmake_section_data, $i );
```

##### Description

Filter the class used for a gallery item.

##### Parameters:


* **$gallery\_class**: _(string)_ The computed gallery class.

* **$item**: _(array)_ The item's data.

* **$ttfmake\_section\_data**: _(array)_ The section data.

* **$i**: _(int)_ The current gallery item number.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L230)

### make\_builder\_get\_gallery\_item\_onclick

```php
apply_filters( 'make_builder_get_gallery_item_onclick', $onclick, $link, $ttfmake_section_data, $i );
```

##### Description

Filter the class used for a gallery item.

##### Parameters:


* **$onclick**: _(string)_ The computed gallery onclick attribute.

* **$link**: _(string)_ The item's link.

* **$ttfmake\_section\_data**: _(array)_ The section data.

* **$i**: _(int)_ The current gallery item number.

##### Changelog:


* **Since**: 1.7.6.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L269)

### make\_builder\_get\_gallery\_item\_image

```php
apply_filters( 'make_builder_get_gallery_item_image', $image, $item, $aspect );
```

##### Description

Alter the generated gallery image.

##### Parameters:


* **$image**: _(string)_ The image HTML.

* **$item**: _(array)_ The item's data.

* **$aspect**: _(string)_ The aspect ratio for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L312)

### make\_builder\_get\_text\_array

```php
apply_filters( 'make_builder_get_text_array', $columns_array, $ttfmake_section_data );
```

##### Description

Filter the array of builder data for the text section.

##### Parameters:


* **$columns\_array**: _(array)_ The ordered data for the text section.

* **$ttfmake\_section\_data**: _(array)_ The raw section data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L365)

### make\_builder\_get\_text\_class

```php
apply_filters( 'make_builder_get_text_class', $text_class, $ttfmake_section_data, $sections );
```

##### Description

Filter the text section class.

##### Parameters:


* **$text\_class**: _(string)_ The computed class string.

* **$ttfmake\_section\_data**: _(array)_ The section data.

* **$sections**: _(array)_ The list of sections.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L414)

### make\_builder\_get\_banner\_array

```php
apply_filters( 'make_builder_get_banner_array', $banner_array, $ttfmake_section_data );
```

##### Description

Filter the data array for a banner section.

##### Parameters:


* **$banner\_array**: _(array)_ The ordered banner data.

* **$ttfmake\_section\_data**: _(array)_ All of the data for the section.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L498)

### make\_builder\_banner\_class

```php
apply_filters( 'make_builder_banner_class', $banner_class, $ttfmake_section_data );
```

##### Description

Filter the class for the banner section.

##### Parameters:


* **$banner\_class**: _(string)_ The banner class.

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L532)

### make\_builder\_get\_banner\_slider\_atts

```php
apply_filters( 'make_builder_get_banner_slider_atts', $data_attributes, $ttfmake_section_data );
```

##### Description

Allow for altering the banner slider attributes.

##### Parameters:


* **$data\_attributes**: _(string)_ The data attributes in string form.

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L637)

### make\_builder\_banner\_slide\_class

```php
apply_filters( 'make_builder_banner_slide_class', $slide_class );
```

##### Description

Allow developers to alter the class for the banner slide.

##### Parameters:


* **$slide\_class**: _(string)_ The banner classes.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L663)

### make\_builder\_banner\_slide\_style

```php
apply_filters( 'make_builder_banner_slide_style', $slide_style, $slide, $ttfmake_section_data );
```

##### Description

Allow developers to change the CSS for a Banner section.

##### Parameters:


* **$slide\_style**: _(string)_ The CSS for the banner.

* **$slide**: _(array)_ The slide data.

* **$ttfmake\_section\_data**: _(array)_ The section data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L700)

### make\_section\_html\_id

```php
apply_filters( 'make_section_html_id' );
```

##### Description

This filter is documented in incbuildercoresave.php

##### Parameters:


##### Changelog:


##### Source:

* [src/inc/builder/setup.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/setup.php#L175)

### make\_get\_section\_data

```php
apply_filters( 'make_get_section_data', $ordered_data, $post_id );
```

##### Description

Filter the section data for a post.

##### Parameters:


* **$ordered\_data**: _(array)_ The array of section data.

* **$post\_id**: _(int)_ The post ID for the retrieved data.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/builder/setup.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/setup.php#L262)

### make\_is\_builder\_page

```php
apply_filters( 'make_is_builder_page', $is_builder_page, $post_id );
```

##### Description

Allow a developer to dynamically change whether the post uses the builder or not.

##### Parameters:


* **$is\_builder\_page**: _(bool)_ Whether or not the post uses the builder.

* **$post\_id**: _(int)_ The ID of post being evaluated.

##### Changelog:


* **Since**: 1.2.3

##### Source:

* [src/inc/builder/setup.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/setup.php#L352)

### make\_customizer\_key\_conversions

```php
apply_filters( 'make_customizer_key_conversions', $conversions );
```

##### Description

Filter the array of Customizer option key conversions.
The keys for some Customizer options have changed between versions. This array
defines each change as $new_key => $old key.

##### Parameters:


* **$conversions**: _(array)_ The array of key conversions.

##### Changelog:


* **Since**: 1.3.0.

##### Source:

* [src/inc/compatibility/keyconverter.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/keyconverter.php#L104)

### make\_compatibility\_mode

```php
apply_filters( 'make_compatibility_mode', $mode );
```

##### Description

Filter: Set the mode for compatibility.
- 'full' will load all the files to enable back compatibility with deprecated code. (Default)
- 'current' will not load any deprecated code. Use with caution! Could result in a fatal PHP error.
- A minor release value, such as '1.5', will load files necessary for back compatibility with version 1.5.x.
Note that there are no separate modes for releases prior to 1.5.
Example: If a site was originally customized with a child theme and Make 1.6.x, setting the mode to 1.6
will load files necessary to enable compatibility with changes made in 1.7.x, but will skip files for 1.5
and 1.6.

##### Parameters:


* **$mode**: _(string)_ The compatibility mode to run the theme in.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/compatibility/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility/methods.php#L168)

### make\_customizer\_panels

```php
apply_filters( 'make_customizer_panels', $panels );
```

##### Description

Filter: Modify the array of panel definitions for the Customizer.

##### Parameters:


* **$panels**: _(array)_ The array of panel definitions.

##### Changelog:


* **Since**: 1.3.0.

##### Source:

* [src/inc/customizer/controls.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/controls.php#L281)

### make\_customizer\_sections

```php
apply_filters( 'make_customizer_sections', $sections );
```

##### Description

Filter: Modify the array of sectioncontrol definitions for the Customizer.

##### Parameters:


* **$sections**: _(array)_ The array of section definitions.

##### Changelog:


* **Since**: 1.3.0.

##### Source:

* [src/inc/customizer/controls.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/controls.php#L356)

### make\_read\_more\_text

```php
apply_filters( 'make_read_more_text' );
```

##### Description

This filter is documented in inctemplate-tags.php

##### Parameters:


##### Changelog:


##### Source:

* [src/inc/customizer/definitions/general.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/definitions/general.php#L53)

### make\_breadcrumb\_override

```php
apply_filters( 'make_breadcrumb_override', $override );
```

##### Description

Filter: Allow override of breadcrumb settings, controls and output

##### Parameters:


* **$override**: _(boolean)_ Wether third party breadcrumbs should be overriden.

##### Changelog:


* **Since**: 1.7.4.

##### Source:

* [src/inc/customizer/definitions/layout.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/definitions/layout.php#L477)

### make\_preview\_font\_data

```php
apply_filters( 'make_preview_font_data', $response, $fonts );
```

##### Description

Filter: Modify the preview font data array before it is converted to JSON and sent as an Ajax response.

##### Parameters:


* **$response**: _(array)_ The array of font data.

* **$fonts**: _(array)_ The font values to preview.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/customizer/preview.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/preview.php#L217)

### make\_show\_errors

```php
apply_filters( 'make_show_errors', $show_errors );
```

##### Description

Filter: Toggle for showing Make errors.

##### Parameters:


* **$show\_errors**: _(bool)_ True to show errors.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/error/collector.php](https://github.com/thethemefoundry/make/blob/master/src/inc/error/collector.php#L51)

### lters('make\_error\_backtrace\_limit

```php
absint( apply_filters( 'make_error_backtrace_limit', $limit );
```

##### Description

Filter: Change the number of steps shown in a Make Error backtrace.

##### Parameters:


* **$limit**: _(int)_ The number of backtrace steps to show.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/error/collector.php](https://github.com/thethemefoundry/make/blob/master/src/inc/error/collector.php#L159)

### make\_add\_font\_source\_'.$source\_i

```php
apply_filters( 'make_add_font_source_' . $source_id, $add_source );
```

##### Description

Filter: Prevent a font source from being added.

##### Parameters:


* **$add\_source**: _(bool)_ True to allow the font source to be added.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/font/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/manager.php#L116)

### make\_font\_stack

```php
apply_filters( 'make_font_stack', $stack, $font );
```

##### Description

Allow developers to filter the full font stack.

##### Parameters:


* **$stack**: _(string)_ The font stack.

* **$font**: _(string)_ The font.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/font/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/manager.php#L295)

### make\_all\_font\_choices

```php
apply_filters( 'make_all_font_choices', $choices );
```

##### Description

Filter the list of font choices.

##### Parameters:


* **$choices**: _(array)_ 

##### Changelog:


* **Since**: 1.0.0.

##### Source:

* [src/inc/font/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/manager.php#L362)

### make\_font\_data\_{$this->id}

```php
apply_filters( "make_font_data_{$this->id}", $font_data );
```

##### Description

Filter: Modify the font data from a particular source.

##### Parameters:


* **$font\_data**: _(array)_ 

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/font/source/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/base.php#L149)

### make\_get\_standard\_fonts

```php
apply_filters( 'make_get_standard_fonts', $fonts );
```

##### Description

Allow for developers to modify the standard fonts.

##### Parameters:


* **$fonts**: _(array)_ The list of standard fonts.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/font/source/generic.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/generic.php#L93)

### make\_all\_fonts

```php
apply_filters( 'make_all_fonts', $fonts );
```

##### Description

Allow for developers to modify the full list of fonts.

##### Parameters:


* **$fonts**: _(array)_ The list of all fonts.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/font/source/generic.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/generic.php#L119)

### make\_get\_google\_fonts

```php
apply_filters( 'make_get_google_fonts', $fonts );
```

##### Description

Allow for developers to modify the standard fonts.

##### Parameters:


* **$fonts**: _(array)_ The list of standard fonts.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/font/source/google.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/google.php#L161)

### make\_font\_google\_stack

```php
apply_filters( 'make_font_google_stack', $stack, $category );
```

##### Description

Filter: Modify the CSS font stack for a particular category of Google font.

##### Parameters:


* **$stack**: _(string)_ The CSS font stack.

* **$category**: _(string)_ The font category.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/font/source/google.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/google.php#L217)

### make\_get\_google\_font\_uri

```php
apply_filters( 'make_get_google_font_uri', $url );
```

##### Description

Filter the Google Fonts URL.

##### Parameters:


* **$url**: _(string)_ The URL to retrieve the Google Fonts.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/font/source/google.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/google.php#L267)

### make\_font\_variants

```php
apply_filters( 'make_font_variants', $variants, $font, $variants );
```

##### Description

Allow developers to alter the font variant choice.

##### Parameters:


* **$variants**: _(array)_ The list of variants for a font.

* **$font**: _(string)_ The font to load variants for.

* **$variants**: _(array)_ The variants for the font.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/font/source/google.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/google.php#L359)

### make\_font\_google\_variants

```php
apply_filters( 'make_font_google_variants', $variants, $font, $variants );
```

##### Description

Allow developers to alter the Google font variant choice.

##### Parameters:


* **$variants**: _(array)_ The list of variants for a font.

* **$font**: _(string)_ The font to load variants for.

* **$variants**: _(array)_ The variants for the font.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/font/source/google.php](https://github.com/thethemefoundry/make/blob/master/src/inc/font/source/google.php#L371)

### make\_format\_builder\_format\_models

```php
apply_filters( 'make_format_builder_format_models', $models );
```

##### Description

Filter the format model definitions and their script locations.
model => URI of the model's script file

##### Parameters:


* **$models**: _(array)_ The array of format models.

##### Changelog:


* **Since**: 1.4.1

##### Source:

* [src/inc/formatting/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/formatting/manager.php#L206)

### make\_style\_formats

```php
apply_filters( 'make_style_formats', $style_formats );
```

##### Description

Filter the styles that are added to the TinyMCE Formats dropdown.

##### Parameters:


* **$style\_formats**: _(array)_ The format items being added to TinyMCE.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/formatting/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/formatting/manager.php#L443)

### make\_jetpack\_infinite\_scroll\_footer\_callback

```php
apply_filters( 'make_jetpack_infinite_scroll_footer_callback', $callback );
```

##### Description

Filter: Change the callback used to render the Infinite Scroll footer.

##### Parameters:


* **$callback**: _(array|string)_ 

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/integration/jetpack.php](https://github.com/thethemefoundry/make/blob/master/src/inc/integration/jetpack.php#L112)

### make\_jetpack\_infinite\_scroll\_render\_callback

```php
apply_filters( 'make_jetpack_infinite_scroll_render_callback', $callback );
```

##### Description

Filter: Change the callback used to render posts retrieved by Infinite Scroll.

##### Parameters:


* **$callback**: _(array|string)_ 

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/integration/jetpack.php](https://github.com/thethemefoundry/make/blob/master/src/inc/integration/jetpack.php#L130)

### make\_add\_integration\_'.$integration\_nam

```php
apply_filters( 'make_add_integration_' . $integration_name, $add_integration );
```

##### Description

Filter: Prevent an integration from being added.

##### Parameters:


* **$add\_integration**: _(bool)_ True to allow the integration to be added.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/integration/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/integration/manager.php#L64)

### make\_get\_view

```php
apply_filters( 'make_get_view', $view, $parent_post_type );
```

##### Description

Allow developers to dynamically change the view.

##### Parameters:


* **$view**: _(string)_ The view name.

* **$parent\_post\_type**: _(string)_ The post type for the parent post of the current post.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/layout/view.php](https://github.com/thethemefoundry/make/blob/master/src/inc/layout/view.php#L414)

### ttfmake\_custom\_logo\_information

```php
apply_filters( 'ttfmake_custom_logo_information', $logo_information );
```

##### Description

Filter the URL and dimensions of the custom logo.
This filter may be useful if you encounter problems getting your custom
logo to appear. Note, however, that using this filter will hard-code the logo
information and settings in the Logo interface in the Customizer won't be
reflected.

##### Parameters:


* **$logo\_information**: _(array)_ The array of information.

##### Changelog:


* **Since**: 1.0.0.

##### Source:

* [src/inc/logo/legacy.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/legacy.php#L369)

### make\_logo\_information

```php
apply_filters( 'make_logo_information', $logo_information );
```

##### Description

Filter the URL and dimensions of the custom logo.
This filter may be useful if you encounter problems getting your custom
logo to appear. Note, however, that using this filter will hard-code the logo
information and settings in the Logo interface in the Customizer won't be
reflected.

##### Parameters:


* **$logo\_information**: _(array)_ The array of information.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/logo/legacy.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/legacy.php#L384)

### ttfmake\_custom\_logo\_max\_width

```php
apply_filters( 'ttfmake_custom_logo_max_width' );
```

##### Description

This filter is documented in inclogomethods.php

##### Parameters:


##### Changelog:


##### Source:

* [src/inc/logo/legacy.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/legacy.php#L422)

### make\_logo\_max\_width

```php
apply_filters( 'make_logo_max_width' );
```

##### Description

This filter is documented in inclogomethods.php

##### Parameters:


##### Changelog:


##### Source:

* [src/inc/logo/legacy.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/legacy.php#L426)

### make\_logo\_load\_legacy

```php
apply_filters( 'make_logo_load_legacy', $load_legacy );
```

##### Description

Filter: Switch to prevent legacy logo functionality from loading.

##### Parameters:


* **$load\_legacy**: _(bool)_ 

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/logo/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/methods.php#L67)

### ttfmake\_custom\_logo\_max\_width

```php
apply_filters( 'ttfmake_custom_logo_max_width', $width );
```

##### Description

Filter the maximum allowable width for a custom logo.

##### Parameters:


* **$width**: _(int)_ The maximum width, in pixels.

##### Changelog:


* **Since**: 1.0.0.

##### Source:

* [src/inc/logo/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/methods.php#L189)

### make\_logo\_max\_width

```php
apply_filters( 'make_logo_max_width', $width );
```

##### Description

Filter the maximum allowable width for a custom logo.

##### Parameters:


* **$width**: _(int)_ The maximum width, in pixels.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/logo/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/logo/methods.php#L199)

### make\_is\_plus

```php
apply_filters( 'make_is_plus', $is_plus );
```

##### Description

Filter: Modify the status of Make Plus.

##### Parameters:


* **$is\_plus**: _(bool)_ True if Make Plus is active.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/plus/methods.php](https://github.com/thethemefoundry/make/blob/master/src/inc/plus/methods.php#L127)

### make\_settings\_{$this->type}\_current\_value

```php
apply_filters( "make_settings_{$this->type}_current_value", $value, $setting_id, $context );
```

##### Description

Filter: Modify the current value for a particular setting.

##### Parameters:


* **$value**: _(mixed)_ The current value of the setting.

* **$setting\_id**: _(string)_ The id of the setting.

* **$context**: _(string)_ Optional. The context in which a setting needs to be sanitized.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/settings/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/base.php#L341)

### make\_settings\_{$this->type}\_default\_value

```php
apply_filters( "make_settings_{$this->type}_default_value", $default_value, $setting_id );
```

##### Description

Filter: Modify the default value for a particular setting.

##### Parameters:


* **$default\_value**: _(string|array)_ The default value of the setting.

* **$setting\_id**: _(string)_ The id of the setting.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/settings/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/base.php#L369)

### make\_settings\_{$this->type}\_sanitize\_callback

```php
apply_filters( "make_settings_{$this->type}_sanitize_callback", $callback, $setting_id, $context );
```

##### Description

Filter: Modify the name of the sanitize callback function for a particular setting.

##### Parameters:


* **$callback**: _(string|array)_ The name of the callback function.

* **$setting\_id**: _(string)_ The id of the setting.

* **$context**: _(string)_ The context in which the setting needs to be sanitized.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/settings/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/base.php#L425)

### make\_settings\_{$this->type}\_sanitize\_callback\_parameters

```php
apply_filters( "make_settings_{$this->type}_sanitize_callback_parameters", $value, $setting_id, $callback );
```

##### Description

Filter: Prepare the array of parameters to feed into the sanitize callback function.
Some callbacks may require more than one parameter. This filter provides an opportunity
to add additional items to the array that will become the callback's parameters.

##### Parameters:


* **$value**: _(array)_ The array of parameters, initially containing only the value to be sanitized.

* **$setting\_id**: _(string)_ The id of the setting being sanitized.

* **$callback**: _(string)_ The callable that will accept parameters.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/settings/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/base.php#L482)

### make\_sanitize\_text\_allowed\_tags

```php
apply_filters( 'make_sanitize_text_allowed_tags', $expandedtags, $string );
```

##### Description

Customize the tags and attributes that are allowed during text sanitization.

##### Parameters:


* **$expandedtags**: _(array)_ The list of allowed tags and attributes.

* **$string**: _(string)_ The text string being sanitized.

##### Changelog:


* **Since**: 1.4.3

##### Source:

* [src/inc/settings/sanitize.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/sanitize.php#L120)

### make\_sanitize\_choice

```php
apply_filters( 'make_sanitize_choice', $value, $setting );
```

##### Description

Deprecated: Filter the sanitized value.

##### Parameters:


* **$value**: _(mixed)_ The sanitized value.

* **$setting**: _(string)_ The key for the setting.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/settings/sanitize.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/sanitize.php#L159)

### make\_sanitize\_font\_choice

```php
apply_filters( 'make_sanitize_font_choice', $value );
```

##### Description

Deprecated: Filter the sanitized font choice.

##### Parameters:


* **$value**: _(string)_ The chosen font value.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/settings/sanitize.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/sanitize.php#L198)

### make\_sanitize\_font\_subset

```php
apply_filters( 'make_sanitize_font_subset', $value );
```

##### Description

Filter the sanitized subset choice.

##### Parameters:


* **$value**: _(string)_ The chosen subset value.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/settings/sanitize.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/sanitize.php#L253)

### make\_setting\_defaults

```php
apply_filters( 'make_setting_defaults', $defaults );
```

##### Description

Deprecated: Filter the default values for the settings.

##### Parameters:


* **$defaults**: _(array)_ The list of default settings.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/settings/thememod.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/thememod.php#L173)

### make\_get\_default

```php
apply_filters( 'make_get_default', $default, $option );
```

##### Description

Deprecated: Filter the retrieved default value.

##### Parameters:


* **$default**: _(mixed)_ The default value.

* **$option**: _(string)_ The name of the default value.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/settings/thememod.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/thememod.php#L278)

### make\_setting\_choices

```php
apply_filters( 'make_setting_choices', $choices, $setting_id );
```

##### Description

Filter the setting choices.

##### Parameters:


* **$choices**: _(array)_ The choices for the setting.

* **$setting\_id**: _(string)_ The setting name.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/settings/thememod.php](https://github.com/thethemefoundry/make/blob/master/src/inc/settings/thememod.php#L354)

### make\_content\_width

```php
apply_filters( 'make_content_width', $new_width, $left, $right );
```

##### Description

Filter to modify the $content_width variable.

##### Parameters:


* **$new\_width**: _(int)_ The new content width.

* **$left**: _(bool)_ True if the current view has a left sidebar.

* **$right**: _(bool)_ True if the current view has a right sidebar.

##### Changelog:


* **Since**: 1.4.8

##### Source:

* [src/inc/setup/misc.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/misc.php#L195)

### make\_enqueue\_parent\_stylesheet

```php
apply_filters( 'make_enqueue_parent_stylesheet', $enqueue );
```

##### Description

Filter: Toggle whether the parent stylesheet loads along with the child one.

##### Parameters:


* **$enqueue**: _(bool)_ True enqueues the parent stylesheet.

##### Changelog:


* **Since**: 1.6.0.

##### Source:

* [src/inc/setup/scripts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/scripts.php#L283)

### make\_located\_file\_url

```php
apply_filters( 'make_located_file_url', $url, $file_names );
```

##### Description

Filter: Modify the URL the theme will use to attempt to access a particular file.
This can be used to set the URL for a file if the get_located_file_url() method is not
determining the correct URL.

##### Parameters:


* **$url**: _(string)_ 

* **$file\_names**: _(string|array)_ 

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/setup/scripts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/scripts.php#L437)

### make\_fitvids\_custom\_selectors

```php
apply_filters( 'make_fitvids_custom_selectors', $selector_array );
```

##### Description

Filter: Allow customization of the selectors that are used to apply FitVids.

##### Parameters:


* **$selector\_array**: _(array)_ The selectors used by FitVids.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/setup/scripts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/scripts.php#L647)

### make\_widget\_display\_args

```php
apply_filters( 'make_widget_display_args', $widget_args, $sidebar_id );
```

##### Description

Filter: Modify the wrapper markup parameters for the widgets in a particular sidebar.

##### Parameters:


* **$widget\_args**: _(array)_ The default widget markup for sidebars.

* **$sidebar\_id**: _(string)_ The ID of the sidebar that the widget markup will apply to.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/setup/widgets.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/widgets.php#L95)

### make\_has\_sidebar

```php
apply_filters( 'make_has_sidebar', $has_sidebar, $location, $view );
```

##### Description

Filter: Dynamically change the result of the "has sidebar" check.

##### Parameters:


* **$has\_sidebar**: _(bool)_ Whether or not to show the sidebar.

* **$location**: _(string)_ The location of the sidebar being evaluated.

* **$view**: _(string)_ The view name.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/setup/widgets.php](https://github.com/thethemefoundry/make/blob/master/src/inc/setup/widgets.php#L236)

### make\_supported\_social\_icons

```php
apply_filters( 'make_supported_social_icons', $icons );
```

##### Description

Filter the supported social icons.
This array uses the url pattern for the key and the CSS class (as dictated by Font Awesome) as the array value.
The URL pattern is used to match the URL used by a menu item.

##### Parameters:


* **$icons**: _(array)_ The array of supported social icons.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L284)

### make\_socialicons\_email

```php
apply_filters( 'make_socialicons_email', $icon );
```

##### Description

Filter: Modify the icon definition for an email address.

##### Parameters:


* **$icon**: _(array)_ The icon definition.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L315)

### make\_socialicons\_rss

```php
apply_filters( 'make_socialicons_rss', $icon );
```

##### Description

Filter: Modify the icon definition for an RSS feed.

##### Parameters:


* **$icon**: _(array)_ The icon definition.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L336)

### make\_socialicons\_default

```php
apply_filters( 'make_socialicons_default', $icon );
```

##### Description

Filter: Modify the icon definition for a URL that doesn't match any icon URL pattern.

##### Parameters:


* **$icon**: _(array)_ The icon definition.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L357)

### make\_socialicons\_render\_override

```php
apply_filters( 'make_socialicons_render_override', $override, $icon_data );
```

##### Description

Filter: Override the default social icons rendered output.

##### Parameters:


* **$override**: _(string|null)_ This value will be returned if it is not null.

* **$icon\_data**: _(array)_ The array of icon data to use for rendering.

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/socialicons/manager.php](https://github.com/thethemefoundry/make/blob/master/src/inc/socialicons/manager.php#L647)

### make\_css\_add

```php
apply_filters( 'make_css_add', $data );
```

##### Description

Filter: Modify CSS rules as they are registered.

##### Parameters:


* **$data**: _(array)_ The selectors and properties to add to the CSS.

##### Changelog:


* **Since**: 1.2.3

##### Source:

* [src/inc/style/css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/css.php#L104)

### make\_parse\_declaration

```php
apply_filters( 'make_parse_declaration', $parsed_value, $property, $value, $t, $n );
```

##### Description

Filter: Modify the final CSS declaration after being parsed.

##### Parameters:


* **$parsed\_value**: _(string)_ The full CSS declaration.

* **$property**: _(string)_ The property being parsed.

* **$value**: _(string)_ The value for the property.

* **$t**: _(string)_ The tab character.

* **$n**: _(string)_ The newline character.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/style/css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/css.php#L271)

### make\_css\_parse\_declarations

```php
apply_filters( 'make_css_parse_declarations', $output, $declarations, $tab );
```

##### Description

Filter: Modify the full list of parsed declarations.

##### Parameters:


* **$output**: _(string)_ The full CSS output.

* **$declarations**: _(array)_ The list of CSS declarations.

* **$tab**: _(string)_ The tab character.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/style/css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/css.php#L283)

### make\_font\_relative\_size

```php
apply_filters( 'make_font_relative_size', $sizes );
```

##### Description

Filter the array of relative font sizes.
Each array item defines a percentage by which to scale a font size compared
to some other font size. Most of these were deprecated in version 1.3.0.

##### Parameters:


* **$sizes**: _(array)_ The array of relative sizes.

##### Changelog:


* **Since**: 1.0.0.

##### Source:

* [src/inc/style/datahelper.php](https://github.com/thethemefoundry/make/blob/master/src/inc/style/datahelper.php#L212)

### make\_read\_more\_text

```php
apply_filters( 'make_read_more_text', $read_more_text );
```

##### Description

Deprecated: Filter the value of the read more text.
This filter hook has been deprecated in favor of a theme option in the Customizer. The theme option
will only be available if no filters have been added to the hook.

##### Parameters:


* **$read\_more\_text**: _(string)_ The read more text value.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L171)

### make\_site\_header\_class

```php
apply_filters( 'make_site_header_class', $classes );
```

##### Description

Filter: Modify the classes applied to the site header element.

##### Parameters:


* **$classes**: _(array)_ 

##### Changelog:


* **Since**: 1.7.0.

##### Source:

* [src/inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L249)

### make\_exif\_shutter\_speed

```php
apply_filters( 'make_exif_shutter_speed', $converted_as, $raw_shutter_speed, $attachment_id );
```

##### Description

Filter the shutter speed value.

##### Parameters:


* **$converted\_as**: _(string)_ The shutter speed value.

* **$raw\_shutter\_speed**: _(float)_ The raw shutter speed value.

* **$attachment\_id**: _(int)_ The ID of the attachment.

##### Changelog:


* **Since**: 1.2.3.

* **Since**: 1.7.0.

##### Source:

* [src/inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L346)

### make\_exif\_aperture

```php
apply_filters( 'make_exif_aperture', $f_stop, $raw_aperture, $attachment_id );
```

##### Description

Filter the aperture value.

##### Parameters:


* **$f\_stop**: _(string)_ The aperture value.

* **$raw\_aperture**: _(int)_ The raw aperture value.

* **$attachment\_id**: _(int)_ The ID of the attachment.

##### Changelog:


* **Since**: 1.2.3.

* **Since**: 1.7.0.

##### Source:

* [src/inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L367)

### make\_get\_exif\_data

```php
apply_filters( 'make_get_exif_data', $output, $attachment_id );
```

##### Description

Alter the exif data output.

##### Parameters:


* **$output**: _(string)_ The EXIF data prepared as HTML.

* **$attachment\_id**: _(int)_ The image being generated.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L439)

### make\_breadcrumb\_output

```php
apply_filters( 'make_breadcrumb_output', $breadcrumb, $before, $after );
```

##### Description

Filter: Modify the output of breadcrumb

##### Parameters:


* **$breadcrumb**: _(string)_ The breadcrumb markup.

* **$before**: _(string)_ The wrapper opening markup.

* **$after**: _(string)_ The wrapper closing markup.

##### Changelog:


* **Since**: 1.8.9.

##### Source:

* [src/inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L588)

### make\_entry\_thumbnail\_size

```php
apply_filters( 'make_entry_thumbnail_size', $size, $layout_setting );
```

##### Description

Filter: Modify the image size used to display a post's featured image (post thumbnail)

##### Parameters:


* **$size**: _(string)_ The ID of the image size to use.

* **$layout\_setting**: _(string)_ The value of the featured image layout setting for the current view.

##### Changelog:


* **Since**: 1.7.4.

##### Source:

* [src/inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L626)

### make\_template\_content\_archive

```php
apply_filters( 'make_template_content_archive', $type, $post );
```

##### Description

Allow for changing the template partial.

##### Parameters:


* **$type**: _(string)_ The default template type to use.

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/index.php](https://github.com/thethemefoundry/make/blob/master/src/index.php#L37)

### make\_template\_content\_page

```php
apply_filters( 'make_template_content_page', $type, $post );
```

##### Description

Allow for changing the template partial.

##### Parameters:


* **$type**: _(string)_ The default template type to use.

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/page.php](https://github.com/thethemefoundry/make/blob/master/src/page.php#L25)

### make\_show\_footer\_credit

```php
apply_filters( 'make_show_footer_credit', $show );
```

##### Description

Allow toggling of the footer credit.

##### Parameters:


* **$show**: _(bool)_ Whether or not to show the footer credit.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/partials/footer-credit.php](https://github.com/thethemefoundry/make/blob/master/src/partials/footer-credit.php#L13)

### make\_template\_content\_search

```php
apply_filters( 'make_template_content_search', $type, $post );
```

##### Description

Allow for changing the template partial.

##### Parameters:


* **$type**: _(string)_ The default template type to use.

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/search.php](https://github.com/thethemefoundry/make/blob/master/src/search.php#L30)

### make\_footer\_1

```php
apply_filters( 'make_footer_1', $footer_id );
```

##### Description

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Parameters:


* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/sidebar-footer-1.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-1.php#L13)

### make\_footer\_2

```php
apply_filters( 'make_footer_2', $footer_id );
```

##### Description

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Parameters:


* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/sidebar-footer-2.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-2.php#L13)

### make\_footer\_3

```php
apply_filters( 'make_footer_3', $footer_id );
```

##### Description

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Parameters:


* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/sidebar-footer-3.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-3.php#L13)

### make\_footer\_4

```php
apply_filters( 'make_footer_4', $footer_id );
```

##### Description

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Parameters:


* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/sidebar-footer-4.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-4.php#L13)

### make\_sidebar\_left

```php
apply_filters( 'make_sidebar_left', $footer_id );
```

##### Description

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Parameters:


* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/sidebar-left.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-left.php#L13)

### make\_sidebar\_right

```php
apply_filters( 'make_sidebar_right', $footer_id );
```

##### Description

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

##### Parameters:


* **$footer\_id**: _(string)_ The ID of the current footer being generated.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/sidebar-right.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-right.php#L13)

### make\_template\_content\_single

```php
apply_filters( 'make_template_content_single', $type, $post );
```

##### Description

Allow for changing the template partial.

##### Parameters:


* **$type**: _(string)_ The default template type to use.

* **$post**: _(WP\_Post)_ The post object for the current post.

##### Changelog:


* **Since**: 1.2.3.

##### Source:

* [src/single.php](https://github.com/thethemefoundry/make/blob/master/src/single.php#L25)
