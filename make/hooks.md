# Actions: 16

## make\_after\_builder\_menu \{.make\}

```
do_action( 'make_after_builder_menu' );
```

Execute code after the builder menu is displayed.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/templates/menu.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/menu.php#L42)

## make\_after\_builder\_stage \{.make\}

```
do_action( 'make_after_builder_stage' );
```

Execute code after the builder stage is displayed.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/templates/stage-footer.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/stage-footer.php#L11)

## make\_before\_builder\_menu \{.make\}

```
do_action( 'make_before_builder_menu' );
```

Execute code before the builder menu is displayed.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/templates/menu.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/menu.php#L18)

## make\_before\_builder\_stage \{.make\}

```
do_action( 'make_before_builder_stage' );
```

Execute code before the builder stage is displayed.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/templates/stage-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/stage-header.php#L16)

## make\_before\_section\_header \{.make\}

```
do_action( 'make_before_section_header' );
```

Execute code before the section header is displayed.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/templates/section-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/section-header.php#L40)

## make\_builder\_data\_saved \{.make\}

```
do_action( 'make_builder_data_saved', $sections, $post_id );
```

Execute code after the section data is saved.

#### Description

While it is possible to use a "save\_post" to hook into the save routine, this action is preferred as it is only called after all validation and sanitization is completed.

#### Parameters

* **$sections**: _(array)_ The clean section data.
* **$post\_id**: _(int)_ The post ID for the saved data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L196)

## make\_builder\_{$data\['section-type'\]}\_css \{.make\}

```
do_action( 'make_builder_{$data['section-type']}_css', $data, $id );
```

Allow section-specific CSS rules to be added to the document head of a Builder page.

#### Parameters

* **$data**: _(array)_ The Builder section's data.
* **$id**: _(int)_ The ID of the Builder section.

#### Changelog

* **Since**: 1.4.5

#### Source

* [inc/extras.php](https://github.com/thethemefoundry/make/blob/master/src/inc/extras.php#L592)

## make\_css \{.make\}

```
do_action( 'make_css' );
```

The hook used to add CSS rules for the generated inline CSS.

#### Description

This hook is the correct hook to use for adding CSS styles to the group of selectors and properties that will be added to inline CSS that is printed in the head. Hooking elsewhere may lead to rules not being registered correctly for the CSS generation. Most Customizer options will use this hook to register additional CSS rules.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/bootstrap.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/bootstrap.php#L568)

## make\_section\_text\_after\_column \{.make\}

```
do_action( 'make_section_text_after_column', $ttfmake_section_data );
```

Execute code after an individual text column is displayed.

#### Parameters

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L142)

## make\_section\_text\_after\_columns \{.make\}

```
do_action( 'make_section_text_after_columns', $ttfmake_section_data );
```

Execute code after all columns are displayed.

#### Parameters

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L198)

## make\_section\_text\_after\_columns\_select \{.make\}

```
do_action( 'make_section_text_after_columns_select', $ttfmake_section_data );
```

Execute code after the columns select input is displayed.

#### Parameters

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L54)

## make\_section\_text\_after\_title \{.make\}

```
do_action( 'make_section_text_after_title', $ttfmake_section_data );
```

Execute code after the section title is displayed.

#### Parameters

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L63)

## make\_section\_text\_before\_column \{.make\}

```
do_action( 'make_section_text_before_column', $ttfmake_section_data );
```

Execute code before an individual text column is displayed.

#### Parameters

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L120)

## make\_section\_text\_before\_columns\_select \{.make\}

```
do_action( 'make_section_text_before_columns_select', $ttfmake_section_data );
```

Execute code before the columns select input is displayed.

#### Parameters

* **$ttfmake\_section\_data**: _(array)_ The data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L45)

## make\_section\_{$ttfmake\_section\_data\['section'\]\['id'\]}\_after \{.make\}

```
do_action( 'make_section_{$ttfmake_section_data['section']['id']}_after', $ttfmake_section_data );
```

Allow for script execution in the footer of a builder section.

#### Description

This action is a variable action that allows a developer to hook into specific section types (e.g., 'text'). Do not confuse "id" in this context as the individual section id (e.g., 14092814910).

#### Parameters

* **$ttfmake\_section\_data**: _(array)_ The array of data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L846)

## make\_section\_{$ttfmake\_section\_data\['section'\]\['id'\]}\_before \{.make\}

```
do_action( 'make_section_{$ttfmake_section_data['section']['id']}_before', $ttfmake_section_data );
```

Allow for script execution in the header of a builder section.

#### Description

This action is a variable action that allows a developer to hook into specific section types (e.g., 'text'). Do not confuse "id" in this context as the individual section id (e.g., 14092814910).

#### Parameters

* **$ttfmake\_section\_data**: _(array)_ The array of data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L817)

# Filters: 109

## make\_add\_section \{.make\}

```
apply_filters( 'make_add_section', $section );
```

Allow the added sections to be filtered.

#### Description

