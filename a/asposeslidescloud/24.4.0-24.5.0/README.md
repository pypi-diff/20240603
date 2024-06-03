# Comparing `tmp/asposeslidescloud-24.4.0.tar.gz` & `tmp/asposeslidescloud-24.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/asposeslidescloud-24.4.0.tar", last modified: Tue May  7 17:32:42 2024, max compression
+gzip compressed data, was "dist/asposeslidescloud-24.5.0.tar", last modified: Sat Jun  1 13:48:35 2024, max compression
```

## Comparing `asposeslidescloud-24.4.0.tar` & `asposeslidescloud-24.5.0.tar`

### file list

```diff
@@ -1,284 +1,285 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/
--rw-r--r--   0 root         (0) root         (0)     1080 2024-05-07 17:32:31.000000 asposeslidescloud-24.4.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     7751 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     7363 2024-05-07 17:32:32.000000 asposeslidescloud-24.4.0/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud/
--rw-rw-r--   0 root         (0) root         (0)    19069 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/__init__.py
--rw-rw-r--   0 root         (0) root         (0)    27782 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/api_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/
--rw-rw-r--   0 root         (0) root         (0)      313 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1945 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/api_base.py
--rw-rw-r--   0 root         (0) root         (0)  1452457 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/slides_api.py
--rw-rw-r--   0 root         (0) root         (0)    37269 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/apis/slides_async_api.py
--rw-rw-r--   0 root         (0) root         (0)     6653 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/configuration.py
--rw-rw-r--   0 root         (0) root         (0)     3604 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/error_message.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/
--rw-rw-r--   0 root         (0) root         (0)    18785 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     5035 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/accent_element.py
--rw-rw-r--   0 root         (0) root         (0)    13005 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/access_permissions.py
--rw-rw-r--   0 root         (0) root         (0)     5373 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/add_layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6257 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/add_master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4992 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/add_shape.py
--rw-rw-r--   0 root         (0) root         (0)     6965 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/add_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4369 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_ceiling_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3589 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_floor_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3603 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_inverse_effect.py
--rw-rw-r--   0 root         (0) root         (0)     3610 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_modulate_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4416 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4287 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4601 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/api_info.py
--rw-rw-r--   0 root         (0) root         (0)     6447 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/arc_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    10971 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/array_element.py
--rw-rw-r--   0 root         (0) root         (0)     7767 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/arrow_head_properties.py
--rw-rw-r--   0 root         (0) root         (0)    19086 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/audio_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7140 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/axes.py
--rw-rw-r--   0 root         (0) root         (0)    48257 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/axis.py
--rw-rw-r--   0 root         (0) root         (0)     3510 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/axis_type.py
--rw-rw-r--   0 root         (0) root         (0)     5740 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/bar_element.py
--rw-rw-r--   0 root         (0) root         (0)     4307 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/base64_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4314 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/bi_level_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4498 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/block_element.py
--rw-rw-r--   0 root         (0) root         (0)     4573 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/blur_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5204 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/blur_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12264 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/border_box_element.py
--rw-rw-r--   0 root         (0) root         (0)     8294 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/box_element.py
--rw-rw-r--   0 root         (0) root         (0)     6363 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/bubble_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     9176 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/bubble_series.py
--rw-rw-r--   0 root         (0) root         (0)    10161 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/camera.py
--rw-rw-r--   0 root         (0) root         (0)    19249 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart.py
--rw-rw-r--   0 root         (0) root         (0)     9502 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_category.py
--rw-rw-r--   0 root         (0) root         (0)     5072 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_lines_format.py
--rw-rw-r--   0 root         (0) root         (0)    22466 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_series_group.py
--rw-rw-r--   0 root         (0) root         (0)     4726 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_title.py
--rw-rw-r--   0 root         (0) root         (0)     8429 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_wall.py
--rw-rw-r--   0 root         (0) root         (0)     3417 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/chart_wall_type.py
--rw-rw-r--   0 root         (0) root         (0)     3546 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/close_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5188 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/color_change_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4393 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/color_replace_effect.py
--rw-rw-r--   0 root         (0) root         (0)    12365 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/color_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     4661 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/comment_author.py
--rw-rw-r--   0 root         (0) root         (0)     4362 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/comment_authors.py
--rw-rw-r--   0 root         (0) root         (0)     5159 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/common_slide_view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     9834 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/connector.py
--rw-rw-r--   0 root         (0) root         (0)     7666 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     4031 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/custom_dash_pattern.py
--rw-rw-r--   0 root         (0) root         (0)     8759 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/data_point.py
--rw-rw-r--   0 root         (0) root         (0)     4611 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/data_source.py
--rw-rw-r--   0 root         (0) root         (0)    10164 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/delimiter_element.py
--rw-rw-r--   0 root         (0) root         (0)     4744 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/disc_usage.py
--rw-rw-r--   0 root         (0) root         (0)     8706 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/document.py
--rw-rw-r--   0 root         (0) root         (0)     4411 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/document_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5707 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/document_property.py
--rw-rw-r--   0 root         (0) root         (0)     5081 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/document_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)     5080 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/duotone_effect.py
--rw-rw-r--   0 root         (0) root         (0)    31358 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/effect.py
--rw-rw-r--   0 root         (0) root         (0)     9702 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/effect_format.py
--rw-rw-r--   0 root         (0) root         (0)     3984 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/entity_exists.py
--rw-rw-r--   0 root         (0) root         (0)     6193 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/error.py
--rw-rw-r--   0 root         (0) root         (0)     4683 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/error_details.py
--rw-rw-r--   0 root         (0) root         (0)     3786 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7040 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5423 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/file_version.py
--rw-rw-r--   0 root         (0) root         (0)     4038 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/file_versions.py
--rw-rw-r--   0 root         (0) root         (0)     4065 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/files_list.py
--rw-rw-r--   0 root         (0) root         (0)     4847 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/files_upload_result.py
--rw-rw-r--   0 root         (0) root         (0)     4654 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fill_format.py
--rw-rw-r--   0 root         (0) root         (0)     4755 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fill_overlay_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5930 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fill_overlay_image_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5671 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_data.py
--rw-rw-r--   0 root         (0) root         (0)     6124 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_fallback_rule.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_set.py
--rw-rw-r--   0 root         (0) root         (0)     5834 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/font_subst_rule.py
--rw-rw-r--   0 root         (0) root         (0)     3968 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fonts_data.py
--rw-rw-r--   0 root         (0) root         (0)     7114 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/format_scheme.py
--rw-rw-r--   0 root         (0) root         (0)     6864 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/fraction_element.py
--rw-rw-r--   0 root         (0) root         (0)     4919 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/function_element.py
--rw-rw-r--   0 root         (0) root         (0)     6399 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_path.py
--rw-rw-r--   0 root         (0) root         (0)     4052 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_paths.py
--rw-rw-r--   0 root         (0) root         (0)    10067 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_shape.py
--rw-rw-r--   0 root         (0) root         (0)     7037 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/gif_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4577 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/glow_effect.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/gradient_fill.py
--rw-rw-r--   0 root         (0) root         (0)     4713 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/gradient_fill_stop.py
--rw-rw-r--   0 root         (0) root         (0)     5403 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/graphical_object.py
--rw-rw-r--   0 root         (0) root         (0)     3582 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/gray_scale_effect.py
--rw-rw-r--   0 root         (0) root         (0)     6112 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/group_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8843 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/grouping_character_element.py
--rw-rw-r--   0 root         (0) root         (0)     8469 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/handout_layouting_options.py
--rw-rw-r--   0 root         (0) root         (0)     8424 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     5525 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/hsl_effect.py
--rw-rw-r--   0 root         (0) root         (0)     8010 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/html5_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    13883 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/html_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    14645 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/hyperlink.py
--rw-rw-r--   0 root         (0) root         (0)     3323 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/i_shape_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5762 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image.py
--rw-rw-r--   0 root         (0) root         (0)     3441 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     6289 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     5618 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_options_base.py
--rw-rw-r--   0 root         (0) root         (0)     4891 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/image_transform_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4258 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/images.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/inner_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5833 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/input.py
--rw-rw-r--   0 root         (0) root         (0)     5375 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/input_file.py
--rw-rw-r--   0 root         (0) root         (0)     5076 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/interactive_sequence.py
--rw-rw-r--   0 root         (0) root         (0)     8009 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/layout_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4475 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/layout_slides.py
--rw-rw-r--   0 root         (0) root         (0)     6044 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/left_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    11324 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/legend.py
--rw-rw-r--   0 root         (0) root         (0)     9070 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/light_rig.py
--rw-rw-r--   0 root         (0) root         (0)     5686 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/limit_element.py
--rw-rw-r--   0 root         (0) root         (0)    17895 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/line_format.py
--rw-rw-r--   0 root         (0) root         (0)     4835 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/line_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     3520 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/literals.py
--rw-rw-r--   0 root         (0) root         (0)     5024 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/luminance_effect.py
--rw-rw-r--   0 root         (0) root         (0)    14076 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/markdown_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     6114 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/master_slide.py
--rw-rw-r--   0 root         (0) root         (0)     4461 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/master_slides.py
--rw-rw-r--   0 root         (0) root         (0)     4862 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/math_element.py
--rw-rw-r--   0 root         (0) root         (0)     3378 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/math_format.py
--rw-rw-r--   0 root         (0) root         (0)     6014 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/math_paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    13599 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/matrix_element.py
--rw-rw-r--   0 root         (0) root         (0)     4426 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/merge.py
--rw-rw-r--   0 root         (0) root         (0)     4739 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/merging_source.py
--rw-rw-r--   0 root         (0) root         (0)     4775 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/move_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)    11633 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/nary_operator_element.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/no_fill.py
--rw-rw-r--   0 root         (0) root         (0)     5421 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/normal_view_restored_properties.py
--rw-rw-r--   0 root         (0) root         (0)    11264 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/notes_comments_layouting_options.py
--rw-rw-r--   0 root         (0) root         (0)     5084 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide.py
--rw-rw-r--   0 root         (0) root         (0)     3766 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)    10510 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide_header_footer.py
--rw-rw-r--   0 root         (0) root         (0)     4781 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/object_exist.py
--rw-rw-r--   0 root         (0) root         (0)    14357 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/ole_object_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7805 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/one_value_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)    15178 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/one_value_series.py
--rw-rw-r--   0 root         (0) root         (0)    11732 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/operation.py
--rw-rw-r--   0 root         (0) root         (0)     5643 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/operation_progress.py
--rw-rw-r--   0 root         (0) root         (0)     4291 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/ordered_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     6346 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/outer_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4607 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/output_file.py
--rw-rw-r--   0 root         (0) root         (0)    31046 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/paragraph.py
--rw-rw-r--   0 root         (0) root         (0)    30740 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/paragraph_format.py
--rw-rw-r--   0 root         (0) root         (0)     4553 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/paragraphs.py
--rw-rw-r--   0 root         (0) root         (0)     5029 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/path_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4960 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/path_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     4665 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     7503 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/pattern_fill.py
--rw-rw-r--   0 root         (0) root         (0)    22614 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/pdf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    12411 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/picture_fill.py
--rw-rw-r--   0 root         (0) root         (0)     6457 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/picture_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4719 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/pipeline.py
--rw-rw-r--   0 root         (0) root         (0)     9383 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/placeholder.py
--rw-rw-r--   0 root         (0) root         (0)     4615 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/placeholders.py
--rw-rw-r--   0 root         (0) root         (0)    10381 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/plot_area.py
--rw-rw-r--   0 root         (0) root         (0)    39730 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/portion.py
--rw-rw-r--   0 root         (0) root         (0)    38640 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/portion_format.py
--rw-rw-r--   0 root         (0) root         (0)     4322 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/portions.py
--rw-rw-r--   0 root         (0) root         (0)     5838 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/pptx_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7159 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/presentation_to_merge.py
--rw-rw-r--   0 root         (0) root         (0)     5515 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/presentations_merge_request.py
--rw-rw-r--   0 root         (0) root         (0)     7553 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/preset_shadow_effect.py
--rw-rw-r--   0 root         (0) root         (0)     9765 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/protection_properties.py
--rw-rw-r--   0 root         (0) root         (0)     6325 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
--rw-rw-r--   0 root         (0) root         (0)     5744 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/radical_element.py
--rw-rw-r--   0 root         (0) root         (0)    16340 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/reflection_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4349 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/remove_shape.py
--rw-rw-r--   0 root         (0) root         (0)     4249 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/remove_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5060 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/reorder_slide.py
--rw-rw-r--   0 root         (0) root         (0)     6804 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/replace_text.py
--rw-rw-r--   0 root         (0) root         (0)     4334 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/request_input_file.py
--rw-rw-r--   0 root         (0) root         (0)     4204 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/reset_slide.py
--rw-rw-r--   0 root         (0) root         (0)     5036 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/resource_base.py
--rw-rw-r--   0 root         (0) root         (0)     7786 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/resource_uri.py
--rw-rw-r--   0 root         (0) root         (0)     3560 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/response_output_file.py
--rw-rw-r--   0 root         (0) root         (0)     6993 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/right_sub_superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     6410 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/save.py
--rw-rw-r--   0 root         (0) root         (0)     7122 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/save_shape.py
--rw-rw-r--   0 root         (0) root         (0)     8662 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/save_slide.py
--rw-rw-r--   0 root         (0) root         (0)     7453 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/scatter_chart_data_point.py
--rw-rw-r--   0 root         (0) root         (0)     6662 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/scatter_series.py
--rw-rw-r--   0 root         (0) root         (0)     6007 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/section.py
--rw-rw-r--   0 root         (0) root         (0)     6977 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/section_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     4457 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/sections.py
--rw-rw-r--   0 root         (0) root         (0)    19377 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/series.py
--rw-rw-r--   0 root         (0) root         (0)     8031 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/series_marker.py
--rw-rw-r--   0 root         (0) root         (0)     7858 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape.py
--rw-rw-r--   0 root         (0) root         (0)    18243 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_base.py
--rw-rw-r--   0 root         (0) root         (0)     6341 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_bevel.py
--rw-rw-r--   0 root         (0) root         (0)     3457 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7557 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_image_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     3436 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_thumbnail_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     3843 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shape_type.py
--rw-rw-r--   0 root         (0) root         (0)     4453 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shapes.py
--rw-rw-r--   0 root         (0) root         (0)     3647 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/shapes_alignment_type.py
--rw-rw-r--   0 root         (0) root         (0)    13365 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide.py
--rw-rw-r--   0 root         (0) root         (0)     5597 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_animation.py
--rw-rw-r--   0 root         (0) root         (0)     6747 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_background.py
--rw-rw-r--   0 root         (0) root         (0)     3925 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comment.py
--rw-rw-r--   0 root         (0) root         (0)     7739 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comment_base.py
--rw-rw-r--   0 root         (0) root         (0)     4363 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comments.py
--rw-rw-r--   0 root         (0) root         (0)     3765 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_export_format.py
--rw-rw-r--   0 root         (0) root         (0)     7997 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_modern_comment.py
--rw-rw-r--   0 root         (0) root         (0)    10980 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5587 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_replace_result.py
--rw-rw-r--   0 root         (0) root         (0)    13162 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_show_properties.py
--rw-rw-r--   0 root         (0) root         (0)    36756 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slide_show_transition.py
--rw-rw-r--   0 root         (0) root         (0)     4413 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slides.py
--rw-rw-r--   0 root         (0) root         (0)     4908 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/slides_layout_options.py
--rw-rw-r--   0 root         (0) root         (0)    15450 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art.py
--rw-rw-r--   0 root         (0) root         (0)     8919 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art_node.py
--rw-rw-r--   0 root         (0) root         (0)     5494 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art_shape.py
--rw-rw-r--   0 root         (0) root         (0)     3961 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/soft_edge_effect.py
--rw-rw-r--   0 root         (0) root         (0)     4159 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/solid_fill.py
--rw-rw-r--   0 root         (0) root         (0)     3448 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/special_slide_type.py
--rw-rw-r--   0 root         (0) root         (0)     4438 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/split_document_result.py
--rw-rw-r--   0 root         (0) root         (0)     4018 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/storage_exist.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/storage_file.py
--rw-rw-r--   0 root         (0) root         (0)     5049 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/subscript_element.py
--rw-rw-r--   0 root         (0) root         (0)     7883 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/summary_zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)     7716 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/summary_zoom_section.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/superscript_element.py
--rw-rw-r--   0 root         (0) root         (0)    18450 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/svg_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    26590 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/swf_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    16063 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table.py
--rw-rw-r--   0 root         (0) root         (0)    22416 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell.py
--rw-rw-r--   0 root         (0) root         (0)     7735 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell_merge_options.py
--rw-rw-r--   0 root         (0) root         (0)     3506 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell_split_type.py
--rw-rw-r--   0 root         (0) root         (0)     3921 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_column.py
--rw-rw-r--   0 root         (0) root         (0)     5461 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/table_row.py
--rw-rw-r--   0 root         (0) root         (0)     4757 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/task.py
--rw-rw-r--   0 root         (0) root         (0)     5843 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_bounds.py
--rw-rw-r--   0 root         (0) root         (0)     4173 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_element.py
--rw-rw-r--   0 root         (0) root         (0)    24377 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_frame_format.py
--rw-rw-r--   0 root         (0) root         (0)     4652 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_item.py
--rw-rw-r--   0 root         (0) root         (0)     4345 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/text_items.py
--rw-rw-r--   0 root         (0) root         (0)     6623 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/theme.py
--rw-rw-r--   0 root         (0) root         (0)    12219 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/three_d_format.py
--rw-rw-r--   0 root         (0) root         (0)    13912 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/tiff_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     4760 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/tint_effect.py
--rw-rw-r--   0 root         (0) root         (0)     5123 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/update_background.py
--rw-rw-r--   0 root         (0) root         (0)     5023 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/update_shape.py
--rw-rw-r--   0 root         (0) root         (0)     5880 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/vba_module.py
--rw-rw-r--   0 root         (0) root         (0)     5175 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/vba_project.py
--rw-rw-r--   0 root         (0) root         (0)     4613 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/vba_reference.py
--rw-rw-r--   0 root         (0) root         (0)    10340 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/video_export_options.py
--rw-rw-r--   0 root         (0) root         (0)    15861 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/video_frame.py
--rw-rw-r--   0 root         (0) root         (0)    16257 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/view_properties.py
--rw-rw-r--   0 root         (0) root         (0)     5848 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/workbook.py
--rw-rw-r--   0 root         (0) root         (0)     5008 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/xaml_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     7214 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/xps_export_options.py
--rw-rw-r--   0 root         (0) root         (0)     9382 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/xy_series.py
--rw-rw-r--   0 root         (0) root         (0)     6856 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/zoom_frame.py
--rw-rw-r--   0 root         (0) root         (0)    10569 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/models/zoom_object.py
--rw-rw-r--   0 root         (0) root         (0)     4398 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/oauth_response.py
--rw-rw-r--   0 root         (0) root         (0)    15494 2024-05-07 17:32:29.000000 asposeslidescloud-24.4.0/asposeslidescloud/rest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/
--rw-r--r--   0 root         (0) root         (0)     7751 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11891 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/asposeslidescloud.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-07 17:32:42.000000 asposeslidescloud-24.4.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      676 2024-05-07 17:32:36.000000 asposeslidescloud-24.4.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/
+-rw-r--r--   0 root         (0) root         (0)     1080 2024-06-01 13:48:21.000000 asposeslidescloud-24.5.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8232 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     7844 2024-06-01 13:48:23.000000 asposeslidescloud-24.5.0/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud/
+-rw-rw-r--   0 root         (0) root         (0)    19142 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)    27782 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/api_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud/apis/
+-rw-rw-r--   0 root         (0) root         (0)      313 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/apis/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1945 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/apis/api_base.py
+-rw-rw-r--   0 root         (0) root         (0)  1452657 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/apis/slides_api.py
+-rw-rw-r--   0 root         (0) root         (0)    37269 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/apis/slides_async_api.py
+-rw-rw-r--   0 root         (0) root         (0)     6653 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/configuration.py
+-rw-rw-r--   0 root         (0) root         (0)     3604 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/error_message.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/
+-rw-rw-r--   0 root         (0) root         (0)    18858 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     5035 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/accent_element.py
+-rw-rw-r--   0 root         (0) root         (0)    13005 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/access_permissions.py
+-rw-rw-r--   0 root         (0) root         (0)     5373 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/add_layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6257 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/add_master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4992 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/add_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     6965 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/add_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4369 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_ceiling_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3589 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_floor_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3603 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_inverse_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     3610 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_modulate_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4416 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4287 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4601 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/api_info.py
+-rw-rw-r--   0 root         (0) root         (0)     6447 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/arc_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    10971 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/array_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7767 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/arrow_head_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    19086 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/audio_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7140 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/axes.py
+-rw-rw-r--   0 root         (0) root         (0)    48908 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/axis.py
+-rw-rw-r--   0 root         (0) root         (0)     3510 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/axis_type.py
+-rw-rw-r--   0 root         (0) root         (0)     5740 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/bar_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4307 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/base64_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4314 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/bi_level_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4498 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/block_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4573 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/blur_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5204 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/blur_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12264 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/border_box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8294 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/box_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6363 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/bubble_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     9176 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/bubble_series.py
+-rw-rw-r--   0 root         (0) root         (0)    10161 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/camera.py
+-rw-rw-r--   0 root         (0) root         (0)    20005 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/chart.py
+-rw-rw-r--   0 root         (0) root         (0)     9502 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/chart_category.py
+-rw-rw-r--   0 root         (0) root         (0)     5072 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/chart_lines_format.py
+-rw-rw-r--   0 root         (0) root         (0)    22466 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/chart_series_group.py
+-rw-rw-r--   0 root         (0) root         (0)     9779 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/chart_title.py
+-rw-rw-r--   0 root         (0) root         (0)     8429 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/chart_wall.py
+-rw-rw-r--   0 root         (0) root         (0)     3417 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/chart_wall_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3546 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/close_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5188 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/color_change_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4393 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/color_replace_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    12365 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/color_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     4661 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/comment_author.py
+-rw-rw-r--   0 root         (0) root         (0)     4362 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/comment_authors.py
+-rw-rw-r--   0 root         (0) root         (0)     5159 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/common_slide_view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     9834 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/connector.py
+-rw-rw-r--   0 root         (0) root         (0)     7666 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     4031 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/custom_dash_pattern.py
+-rw-rw-r--   0 root         (0) root         (0)     8759 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     4611 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/data_source.py
+-rw-rw-r--   0 root         (0) root         (0)    10164 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/delimiter_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4744 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/disc_usage.py
+-rw-rw-r--   0 root         (0) root         (0)     8706 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/document.py
+-rw-rw-r--   0 root         (0) root         (0)     4411 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/document_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5707 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/document_property.py
+-rw-rw-r--   0 root         (0) root         (0)     5081 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/document_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)     5080 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/duotone_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    31358 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9702 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/effect_format.py
+-rw-rw-r--   0 root         (0) root         (0)     3984 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/entity_exists.py
+-rw-rw-r--   0 root         (0) root         (0)     6193 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/error.py
+-rw-rw-r--   0 root         (0) root         (0)     4683 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/error_details.py
+-rw-rw-r--   0 root         (0) root         (0)     3786 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7040 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5423 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/file_version.py
+-rw-rw-r--   0 root         (0) root         (0)     4038 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/file_versions.py
+-rw-rw-r--   0 root         (0) root         (0)     4065 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/files_list.py
+-rw-rw-r--   0 root         (0) root         (0)     4847 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/files_upload_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4654 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/fill_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4755 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/fill_overlay_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5930 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/fill_overlay_image_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5671 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/font_data.py
+-rw-rw-r--   0 root         (0) root         (0)     6124 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/font_fallback_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/font_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/font_set.py
+-rw-rw-r--   0 root         (0) root         (0)     5834 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/font_subst_rule.py
+-rw-rw-r--   0 root         (0) root         (0)     3968 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/fonts_data.py
+-rw-rw-r--   0 root         (0) root         (0)     7114 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/format_scheme.py
+-rw-rw-r--   0 root         (0) root         (0)     6864 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/fraction_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4919 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/function_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6399 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/geometry_path.py
+-rw-rw-r--   0 root         (0) root         (0)     4052 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/geometry_paths.py
+-rw-rw-r--   0 root         (0) root         (0)    10067 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/geometry_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     7037 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/gif_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4577 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/glow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/gradient_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     4713 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/gradient_fill_stop.py
+-rw-rw-r--   0 root         (0) root         (0)     5403 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/graphical_object.py
+-rw-rw-r--   0 root         (0) root         (0)     3582 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/gray_scale_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     6112 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/group_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8843 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/grouping_character_element.py
+-rw-rw-r--   0 root         (0) root         (0)     8469 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/handout_layouting_options.py
+-rw-rw-r--   0 root         (0) root         (0)     8424 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     5525 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/hsl_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     8010 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/html5_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    13883 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/html_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    14645 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/hyperlink.py
+-rw-rw-r--   0 root         (0) root         (0)     3323 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/i_shape_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5762 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/image.py
+-rw-rw-r--   0 root         (0) root         (0)     3441 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/image_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     6289 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5618 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/image_export_options_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4891 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/image_transform_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4258 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/images.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/inner_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5833 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/input.py
+-rw-rw-r--   0 root         (0) root         (0)     5375 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5076 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/interactive_sequence.py
+-rw-rw-r--   0 root         (0) root         (0)     8009 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/layout_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4475 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/layout_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     6044 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/left_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    11324 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/legend.py
+-rw-rw-r--   0 root         (0) root         (0)     9070 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/light_rig.py
+-rw-rw-r--   0 root         (0) root         (0)     5686 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/limit_element.py
+-rw-rw-r--   0 root         (0) root         (0)    17895 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/line_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4835 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/line_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     3520 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/literals.py
+-rw-rw-r--   0 root         (0) root         (0)     5024 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/luminance_effect.py
+-rw-rw-r--   0 root         (0) root         (0)    14076 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/markdown_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     6114 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/master_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     4461 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/master_slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4862 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/math_element.py
+-rw-rw-r--   0 root         (0) root         (0)     3378 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/math_format.py
+-rw-rw-r--   0 root         (0) root         (0)     6014 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/math_paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    13599 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/matrix_element.py
+-rw-rw-r--   0 root         (0) root         (0)     4426 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/merge.py
+-rw-rw-r--   0 root         (0) root         (0)     4739 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/merging_source.py
+-rw-rw-r--   0 root         (0) root         (0)     4775 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/move_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)    11633 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/nary_operator_element.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/no_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     5421 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/normal_view_restored_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    11264 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/notes_comments_layouting_options.py
+-rw-rw-r--   0 root         (0) root         (0)     5084 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/notes_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     3766 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/notes_slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)    10510 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/notes_slide_header_footer.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/object_exist.py
+-rw-rw-r--   0 root         (0) root         (0)    14357 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/ole_object_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7805 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/one_value_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)    15178 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/one_value_series.py
+-rw-rw-r--   0 root         (0) root         (0)    11732 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/operation.py
+-rw-rw-r--   0 root         (0) root         (0)     5643 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/operation_progress.py
+-rw-rw-r--   0 root         (0) root         (0)     4291 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/ordered_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     6346 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/outer_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4607 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/output_file.py
+-rw-rw-r--   0 root         (0) root         (0)    31046 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/paragraph.py
+-rw-rw-r--   0 root         (0) root         (0)    30740 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/paragraph_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4553 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/paragraphs.py
+-rw-rw-r--   0 root         (0) root         (0)     5029 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/path_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4960 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/path_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4665 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     7503 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/pattern_fill.py
+-rw-rw-r--   0 root         (0) root         (0)    22614 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/pdf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4136 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/pdf_import_options.py
+-rw-rw-r--   0 root         (0) root         (0)    12411 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/picture_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     6457 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/picture_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4719 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/pipeline.py
+-rw-rw-r--   0 root         (0) root         (0)     9383 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/placeholder.py
+-rw-rw-r--   0 root         (0) root         (0)     4615 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/placeholders.py
+-rw-rw-r--   0 root         (0) root         (0)    10381 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/plot_area.py
+-rw-rw-r--   0 root         (0) root         (0)    39730 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/portion.py
+-rw-rw-r--   0 root         (0) root         (0)    38640 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/portion_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4322 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/portions.py
+-rw-rw-r--   0 root         (0) root         (0)     5838 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/pptx_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7159 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/presentation_to_merge.py
+-rw-rw-r--   0 root         (0) root         (0)     5515 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/presentations_merge_request.py
+-rw-rw-r--   0 root         (0) root         (0)     7553 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/preset_shadow_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     9765 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/protection_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     6325 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py
+-rw-rw-r--   0 root         (0) root         (0)     5744 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/radical_element.py
+-rw-rw-r--   0 root         (0) root         (0)    16340 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/reflection_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4349 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/remove_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     4249 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/remove_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5060 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/reorder_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     6804 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/replace_text.py
+-rw-rw-r--   0 root         (0) root         (0)     4334 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/request_input_file.py
+-rw-rw-r--   0 root         (0) root         (0)     4204 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/reset_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5036 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/resource_base.py
+-rw-rw-r--   0 root         (0) root         (0)     7786 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/resource_uri.py
+-rw-rw-r--   0 root         (0) root         (0)     3560 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/response_output_file.py
+-rw-rw-r--   0 root         (0) root         (0)     6993 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/right_sub_superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     6410 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/save.py
+-rw-rw-r--   0 root         (0) root         (0)     7122 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/save_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     8662 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/save_slide.py
+-rw-rw-r--   0 root         (0) root         (0)     7453 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/scatter_chart_data_point.py
+-rw-rw-r--   0 root         (0) root         (0)     6662 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/scatter_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6007 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/section.py
+-rw-rw-r--   0 root         (0) root         (0)     6977 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/section_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     4457 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/sections.py
+-rw-rw-r--   0 root         (0) root         (0)    19377 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/series.py
+-rw-rw-r--   0 root         (0) root         (0)     8031 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/series_marker.py
+-rw-rw-r--   0 root         (0) root         (0)     7858 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shape.py
+-rw-rw-r--   0 root         (0) root         (0)    18243 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shape_base.py
+-rw-rw-r--   0 root         (0) root         (0)     6341 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shape_bevel.py
+-rw-rw-r--   0 root         (0) root         (0)     3457 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shape_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7557 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shape_image_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3436 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shape_thumbnail_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     3843 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shape_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4453 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shapes.py
+-rw-rw-r--   0 root         (0) root         (0)     3647 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/shapes_alignment_type.py
+-rw-rw-r--   0 root         (0) root         (0)    13365 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide.py
+-rw-rw-r--   0 root         (0) root         (0)     5597 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_animation.py
+-rw-rw-r--   0 root         (0) root         (0)     6747 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_background.py
+-rw-rw-r--   0 root         (0) root         (0)     3925 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_comment.py
+-rw-rw-r--   0 root         (0) root         (0)     7739 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_comment_base.py
+-rw-rw-r--   0 root         (0) root         (0)     4363 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_comments.py
+-rw-rw-r--   0 root         (0) root         (0)     3765 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_export_format.py
+-rw-rw-r--   0 root         (0) root         (0)     7997 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_modern_comment.py
+-rw-rw-r--   0 root         (0) root         (0)    10980 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5587 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_replace_result.py
+-rw-rw-r--   0 root         (0) root         (0)    13162 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_show_properties.py
+-rw-rw-r--   0 root         (0) root         (0)    36756 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slide_show_transition.py
+-rw-rw-r--   0 root         (0) root         (0)     4413 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slides.py
+-rw-rw-r--   0 root         (0) root         (0)     4908 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/slides_layout_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15450 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/smart_art.py
+-rw-rw-r--   0 root         (0) root         (0)     8919 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/smart_art_node.py
+-rw-rw-r--   0 root         (0) root         (0)     5494 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/smart_art_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     3961 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/soft_edge_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     4159 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/solid_fill.py
+-rw-rw-r--   0 root         (0) root         (0)     3448 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/special_slide_type.py
+-rw-rw-r--   0 root         (0) root         (0)     4438 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/split_document_result.py
+-rw-rw-r--   0 root         (0) root         (0)     4018 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/storage_exist.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/storage_file.py
+-rw-rw-r--   0 root         (0) root         (0)     5049 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/subscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)     7883 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/summary_zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)     7716 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/summary_zoom_section.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/superscript_element.py
+-rw-rw-r--   0 root         (0) root         (0)    18450 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/svg_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    26590 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/swf_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    16063 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/table.py
+-rw-rw-r--   0 root         (0) root         (0)    22416 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/table_cell.py
+-rw-rw-r--   0 root         (0) root         (0)     7735 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/table_cell_merge_options.py
+-rw-rw-r--   0 root         (0) root         (0)     3506 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/table_cell_split_type.py
+-rw-rw-r--   0 root         (0) root         (0)     3921 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/table_column.py
+-rw-rw-r--   0 root         (0) root         (0)     5461 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/table_row.py
+-rw-rw-r--   0 root         (0) root         (0)     4757 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/task.py
+-rw-rw-r--   0 root         (0) root         (0)     5843 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/text_bounds.py
+-rw-rw-r--   0 root         (0) root         (0)     4173 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/text_element.py
+-rw-rw-r--   0 root         (0) root         (0)    24377 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/text_frame_format.py
+-rw-rw-r--   0 root         (0) root         (0)     4652 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/text_item.py
+-rw-rw-r--   0 root         (0) root         (0)     4345 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/text_items.py
+-rw-rw-r--   0 root         (0) root         (0)     6623 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/theme.py
+-rw-rw-r--   0 root         (0) root         (0)    12219 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/three_d_format.py
+-rw-rw-r--   0 root         (0) root         (0)    13912 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/tiff_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     4760 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/tint_effect.py
+-rw-rw-r--   0 root         (0) root         (0)     5123 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/update_background.py
+-rw-rw-r--   0 root         (0) root         (0)     5023 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/update_shape.py
+-rw-rw-r--   0 root         (0) root         (0)     5880 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/vba_module.py
+-rw-rw-r--   0 root         (0) root         (0)     5175 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/vba_project.py
+-rw-rw-r--   0 root         (0) root         (0)     4613 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/vba_reference.py
+-rw-rw-r--   0 root         (0) root         (0)    10340 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/video_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)    15861 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/video_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    16257 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/view_properties.py
+-rw-rw-r--   0 root         (0) root         (0)     5848 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/workbook.py
+-rw-rw-r--   0 root         (0) root         (0)     5008 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/xaml_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     7214 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/xps_export_options.py
+-rw-rw-r--   0 root         (0) root         (0)     9382 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/xy_series.py
+-rw-rw-r--   0 root         (0) root         (0)     6856 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/zoom_frame.py
+-rw-rw-r--   0 root         (0) root         (0)    10569 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/models/zoom_object.py
+-rw-rw-r--   0 root         (0) root         (0)     4398 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/oauth_response.py
+-rw-rw-r--   0 root         (0) root         (0)    15494 2024-06-01 13:48:19.000000 asposeslidescloud-24.5.0/asposeslidescloud/rest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8232 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11938 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/asposeslidescloud.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-06-01 13:48:35.000000 asposeslidescloud-24.5.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      676 2024-06-01 13:48:27.000000 asposeslidescloud-24.5.0/setup.py
```

### Comparing `asposeslidescloud-24.4.0/LICENSE` & `asposeslidescloud-24.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/PKG-INFO` & `asposeslidescloud-24.5.0/README`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: asposeslidescloud
-Version: 24.4.0
-Summary: Aspose.Slides Cloud SDK for Python
-Home-page: 
-Author: Victor Putrov
-Author-email: vistor.putrov@aspose.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposeslidescloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposeslidescloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/asposeslidescloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/asposeslidescloud) [![GitHub license](https://img.shields.io/github/license/aspose-slides-cloud/aspose-slides-cloud-python)](https://github.com/aspose-slides-cloud/aspose-slides-cloud-python/blob/master/LICENSE)
 
 # Python REST API to Process Presentation in Cloud
 This repository contains Aspose.Slides Cloud SDK for Python source code. This SDK allows you to [process & manipulate PPT, PPTX, ODP, OTP](https://products.aspose.cloud/slides/python) using Aspose.slides Cloud REST APIs in your Python applications.
 
 You may want to check out Aspose free [Powerpoint to PDF](https://products.aspose.app/slides/conversion), [Powerpoint to Word](https://products.aspose.app/slides/conversion/ppt-to-word), [Powerpoint to JPG](https://products.aspose.app/slides/conversion/ppt-to-jpg), [Powerpoint to PNG](https://products.aspose.app/slides/conversion/ppt-to-png), [PDF to Powerpoint](https://products.aspose.app/slides/import/pdf-to-powerpoint), [JPG to Powerpoint](https://products.aspose.app/slides/import/jpg-to-ppt), and [PNG to Powerpoint](https://products.aspose.app/slides/import/png-to-ppt) converters because they are live implementations of popular conversion processes.
 
@@ -36,14 +23,21 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.5
+
+* Added **options** parameter to **ImportFromPdf** method. You can specify **options.DetectTables** property to control import behavior.
+* Added **Title** property to **Axis** class for charts.
+* Added **X**, **Y**, **Width**, **Height**, **Overlay**, **FillFormat**, **EffectFormat** and **LineFormat** properties to **ChartTitle** class.
+* Added **HasTitle** property to **Chart** class; removed **HasTitle** property from **ChartTitle** class.
+
 ## Enhancements in Version 24.4
 
 * Added **DownloadMathPortion** and **SaveMathPortion** methods to convert math portions to math markup formats (MathML or LaTeX). See [documentation](https://docs.aspose.cloud/slides/export-a-math-formula/) for more info. **DownloadPortionAsMathML** and **SavePortionAsMathML** methods are deprecated and will be removed after 24.6.
 * Added **Marker** property to **DataPoint** class.
 
 ## Enhancements in Version 24.3
```