This filters allows for dynamically altering sections as they get added. This can help enforce policies for sections by sanitizing the registered values.

#### Returns

* **$section**: _(array)_ The section being added.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/api.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/api.php#L96)

## make\_all\_font\_choices \{.make\}

```
apply_filters( 'make_all_font_choices', $choices );
```

Allow for developers to modify the full list of fonts.

#### Returns

* **$choices**: _(array)_ The list of all fonts.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L638)

## make\_all\_fonts \{.make\}

```
apply_filters( 'make_all_fonts', $fonts );
```

Allow for developers to modify the full list of fonts.

#### Returns

* **$fonts**: _(array)_ The list of all fonts.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L684)

## make\_banner\_slide\_configuration \{.make\}

```
apply_filters( 'make_banner_slide_configuration' );
```

#### Source

* [inc/builder/sections/builder-templates/banner-slide.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/banner-slide.php#L63)

## make\_builder\_banner\_class \{.make\}

```
apply_filters( 'make_builder_banner_class', $banner_class, $ttfmake_section_data );
```

Filter the class for the banner section.

#### Returns

* **$banner\_class**: _(string)_ The banner class.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ The section data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L410)

## make\_builder\_banner\_slide\_class \{.make\}

```
apply_filters( 'make_builder_banner_slide_class', $slide_class );
```

Allow developers to alter the class for the banner slide.

#### Returns

* **$slide\_class**: _(string)_ The banner classes.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L497)

## make\_builder\_banner\_slide\_style \{.make\}

```
apply_filters( 'make_builder_banner_slide_style', $slide_style, $slide, $ttfmake_section_data );
```

Allow developers to change the CSS for a Banner section.

#### Returns

* **$slide\_style**: _(string)_ The CSS for the banner.

#### Other parameters

* **$slide**: _(array)_ The slide data.
* **$ttfmake\_section\_data**: _(array)_ The section data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L534)

## make\_builder\_get\_banner\_array \{.make\}

```
apply_filters( 'make_builder_get_banner_array', $banner_array, $ttfmake_section_data );
```

Filter the data array for a banner section.

#### Returns

* **$banner\_array**: _(array)_ The ordered banner data.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ All of the data for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L383)

## make\_builder\_get\_banner\_slider\_atts \{.make\}

```
apply_filters( 'make_builder_get_banner_slider_atts', $data_attributes, $ttfmake_section_data );
```

Allow for altering the banner slider attributes.

#### Returns

* **$data\_attributes**: _(string)_ The data attributes in string form.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ The section data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L471)

## make\_builder\_get\_gallery\_array \{.make\}

```
apply_filters( 'make_builder_get_gallery_array', $gallery_array, $ttfmake_section_data );
```

Filter the gallery item data.

#### Returns

* **$gallery\_array**: _(array)_ The array of gallery item data.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ The section data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L68)

## make\_builder\_get\_gallery\_item\_class \{.make\}

```
apply_filters( 'make_builder_get_gallery_item_class', $gallery_class, $item, $ttfmake_section_data, $i );
```

Filter the class used for a gallery item.

#### Returns

* **$gallery\_class**: _(string)_ The computed gallery class.

#### Other parameters

* **$item**: _(array)_ The item's data.
* **$ttfmake\_section\_data**: _(array)_ The section data.
* **$i**: _(int)_ The current gallery item number.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L217)

## make\_builder\_get\_gallery\_item\_image \{.make\}

```
apply_filters( 'make_builder_get_gallery_item_image', $image, $item, $aspect );
```

Alter the generated gallery image.

#### Returns

* **$image**: _(string)_ The image HTML.

#### Other parameters

* **$item**: _(array)_ The item's data.
* **$aspect**: _(string)_ The aspect ratio for the section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L260)

## make\_builder\_get\_gallery\_style \{.make\}

```
apply_filters( 'make_builder_get_gallery_style', $gallery_style, $ttfmake_section_data );
```

Filter the style added to a gallery section.

#### Returns

* **$gallery\_style**: _(string)_ The style applied to the gallery.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ The section data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L171)

## make\_builder\_get\_text\_array \{.make\}

```
apply_filters( 'make_builder_get_text_array', $columns_array, $ttfmake_section_data );
```

Filter the array of builder data for the text section.

#### Returns

* **$columns\_array**: _(array)_ The ordered data for the text section.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ The raw section data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L308)

## make\_builder\_get\_text\_class \{.make\}

```
apply_filters( 'make_builder_get_text_class', $text_class, $ttfmake_section_data, $sections );
```

Filter the text section class.

#### Returns

* **$text\_class**: _(string)_ The computed class string.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ The section data.
* **$sections**: _(array)_ The list of sections.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L343)

## make\_builder\_is\_section\_type \{.make\}

```
apply_filters( 'make_builder_is_section_type', $is_section_type, $type, $data );
```

Allow developers to alter if a set of data is a specified section type.

#### Returns

* **$is\_section\_type**: _(bool)_ Whether or not the data represents a specific section.

#### Other parameters

* **$type**: _(string)_ The section type to check.
* **$data**: _(array)_ The section data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L27)

## make\_builder\_section\_links \{.make\}

```
apply_filters( 'make_builder_section_links' );
```

#### Source

* [inc/builder/core/templates/section-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/section-header.php#L27)

## make\_column\_buttons \{.make\}

```
apply_filters( 'make_column_buttons', $column_buttons, $ttfmake_section_data );
```

Filter the buttons added to a text column.

#### Returns

* **$column\_buttons**: _(array)_ The current list of buttons.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ All data for the section.

#### Changelog

* **Since**: 1.4.0.

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L104)

## make\_column\_configuration \{.make\}

```
apply_filters( 'make_column_configuration' );
```

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L153)

## make\_configuration\_overlay\_input \{.make\}

```
apply_filters( 'make_configuration_overlay_input', $this_output, $args, $section_data );
```

Filter the HTML for the input.

#### Returns

* **$this\_output**: _(string)_ The HTML for the input.

#### Other parameters

* **$args**: _(string)_ The input data.
* **$section\_data**: _(string)_ The data for the section.

#### Changelog

* **Since**: 1.4.0.

#### Source

* [inc/builder/core/configuration-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/configuration-helpers.php#L200)

## make\_configuration\_overlay\_input\_wrap \{.make\}

```
apply_filters( 'make_configuration_overlay_input_wrap', $wrapper, $args, $section_data );
```

Filter the wrapped used for the inputs.

#### Returns

* **$wrapper**: _(string)_ The HTML to wrap around the input.

#### Other parameters

* **$args**: _(string)_ The input data that is wrapped.
* **$section\_data**: _(string)_ The data for the section.

#### Changelog

* **Since**: 1.4.0.

#### Source

* [inc/builder/core/configuration-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/configuration-helpers.php#L189)

## make\_css\_add \{.make\}

```
apply_filters( 'make_css_add', $data );
```

Filter CSS as it is registered.

#### Returns

* **$data**: _(array)_ The selectors and properties to add to the CSS.

#### Changelog

* **Since**: 1.2.3

#### Source

* [inc/customizer/helpers-css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-css.php#L122)

## make\_css\_font\_properties \{.make\}

```
apply_filters( 'make_css_font_properties' );
```

Body

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L255)

## make\_css\_parse\_declarations \{.make\}

```
apply_filters( 'make_css_parse_declarations', $output, $declarations, $tab );
```

Filter the full list of parsed declarations.

#### Returns

* **$output**: _(string)_ The full CSS output.

#### Other parameters

* **$declarations**: _(array)_ The list of CSS declarations.
* **$tab**: _(string)_ The tab character.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-css.php#L280)

## make\_customizer\_colorscheme\_sections \{.make\}

```
apply_filters( 'make_customizer_colorscheme_sections' );
```

Footer

#### Source

* [inc/customizer/sections/color-scheme.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/sections/color-scheme.php#L210)

## make\_customizer\_contentlayout\_sections \{.make\}

```
apply_filters( 'make_customizer_contentlayout_sections' );
```

Pages

#### Source

* [inc/customizer/sections/content-layout.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/sections/content-layout.php#L938)

## make\_customizer\_footer\_sections \{.make\}

```
apply_filters( 'make_customizer_footer_sections' );
```

White Label

#### Source

* [inc/customizer/sections/footer.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/sections/footer.php#L170)

## make\_customizer\_general\_sections \{.make\}

```
apply_filters( 'make_customizer_general_sections' );
```

Social Profiles & RSS

#### Source

* [inc/customizer/sections/general.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/sections/general.php#L239)

## make\_customizer\_header\_sections \{.make\}

```
apply_filters( 'make_customizer_header_sections' );
```

Layout

#### Source

* [inc/customizer/sections/header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/sections/header.php#L159)

## make\_customizer\_key\_conversions \{.make\}

```
apply_filters( 'make_customizer_key_conversions' );
```

Sets are defined by the theme version they pertain to: $theme\_version => array     $old => $new

#### Source

* [inc/compatibility.php](https://github.com/thethemefoundry/make/blob/master/src/inc/compatibility.php#L206)

## make\_customizer\_panels \{.make\}

```
apply_filters( 'make_customizer_panels' );
```

#### Source

* [inc/customizer/bootstrap.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/bootstrap.php#L75)

## make\_customizer\_sections \{.make\}

```
apply_filters( 'make_customizer_sections' );
```

#### Source

* [inc/customizer/bootstrap.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/bootstrap.php#L127)

## make\_customizer\_typography\_sections \{.make\}

```
apply_filters( 'make_customizer_typography_sections' );
```

Headers & Body

#### Source

* [inc/customizer/sections/typography.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/sections/typography.php#L358)

## make\_exif\_aperture \{.make\}

```
apply_filters( 'make_exif_aperture', $f_stop, $raw_aperture );
```

Filter the aperture value.

#### Returns

* **$f\_stop**: _(string)_ The aperture value.

#### Other parameters

* **$raw\_aperture**: _(int)_ The raw aperture value.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L523)

## make\_exif\_shutter\_speed \{.make\}

```
apply_filters( 'make_exif_shutter_speed', $converted_as, $raw_shutter_speed );
```

Filter the shutter speed value.

#### Returns

* **$converted\_as**: _(string)_ The shutter speed value.

#### Other parameters

* **$raw\_shutter\_speed**: _(float)_ The raw shutter speed value.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L504)

## make\_fitvids\_custom\_selectors \{.make\}

```
apply_filters( 'make_fitvids_custom_selectors', $selector_array );
```

Allow for changing of the selectors that are used to apply FitVids.

#### Returns

* **$selector\_array**: _(array)_ The selectors used by FitVids.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [functions.php](https://github.com/thethemefoundry/make/blob/master/src/functions.php#L342)

## make\_font\_relative\_size \{.make\}

```
apply_filters( 'make_font_relative_size' );
```

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L16)

## make\_font\_stack \{.make\}

```
apply_filters( 'make_font_stack', $stack, $font );
```

Allow developers to filter the full font stack.

#### Returns

* **$stack**: _(string)_ The font stack.

#### Other parameters

* **$font**: _(string)_ The font.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L310)

## make\_font\_variants \{.make\}

```
apply_filters( 'make_font_variants', $variants, $font );
```

Allow developers to alter the font variant choice.

#### Returns

* **$variants**: _(array)_ The variants for the font.

#### Other parameters

* **$font**: _(string)_ The font to load variants for.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L510)

## make\_footer\_1 \{.make\}

```
apply_filters( 'make_footer_1', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

#### Returns

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [sidebar-footer-1.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-1.php#L13)

## make\_footer\_2 \{.make\}

```
apply_filters( 'make_footer_2', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

#### Returns

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [sidebar-footer-2.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-2.php#L13)

## make\_footer\_3 \{.make\}

```
apply_filters( 'make_footer_3', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

#### Returns

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [sidebar-footer-3.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-3.php#L13)

## make\_footer\_4 \{.make\}

```
apply_filters( 'make_footer_4', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

#### Returns

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [sidebar-footer-4.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-footer-4.php#L13)

## make\_format\_builder\_format\_models \{.make\}

```
apply_filters( 'make_format_builder_format_models' );
```

Format Builder

#### Source

* [inc/formatting/formatting.php](https://github.com/thethemefoundry/make/blob/master/src/inc/formatting/formatting.php#L294)

## make\_gallery\_class \{.make\}

```
apply_filters( 'make_gallery_class', $gallery_class, $ttfmake_section_data, $sections );
```

Filter the class applied to a gallery.

#### Returns

* **$gallery\_class**: _(string)_ The class applied to the gallery.

#### Other parameters

* **$ttfmake\_section\_data**: _(array)_ The section data.
* **$sections**: _(array)_ The list of sections.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-front-end-helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-front-end-helpers.php#L125)

## make\_gallery\_item\_configuration \{.make\}

```
apply_filters( 'make_gallery_item_configuration' );
```

#### Source

* [inc/builder/sections/builder-templates/gallery-item.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/gallery-item.php#L61)

## make\_generate\_post\_content \{.make\}

```
apply_filters( 'make_generate_post_content', $post_content, $data );
```

Filter the generated post content.

#### Description

This content is the full HTML version of the content that will be saved as "post\_content".

#### Returns

* **$post\_content**: _(string)_ The fully generated post content.

#### Other parameters

* **$data**: _(array)_ The data used to generate the content.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L385)

## make\_get\_default \{.make\}

```
apply_filters( 'make_get_default', $default, $option );
```

Filter the retrieved default value.

#### Returns

* **$default**: _(mixed)_ The default value.

#### Other parameters

* **$option**: _(string)_ The name of the default value.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-defaults.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-defaults.php#L273)

## make\_get\_exif\_data \{.make\}

```
apply_filters( 'make_get_exif_data', $output, $attachment_id );
```

Alter the exif data output.

#### Returns

* **$output**: _(string)_ The EXIF data prepared as HTML.

#### Other parameters

* **$attachment\_id**: _(int)_ The image being generated.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L576)

## make\_get\_google\_font\_subsets \{.make\}

```
apply_filters( 'make_get_google_font_subsets', $subsets );
```

Filter the list of supported Google Font subsets.

#### Returns

* **$subsets**: _(array)_ The list of subsets.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L555)

## make\_get\_google\_font\_uri \{.make\}

```
apply_filters( 'make_get_google_font_uri', $url );
```

Filter the Google Fonts URL.

#### Returns

* **$url**: _(string)_ The URL to retrieve the Google Fonts.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L457)

## make\_get\_google\_fonts \{.make\}

```
apply_filters( 'make_get_google_fonts', $fonts );
```

Allow developers to modify the allowed Google fonts.

#### Returns

* **$fonts**: _(array)_ The list of Google fonts with variants and subsets.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/google-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/google-fonts.php#L24)

## make\_get\_image \{.make\}

```
apply_filters( 'make_get_image', $return, $image_id, $size );
```

Filter the image HTML.

#### Returns

* **$return**: _(string)_ The image HTML.

#### Other parameters

* **$image\_id**: _(int)_ The ID for the image.
* **$size**: _(bool)_ The requested image size.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L991)

## make\_get\_image\_src \{.make\}

```
apply_filters( 'make_get_image_src', $src, $image_id, $size );
```

Filter the image source attributes.

#### Returns

* **$src**: _(string)_ The image source attributes.

#### Other parameters

* **$image\_id**: _(int)_ The ID for the image.
* **$size**: _(bool)_ The requested image size.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L1036)

## make\_get\_next\_section\_data \{.make\}

```
apply_filters( 'make_get_next_section_data', $next_data, $current_section, $sections );
```

Allow developers to alter the "next" section data.

#### Returns

* **$next\_data**: _(array)_ The data for the next section.

#### Other parameters

* **$current\_section**: _(array)_ The data for the current section.
* **$sections**: _(array)_ The list of all sections.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L518)

## make\_get\_placeholder\_image \{.make\}

```
apply_filters( 'make_get_placeholder_image', $return, $image_id, $ttfmake_placeholder_images );
```

Filter the image source attributes.

#### Returns

* **$return**: _(string)_ The image source attributes.

#### Other parameters

* **$image\_id**: _(int)_ The ID for the image.
* **$ttfmake\_placeholder\_images**: _(bool)_ The list of placeholder images.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L1068)

## make\_get\_section\_data \{.make\}

```
apply_filters( 'make_get_section_data', $ordered_data, $post_id );
```

Filter the section data for a post.

#### Returns

* **$ordered\_data**: _(array)_ The array of section data.

#### Other parameters

* **$post\_id**: _(int)_ The post ID for the retrieved data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/extras.php](https://github.com/thethemefoundry/make/blob/master/src/inc/extras.php#L474)

## make\_get\_section\_default \{.make\}

```
apply_filters( 'make_get_section_default', $value, $key, $section_type );
```

Filter the default section data that is received.

#### Returns

* **$value**: _(mixed)_ The section value.

#### Other parameters

* **$key**: _(string)_ The key to get data for.
* **$section\_type**: _(string)_ The type of section the data is for.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L734)

## make\_get\_section\_name \{.make\}

```
apply_filters( 'make_get_section_name', $name, $data, $is_js_template );
```

Alter section name.

#### Returns

* **$name**: _(string)_ The name of the section.

#### Other parameters

* **$data**: _(array)_ The section data.
* **$is\_js\_template**: _(bool)_ Whether or not this is in the context of a JS template.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L952)

## make\_get\_standard\_fonts \{.make\}

```
apply_filters( 'make_get_standard_fonts', $fonts );
```

Allow for developers to modify the standard fonts.

#### Returns

* **$fonts**: _(array)_ The list of standard fonts.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L704)

## make\_get\_view \{.make\}

```
apply_filters( 'make_get_view', $view, $parent_post_type );
```

Allow developers to dynamically change the view.

#### Returns

* **$view**: _(string)_ The view name.

#### Other parameters

* **$parent\_post\_type**: _(string)_ The post type for the parent post of the current post.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/extras.php](https://github.com/thethemefoundry/make/blob/master/src/inc/extras.php#L296)

## make\_get\_wp\_editor\_id \{.make\}

```
apply_filters( 'make_get_wp_editor_id', $id, $data, $is_js_template );
```

Alter the wp\_editor ID.

#### Returns

* **$id**: _(string)_ The ID for the editor.

#### Other parameters

* **$data**: _(array)_ The section data.
* **$is\_js\_template**: _(bool)_ Whether or not this is in the context of a JS template.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L920)

## make\_has\_sidebar \{.make\}

```
apply_filters( 'make_has_sidebar', $show_sidebar, $location, $view );
```

Allow developers to dynamically changed the result of the "has sidebar" check.

#### Returns

* **$show\_sidebar**: _(bool)_ Whether or not to show the sidebar.

#### Other parameters

* **$location**: _(string)_ The location of the sidebar being evaluated.
* **$view**: _(string)_ The view name.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/extras.php](https://github.com/thethemefoundry/make/blob/master/src/inc/extras.php#L338)

## make\_insert\_post\_data\_sections \{.make\}

```
apply_filters( 'make_insert_post_data_sections', $data );
```

Filter the section data.

#### Returns

* **$data**: _(array)_ The sanitized data.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L308)