### Comparing `asposeslidescloud-24.4.0/README` & `asposeslidescloud-24.5.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: asposeslidescloud
+Version: 24.5.0
+Summary: Aspose.Slides Cloud SDK for Python
+Home-page: 
+Author: Victor Putrov
+Author-email: vistor.putrov@aspose.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 ![](https://img.shields.io/badge/api-v3.0-lightgrey) ![PyPI](https://img.shields.io/pypi/v/asposeslidescloud) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/asposeslidescloud) ![PyPI - Implementation](https://img.shields.io/pypi/implementation/asposeslidescloud) ![PyPI - Wheel](https://img.shields.io/pypi/wheel/asposeslidescloud) [![GitHub license](https://img.shields.io/github/license/aspose-slides-cloud/aspose-slides-cloud-python)](https://github.com/aspose-slides-cloud/aspose-slides-cloud-python/blob/master/LICENSE)
 
 # Python REST API to Process Presentation in Cloud
 This repository contains Aspose.Slides Cloud SDK for Python source code. This SDK allows you to [process & manipulate PPT, PPTX, ODP, OTP](https://products.aspose.cloud/slides/python) using Aspose.slides Cloud REST APIs in your Python applications.
 
 You may want to check out Aspose free [Powerpoint to PDF](https://products.aspose.app/slides/conversion), [Powerpoint to Word](https://products.aspose.app/slides/conversion/ppt-to-word), [Powerpoint to JPG](https://products.aspose.app/slides/conversion/ppt-to-jpg), [Powerpoint to PNG](https://products.aspose.app/slides/conversion/ppt-to-png), [PDF to Powerpoint](https://products.aspose.app/slides/import/pdf-to-powerpoint), [JPG to Powerpoint](https://products.aspose.app/slides/import/jpg-to-ppt), and [PNG to Powerpoint](https://products.aspose.app/slides/import/png-to-ppt) converters because they are live implementations of popular conversion processes.
 
@@ -23,14 +36,21 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.5
+
+* Added **options** parameter to **ImportFromPdf** method. You can specify **options.DetectTables** property to control import behavior.
+* Added **Title** property to **Axis** class for charts.
+* Added **X**, **Y**, **Width**, **Height**, **Overlay**, **FillFormat**, **EffectFormat** and **LineFormat** properties to **ChartTitle** class.
+* Added **HasTitle** property to **Chart** class; removed **HasTitle** property from **ChartTitle** class.
+
 ## Enhancements in Version 24.4
 
 * Added **DownloadMathPortion** and **SaveMathPortion** methods to convert math portions to math markup formats (MathML or LaTeX). See [documentation](https://docs.aspose.cloud/slides/export-a-math-formula/) for more info. **DownloadPortionAsMathML** and **SavePortionAsMathML** methods are deprecated and will be removed after 24.6.
 * Added **Marker** property to **DataPoint** class.
 
 ## Enhancements in Version 24.3
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/__init__.py` & `asposeslidescloud-24.5.0/asposeslidescloud/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -186,14 +186,15 @@
 from asposeslidescloud.models.paragraph_format import ParagraphFormat
 from asposeslidescloud.models.paragraphs import Paragraphs
 from asposeslidescloud.models.path_input_file import PathInputFile
 from asposeslidescloud.models.path_output_file import PathOutputFile
 from asposeslidescloud.models.path_segment import PathSegment
 from asposeslidescloud.models.pattern_fill import PatternFill
 from asposeslidescloud.models.pdf_export_options import PdfExportOptions
+from asposeslidescloud.models.pdf_import_options import PdfImportOptions
 from asposeslidescloud.models.picture_fill import PictureFill
 from asposeslidescloud.models.picture_frame import PictureFrame
 from asposeslidescloud.models.pipeline import Pipeline
 from asposeslidescloud.models.placeholder import Placeholder
 from asposeslidescloud.models.placeholders import Placeholders
 from asposeslidescloud.models.plot_area import PlotArea
 from asposeslidescloud.models.portion import Portion
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/api_client.py` & `asposeslidescloud-24.5.0/asposeslidescloud/api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     def __init__(self, configuration=None):
         if configuration is None:
             configuration = Configuration()
         self.configuration = configuration
 
         self.pool = None
         self.rest_client = RESTClientObject(configuration)
-        self.default_headers = {'x-aspose-client': 'python sdk v24.4.0'}
+        self.default_headers = {'x-aspose-client': 'python sdk v24.5.0'}
         if configuration.timeout:
             self.default_headers['x-aspose-timeout'] = configuration.timeout
         self.default_headers.update(configuration.custom_headers)
 
     def __del__(self):
         if not self.pool is None:
             self.pool.close()
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/apis/api_base.py` & `asposeslidescloud-24.5.0/asposeslidescloud/apis/api_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/apis/slides_api.py` & `asposeslidescloud-24.5.0/asposeslidescloud/apis/slides_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -22060,50 +22060,52 @@
             auth_settings=auth_settings,
             is_async=params.get('is_async'),
             _return_http_data_only=params.get('_return_http_data_only'),
             _preload_content=params.get('_preload_content', False),
             _request_timeout=params.get('_request_timeout'),
             collection_formats=collection_formats)
 
-    def import_from_pdf(self, name, pdf, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+    def import_from_pdf(self, name, pdf, options = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create presentation document from pdf or append pdf to an existing presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
-        >>> thread = api.(name, pdf, password, folder, storage, is_async=True)
+        >>> thread = api.(name, pdf, options, password, folder, storage, is_async=True)
         >>> result = thread.get()
 
         :param is_async bool
         :param name Document name.
         :param pdf PDF data.
+        :param options Import options.
         :param password Document password.
         :param folder Document folder.
         :param storage Document storage.
         :return: Document
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('is_async'):
-            return self.import_from_pdf_with_http_info(name, pdf, password, folder, storage, **kwargs)  # noqa: E501
+            return self.import_from_pdf_with_http_info(name, pdf, options, password, folder, storage, **kwargs)  # noqa: E501
         else:
-            (data) = self.import_from_pdf_with_http_info(name, pdf, password, folder, storage, **kwargs)  # noqa: E501
+            (data) = self.import_from_pdf_with_http_info(name, pdf, options, password, folder, storage, **kwargs)  # noqa: E501
             return data
 
-    def import_from_pdf_with_http_info(self, name, pdf, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
+    def import_from_pdf_with_http_info(self, name, pdf, options = None, password = None, folder = None, storage = None, **kwargs):  # noqa: E501
         """Create presentation document from pdf or append pdf to an existing presentation.  # noqa: E501
 
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass is_async=True
-        >>> thread = api.import_from_pdf_with_http_info(name, pdf, password, folder, storage, is_async=True)
+        >>> thread = api.import_from_pdf_with_http_info(name, pdf, options, password, folder, storage, is_async=True)
         >>> result = thread.get()
 
         :param is_async bool
         :param name Document name.
         :param pdf PDF data.
+        :param options Import options.
         :param password Document password.
         :param folder Document folder.
         :param storage Document storage.
         :return: Document
                  If the method is called asynchronously,
                  returns the request thread.
         """
@@ -22147,14 +22149,16 @@
 
         form_params = []
         param_files = {}
         if pdf:
             param_files['pdf'] = pdf  # noqa: E501
 
         body_params = None
+        if options:
+            body_params = options
 
         # HTTP header `Content-Type`
         header_params['Content-Type'] = self.api_client.select_header_content_type(  # noqa: E501
             ['application/json'])  # noqa: E501
 
         # Authentication setting
         auth_settings = ['JWT']  # noqa: E501
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/apis/slides_async_api.py` & `asposeslidescloud-24.5.0/asposeslidescloud/apis/slides_async_api.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/configuration.py` & `asposeslidescloud-24.5.0/asposeslidescloud/configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -192,9 +192,9 @@
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
                "Version of the API: 3.0\n"\
-               "SDK Package Version: 24.4.0".\
+               "SDK Package Version: 24.5.0".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/error_message.py` & `asposeslidescloud-24.5.0/asposeslidescloud/error_message.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/__init__.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -178,14 +178,15 @@
 from asposeslidescloud.models.paragraph_format import ParagraphFormat
 from asposeslidescloud.models.paragraphs import Paragraphs
 from asposeslidescloud.models.path_input_file import PathInputFile
 from asposeslidescloud.models.path_output_file import PathOutputFile
 from asposeslidescloud.models.path_segment import PathSegment
 from asposeslidescloud.models.pattern_fill import PatternFill
 from asposeslidescloud.models.pdf_export_options import PdfExportOptions
+from asposeslidescloud.models.pdf_import_options import PdfImportOptions
 from asposeslidescloud.models.picture_fill import PictureFill
 from asposeslidescloud.models.picture_frame import PictureFrame
 from asposeslidescloud.models.pipeline import Pipeline
 from asposeslidescloud.models.placeholder import Placeholder
 from asposeslidescloud.models.placeholders import Placeholders
 from asposeslidescloud.models.plot_area import PlotArea
 from asposeslidescloud.models.portion import Portion
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/accent_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/accent_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/access_permissions.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/access_permissions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/add_layout_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/add_layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/add_master_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/add_master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/add_shape.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/add_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/add_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/add_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_bi_level_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_ceiling_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_ceiling_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_floor_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_floor_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_inverse_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_inverse_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_modulate_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_modulate_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_modulate_fixed_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/alpha_replace_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/alpha_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/api_info.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/api_info.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/arc_to_path_segment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/arc_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/array_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/array_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/arrow_head_properties.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/arrow_head_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/audio_frame.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/audio_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/axes.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/axes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/axis.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/axis.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,15 @@
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'is_visible': 'bool',
         'has_title': 'bool',
+        'title': 'ChartTitle',
         'position': 'str',
         'display_unit': 'str',
         'base_unit_scale': 'str',
         'is_automatic_major_unit': 'bool',
         'major_unit': 'float',
         'major_unit_scale': 'str',
         'major_tick_mark': 'str',
@@ -81,14 +82,15 @@
         'major_grid_lines_format': 'ChartLinesFormat',
         'minor_grid_lines_format': 'ChartLinesFormat'
     }
 
     attribute_map = {
         'is_visible': 'isVisible',
         'has_title': 'hasTitle',
+        'title': 'title',
         'position': 'position',
         'display_unit': 'displayUnit',
         'base_unit_scale': 'baseUnitScale',
         'is_automatic_major_unit': 'isAutomaticMajorUnit',
         'major_unit': 'majorUnit',
         'major_unit_scale': 'majorUnitScale',
         'major_tick_mark': 'majorTickMark',
@@ -122,19 +124,20 @@
         'major_grid_lines_format': 'majorGridLinesFormat',
         'minor_grid_lines_format': 'minorGridLinesFormat'
     }
 
     type_determiners = {
     }
 
-    def __init__(self, is_visible=None, has_title=None, position=None, display_unit=None, base_unit_scale=None, is_automatic_major_unit=None, major_unit=None, major_unit_scale=None, major_tick_mark=None, is_automatic_minor_unit=None, minor_unit=None, minor_unit_scale=None, minor_tick_mark=None, is_automatic_max_value=None, max_value=None, is_automatic_min_value=None, min_value=None, is_logarithmic=None, log_base=None, category_axis_type=None, axis_between_categories=None, label_offset=None, is_plot_order_reversed=None, is_number_format_linked_to_source=None, number_format=None, cross_type=None, cross_at=None, is_automatic_tick_marks_spacing=None, tick_marks_spacing=None, is_automatic_tick_label_spacing=None, tick_label_spacing=None, tick_label_position=None, tick_label_rotation_angle=None, fill_format=None, effect_format=None, line_format=None, major_grid_lines_format=None, minor_grid_lines_format=None):  # noqa: E501
+    def __init__(self, is_visible=None, has_title=None, title=None, position=None, display_unit=None, base_unit_scale=None, is_automatic_major_unit=None, major_unit=None, major_unit_scale=None, major_tick_mark=None, is_automatic_minor_unit=None, minor_unit=None, minor_unit_scale=None, minor_tick_mark=None, is_automatic_max_value=None, max_value=None, is_automatic_min_value=None, min_value=None, is_logarithmic=None, log_base=None, category_axis_type=None, axis_between_categories=None, label_offset=None, is_plot_order_reversed=None, is_number_format_linked_to_source=None, number_format=None, cross_type=None, cross_at=None, is_automatic_tick_marks_spacing=None, tick_marks_spacing=None, is_automatic_tick_label_spacing=None, tick_label_spacing=None, tick_label_position=None, tick_label_rotation_angle=None, fill_format=None, effect_format=None, line_format=None, major_grid_lines_format=None, minor_grid_lines_format=None):  # noqa: E501
         """Axis - a model defined in Swagger"""  # noqa: E501
 
         self._is_visible = None
         self._has_title = None
+        self._title = None
         self._position = None
         self._display_unit = None
         self._base_unit_scale = None
         self._is_automatic_major_unit = None
         self._major_unit = None
         self._major_unit_scale = None
         self._major_tick_mark = None
@@ -168,14 +171,16 @@
         self._major_grid_lines_format = None
         self._minor_grid_lines_format = None
 
         if is_visible is not None:
             self.is_visible = is_visible
         if has_title is not None:
             self.has_title = has_title
+        if title is not None:
+            self.title = title
         if position is not None:
             self.position = position
         if display_unit is not None:
             self.display_unit = display_unit
         if base_unit_scale is not None:
             self.base_unit_scale = base_unit_scale
         if is_automatic_major_unit is not None:
@@ -286,14 +291,36 @@
 
         :param has_title: The has_title of this Axis.  # noqa: E501
         :type: bool
         """
         self._has_title = has_title
 
     @property
+    def title(self):
+        """Gets the title of this Axis.  # noqa: E501
+
+        Axis title  # noqa: E501
+
+        :return: The title of this Axis.  # noqa: E501
+        :rtype: ChartTitle
+        """
+        return self._title
+
+    @title.setter
+    def title(self, title):
+        """Sets the title of this Axis.
+
+        Axis title  # noqa: E501
+
+        :param title: The title of this Axis.  # noqa: E501
+        :type: ChartTitle
+        """
+        self._title = title
+
+    @property
     def position(self):
         """Gets the position of this Axis.  # noqa: E501
 
         Axis position  # noqa: E501
 
         :return: The position of this Axis.  # noqa: E501
         :rtype: str
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/axis_type.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/axis_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/bar_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/bar_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/base64_input_file.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/base64_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/bi_level_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/bi_level_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/block_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/block_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/blur_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/blur_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/blur_image_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/blur_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/border_box_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/border_box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/box_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/box_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/bubble_chart_data_point.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/bubble_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/bubble_series.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/bubble_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/camera.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/camera.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/chart.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/chart.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,15 @@
         'hyperlink_mouse_over': 'Hyperlink',
         'type': 'str',
         'chart_type': 'str',
         'show_data_labels_over_maximum': 'bool',
         'series': 'list[Series]',
         'categories': 'list[ChartCategory]',
         'data_source_for_categories': 'DataSource',
+        'has_title': 'bool',
         'title': 'ChartTitle',
         'back_wall': 'ChartWall',
         'side_wall': 'ChartWall',
         'floor': 'ChartWall',
         'legend': 'Legend',
         'axes': 'Axes',
         'plot_area': 'PlotArea',
@@ -99,14 +100,15 @@
         'hyperlink_mouse_over': 'hyperlinkMouseOver',
         'type': 'type',
         'chart_type': 'chartType',
         'show_data_labels_over_maximum': 'showDataLabelsOverMaximum',
         'series': 'series',
         'categories': 'categories',
         'data_source_for_categories': 'dataSourceForCategories',
+        'has_title': 'hasTitle',
         'title': 'title',
         'back_wall': 'backWall',
         'side_wall': 'sideWall',
         'floor': 'floor',
         'legend': 'legend',
         'axes': 'axes',
         'plot_area': 'plotArea',
@@ -114,23 +116,24 @@
         'series_groups': 'seriesGroups'
     }
 
     type_determiners = {
         'type': 'Chart',
     }
 
-    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Chart', chart_type=None, show_data_labels_over_maximum=None, series=None, categories=None, data_source_for_categories=None, title=None, back_wall=None, side_wall=None, floor=None, legend=None, axes=None, plot_area=None, has_rounded_corners=None, series_groups=None):  # noqa: E501
+    def __init__(self, self_uri=None, alternate_links=None, name=None, width=None, height=None, alternative_text=None, alternative_text_title=None, hidden=None, is_decorative=None, x=None, y=None, z_order_position=None, fill_format=None, effect_format=None, three_d_format=None, line_format=None, hyperlink_click=None, hyperlink_mouse_over=None, type='Chart', chart_type=None, show_data_labels_over_maximum=None, series=None, categories=None, data_source_for_categories=None, has_title=None, title=None, back_wall=None, side_wall=None, floor=None, legend=None, axes=None, plot_area=None, has_rounded_corners=None, series_groups=None):  # noqa: E501
         """Chart - a model defined in Swagger"""  # noqa: E501
         super(Chart, self).__init__(self_uri, alternate_links, name, width, height, alternative_text, alternative_text_title, hidden, is_decorative, x, y, z_order_position, fill_format, effect_format, three_d_format, line_format, hyperlink_click, hyperlink_mouse_over, type)
 
         self._chart_type = None
         self._show_data_labels_over_maximum = None
         self._series = None
         self._categories = None
         self._data_source_for_categories = None
+        self._has_title = None
         self._title = None
         self._back_wall = None
         self._side_wall = None
         self._floor = None
         self._legend = None
         self._axes = None
         self._plot_area = None
@@ -143,14 +146,16 @@
             self.show_data_labels_over_maximum = show_data_labels_over_maximum
         if series is not None:
             self.series = series
         if categories is not None:
             self.categories = categories
         if data_source_for_categories is not None:
             self.data_source_for_categories = data_source_for_categories
+        if has_title is not None:
+            self.has_title = has_title
         if title is not None:
             self.title = title
         if back_wall is not None:
             self.back_wall = back_wall
         if side_wall is not None:
             self.side_wall = side_wall
         if floor is not None:
@@ -289,14 +294,36 @@
 
         :param data_source_for_categories: The data_source_for_categories of this Chart.  # noqa: E501
         :type: DataSource
         """
         self._data_source_for_categories = data_source_for_categories
 
     @property
+    def has_title(self):
+        """Gets the has_title of this Chart.  # noqa: E501
+
+        True if the chart has a title.  # noqa: E501
+
+        :return: The has_title of this Chart.  # noqa: E501
+        :rtype: bool
+        """
+        return self._has_title
+
+    @has_title.setter
+    def has_title(self, has_title):
+        """Sets the has_title of this Chart.
+
+        True if the chart has a title.  # noqa: E501
+
+        :param has_title: The has_title of this Chart.  # noqa: E501
+        :type: bool
+        """
+        self._has_title = has_title
+
+    @property
     def title(self):
         """Gets the title of this Chart.  # noqa: E501
 
         Gets or sets the title.  # noqa: E501
 
         :return: The title of this Chart.  # noqa: E501
         :rtype: ChartTitle
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_category.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/chart_category.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_lines_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/chart_lines_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_series_group.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/chart_series_group.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_title.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/path_output_file.py`

 * *Files 15% similar despite different names*

```diff
@@ -26,91 +26,98 @@
 # -----------------------------------------------------------------------------------
 
 import pprint
 import re  # noqa: F401
 
 import six
 
+from asposeslidescloud.models.output_file import OutputFile
 
-class ChartTitle(object):
+class PathOutputFile(OutputFile):
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'text': 'str',
-        'has_title': 'bool'
+        'type': 'str',
+        'path': 'str',
+        'storage': 'str'
     }
 
     attribute_map = {
-        'text': 'text',
-        'has_title': 'hasTitle'
+        'type': 'type',
+        'path': 'path',
+        'storage': 'storage'
     }
 
     type_determiners = {
+        'type': 'Path',
     }
 
-    def __init__(self, text=None, has_title=None):  # noqa: E501
-        """ChartTitle - a model defined in Swagger"""  # noqa: E501
-
-        self._text = None
-        self._has_title = None
-
-        if text is not None:
-            self.text = text
-        self.has_title = has_title
+    def __init__(self, type='Path', path=None, storage=None):  # noqa: E501
+        """PathOutputFile - a model defined in Swagger"""  # noqa: E501
+        super(PathOutputFile, self).__init__(type)
+
+        self._path = None
+        self._storage = None
+        self.type = 'Path'
+
+        if path is not None:
+            self.path = path
+        if storage is not None:
+            self.storage = storage
 
     @property
-    def text(self):
-        """Gets the text of this ChartTitle.  # noqa: E501
+    def path(self):
+        """Gets the path of this PathOutputFile.  # noqa: E501
 
-        Get or sets the text.  # noqa: E501
+        Get or sets path to file.  # noqa: E501
 
-        :return: The text of this ChartTitle.  # noqa: E501
+        :return: The path of this PathOutputFile.  # noqa: E501
         :rtype: str
         """
-        return self._text
+        return self._path
 
-    @text.setter
-    def text(self, text):
-        """Sets the text of this ChartTitle.
+    @path.setter
+    def path(self, path):
+        """Sets the path of this PathOutputFile.
 
-        Get or sets the text.  # noqa: E501
+        Get or sets path to file.  # noqa: E501
 
-        :param text: The text of this ChartTitle.  # noqa: E501
+        :param path: The path of this PathOutputFile.  # noqa: E501
         :type: str
         """
-        self._text = text
+        self._path = path
 
     @property
-    def has_title(self):
-        """Gets the has_title of this ChartTitle.  # noqa: E501
+    def storage(self):
+        """Gets the storage of this PathOutputFile.  # noqa: E501
 
-        Get or sets value determines visibility of title  # noqa: E501
+        Get or sets name of storage.  # noqa: E501
 
-        :return: The has_title of this ChartTitle.  # noqa: E501
-        :rtype: bool
+        :return: The storage of this PathOutputFile.  # noqa: E501
+        :rtype: str
         """
-        return self._has_title
+        return self._storage
 
-    @has_title.setter
-    def has_title(self, has_title):
-        """Sets the has_title of this ChartTitle.
+    @storage.setter
+    def storage(self, storage):
+        """Sets the storage of this PathOutputFile.
 
-        Get or sets value determines visibility of title  # noqa: E501
+        Get or sets name of storage.  # noqa: E501
 
-        :param has_title: The has_title of this ChartTitle.  # noqa: E501
-        :type: bool
+        :param storage: The storage of this PathOutputFile.  # noqa: E501
+        :type: str
         """
-        self._has_title = has_title
+        self._storage = storage
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -138,15 +145,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, ChartTitle):
+        if not isinstance(other, PathOutputFile):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_wall.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/chart_wall.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/chart_wall_type.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/chart_wall_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/close_path_segment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/close_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/color_change_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/color_change_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/color_replace_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/color_replace_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/color_scheme.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/color_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/comment_author.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/comment_author.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/comment_authors.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/comment_authors.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/common_slide_view_properties.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/common_slide_view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/connector.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/connector.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/cubic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/custom_dash_pattern.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/custom_dash_pattern.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/data_point.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/data_source.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/data_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/delimiter_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/delimiter_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/disc_usage.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/disc_usage.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/document.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/document.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/document_properties.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/document_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/document_property.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/document_property.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/document_replace_result.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/document_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/duotone_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/duotone_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/effect_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/effect_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/entity_exists.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/entity_exists.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/error.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/error.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/error_details.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/error_details.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/export_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/file_version.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/file_version.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/file_versions.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/file_versions.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/files_list.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/files_list.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/files_upload_result.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/files_upload_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/fill_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/fill_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/fill_overlay_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/fill_overlay_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/fill_overlay_image_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/fill_overlay_image_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/font_data.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/font_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/font_fallback_rule.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/font_fallback_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/font_scheme.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/font_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/font_set.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/font_set.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/font_subst_rule.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/font_subst_rule.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/fonts_data.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/fonts_data.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/format_scheme.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/format_scheme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/fraction_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/fraction_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/function_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/function_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_path.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/geometry_path.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_paths.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/geometry_paths.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/geometry_shape.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/geometry_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/gif_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/gif_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/glow_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/glow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/gradient_fill.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/gradient_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/gradient_fill_stop.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/gradient_fill_stop.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/graphical_object.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/graphical_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/gray_scale_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/gray_scale_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/group_shape.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/group_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/grouping_character_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/grouping_character_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/handout_layouting_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/handout_layouting_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/header_footer.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/hsl_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/hsl_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/html5_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/html5_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/html_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/html_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/hyperlink.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/hyperlink.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/i_shape_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/i_shape_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/image.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/image.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/image_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/image_export_options_base.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/image_export_options_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/image_transform_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/image_transform_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/images.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/images.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/inner_shadow_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/inner_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/input.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/input.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/input_file.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/interactive_sequence.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/interactive_sequence.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/layout_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/layout_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/layout_slides.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/layout_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/left_sub_superscript_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/left_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/legend.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/legend.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/light_rig.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/light_rig.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/limit_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/limit_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/line_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/line_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/line_to_path_segment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/line_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/literals.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/literals.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/luminance_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/luminance_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/markdown_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/markdown_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/master_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/master_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/master_slides.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/master_slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/math_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/math_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/math_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/math_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/math_paragraph.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/math_paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/matrix_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/matrix_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/merge.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/merging_source.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/merging_source.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/move_to_path_segment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/move_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/nary_operator_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/nary_operator_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/no_fill.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/no_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/normal_view_restored_properties.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/normal_view_restored_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/notes_comments_layouting_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/notes_comments_layouting_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/notes_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide_export_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/notes_slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/notes_slide_header_footer.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/notes_slide_header_footer.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/object_exist.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/object_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/ole_object_frame.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/ole_object_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/one_value_chart_data_point.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/one_value_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/one_value_series.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/one_value_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/operation.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/operation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/operation_progress.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/operation_progress.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/ordered_merge_request.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/ordered_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/outer_shadow_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/outer_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/output_file.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/paragraph.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/paragraph.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/paragraph_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/paragraph_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/paragraphs.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/paragraphs.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/path_input_file.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/path_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/path_output_file.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/portions.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,98 +26,71 @@
 # -----------------------------------------------------------------------------------
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-from asposeslidescloud.models.output_file import OutputFile
+from asposeslidescloud.models.resource_base import ResourceBase
 
-class PathOutputFile(OutputFile):
+class Portions(ResourceBase):
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
-        'type': 'str',
-        'path': 'str',
-        'storage': 'str'
+        'self_uri': 'ResourceUri',
+        'alternate_links': 'list[ResourceUri]',
+        'items': 'list[Portion]'
     }
 
     attribute_map = {
-        'type': 'type',
-        'path': 'path',
-        'storage': 'storage'
+        'self_uri': 'selfUri',
+        'alternate_links': 'alternateLinks',
+        'items': 'items'
     }
 
     type_determiners = {
-        'type': 'Path',
     }
 
-    def __init__(self, type='Path', path=None, storage=None):  # noqa: E501
-        """PathOutputFile - a model defined in Swagger"""  # noqa: E501
-        super(PathOutputFile, self).__init__(type)
-
-        self._path = None
-        self._storage = None
-        self.type = 'Path'
-
-        if path is not None:
-            self.path = path
-        if storage is not None:
-            self.storage = storage
+    def __init__(self, self_uri=None, alternate_links=None, items=None):  # noqa: E501
+        """Portions - a model defined in Swagger"""  # noqa: E501
+        super(Portions, self).__init__(self_uri, alternate_links)
 
-    @property
-    def path(self):
-        """Gets the path of this PathOutputFile.  # noqa: E501
-
-        Get or sets path to file.  # noqa: E501
-
-        :return: The path of this PathOutputFile.  # noqa: E501
-        :rtype: str
-        """
-        return self._path
+        self._items = None
 
-    @path.setter
-    def path(self, path):
-        """Sets the path of this PathOutputFile.
-
-        Get or sets path to file.  # noqa: E501
-
-        :param path: The path of this PathOutputFile.  # noqa: E501
-        :type: str
-        """
-        self._path = path
+        if items is not None:
+            self.items = items
 
     @property
-    def storage(self):
-        """Gets the storage of this PathOutputFile.  # noqa: E501
+    def items(self):
+        """Gets the items of this Portions.  # noqa: E501
 
-        Get or sets name of storage.  # noqa: E501
+        List of portion links.  # noqa: E501
 
-        :return: The storage of this PathOutputFile.  # noqa: E501
-        :rtype: str
+        :return: The items of this Portions.  # noqa: E501
+        :rtype: list[Portion]
         """
-        return self._storage
+        return self._items
 
-    @storage.setter
-    def storage(self, storage):
-        """Sets the storage of this PathOutputFile.
+    @items.setter
+    def items(self, items):
+        """Sets the items of this Portions.
 
-        Get or sets name of storage.  # noqa: E501
+        List of portion links.  # noqa: E501
 
-        :param storage: The storage of this PathOutputFile.  # noqa: E501
-        :type: str
+        :param items: The items of this Portions.  # noqa: E501
+        :type: list[Portion]
         """
-        self._storage = storage
+        self._items = items
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
@@ -145,15 +118,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PathOutputFile):
+        if not isinstance(other, Portions):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/path_segment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/pattern_fill.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/pattern_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/pdf_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/pdf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/picture_fill.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/picture_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/picture_frame.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/picture_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/pipeline.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/pipeline.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/placeholder.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/placeholder.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/placeholders.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/placeholders.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/plot_area.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/plot_area.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/portion.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/portion.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/portion_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/portion_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/portions.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/text_items.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,67 +28,67 @@
 import pprint
 import re  # noqa: F401
 
 import six
 
 from asposeslidescloud.models.resource_base import ResourceBase
 