## make\_is\_builder\_page \{.make\}

```
apply_filters( 'make_is_builder_page', $is_builder_page, $post_id );
```

Allow a developer to dynamically change whether the post uses the builder or not.

#### Returns

* **$is\_builder\_page**: _(bool)_ Whether or not the post uses the builder.

#### Other parameters

* **$post\_id**: _(int)_ The ID of post being evaluated.

#### Changelog

* **Since**: 1.2.3

#### Source

* [inc/extras.php](https://github.com/thethemefoundry/make/blob/master/src/inc/extras.php#L564)

## make\_load\_section\_template \{.make\}

```
apply_filters( 'make_load_section_template', $templates, $slug, $path );
```

Filter the templates to try and load.

#### Returns

* **$templates**: _(array)_ The list of template to try and load.

#### Other parameters

* **$slug**: _(string)_ The template slug.
* **$path**: _(string)_ The path to the template.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L879)

## make\_parse\_declaration \{.make\}

```
apply_filters( 'make_parse_declaration', $parsed_value, $property, $value, $t, $n );
```

Filter the final CSS declaration after being parsed.

#### Returns

* **$parsed\_value**: _(string)_ The full CSS declaration.

#### Other parameters

* **$property**: _(string)_ The property being parsed.
* **$value**: _(string)_ The value for the property.
* **$t**: _(string)_ The tab character.
* **$n**: _(string)_ The newline character.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-css.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-css.php#L268)

## make\_prepare\_data \{.make\}

```
apply_filters( 'make_prepare_data', $clean_sections, $sections, $order );
```

Filter the full set of data for a post.

#### Returns

* **$clean\_sections**: _(array)_ The clean sections.

#### Other parameters

* **$sections**: _(array)_ The raw sections.
* **$order**: _(array)_ The order for the sections.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L157)

## make\_prepare\_data\_section \{.make\}

```
apply_filters( 'make_prepare_data_section', $data, $section_type );
```

Filter the prepared data for an individual section.

#### Description

The result of the call\_user\_func\_array() call is an array of data representing the data for the section. This filter allows a developer to alter that data after it is handled.

#### Returns

* **$data**: _(array)_ The raw section data.

#### Other parameters

* **$section\_type**: _(string)_ The type of section being handled.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L141)

## make\_read\_more\_text \{.make\}

```
apply_filters( 'make_read_more_text', $read_more_text );
```

Filter the value of the read more text.

#### Returns

* **$read\_more\_text**: _(string)_ The read more text value.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L164)

## make\_sanitize\_choice \{.make\}

```
apply_filters( 'make_sanitize_choice', $value, $setting );
```

Filter the sanitized value.

#### Returns

* **$value**: _(mixed)_ The sanitized value.

#### Other parameters