-class Portions(ResourceBase):
+class TextItems(ResourceBase):
 
 
     """
     Attributes:
       swagger_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'self_uri': 'ResourceUri',
         'alternate_links': 'list[ResourceUri]',
-        'items': 'list[Portion]'
+        'items': 'list[TextItem]'
     }
 
     attribute_map = {
         'self_uri': 'selfUri',
         'alternate_links': 'alternateLinks',
         'items': 'items'
     }
 
     type_determiners = {
     }
 
     def __init__(self, self_uri=None, alternate_links=None, items=None):  # noqa: E501
-        """Portions - a model defined in Swagger"""  # noqa: E501
-        super(Portions, self).__init__(self_uri, alternate_links)
+        """TextItems - a model defined in Swagger"""  # noqa: E501
+        super(TextItems, self).__init__(self_uri, alternate_links)
 
         self._items = None
 
         if items is not None:
             self.items = items
 
     @property
     def items(self):
-        """Gets the items of this Portions.  # noqa: E501
+        """Gets the items of this TextItems.  # noqa: E501
 
-        List of portion links.  # noqa: E501
+        Gets or sets the text items.  # noqa: E501
 
-        :return: The items of this Portions.  # noqa: E501
-        :rtype: list[Portion]
+        :return: The items of this TextItems.  # noqa: E501
+        :rtype: list[TextItem]
         """
         return self._items
 
     @items.setter
     def items(self, items):