* **$setting**: _(string)_ The key for the setting.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers.php#L36)

## make\_sanitize\_font\_choice \{.make\}

```
apply_filters( 'make_sanitize_font_choice', $value );
```

Filter the sanitized font choice.

#### Returns

* **$value**: _(string)_ The chosen font value.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L596)

## make\_sanitize\_font\_subset \{.make\}

```
apply_filters( 'make_sanitize_font_subset', $value );
```

Filter the sanitized subset choice.

#### Returns

* **$value**: _(string)_ The chosen subset value.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-fonts.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-fonts.php#L535)

## make\_sanitize\_section\_choice \{.make\}

```
apply_filters( 'make_sanitize_section_choice', $value, $key, $section_type );
```

Allow developers to alter a section choice during the sanitization process.

#### Returns

* **$value**: _(mixed)_ The value for the section choice.

#### Other parameters

* **$key**: _(string)_ The key for the section choice.
* **$section\_type**: _(string)_ The section type.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L781)

## make\_sanitize\_text\_allowed\_tags \{.make\}

```
apply_filters( 'make_sanitize_text_allowed_tags', $expandedtags, $string );
```

Customize the tags and attributes that are allows during text sanitization.

#### Returns

* **$expandedtags**: _(array)_ The list of allowed tags and attributes.

#### Other parameters

* **$string**: _(string)_ The text string being sanitized.

#### Changelog

* **Since**: 1.4.3

#### Source

* [inc/extras.php](https://github.com/thethemefoundry/make/blob/master/src/inc/extras.php#L148)

## make\_section\_choices \{.make\}

```
apply_filters( 'make_section_choices', $choices, $key, $section_type );
```

Filter the section choices.

#### Returns

* **$choices**: _(array)_ The default section choices.

#### Other parameters

* **$key**: _(string)_ The key for the data.
* **$section\_type**: _(string)_ The type of section this relates to.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L705)

## make\_section\_classes \{.make\}

```
apply_filters( 'make_section_classes', $classes, $current_section );
```

Filter the section classes.

#### Returns

* **$classes**: _(string)_ The sting of classes.

#### Other parameters

* **$current\_section**: _(array)_ The array of data for the current section.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L587)

## make\_section\_defaults \{.make\}

```
apply_filters( 'make_section_defaults', $defaults );
```

Filter the section defaults.

#### Returns

* **$defaults**: _(array)_ The default section data

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/sections/section-definitions.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/section-definitions.php#L676)

## make\_setting\_choices \{.make\}

```
apply_filters( 'make_setting_choices', $choices, $setting );
```

Filter the setting choices.

#### Returns

* **$choices**: _(array)_ The choices for the setting.

#### Other parameters

* **$setting**: _(string)_ The setting name.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers.php#L207)

## make\_setting\_defaults \{.make\}

```
apply_filters( 'make_setting_defaults', $defaults );
```

Filter the default values for the settings.

#### Returns

* **$defaults**: _(array)_ The list of default settings.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers-defaults.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-defaults.php#L248)

## make\_show\_footer\_credit \{.make\}

```
apply_filters( 'make_show_footer_credit', $show );
```

Allow toggling of the footer credit.

#### Returns

* **$show**: _(bool)_ Whether or not to show the footer credit.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [partials/footer-credit.php](https://github.com/thethemefoundry/make/blob/master/src/partials/footer-credit.php#L15)

## make\_sidebar\_left \{.make\}

```
apply_filters( 'make_sidebar_left', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

#### Returns

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [sidebar-left.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-left.php#L13)

## make\_sidebar\_list\_enabled \{.make\}

```
apply_filters( 'make_sidebar_list_enabled', $enabled_views, $location );
```

Filter the list of sidebars that are available for a specific location.

#### Returns

* **$enabled\_views**: _(array)_ The list of views enabled for the sidebar.

#### Other parameters

* **$location**: _(string)_ The location of the sidebar being evaulated.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/extras.php](https://github.com/thethemefoundry/make/blob/master/src/inc/extras.php#L421)

## make\_sidebar\_right \{.make\}

```
apply_filters( 'make_sidebar_right', $footer_id );
```

Filter the sidebar ID to allow developers to programmatically change the sidebar displayed.

#### Returns

* **$footer\_id**: _(string)_ The ID of the current footer being generated.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [sidebar-right.php](https://github.com/thethemefoundry/make/blob/master/src/sidebar-right.php#L13)

## make\_social\_links \{.make\}

```
apply_filters( 'make_social_links', $services_with_links );
```

Filter the social links added to the site.

#### Returns

* **$services\_with\_links**: _(array)_ The social services and links.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/customizer/helpers.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers.php#L360)

## make\_style\_formats \{.make\}

```
apply_filters( 'make_style_formats', $style_formats );
```

Filter the styles that are added to the TinyMCE Formats dropdown.

#### Returns

* **$style\_formats**: _(array)_ The format items being added to TinyMCE.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/formatting/formatting.php](https://github.com/thethemefoundry/make/blob/master/src/inc/formatting/formatting.php#L417)

## make\_supported\_social\_icons \{.make\}

```
apply_filters( 'make_supported_social_icons', $icons );
```

Filter the supported social icons.

#### Description

This array uses the url pattern for the key and the CSS class (as dictated by Font Awesome) as the array value. The URL pattern is used to match the URL used by a menu item.

#### Returns

* **$icons**: _(array)_ The array of supported social icons.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/template-tags.php](https://github.com/thethemefoundry/make/blob/master/src/inc/template-tags.php#L354)

## make\_template\_content\_archive \{.make\}

```
apply_filters( 'make_template_content_archive', $type, $post );
```

Allow for changing the template partial.

#### Returns

* **$type**: _(string)_ The default template type to use.

#### Other parameters

* **$post**: _(WP\_Post)_ The post object for the current post.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [index.php](https://github.com/thethemefoundry/make/blob/master/src/index.php#L25)

## make\_template\_content\_page \{.make\}

```
apply_filters( 'make_template_content_page', $type, $post );
```

Allow for changing the template partial.

#### Returns

* **$type**: _(string)_ The default template type to use.

#### Other parameters

* **$post**: _(WP\_Post)_ The post object for the current post.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [page.php](https://github.com/thethemefoundry/make/blob/master/src/page.php#L25)

## make\_template\_content\_search \{.make\}

```
apply_filters( 'make_template_content_search', $type, $post );
```

Allow for changing the template partial.

#### Returns

* **$type**: _(string)_ The default template type to use.

#### Other parameters

* **$post**: _(WP\_Post)_ The post object for the current post.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [search.php](https://github.com/thethemefoundry/make/blob/master/src/search.php#L29)

## make\_template\_content\_single \{.make\}

```
apply_filters( 'make_template_content_single', $type, $post );
```

Allow for changing the template partial.

#### Returns

* **$type**: _(string)_ The default template type to use.

#### Other parameters

* **$post**: _(WP\_Post)_ The post object for the current post.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [single.php](https://github.com/thethemefoundry/make/blob/master/src/single.php#L25)

## make\_the\_builder\_content \{.make\}

```
apply_filters( 'make_the_builder_content', $content );
```

Filter the content used for "post\_content" when the builder is used to generate content.

#### Returns

* **$content**: _(string)_ The post content.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/save.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/save.php#L606)

## make\_will\_be\_builder\_page \{.make\}

```
apply_filters( 'make_will_be_builder_page', $will_be_builder_page, $template, $use_builder );
```

Allow developers to dynamically change the builder page status.

#### Returns

* **$will\_be\_builder\_page**: _(bool)_ Whether or not this page will be a builder page.

#### Other parameters

* **$template**: _(string)_ The template name.
* **$use\_builder**: _(int)_ Value of the "use-builder" input. 1 === use builder. 0 === do not use builder.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L791)

## ttfmake-text-column-classes \{.make\}

```
apply_filters( 'ttfmake-text-column-classes' );
```

#### Source

* [inc/builder/sections/builder-templates/text.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/sections/builder-templates/text.php#L107)

## ttfmake\_builder\_js\_dependencies \{.make\}

```
apply_filters( 'ttfmake_builder_js_dependencies', $dependencies );
```

Filter the dependencies for the Make builder JS.

#### Returns

* **$dependencies**: _(array)_ The list of dependencies.

#### Changelog

* **Since**: 1.2.3.

#### Source

* [inc/builder/core/base.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/base.php#L309)

## ttfmake\_builder\_section\_footer\_links \{.make\}

```
apply_filters( 'ttfmake_builder_section_footer_links' );
```

#### Source

* [inc/builder/core/templates/section-header.php](https://github.com/thethemefoundry/make/blob/master/src/inc/builder/core/templates/section-header.php#L27)

## ttfmake\_custom\_logo\_information \{.make\}

```
apply_filters( 'ttfmake_custom_logo_information' );
```

#### Source

* [inc/customizer/helpers-logo.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-logo.php#L301)

## ttfmake\_custom\_logo\_max\_width \{.make\}

```
apply_filters( 'ttfmake_custom_logo_max_width' );
```

#### Source

* [inc/customizer/helpers-logo.php](https://github.com/thethemefoundry/make/blob/master/src/inc/customizer/helpers-logo.php#L314)

## ttfmp\_perpage\_keys \{.make\}

```
apply_filters( 'ttfmp_perpage_keys' );
```

#### Source

* [components/per-page/class-options.php](https://github.com/thethemefoundry/make/blob/master/src/components/per-page/class-options.php#L97)

## ttfmp\_perpage\_post\_types \{.make\}

```
apply_filters( 'ttfmp_perpage_post_types' );
```

#### Source

* [components/per-page/class-metabox.php](https://github.com/thethemefoundry/make/blob/master/src/components/per-page/class-metabox.php#L97)

## ttfmp\_perpage\_view \{.make\}

```
apply_filters( 'ttfmp_perpage_view' );
```

#### Source

* [components/per-page/per-page.php](https://github.com/thethemefoundry/make/blob/master/src/components/per-page/per-page.php#L132)

## ttfmp\_post\_list\_output \{.make\}

```
apply_filters( 'ttfmp_post_list_output' );
```

#### Source

* [components/post-list/post-list.php](https://github.com/thethemefoundry/make/blob/master/src/components/post-list/post-list.php#L298)

## ttfmp\_post\_list\_template\_paths \{.make\}

```
apply_filters( 'ttfmp_post_list_template_paths' );
```

#### Source

* [components/post-list/post-list.php](https://github.com/thethemefoundry/make/blob/master/src/components/post-list/post-list.php#L237)

## ttfmp\_posts\_list\_thumbnail\_size \{.make\}

```
apply_filters( 'ttfmp_posts_list_thumbnail_size' );
```

#### Source

* [components/post-list/templates/post-list-item.php](https://github.com/thethemefoundry/make/blob/master/src/components/post-list/templates/post-list-item.php#L9)

## ttfmp\_shop\_layout\_product\_description \{.make\}

```
apply_filters( 'ttfmp_shop_layout_product_description' );
```

#### Source

* [shared/shop-settings/layout-product.php](https://github.com/thethemefoundry/make/blob/master/src/shared/shop-settings/layout-product.php#L20)

## ttfmp\_shop\_layout\_shop\_description \{.make\}

```
apply_filters( 'ttfmp_shop_layout_shop_description' );
```

#### Source

* [shared/shop-settings/layout-shop.php](https://github.com/thethemefoundry/make/blob/master/src/shared/shop-settings/layout-shop.php#L20)

## ttfmp\_style\_kit\_definitions \{.make\}

```
apply_filters( 'ttfmp_style_kit_definitions' );
```

#### Source

* [components/style-kits/definitions.php](https://github.com/thethemefoundry/make/blob/master/src/components/style-kits/definitions.php#L420)

## ttfmp\_woocommerce\_product\_grid\_output \{.make\}

```
apply_filters( 'ttfmp_woocommerce_product_grid_output' );
```

#### Source

* [components/woocommerce/class-shortcode.php](https://github.com/thethemefoundry/make/blob/master/src/components/woocommerce/class-shortcode.php#L305)

## ttfmp\_woocommerce\_product\_grid\_query\_args \{.make\}

```
apply_filters( 'ttfmp_woocommerce_product_grid_query_args' );
```

#### Source

* [components/woocommerce/class-shortcode.php](https://github.com/thethemefoundry/make/blob/master/src/components/woocommerce/class-shortcode.php#L192)