-        """Sets the items of this Portions.
+        """Sets the items of this TextItems.
 
-        List of portion links.  # noqa: E501
+        Gets or sets the text items.  # noqa: E501
 
-        :param items: The items of this Portions.  # noqa: E501
-        :type: list[Portion]
+        :param items: The items of this TextItems.  # noqa: E501
+        :type: list[TextItem]
         """
         self._items = items
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
@@ -118,15 +118,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Portions):
+        if not isinstance(other, TextItems):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/pptx_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/pptx_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/presentation_to_merge.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/presentation_to_merge.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/presentations_merge_request.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/presentations_merge_request.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/preset_shadow_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/preset_shadow_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/protection_properties.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/protection_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/quadratic_bezier_to_path_segment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/radical_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/radical_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/reflection_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/reflection_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/remove_shape.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/remove_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/remove_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/remove_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/reorder_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/reorder_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/replace_text.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/replace_text.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/request_input_file.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/request_input_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/reset_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/reset_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/resource_base.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/resource_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/resource_uri.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/resource_uri.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/response_output_file.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/response_output_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/right_sub_superscript_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/right_sub_superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/save.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/save.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/save_shape.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/save_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/save_slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/save_slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/scatter_chart_data_point.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/scatter_chart_data_point.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/scatter_series.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/scatter_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/section.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/section_zoom_frame.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/section_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/sections.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/sections.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/series.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/series_marker.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/series_marker.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shape.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_base.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shape_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_bevel.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shape_bevel.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_export_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shape_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_image_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shape_image_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_thumbnail_bounds.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shape_thumbnail_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shape_type.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shape_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shapes.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shapes.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/shapes_alignment_type.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/shapes_alignment_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_animation.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_animation.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_background.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comment_base.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_comment_base.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_comments.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_comments.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_export_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_export_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_modern_comment.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_modern_comment.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_properties.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_replace_result.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_replace_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_show_properties.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_show_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slide_show_transition.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slide_show_transition.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slides.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slides.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/slides_layout_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/slides_layout_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/smart_art.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art_node.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/smart_art_node.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/smart_art_shape.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/smart_art_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/soft_edge_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/soft_edge_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/solid_fill.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/solid_fill.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/special_slide_type.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/special_slide_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/split_document_result.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/split_document_result.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/storage_exist.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/storage_exist.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/storage_file.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/storage_file.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/subscript_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/subscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/summary_zoom_frame.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/summary_zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/summary_zoom_section.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/summary_zoom_section.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/superscript_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/superscript_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/svg_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/svg_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/swf_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/swf_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/table.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/table.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/table_cell.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell_merge_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/table_cell_merge_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/table_cell_split_type.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/table_cell_split_type.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/table_column.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/table_column.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/table_row.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/table_row.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/task.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/task.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/text_bounds.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/text_bounds.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/text_element.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/text_element.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/text_frame_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/text_frame_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/text_item.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/text_item.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/theme.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/theme.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/three_d_format.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/three_d_format.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/tiff_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/tiff_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/tint_effect.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/tint_effect.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/update_background.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/update_background.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/update_shape.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/update_shape.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/vba_module.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/vba_module.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/vba_project.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/vba_project.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/vba_reference.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/vba_reference.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/video_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/video_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/video_frame.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/video_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/view_properties.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/view_properties.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/workbook.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/workbook.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/xaml_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/xaml_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/xps_export_options.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/xps_export_options.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/xy_series.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/xy_series.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/zoom_frame.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/zoom_frame.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/models/zoom_object.py` & `asposeslidescloud-24.5.0/asposeslidescloud/models/zoom_object.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/oauth_response.py` & `asposeslidescloud-24.5.0/asposeslidescloud/oauth_response.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud/rest.py` & `asposeslidescloud-24.5.0/asposeslidescloud/rest.py`

 * *Files identical despite different names*

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud.egg-info/PKG-INFO` & `asposeslidescloud-24.5.0/asposeslidescloud.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asposeslidescloud
-Version: 24.4.0
+Version: 24.5.0
 Summary: Aspose.Slides Cloud SDK for Python
 Home-page: 
 Author: Victor Putrov
 Author-email: vistor.putrov@aspose.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -36,14 +36,21 @@
 ## Save Presentation As
 
 **Fixed Layout:** XPS
 **Images:** JPEG, PNG, BMP, TIFF, GIF, SVG
 **Web:** HTML/HTML5
 **Other:** MPEG4, SWF (export whole presentations)
 
+## Enhancements in Version 24.5
+
+* Added **options** parameter to **ImportFromPdf** method. You can specify **options.DetectTables** property to control import behavior.
+* Added **Title** property to **Axis** class for charts.
+* Added **X**, **Y**, **Width**, **Height**, **Overlay**, **FillFormat**, **EffectFormat** and **LineFormat** properties to **ChartTitle** class.
+* Added **HasTitle** property to **Chart** class; removed **HasTitle** property from **ChartTitle** class.
+
 ## Enhancements in Version 24.4
 
 * Added **DownloadMathPortion** and **SaveMathPortion** methods to convert math portions to math markup formats (MathML or LaTeX). See [documentation](https://docs.aspose.cloud/slides/export-a-math-formula/) for more info. **DownloadPortionAsMathML** and **SavePortionAsMathML** methods are deprecated and will be removed after 24.6.
 * Added **Marker** property to **DataPoint** class.
 
 ## Enhancements in Version 24.3
```

### Comparing `asposeslidescloud-24.4.0/asposeslidescloud.egg-info/SOURCES.txt` & `asposeslidescloud-24.5.0/asposeslidescloud.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -166,14 +166,15 @@
 asposeslidescloud/models/paragraph_format.py
 asposeslidescloud/models/paragraphs.py
 asposeslidescloud/models/path_input_file.py
 asposeslidescloud/models/path_output_file.py
 asposeslidescloud/models/path_segment.py
 asposeslidescloud/models/pattern_fill.py
 asposeslidescloud/models/pdf_export_options.py
+asposeslidescloud/models/pdf_import_options.py
 asposeslidescloud/models/picture_fill.py
 asposeslidescloud/models/picture_frame.py
 asposeslidescloud/models/pipeline.py
 asposeslidescloud/models/placeholder.py
 asposeslidescloud/models/placeholders.py
 asposeslidescloud/models/plot_area.py
 asposeslidescloud/models/portion.py
```

### Comparing `asposeslidescloud-24.4.0/setup.py` & `asposeslidescloud-24.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="asposeslidescloud",
-    version="24.4.0",
+    version="24.5.0",
     author="Victor Putrov",
     author_email="vistor.putrov@aspose.com",
     description="Aspose.Slides Cloud SDK for Python",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="",
     packages=setuptools.find_packages(),
```

