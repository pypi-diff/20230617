# Comparing `tmp/ezdxf-1.1.0b3.zip` & `tmp/ezdxf-1.1.0b4.zip`

## zipinfo {}

```diff
@@ -1,841 +1,843 @@
-Zip file size: 2111295 bytes, number of entries: 839
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/LICENSE
--rw-rw-rw-  2.0 fat      302 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/MANIFEST.in
--rw-rw-rw-  2.0 fat   101826 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/NEWS.md
--rw-rw-rw-  2.0 fat    69693 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/PKG-INFO
--rw-rw-rw-  2.0 fat     6142 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/README.md
--rw-rw-rw-  2.0 fat       55 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/requirements.txt
--rw-rw-rw-  2.0 fat       74 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/setup.cfg
--rw-rw-rw-  2.0 fat     5402 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat      410 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/conftest.py
--rw-rw-rw-  2.0 fat     1054 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     4686 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4133 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      871 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      998 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1558 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      905 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_hpgl2_addon.py
--rw-rw-rw-  2.0 fat      630 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     2230 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2392 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6944 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     5375 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     3060 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat     1592 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    16295 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/PLOTFILE.plt
--rw-rw-rw-  2.0 fat    28788 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4710 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19818 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5324 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7888 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    14858 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    31103 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22100 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    52708 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat    16248 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    13948 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10333 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107500 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat     3241 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/npshapes.py
--rw-rw-rw-  2.0 fat     2567 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    33129 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9580 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    30769 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat    10364 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5750 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    63359 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    10898 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     2566 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     3259 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6072 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat     9983 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    12964 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat       90 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/construct.pxd
--rw-rw-rw-  2.0 fat     6584 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3113 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23989 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      386 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    23742 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     2014 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23705 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1784 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.cpp
--rw-rw-rw-  2.0 fat      599 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.hpp
--rw-rw-rw-  2.0 fat      424 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.pxd
--rw-rw-rw-  2.0 fat      960 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.cpp
--rw-rw-rw-  2.0 fat      464 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.hpp
--rw-rw-rw-  2.0 fat      407 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.pxd
--rw-rw-rw-  2.0 fat     2135 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.hpp
--rw-rw-rw-  2.0 fat      572 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.pxd
--rw-rw-rw-  2.0 fat     1265 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6393 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      884 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5484 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6726 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2980 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28991 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4088 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12823 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18690 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13184 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26415 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31371 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22037 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    36445 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8940 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13528 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16400 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22496 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27198 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7615 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    12789 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     3842 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/xplayer.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat    10023 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29367 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1281 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    21111 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     2214 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1382 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     7319 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat     3960 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/clipper.py
--rw-rw-rw-  2.0 fat     9824 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     1707 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      514 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat     7295 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/dxf.py
--rw-rw-rw-  2.0 fat    47447 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1823 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    19510 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/hpgl2.py
--rw-rw-rw-  2.0 fat    14662 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/layout.py
--rw-rw-rw-  2.0 fat    12506 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     9878 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    38974 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    14612 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pymupdf.py
--rw-rw-rw-  2.0 fat    11034 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    22624 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat     9998 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/recorder.py
--rw-rw-rw-  2.0 fat    14923 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/svg.py
--rw-rw-rw-  2.0 fat    13023 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat      963 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      314 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/unified_text_renderer.py
--rw-rw-rw-  2.0 fat      171 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat    13459 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     8584 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      563 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat    16079 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4836 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat    11774 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1708 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     5615 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     6222 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat    19451 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/viewer.py
--rw-rw-rw-  2.0 fat      164 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     4757 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    18315 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat    25923 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4890 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    26138 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10536 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50143 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7961 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat    23664 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48743 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35012 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23829 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    42404 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    26923 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15279 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23699 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13746 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4170 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23785 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    26057 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    27932 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    27834 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14252 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    12978 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9677 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    18878 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19653 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    18435 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57367 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37144 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48153 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6284 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2111 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16427 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40087 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10443 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat    24085 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8246 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat    17602 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9035 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3597 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14366 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    28300 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8495 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3127 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    24773 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/fonts.py
--rw-rw-rw-  2.0 fat     2242 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/font_face.py
--rw-rw-rw-  2.0 fat    17004 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/font_manager.py
--rw-rw-rw-  2.0 fat     1702 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/font_measurements.py
--rw-rw-rw-  2.0 fat      825 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/glyphs.py
--rw-rw-rw-  2.0 fat    10794 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/lff.py
--rw-rw-rw-  2.0 fat    35217 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/shapefile.py
--rw-rw-rw-  2.0 fat     7219 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/ttfonts.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/__init__.py
--rw-rw-rw-  2.0 fat    16696 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    29785 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16500 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     1614 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    17013 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7447 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    13058 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14336 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat     8952 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12064 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17069 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19193 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    16270 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9318 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2452 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    52916 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9002 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    24003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    12236 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26265 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1283 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    22048 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    38883 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10231 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8256 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15921 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11867 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     3910 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat     2568 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/surfaces.py
--rw-rw-rw-  2.0 fat    12155 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3631 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    16976 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     7213 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    12967 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat     7272 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2261 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24954 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    27606 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25912 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     2003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1306 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    39194 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     6748 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    20453 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10140 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34708 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat     2987 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.css
--rw-rw-rw-  2.0 fat     1148 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.html
--rw-rw-rw-  2.0 fat    11304 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.js
--rw-rw-rw-  2.0 fat    17144 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.py
--rw-rw-rw-  2.0 fat     3770 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/pprint.py
--rw-rw-rw-  2.0 fat      812 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.css
--rw-rw-rw-  2.0 fat      316 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.html
--rw-rw-rw-  2.0 fat     2545 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.py
--rw-rw-rw-  2.0 fat     6896 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/reflinks.py
--rw-rw-rw-  2.0 fat      123 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/__init__.py
--rw-rw-rw-  2.0 fat    10039 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17749 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    52028 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    24213 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    64121 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60923 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22541 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16508 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11953 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    60696 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26581 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20434 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7645 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1256 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6049 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    65523 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54234 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6893 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3077 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     3564 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       47 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    69693 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      302 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    31857 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/
--rw-rw-rw-  2.0 fat      410 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/conftest.py
--rw-rw-rw-  2.0 fat     2336 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5456 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8168 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8682 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
--rw-rw-rw-  2.0 fat     1500 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat    11689 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4001 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9199 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8242 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     4947 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     6312 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5930 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6882 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7181 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12020 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15116 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis.py
--rw-rw-rw-  2.0 fat     6799 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis_2.py
--rw-rw-rw-  2.0 fat     1854 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_surface.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11313 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4795 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat      821 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12327 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7289 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat   112800 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      579 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_507_dxf_pretty_printer.py
--rw-rw-rw-  2.0 fat      657 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    17710 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     9269 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_515a_fonts_truetype.py
--rw-rw-rw-  2.0 fat     4729 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_515b_fonts_shapefiles.py
--rw-rw-rw-  2.0 fat     2225 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_515c_fonts_lff.py
--rw-rw-rw-  2.0 fat     4002 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24496 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     5207 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12366 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    43206 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    47978 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     6887 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat     3159 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_539_npshapes.py
--rw-rw-rw-  2.0 fat     2605 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_540_lff_parser.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7460 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14651 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2801 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9738 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    13943 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     2586 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_613_point_in_poygon.py
--rw-rw-rw-  2.0 fat    10913 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     6384 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    18821 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    11327 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10809 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10714 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10204 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4021 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    19463 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    10941 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     8993 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     4243 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9011 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3168 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11628 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34220 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     3852 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    33834 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27351 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3633 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4118 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11778 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12386 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    10862 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    11353 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_811a_drawing_frontend.py
--rw-rw-rw-  2.0 fat     4310 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_811b_drawing_recorder.py
--rw-rw-rw-  2.0 fat     2898 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_811c_viewport_processing.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    12547 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    14853 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15655 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1376 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat      976 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_822_clipper.py
--rw-rw-rw-  2.0 fat     5284 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_823_drawing_layout.py
--rw-rw-rw-  2.0 fat     3255 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_824_svg_drawing_backend.py
--rw-rw-rw-  2.0 fat     1965 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
--rw-rw-rw-  2.0 fat     2527 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     2142 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3158 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1452 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4755 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_749_text_layout.py
--rw-rw-rw-  2.0 fat    11094 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
-839 files, 8700179 bytes uncompressed, 1960443 bytes compressed:  77.5%
+Zip file size: 2119905 bytes, number of entries: 841
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/LICENSE
+-rw-rw-rw-  2.0 fat      302 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/MANIFEST.in
+-rw-rw-rw-  2.0 fat   102011 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/NEWS.md
+-rw-rw-rw-  2.0 fat    69878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/PKG-INFO
+-rw-rw-rw-  2.0 fat     6142 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/README.md
+-rw-rw-rw-  2.0 fat       55 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/requirements.txt
+-rw-rw-rw-  2.0 fat       74 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/setup.cfg
+-rw-rw-rw-  2.0 fat     5576 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      410 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4133 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      871 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      905 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_hpgl2_addon.py
+-rw-rw-rw-  2.0 fat      630 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     5375 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat     1592 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    16295 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/PLOTFILE.plt
+-rw-rw-rw-  2.0 fat    28788 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4710 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19818 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7888 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    14858 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    31103 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22100 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    52708 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat    16248 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    13948 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10333 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107500 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat    16588 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     2743 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    33129 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9580 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    30769 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat    10364 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5750 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    63359 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    10898 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     2566 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     3259 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6072 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat     9983 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    12964 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat       90 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/construct.pxd
+-rw-rw-rw-  2.0 fat     6584 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3113 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23989 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      386 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    23742 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     1688 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/np_support.pyx
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23701 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+-rw-rw-rw-  2.0 fat      599 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+-rw-rw-rw-  2.0 fat      424 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+-rw-rw-rw-  2.0 fat      960 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.cpp
+-rw-rw-rw-  2.0 fat      464 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.hpp
+-rw-rw-rw-  2.0 fat      407 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.pxd
+-rw-rw-rw-  2.0 fat     2135 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.hpp
+-rw-rw-rw-  2.0 fat      572 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.pxd
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6393 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      884 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     5484 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6726 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2980 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28991 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4088 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    12823 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18690 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13184 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26415 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31371 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22037 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    39755 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8940 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13528 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16400 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22496 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27198 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7615 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12786 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     3351 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/xplayer.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat    10023 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29367 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1281 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    21111 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1382 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     7419 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat     4562 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/clipper.py
+-rw-rw-rw-  2.0 fat     9824 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1570 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      514 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat    18549 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/designer.py
+-rw-rw-rw-  2.0 fat     7222 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/dxf.py
+-rw-rw-rw-  2.0 fat    34083 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    19568 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/hpgl2.py
+-rw-rw-rw-  2.0 fat    14662 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/layout.py
+-rw-rw-rw-  2.0 fat    11532 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    38974 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    14436 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pymupdf.py
+-rw-rw-rw-  2.0 fat    10569 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    22624 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat    14399 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/recorder.py
+-rw-rw-rw-  2.0 fat    14803 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/svg.py
+-rw-rw-rw-  2.0 fat    13023 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat     1194 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      314 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     2559 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat    13459 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     8570 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      561 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat    16079 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat    11766 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5615 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     6222 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat    19451 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/viewer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     4757 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    18315 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat    25923 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4890 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    26138 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10536 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    50143 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7961 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat    23664 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48743 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35012 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23829 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    42404 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    26923 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    15279 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23699 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13746 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4170 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23785 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    26057 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    27932 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    27834 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14252 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    12978 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9677 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    18878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19653 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    18435 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57367 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37144 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48153 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6284 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2111 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16427 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40087 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10443 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat    24085 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8246 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat    17602 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9035 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3597 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14366 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    28300 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8495 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3127 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    25322 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/fonts.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/font_face.py
+-rw-rw-rw-  2.0 fat    17287 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/font_manager.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/font_measurements.py
+-rw-rw-rw-  2.0 fat     1175 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/glyphs.py
+-rw-rw-rw-  2.0 fat    10763 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/lff.py
+-rw-rw-rw-  2.0 fat    35446 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/shapefile.py
+-rw-rw-rw-  2.0 fat     7244 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/ttfonts.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/fonts/__init__.py
+-rw-rw-rw-  2.0 fat    16696 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    29785 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16500 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     1614 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    17013 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7447 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    13058 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14336 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat     8952 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12064 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17069 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19193 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    16270 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9318 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2452 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    52916 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9002 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    24220 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    12236 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26265 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1283 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    22048 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    38883 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10231 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8256 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15921 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11867 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     3910 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat     2568 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/surfaces.py
+-rw-rw-rw-  2.0 fat    12155 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3631 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    16976 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     7213 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    12967 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat     7272 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2261 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24954 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    27606 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25912 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     2003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    31244 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     5868 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    18249 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10140 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34217 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat     2987 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.css
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.html
+-rw-rw-rw-  2.0 fat    11304 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.js
+-rw-rw-rw-  2.0 fat    17144 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.py
+-rw-rw-rw-  2.0 fat     3770 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/pprint.py
+-rw-rw-rw-  2.0 fat      812 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.css
+-rw-rw-rw-  2.0 fat      316 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.html
+-rw-rw-rw-  2.0 fat     2545 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/reflinks.py
+-rw-rw-rw-  2.0 fat      123 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/pp/__init__.py
+-rw-rw-rw-  2.0 fat    10039 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17749 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    52044 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    24198 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    64121 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60923 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22541 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    16508 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11953 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    60696 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26581 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20434 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7645 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1256 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6049 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    65523 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54234 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6893 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3077 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     3564 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       47 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    69878 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      302 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    31923 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      410 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5456 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8168 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8682 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4001 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9199 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8242 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     4947 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     6312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6882 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7181 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12020 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15116 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis.py
+-rw-rw-rw-  2.0 fat     6799 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis_2.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_surface.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11313 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     5713 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4795 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat      821 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12327 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     7289 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      579 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_507_dxf_pretty_printer.py
+-rw-rw-rw-  2.0 fat      657 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    17710 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     9269 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_515a_fonts_truetype.py
+-rw-rw-rw-  2.0 fat     4752 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_515b_fonts_shapefiles.py
+-rw-rw-rw-  2.0 fat     2469 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_515c_fonts_lff.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5207 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12366 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7533 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    43259 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    47978 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     6887 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat    16358 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     2605 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_05_tools/test_540_lff_parser.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7460 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14651 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2801 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9738 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    13943 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_613_point_in_poygon.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     6384 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18821 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11327 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10809 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10714 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10204 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4021 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    19575 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    10941 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     8993 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9024 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3168 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11654 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34220 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     4459 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    33999 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27351 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3261 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4121 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11778 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    12386 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    15467 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    10862 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    11597 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_811a_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     8684 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_811b_drawing_recorder.py
+-rw-rw-rw-  2.0 fat     2898 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_811c_viewport_processing.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    13751 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15655 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1376 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat     1028 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_822_clipper.py
+-rw-rw-rw-  2.0 fat     5284 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_823_drawing_layout.py
+-rw-rw-rw-  2.0 fat     3312 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_824_svg_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     2142 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1452 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4755 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_749_text_layout.py
+-rw-rw-rw-  2.0 fat    11094 b- defN 23-Jun-17 05:09 ezdxf-1.1.0b4/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+841 files, 8737649 bytes uncompressed, 1968717 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,2518 +1,2524 @@
-Filename: ezdxf-1.1.0b3/
+Filename: ezdxf-1.1.0b4/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/
+Filename: ezdxf-1.1.0b4/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/
+Filename: ezdxf-1.1.0b4/src/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/
+Filename: ezdxf-1.1.0b4/tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/LICENSE
+Filename: ezdxf-1.1.0b4/LICENSE
 Comment: 
 
-Filename: ezdxf-1.1.0b3/MANIFEST.in
+Filename: ezdxf-1.1.0b4/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.1.0b3/NEWS.md
+Filename: ezdxf-1.1.0b4/NEWS.md
 Comment: 
 
-Filename: ezdxf-1.1.0b3/PKG-INFO
+Filename: ezdxf-1.1.0b4/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b3/README.md
+Filename: ezdxf-1.1.0b4/README.md
 Comment: 
 
-Filename: ezdxf-1.1.0b3/requirements.txt
+Filename: ezdxf-1.1.0b4/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b3/setup.cfg
+Filename: ezdxf-1.1.0b4/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.1.0b3/setup.py
+Filename: ezdxf-1.1.0b4/setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/
+Filename: ezdxf-1.1.0b4/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/conftest.py
+Filename: ezdxf-1.1.0b4/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_acad_table.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_document_guid.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_geo.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_groups.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_hpgl2_addon.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_hpgl2_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_launcher.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_odafc.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_r12export.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_r12strict.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_r12writer.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_recover.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.1.0b4/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/groups.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/PLOTFILE.plt
+Filename: ezdxf-1.1.0b4/integration_tests/data/PLOTFILE.plt
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.1.0b4/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.1.0b4/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.1.0b4/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.1.0b4/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b3/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.1.0b4/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/
+Filename: ezdxf-1.1.0b4/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/
+Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/
+Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/path/
+Filename: ezdxf-1.1.0b4/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/appsettings.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/audit.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/bbox.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/colors.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/commands.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/comments.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/disassemble.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/document.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entitydb.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/enums.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/explode.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/eztypes.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/groupby.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/npshapes.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/protocols.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/py.typed
+Filename: ezdxf-1.1.0b4/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/query.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/queryparser.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/r12strict.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/recover.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/reorder.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/transform.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/units.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/upright.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/urecord.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/version.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/xref.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/zoom.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/_options.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/__main__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/construct.pxd
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/construct.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/np_support.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.cpp
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.hpp
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.pxd
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.hpp
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.pxd
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/api.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/const.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.1.0b4/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/xplayer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/xplayer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/clipper.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/dxf.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/designer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/dxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/hpgl2.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/layout.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pymupdf.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pymupdf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/recorder.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/svg.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/svg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/unified_text_renderer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/viewer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/viewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/block.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/image.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/light.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/line.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/material.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/point.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/table.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/text.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/view.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/fonts.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/font_face.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/font_manager.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/fonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/font_measurements.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/font_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/glyphs.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/lff.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/font_measurements.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/shapefile.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/glyphs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/ttfonts.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/fonts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/arc.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/box.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/circle.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/line.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/shape.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/surfaces.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/surfaces.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/path/commands.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/path/converter.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/path/path.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/path/tools.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.css
+Filename: ezdxf-1.1.0b4/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.html
+Filename: ezdxf-1.1.0b4/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.js
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/pprint.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.js
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.css
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.html
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/pprint.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/reflinks.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/pp/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/pp/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/curves.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/forms.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/leader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/mline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/point.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/trace.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/header.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/table.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/test.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/text.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.1.0b4/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/
+Filename: ezdxf-1.1.0b4/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/
+Filename: ezdxf-1.1.0b4/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.1.0b4/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_10_issues/
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/conftest.py
+Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.1.0b4/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.1.0b4/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis_2.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_surface.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_surface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_507_dxf_pretty_printer.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_507_dxf_pretty_printer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_515a_fonts_truetype.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_515b_fonts_shapefiles.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_515c_fonts_lff.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_515a_fonts_truetype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_515b_fonts_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_515c_fonts_lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_539_npshapes.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_540_lff_parser.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/conftest.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.1.0b4/tests/test_05_tools/test_540_lff_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_613_point_in_poygon.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_613_point_in_poygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.1.0b4/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.1.0b4/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_811a_drawing_frontend.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_811b_drawing_recorder.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_811c_viewport_processing.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_811a_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_811b_drawing_recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_811c_viewport_processing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_822_clipper.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_823_drawing_layout.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_824_svg_drawing_backend.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_822_clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_823_drawing_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_824_svg_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.1.0b4/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_901_acc_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_902_acc_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_906_acc_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_414_bbox_calculation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_574_flattening_error.py
 Comment: 
 
-Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Comment: 
+
+Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_749_text_layout.py
+Comment: 
+
+Filename: ezdxf-1.1.0b4/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.1.0b3/LICENSE` & `ezdxf-1.1.0b4/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/NEWS.md` & `ezdxf-1.1.0b4/NEWS.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 
 News
 ====
 
-Version 1.1.0b2 - dev
----------------------
+Version 1.1.0 Beta
+------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
-- NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
 - NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF, PNG
 - NEW: native `SVG`, `HPGL/2`  and `DXF` backends for the `drawing` add-on, these backends 
   do not need additional libraries to work
 - NEW: `PyMuPdf` backend for the `drawing` add-on, support for PDF, PNG, PPM and PBM export
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
@@ -32,19 +31,23 @@
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
+- CHANGED: `BackendInterface` and all derived backends support only 2D shapes
+- REMOVED: Matplotlib/Qt path converters from `ezdxf.path.converter`
 - REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
+- BUGFIX: [#898](https://github.com/mozman/ezdxf/issues/898)
+  use `dimclrd` color for dimension arrow blocks 
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.1.0b3/PKG-INFO` & `ezdxf-1.1.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b3
+Version: 1.1.0b4
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -211,24 +211,23 @@
 Feedback is greatly appreciated.
 
 Manfred
 
 News
 ====
 
-Version 1.1.0b2 - dev
----------------------
+Version 1.1.0 Beta
+------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
-- NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
 - NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF, PNG
 - NEW: native `SVG`, `HPGL/2`  and `DXF` backends for the `drawing` add-on, these backends 
   do not need additional libraries to work
 - NEW: `PyMuPdf` backend for the `drawing` add-on, support for PDF, PNG, PPM and PBM export
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
@@ -245,19 +244,23 @@
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
+- CHANGED: `BackendInterface` and all derived backends support only 2D shapes
+- REMOVED: Matplotlib/Qt path converters from `ezdxf.path.converter`
 - REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
+- BUGFIX: [#898](https://github.com/mozman/ezdxf/issues/898)
+  use `dimclrd` color for dimension arrow blocks 
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.1.0b3/README.md` & `ezdxf-1.1.0b4/README.md`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/setup.py` & `ezdxf-1.1.0b4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,14 +71,22 @@
         "ezdxf.acc.linetypes",
         [
             "src/ezdxf/acc/linetypes.pyx",
         ],
         optional=True,
         language="c++",
     ),
+    Extension(
+        "ezdxf.acc.np_support",
+        [
+            "src/ezdxf/acc/np_support.pyx",
+        ],
+        optional=True,
+        language="c++",
+    ),
 
 ]
 try:
     from Cython.Distutils import build_ext
 
     commands = {"build_ext": build_ext}
 except ImportError:
```

## Comparing `ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.1.0b4/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_acad_table.py` & `ezdxf-1.1.0b4/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.1.0b4/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.1.0b4/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.1.0b4/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.1.0b4/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_audit_layouts.py` & `ezdxf-1.1.0b4/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.1.0b4/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.1.0b4/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_document_guid.py` & `ezdxf-1.1.0b4/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_document_page_setup.py` & `ezdxf-1.1.0b4/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.1.0b4/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_entities_iterator.py` & `ezdxf-1.1.0b4/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.1.0b4/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_geo.py` & `ezdxf-1.1.0b4/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_groups.py` & `ezdxf-1.1.0b4/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_hpgl2_addon.py` & `ezdxf-1.1.0b4/integration_tests/test_hpgl2_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.1.0b4/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_launcher.py` & `ezdxf-1.1.0b4/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.1.0b4/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.1.0b4/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.1.0b4/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_mtext_columns.py` & `ezdxf-1.1.0b4/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.1.0b4/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.1.0b4/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_new_table_entries.py` & `ezdxf-1.1.0b4/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.1.0b4/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_odafc.py` & `ezdxf-1.1.0b4/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.1.0b4/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.1.0b4/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.1.0b4/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_open_R13_R14.py` & `ezdxf-1.1.0b4/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_polyline_entity.py` & `ezdxf-1.1.0b4/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.1.0b4/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_r12export.py` & `ezdxf-1.1.0b4/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_r12strict.py` & `ezdxf-1.1.0b4/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_r12writer.py` & `ezdxf-1.1.0b4/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.1.0b4/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.1.0b4/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_recover.py` & `ezdxf-1.1.0b4/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_redraw_order.py` & `ezdxf-1.1.0b4/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.1.0b4/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_surface_entities.py` & `ezdxf-1.1.0b4/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.1.0b4/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_write_without_handles.py` & `ezdxf-1.1.0b4/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/test_xref_detach.py` & `ezdxf-1.1.0b4/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.1.0b4/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.1.0b4/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.1.0b4/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.1.0b4/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.1.0b4/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.1.0b4/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.1.0b4/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.1.0b4/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/empty_handles.dxf` & `ezdxf-1.1.0b4/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/groups.dxf` & `ezdxf-1.1.0b4/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.1.0b4/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/MODEL.dxf` & `ezdxf-1.1.0b4/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.1.0b4/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.1.0b4/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.1.0b4/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/no_layouts.dxf` & `ezdxf-1.1.0b4/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/PLOTFILE.plt` & `ezdxf-1.1.0b4/integration_tests/data/PLOTFILE.plt`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.1.0b4/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/recover01.dxf` & `ezdxf-1.1.0b4/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/recover02.dxf` & `ezdxf-1.1.0b4/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/small_r13.dxf` & `ezdxf-1.1.0b4/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/small_r14.dxf` & `ezdxf-1.1.0b4/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.1.0b4/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.1.0b4/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.1.0b4/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/appsettings.py` & `ezdxf-1.1.0b4/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/audit.py` & `ezdxf-1.1.0b4/src/ezdxf/audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/bbox.py` & `ezdxf-1.1.0b4/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/blkrefs.py` & `ezdxf-1.1.0b4/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/colors.py` & `ezdxf-1.1.0b4/src/ezdxf/colors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/commands.py` & `ezdxf-1.1.0b4/src/ezdxf/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/comments.py` & `ezdxf-1.1.0b4/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/disassemble.py` & `ezdxf-1.1.0b4/src/ezdxf/disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/document.py` & `ezdxf-1.1.0b4/src/ezdxf/document.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/dwginfo.py` & `ezdxf-1.1.0b4/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entitydb.py` & `ezdxf-1.1.0b4/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/enums.py` & `ezdxf-1.1.0b4/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/explode.py` & `ezdxf-1.1.0b4/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/eztypes.py` & `ezdxf-1.1.0b4/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/filemanagement.py` & `ezdxf-1.1.0b4/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/gfxattribs.py` & `ezdxf-1.1.0b4/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/graphicsfactory.py` & `ezdxf-1.1.0b4/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/groupby.py` & `ezdxf-1.1.0b4/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/npshapes.py` & `ezdxf-1.1.0b4/src/ezdxf/math/shape.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,96 +1,112 @@
-#  Copyright (c) 2023, Manfred Moitzi
-#  License: MIT License
+# Copyright (c) 2019-2022 Manfred Moitzi
+# License: MIT License
 from __future__ import annotations
-from typing import Iterable
-import abc
+from typing import Union, Iterable, Optional
+import math
+from ezdxf.math import Vec2, UVec
+from .construct2d import convex_hull_2d
+from .offset2d import offset_vertices_2d
+from .bbox import BoundingBox2d
 
-import numpy as np
-from ezdxf.math import Matrix44, Vec2, UVec
-from ezdxf.path import AbstractPath, Path2d, Command
 
-__all__ = ["NumpyPath2d", "NumpyPoints2d", "NumpyShapesException", "EmptyShapeError"]
+__all__ = ["Shape2d"]
 
 
-class NumpyShapesException(Exception):
-    pass
+class Shape2d:
+    """Construction tools for 2D shapes.
 
+    A 2D geometry object as list of :class:`Vec2` objects, vertices can be
+    moved, rotated and scaled.
 
-class EmptyShapeError(NumpyShapesException):
-    pass
+    Args:
+        vertices: iterable of :class:`Vec2` compatible objects.
 
-
-class NumpyShape2d(abc.ABC):
-    """This is an optimization to store many 2D paths and polylines in a compact way
-    without sacrificing basic functions like transformation and bounding box calculation.
     """
 
-    _vertices: np.ndarray
-
-    def extents(self) -> tuple[Vec2, Vec2]:
-        """Returns the extents of the bounding box as tuple (extmin, extmax)."""
-        v = self._vertices
-        if len(v) > 0:
-            return Vec2(v.min(0)), Vec2(v.max(0))
-        else:
-            raise EmptyShapeError("empty shape has no extends")
-
-    def transform_inplace(self, m: Matrix44) -> None:
-        """Transforms the vertices of the shape inplace."""
-        v = self._vertices
-        if len(v) == 0:
-            return
-        m.transform_array_inplace(v, 2)
-
-    def vertices(self) -> list[Vec2]:
-        """Returns the shape vertices as list of :class:`Vec2`."""
-        return Vec2.list(self._vertices)
-
+    def __init__(self, vertices: Optional[Iterable[UVec]] = None):
+        self.vertices: list[Vec2] = (
+            [] if vertices is None else Vec2.list(vertices)
+        )
+
+    @property
+    def bounding_box(self) -> BoundingBox2d:
+        """:class:`BoundingBox2d`"""
+        return BoundingBox2d(self.vertices)
+
+    def copy(self) -> Shape2d:
+        return self.__class__(self.vertices)
+
+    __copy__ = copy
+
+    def translate(self, vector: UVec) -> None:
+        """Translate shape about `vector`."""
+        delta = Vec2(vector)
+        self.vertices = [v + delta for v in self.vertices]
+
+    def scale(self, sx: float = 1.0, sy: float = 1.0) -> None:
+        """Scale shape about `sx` in x-axis and `sy` in y-axis."""
+        self.vertices = [Vec2((v.x * sx, v.y * sy)) for v in self.vertices]
+
+    def scale_uniform(self, scale: float) -> None:
+        """Scale shape uniform about `scale` in x- and y-axis."""
+        self.vertices = [v * scale for v in self.vertices]
+
+    def rotate(self, angle: float, center: Optional[UVec] = None) -> None:
+        """Rotate shape around rotation `center` about `angle` in degrees."""
+        self.rotate_rad(math.radians(angle), center)
+
+    def rotate_rad(self, angle: float, center: Optional[UVec] = None) -> None:
+        """Rotate shape around rotation `center` about `angle` in radians."""
+        if center is not None:
+            center = Vec2(center)
+            self.translate(-center)  # faster than a Matrix44 multiplication
+        self.vertices = [v.rotate(angle) for v in self.vertices]
+        if center is not None:
+            self.translate(center)  # faster than a Matrix44 multiplication
+
+    def offset(self, offset: float, closed: bool = False) -> Shape2d:
+        """Returns a new offset shape, for more information see also
+        :func:`ezdxf.math.offset_vertices_2d` function.
+
+        Args:
+            offset: line offset perpendicular to direction of shape segments
+                defined by vertices order, offset > ``0`` is 'left' of line
+                segment, offset < ``0`` is 'right' of line segment
+            closed: ``True`` to handle as closed shape
+
+        """
+        return self.__class__(
+            offset_vertices_2d(self.vertices, offset=offset, closed=closed)
+        )
+
+    def convex_hull(self) -> Shape2d:
+        """Returns convex hull as new shape."""
+        return self.__class__(convex_hull_2d(self.vertices))
 
-class NumpyPoints2d(NumpyShape2d):
-    """Represents an array of 2D points stored as a ndarray."""
+    # Sequence interface
+    def __len__(self) -> int:
+        """Returns `count` of vertices."""
+        return len(self.vertices)
 
-    def __init__(self, points: Iterable[UVec]) -> None:
-        self._vertices = np.array(Vec2.list(points), dtype=np.float64)
+    def __getitem__(self, item: Union[int, slice]) -> Vec2:
+        """Get vertex by index `item`, supports ``list`` like slicing."""
+        return self.vertices[item]
 
-    def __len__(self) -> int:
-        return len(self._vertices)
+    # limited List interface
+    def append(self, vertex: UVec) -> None:
+        """Append single `vertex`.
 
+        Args:
+             vertex: vertex as :class:`Vec2` compatible object
 
-class NumpyPath2d(NumpyShape2d):
-    """Represents a 2D path, the path control vertices and commands are stored as ndarray."""
+        """
+        self.vertices.append(Vec2(vertex))
 
-    def __init__(self, path: AbstractPath) -> None:
-        vertices = Vec2.list(path.control_vertices())
-        if len(vertices) == 0:
-            try:  # control_vertices() does not return start point of empty paths
-                vertices = [path.start]
-            except IndexError:
-                vertices = [Vec2()]  # default start point of empty paths
-        self._vertices = np.array(vertices, dtype=np.float64)
-        self._commands = np.array(path.command_codes(), dtype=np.int8)
+    def extend(self, vertices: Iterable) -> None:
+        """Append multiple `vertices`.
 
-    def __len__(self) -> int:
-        return len(self._commands)
+        Args:
+             vertices: iterable of vertices as :class:`Vec2` compatible objects
 
-    def to_path2d(self) -> Path2d:
-        v = self._vertices
-        if len(v) == 0:
-            return Path2d()
-        path = Path2d(v[0])
-        index = 1
-        for command in self._commands:
-            if command == Command.MOVE_TO:
-                path.move_to(v[index])
-                index += 1
-            elif command == Command.LINE_TO:
-                path.line_to(v[index])
-                index += 1
-            elif command == Command.CURVE3_TO:
-                path.curve3_to(v[index + 1], v[index])
-                index += 2
-            elif command == Command.CURVE4_TO:
-                path.curve4_to(v[index + 2], v[index], v[index + 1])
-                index += 3
-            else:
-                raise ValueError(f"invalid command: {command}")
-        return path
+        """
+        self.vertices.extend(Vec2.generate(vertices))
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/protocols.py` & `ezdxf-1.1.0b4/src/ezdxf/protocols.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from __future__ import annotations
 from typing import TYPE_CHECKING, Iterator, Iterable
 from typing_extensions import Protocol, runtime_checkable
 from ezdxf.query import EntityQuery
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFGraphic, DXFEntity
-    from ezdxf.math import Matrix44
+    from ezdxf.math import Matrix44, AbstractBoundingBox
 
 
 # Protocol implemented for:
 # - DXFTagStorage
 # - ACAD_PROXY_ENTITY
 # - INSERT
 # - DIMENSION
@@ -77,7 +77,14 @@
     """Returns the handles to the BLOCK_RECORD entities for all BLOCK
     definitions used by an entity.
     """
     if isinstance(entity, ReferencedBlocks):
         return entity.__referenced_blocks__()
     else:
         return _EMPTY_TUPLE
+
+
+class SupportsBoundingBox(Protocol):
+    def bbox(self) -> AbstractBoundingBox:
+        """Returns the bounding box of an object."""
+        ...
+
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/proxygraphic.py` & `ezdxf-1.1.0b4/src/ezdxf/proxygraphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/query.py` & `ezdxf-1.1.0b4/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/queryparser.py` & `ezdxf-1.1.0b4/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/r12strict.py` & `ezdxf-1.1.0b4/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/recover.py` & `ezdxf-1.1.0b4/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/reorder.py` & `ezdxf-1.1.0b4/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/transform.py` & `ezdxf-1.1.0b4/src/ezdxf/transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/units.py` & `ezdxf-1.1.0b4/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/upright.py` & `ezdxf-1.1.0b4/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/urecord.py` & `ezdxf-1.1.0b4/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/version.py` & `ezdxf-1.1.0b4/src/ezdxf/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 1, 0, "b3")
-__version__ = "1.1.0b3"
+version = (1, 1, 0, "b4")
+__version__ = "1.1.0b4"
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/xref.py` & `ezdxf-1.1.0b4/src/ezdxf/xref.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/zoom.py` & `ezdxf-1.1.0b4/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/_options.py` & `ezdxf-1.1.0b4/src/ezdxf/_options.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/__init__.py` & `ezdxf-1.1.0b4/src/ezdxf/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/__main__.py` & `ezdxf-1.1.0b4/src/ezdxf/__main__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.1.0b4/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.1.0b4/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.1.0b4/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/construct.pyx` & `ezdxf-1.1.0b4/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.1.0b4/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.1.0b4/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.1.0b4/src/ezdxf/acc/matrix44.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/vector.pxd` & `ezdxf-1.1.0b4/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/vector.pyx` & `ezdxf-1.1.0b4/src/ezdxf/acc/vector.pyx`

 * *Files 0% similar despite different names*

```diff
@@ -194,15 +194,15 @@
         return res
 
     reversed = __neg__
 
     def __bool__(self) -> bool:
         return self.x != 0 or self.y != 0
 
-    def isclose(self, other: "AnyVec", *, double rel_tol=REL_TOL,
+    def isclose(self, other: UVec, *, double rel_tol=REL_TOL,
                 double abs_tol = ABS_TOL) -> bool:
         cdef Vec2 o = Vec2(other)
         return isclose(self.x, o.x, rel_tol, abs_tol) and \
                isclose(self.y, o.y, rel_tol, abs_tol)
 
     def __eq__(self, other: UVec) -> bool:
         if not isinstance(other, Vec2):
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.cpp` & `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.hpp` & `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_cubic_bezier.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.cpp` & `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_quad_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.hpp` & `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.pxd` & `ezdxf-1.1.0b4/src/ezdxf/acc/_cpp_vec3.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acc/__init__.py` & `ezdxf-1.1.0b4/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/abstract.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/api.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/const.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/dbg.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/dxf.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/entities.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/hdr.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/mesh.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/sab.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/acis/sat.py` & `ezdxf-1.1.0b4/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/acadctb.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/binpacking.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/dimlines.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/geo.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/geo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,53 +1,61 @@
-#  Copyright (c) 2020-2022, Manfred Moitzi
+#  Copyright (c) 2020-2023, Manfred Moitzi
 #  License: MIT License
 """
 Implementation of the `__geo_interface__`: https://gist.github.com/sgillies/2217756
 
 Which is also supported by Shapely: https://pypi.org/project/Shapely/
 
 Type definitions see GeoJson Standard: https://tools.ietf.org/html/rfc7946
 and examples : https://tools.ietf.org/html/rfc7946#appendix-A
 
+GeoJSON Linter: https://geojsonlint.com/
+
 """
 from __future__ import annotations
 from typing import (
     Iterable,
+    Iterator,
     Union,
     cast,
     Callable,
     Sequence,
     Optional,
+    Any,
+    MutableMapping,
 )
+from typing_extensions import TypeAlias, Self
 import numbers
 import copy
 import math
+import enum
 from ezdxf.math import Vec3, has_clockwise_orientation, Matrix44
-from ezdxf.path import make_path, from_hatch_boundary_path, fast_bbox_detection
-from ezdxf.entities import DXFGraphic, LWPolyline, Point, Polyline, Line, Solid
+from ezdxf.path import make_path, from_hatch_boundary_path, make_polygon_structure
+from ezdxf.entities import DXFGraphic, LWPolyline, Point, Polyline, Line
 from ezdxf.entities.polygon import DXFPolygon
 from ezdxf.lldxf import const
 from ezdxf.entities import factory
 
 
-__all__ = ["proxy", "dxf_entities", "gfilter", "GeoProxy"]
+__all__ = ["proxy", "dxf_entities", "gfilter", "GeoProxy", "PolygonConversion"]
 
 TYPE = "type"
 COORDINATES = "coordinates"
 POINT = "Point"
 MULTI_POINT = "MultiPoint"
 LINE_STRING = "LineString"
 MULTI_LINE_STRING = "MultiLineString"
 POLYGON = "Polygon"
 MULTI_POLYGON = "MultiPolygon"
 GEOMETRY_COLLECTION = "GeometryCollection"
 GEOMETRIES = "geometries"
 GEOMETRY = "geometry"
 FEATURES = "features"
 FEATURE = "Feature"
+PROPERTIES = "properties"
 FEATURE_COLLECTION = "FeatureCollection"
 MAX_FLATTENING_DISTANCE = 0.1
 SUPPORTED_DXF_TYPES = {
     "POINT",
     "LINE",
     "LWPOLYLINE",
     "POLYLINE",
@@ -58,20 +66,40 @@
     "3DFACE",
     "CIRCLE",
     "ARC",
     "ELLIPSE",
     "SPLINE",
 }
 
+GeoMapping: TypeAlias = MutableMapping[str, Any]
+PostProcessFunc: TypeAlias = Callable[[DXFGraphic, GeoMapping], None]
+
+
+class PolygonConversion(enum.IntEnum):
+    """Polygon conversion types as :class:`IntEnum`.
+
+    Attributes:
+        HATCH:
+        POLYLINE:
+        HATCH_AND_POLYLINE:
+        MPOLYGON:
+
+    """
+
+    HATCH = 1
+    POLYLINE = 2
+    HATCH_AND_POLYLINE = 3
+    MPOLYGON = 4
+
 
 def proxy(
     entity: Union[DXFGraphic, Iterable[DXFGraphic]],
     distance: float = MAX_FLATTENING_DISTANCE,
     force_line_string: bool = False,
-) -> "GeoProxy":
+) -> GeoProxy:
     """Returns a :class:`GeoProxy` object.
 
     Args:
         entity: a single DXF entity or iterable of DXF entities
         distance: maximum flattening distance for curve approximations
         force_line_string: by default this function returns Polygon objects for
             closed geometries like CIRCLE, SOLID, closed POLYLINE and so on,
@@ -79,60 +107,70 @@
             will be returned as LineString objects.
 
     """
     return GeoProxy.from_dxf_entities(entity, distance, force_line_string)
 
 
 def dxf_entities(
-    geo_mapping, polygon: int = 1, dxfattribs = None
-) -> Iterable[DXFGraphic]:
+    geo_mapping: GeoMapping,
+    polygon=PolygonConversion.HATCH,
+    dxfattribs=None,
+    *,
+    post_process: Optional[PostProcessFunc] = None,
+) -> Iterator[DXFGraphic]:
     """Returns ``__geo_interface__`` mappings as DXF entities.
 
-    The `polygon` argument determines the method to convert polygons,
-    use 1 for :class:`~ezdxf.entities.Hatch` entity, 2 for
-    :class:`~ezdxf.entities.LWPolyline` or 3 for both.
-    Option 2 returns for the exterior path and each hole a separated
-    :class:`LWPolyline` entity. The :class:`Hatch` entity supports holes,
-    but has no explicit border line.
+    The enum `polygon` determines the method to convert polygons,
+    use :attr:`PolygonConversion.HATCH` for :class:`~ezdxf.entities.Hatch` entity,
+    :attr:`PolygonConversion.POLYLINE` for :class:`~ezdxf.entities.LWPolyline` or
+    :attr:`PolygonConversion.HATCH_AND_POLYLINE` for both.
+    Option :attr:`PolygonConversion.POLYLINE` returns for the exterior path and each hole
+    a separated :class:`LWPolyline` entity. The :class:`Hatch` entity supports holes,
+    but has no explicit borderline.
 
     Yields :class:`Hatch` always before :class:`LWPolyline` entities.
 
-    :class:`~ezdxf.entities.MPolygon` support was added in v0.16.6, which is
-    like a :class:`~ezdxf.entities.Hatch` entity  with additional border
-    lines, but the MPOLYGON entity is not a core DXF entity and DXF viewers,
+    :attr:`PolygonConversion.MPOLYGON` support was added in v0.16.6, which is
+    like a :class:`~ezdxf.entities.Hatch` entity  with additional borderlines,
+    but the MPOLYGON entity is not a core DXF entity and DXF viewers,
     applications and libraries my not support this entity. The DXF attribute
-    `color` defines the border line color and `fill_color` the color of the
+    `color` defines the borderline color and `fill_color` the color of the
     solid filling.
 
     The returned DXF entities can be added to a layout by the
     :meth:`Layout.add_entity` method.
 
     Args:
         geo_mapping: ``__geo__interface__`` mapping as :class:`dict` or a Python
             object with a :attr:`__geo__interface__` property
-        polygon: method to convert polygons (1-2-3-4)
+        polygon: see :class:`PolygonConversion`
         dxfattribs: dict with additional DXF attributes
+        post_process: post process function of type :class:`PostProcesFunc` that get the
+            created DXF entity and the geo mapping as input, see reference implementation
+            :func:`assign_layers`
 
     """
-    return GeoProxy.parse(geo_mapping).to_dxf_entities(polygon, dxfattribs)
+    return GeoProxy.parse(geo_mapping).to_dxf_entities(
+        polygon, dxfattribs, post_process=post_process
+    )
 
 
-def gfilter(entities: Iterable[DXFGraphic]) -> Iterable[DXFGraphic]:
+def gfilter(entities: Iterable[DXFGraphic]) -> Iterator[DXFGraphic]:
     """Filter DXF entities from iterable `entities`, which are incompatible to
     the ``__geo_reference__`` interface.
     """
     for e in entities:
         if isinstance(e, Polyline):
             if e.is_2d_polyline or e.is_3d_polyline:
                 yield e
         elif e.dxftype() in SUPPORTED_DXF_TYPES:
             yield e
 
 
-TFunc = Callable[[Vec3], Vec3]
+TFunc: TypeAlias = Callable[[Vec3], Vec3]
 
 
 class GeoProxy:
     """Stores the ``__geo_interface__`` mapping in a parsed and compiled form.
 
     Stores coordinates as :class:`Vec3` objects and represents "Polygon"
     always as tuple (exterior, holes) even without holes.
@@ -144,79 +182,83 @@
 
     Args:
         geo_mapping: parsed and compiled ``__geo_interface__`` mapping
         places: decimal places to round for ``__geo_interface__`` export
 
     """
 
-    def __init__(self, geo_mapping: dict, places: int = 6):
+    def __init__(self, geo_mapping: GeoMapping, places: int = 6):
         self._root = geo_mapping
         self.places = places
 
     @classmethod
-    def parse(cls, geo_mapping) -> "GeoProxy":
+    def parse(cls, geo_mapping: GeoMapping) -> Self:
         """Parse and compile a ``__geo_interface__`` mapping as :class:`dict`
         or a Python object with a ``__geo_interface__`` property, does some
         basic syntax checks, converts all coordinates into :class:`Vec3`
         objects, represents "Polygon" always as tuple (exterior, holes) even
         without holes.
 
         """
         if hasattr(geo_mapping, "__geo_interface__"):
             geo_mapping = geo_mapping.__geo_interface__
         return cls(parse(geo_mapping))
 
     @property
-    def root(self) -> dict:
+    def root(self) -> GeoMapping:
         return self._root
 
     @property
     def geotype(self):
         """Property returns the top level entity type or ``None``."""
         return self._root.get("type")
 
-    def __copy__(self) -> "GeoProxy":
+    def __copy__(self) -> GeoProxy:
         """Returns a deep copy."""
         return copy.deepcopy(self)
 
     copy = __copy__
 
     @property
-    def __geo_interface__(self) -> dict:
+    def __geo_interface__(self) -> GeoMapping:
         """Returns the ``__geo_interface__`` compatible mapping as
         :class:`dict`.
         """
         return _rebuild(self._root, self.places)
 
-    def __iter__(self) -> Iterable[dict]:
-        """Iterate over all geo content objects.
+    def __iter__(self) -> Iterator[GeoMapping]:
+        """Iterate over all geometry entities.
 
         Yields only "Point", "LineString", "Polygon", "MultiPoint",
         "MultiLineString" and "MultiPolygon" objects, returns the content of
         "GeometryCollection", "FeatureCollection" and "Feature" as geometry
         objects ("Point", ...).
 
         """
 
-        def _iter(root):
-            type_ = root[TYPE]
+        def _iter(node: GeoMapping) -> Iterator[GeoMapping]:
+            type_ = node[TYPE]
             if type_ == FEATURE_COLLECTION:
-                for feature in root[FEATURES]:
+                for feature in node[FEATURES]:
                     yield from _iter(feature)
             elif type_ == GEOMETRY_COLLECTION:
-                for geometry in root[GEOMETRIES]:
+                for geometry in node[GEOMETRIES]:
                     yield from _iter(geometry)
             elif type_ == FEATURE:
-                yield root[GEOMETRY]
+                geometry = node[GEOMETRY]
+                if geometry[TYPE] == GEOMETRY_COLLECTION:
+                    yield from _iter(geometry)
+                else:
+                    yield geometry
             else:
-                yield root
+                yield node
 
         yield from _iter(self._root)
 
-    def filter(self, func: Callable[["GeoProxy"], bool]) -> None:
+    def filter(self, func: Callable[[GeoProxy], bool]) -> None:
         """Removes all mappings for which `func()` returns ``False``.
         The function only has to handle Point, LineString and Polygon entities,
         other entities like MultiPolygon are divided into separate entities
         also any collection.
 
         """
 
@@ -344,15 +386,15 @@
         coordinates.
 
         Args:
             func: transformation function as Callable[[Vec3], Vec3]
 
         """
 
-        def process(entity: dict):
+        def process(entity: GeoMapping):
             def transform(coords):
                 if isinstance(coords, Vec3):
                     return func(coords)
                 else:
                     return [transform(c) for c in coords]
 
             entity[COORDINATES] = transform(entity[COORDINATES])
@@ -362,15 +404,15 @@
 
     @classmethod
     def from_dxf_entities(
         cls,
         entity: Union[DXFGraphic, Iterable[DXFGraphic]],
         distance: float = MAX_FLATTENING_DISTANCE,
         force_line_string: bool = False,
-    ) -> "GeoProxy":
+    ) -> GeoProxy:
         """Constructor from a single DXF entity or an iterable of DXF entities.
 
         Args:
             entity: DXF entity or entities
             distance: maximum flattening distance for curve approximations
             force_line_string: by default this function returns Polygon objects for
                 closed geometries like CIRCLE, SOLID, closed POLYLINE and so on,
@@ -381,40 +423,47 @@
         if isinstance(entity, DXFGraphic):
             m = mapping(entity, distance, force_line_string)
         else:
             m = collection(entity, distance, force_line_string)
         return cls(m)
 
     def to_dxf_entities(
-        self, polygon: int = 1, dxfattribs = None
-    ) -> Iterable[DXFGraphic]:
+        self,
+        polygon=PolygonConversion.HATCH,
+        dxfattribs=None,
+        *,
+        post_process: Optional[PostProcessFunc] = None,
+    ) -> Iterator[DXFGraphic]:
         """Returns stored ``__geo_interface__`` mappings as DXF entities.
 
         The `polygon` argument determines the method to convert polygons,
         use 1 for :class:`~ezdxf.entities.Hatch` entity, 2 for
         :class:`~ezdxf.entities.LWPolyline` or 3 for both.
         Option 2 returns for the exterior path and each hole a separated
         :class:`LWPolyline` entity. The :class:`Hatch` entity supports holes,
-        but has no explicit border line.
+        but has no explicit borderline.
 
         Yields :class:`Hatch` always before :class:`LWPolyline` entities.
 
         :class:`~ezdxf.entities.MPolygon` support was added in v0.16.6, which is
-        like a :class:`~ezdxf.entities.Hatch` entity  with additional border
-        lines, but the MPOLYGON entity is not a core DXF entity and DXF viewers,
+        like a :class:`~ezdxf.entities.Hatch` entity  with additional borderlines,
+        but the MPOLYGON entity is not a core DXF entity and DXF viewers,
         applications and libraries my not support this entity. The DXF attribute
-        `color` defines the border line color and `fill_color` the color of the
+        `color` defines the borderline color and `fill_color` the color of the
         solid filling.
 
         The returned DXF entities can be added to a layout by the
         :meth:`Layout.add_entity` method.
 
         Args:
-            polygon: method to convert polygons (1-2-3-4)
+            polygon: see :class:`PolygonConversion`
             dxfattribs: dict with additional DXF attributes
+            post_process: post process function of type :class:`PostProcesFunc` that get the
+                created DXF entity and the geo mapping as input, see reference implementation
+                :func:`assign_layers`
 
         """
 
         def point(vertex: Sequence) -> Point:
             point = cast(Point, factory.new("POINT", dxfattribs=dxfattribs))
             point.dxf.location = vertex
             return point
@@ -422,32 +471,30 @@
         def lwpolyline(vertices: Sequence) -> LWPolyline:
             polyline = cast(
                 LWPolyline, factory.new("LWPOLYLINE", dxfattribs=dxfattribs)
             )
             polyline.append_points(vertices, format="xy")
             return polyline
 
-        def polygon_(exterior: list, holes: list) -> Iterable[DXFGraphic]:
-            if polygon & 4:  # MPOLYGON
+        def polygon_(exterior: list, holes: list) -> Iterator[DXFGraphic]:
+            if polygon == PolygonConversion.MPOLYGON:
                 yield mpolygon_(exterior, holes)
                 # the following DXF entities do not support the
                 # "fill_color" attribute
                 return
-            if polygon & 1:  # HATCH
+            if polygon & PolygonConversion.HATCH:
                 yield hatch_(exterior, holes)
-            if polygon & 2:  # LWPOLYLINE
+            if polygon & PolygonConversion.POLYLINE:
                 for path in [exterior] + holes:
                     yield lwpolyline(path)
 
         def dxf_polygon_(
             dxftype: str, exterior: Sequence, holes: Sequence
         ) -> DXFPolygon:
-            dxf_polygon = cast(
-                DXFPolygon, factory.new(dxftype, dxfattribs=dxfattribs)
-            )
+            dxf_polygon = cast(DXFPolygon, factory.new(dxftype, dxfattribs=dxfattribs))
             dxf_polygon.dxf.hatch_style = const.HATCH_STYLE_OUTERMOST
             dxf_polygon.paths.add_polyline_path(
                 exterior, flags=const.BOUNDARY_PATH_EXTERNAL
             )
             for hole in holes:
                 dxf_polygon.paths.add_polyline_path(
                     hole, flags=const.BOUNDARY_PATH_OUTERMOST
@@ -456,15 +503,15 @@
 
         def hatch_(exterior: Sequence, holes: Sequence) -> DXFPolygon:
             return dxf_polygon_("HATCH", exterior, holes)
 
         def mpolygon_(exterior: Sequence, holes: Sequence) -> DXFPolygon:
             return dxf_polygon_("MPOLYGON", exterior, holes)
 
-        def entity(type_, coordinates) -> Iterable[DXFGraphic]:
+        def entity(type_, coordinates) -> Iterator[DXFGraphic]:
             if type_ == POINT:
                 yield point(coordinates)
             elif type_ == LINE_STRING:
                 yield lwpolyline(coordinates)
             elif type_ == POLYGON:
                 exterior, holes = coordinates
                 yield from polygon_(exterior, holes)
@@ -479,19 +526,56 @@
                     exterior, holes = data
                     yield from polygon_(exterior, holes)
 
         if polygon < 1 or polygon > 4:
             raise ValueError(f"invalid value for polygon: {polygon}")
 
         dxfattribs = dict(dxfattribs or {})
-        for _mapping in self.__iter__():
-            yield from entity(_mapping.get(TYPE), _mapping.get(COORDINATES))
+        for feature, geometry in iter_features(self._root):
+            type_ = geometry.get(TYPE)
+            for e in entity(type_, geometry.get(COORDINATES)):
+                if post_process:
+                    post_process(e, feature)
+                yield e
+
 
+def iter_features(geo_mapping: GeoMapping) -> Iterator[tuple[GeoMapping, GeoMapping]]:
+    """Yields all geometries of a ``__geo_mapping__`` as (`feature`, `geometry`) tuples.
 
-def parse(geo_mapping: dict) -> dict:
+    If no feature is defined the `feature` value is an empty ``dict``. When a `feature`
+    contains `GeometryCollections`, the function yields for each sub-geometry a separate
+    (`feature`, `geometry`) tuple.
+
+    """
+    current_feature: GeoMapping = {}
+
+    def features(node: GeoMapping) -> Iterator[tuple[GeoMapping, GeoMapping]]:
+        nonlocal current_feature
+
+        type_ = node[TYPE]
+        if type_ == FEATURE_COLLECTION:
+            for feature in node[FEATURES]:
+                yield from features(feature)
+        elif type_ == GEOMETRY_COLLECTION:
+            for geometry in node[GEOMETRIES]:
+                yield from features(geometry)
+        elif type_ == FEATURE:
+            current_feature = node
+            geometry = node[GEOMETRY]
+            if geometry[TYPE] == GEOMETRY_COLLECTION:
+                yield from features(geometry)
+            else:
+                yield current_feature, geometry
+        else:
+            yield current_feature, node
+
+    yield from features(geo_mapping)
+
+
+def parse(geo_mapping: GeoMapping) -> GeoMapping:
     """Parse ``__geo_interface__`` convert all coordinates into
     :class:`Vec3` objects, Polygon['coordinates'] is always a
     tuple (exterior, holes), holes maybe an empty list.
 
     """
     geo_mapping = copy.deepcopy(geo_mapping)
     type_ = geo_mapping.get(TYPE)
@@ -507,17 +591,15 @@
             raise ValueError(f'Missing key "{FEATURES}" in FeatureCollection.')
     elif type_ == GEOMETRY_COLLECTION:
         # It is possible for this array to be empty.
         geometries = geo_mapping.get(GEOMETRIES)
         if geometries:
             geo_mapping[GEOMETRIES] = [parse(g) for g in geometries]
         else:
-            raise ValueError(
-                f'Missing key "{GEOMETRIES}" in GeometryCollection.'
-            )
+            raise ValueError(f'Missing key "{GEOMETRIES}" in GeometryCollection.')
     elif type_ == FEATURE:
         # The value of the geometry member SHALL be either a Geometry object
         # or, in the case that the Feature is unlocated, a JSON null value.
         if GEOMETRY in geo_mapping:
             geometry = geo_mapping.get(GEOMETRY)
             geo_mapping[GEOMETRY] = parse(geometry) if geometry else None
         else:
@@ -571,15 +653,15 @@
         holes: Sequence = []
     else:
         exterior = coordinates[0]
         holes = coordinates[1:]
     return Vec3.list(exterior), [Vec3.list(h) for h in holes]
 
 
-def _rebuild(geo_mapping: dict, places: int = 6) -> dict:
+def _rebuild(geo_mapping: GeoMapping, places: int = 6) -> GeoMapping:
     """Returns ``__geo_interface__`` compatible mapping as :class:`dict` from
     compiled internal representation.
 
     """
 
     def pnt(v: Vec3) -> tuple[float, float]:
         return round(v.x, places), round(v.y, places)
@@ -590,17 +672,15 @@
         return [[pnt(v) for v in ring] for ring in [exterior] + holes]
 
     geo_interface = dict(geo_mapping)
     type_ = geo_interface[TYPE]
     if type_ == FEATURE_COLLECTION:
         geo_interface[FEATURES] = [_rebuild(f) for f in geo_interface[FEATURES]]
     elif type_ == GEOMETRY_COLLECTION:
-        geo_interface[GEOMETRIES] = [
-            _rebuild(g) for g in geo_interface[GEOMETRIES]
-        ]
+        geo_interface[GEOMETRIES] = [_rebuild(g) for g in geo_interface[GEOMETRIES]]
     elif type_ == FEATURE:
         geo_interface[GEOMETRY] = _rebuild(geo_interface[GEOMETRY])
     elif type_ == POINT:
         v = geo_interface[COORDINATES]
         geo_interface[COORDINATES] = pnt(v)
     elif type_ in (LINE_STRING, MULTI_POINT):
         coordinates = geo_interface[COORDINATES]
@@ -609,25 +689,24 @@
         coordinates = []
         for line in geo_interface[COORDINATES]:
             coordinates.append([pnt(v) for v in line])
     elif type_ == POLYGON:
         geo_interface[COORDINATES] = _polygon(*geo_interface[COORDINATES])
     elif type_ == MULTI_POLYGON:
         geo_interface[COORDINATES] = [
-            _polygon(exterior, holes)
-            for exterior, holes in geo_interface[COORDINATES]
+            _polygon(exterior, holes) for exterior, holes in geo_interface[COORDINATES]
         ]
     return geo_interface
 
 
 def mapping(
     entity: DXFGraphic,
     distance: float = MAX_FLATTENING_DISTANCE,
     force_line_string: bool = False,
-) -> dict:
+) -> GeoMapping:
     """Create the compiled ``__geo_interface__`` mapping as :class:`dict`
     for the given DXF `entity`, all coordinates are :class:`Vec3` objects and
     represents "Polygon" always as tuple (exterior, holes) even without holes.
 
 
     Internal API - result is **not** a valid ``_geo_interface__`` mapping!
 
@@ -669,32 +748,30 @@
         )
     elif isinstance(entity, DXFPolygon):
         return _hatch_as_polygon(entity, distance, force_line_string)
     else:
         raise TypeError(dxftype)
 
 
-def _line_string_or_polygon_mapping(
-    points: list[Vec3], force_line_string: bool
-):
+def _line_string_or_polygon_mapping(points: list[Vec3], force_line_string: bool):
     len_ = len(points)
     if len_ < 2:
         raise ValueError("Invalid vertex count.")
     if len_ == 2 or force_line_string:
         return line_string_mapping(points)
     else:
         if is_linear_ring(points):
             return polygon_mapping(points, [])
         else:
             return line_string_mapping(points)
 
 
 def _hatch_as_polygon(
     hatch: DXFPolygon, distance: float, force_line_string: bool
-) -> dict:
+) -> GeoMapping:
     def boundary_to_vertices(boundary) -> list[Vec3]:
         path = from_hatch_boundary_path(boundary, ocs, elevation)
         return path_to_vertices(path)
 
     def path_to_vertices(path) -> list[Vec3]:
         path.close()
         return list(path.flattening(distance))
@@ -717,57 +794,50 @@
     if count == 1 or hatch_style == const.HATCH_STYLE_IGNORE:
         points = boundary_to_vertices(exterior)
         return _line_string_or_polygon_mapping(points, force_line_string)
     else:
         if force_line_string:
             # Build a MultiString collection:
             points = boundary_to_vertices(exterior)
-            geometries = [
-                _line_string_or_polygon_mapping(points, force_line_string)
-            ]
+            geometries = [_line_string_or_polygon_mapping(points, force_line_string)]
             # All other boundary paths are treated as holes
             for hole in boundaries[1:]:
                 points = boundary_to_vertices(hole)
                 geometries.append(
                     _line_string_or_polygon_mapping(points, force_line_string)
                 )
             return join_multi_single_type_mappings(geometries)
         else:
             # Multiple separated polygons are possible in one HATCH entity:
             polygons = []
-            for exterior, holes in _boundaries_to_polygons(
-                boundaries, ocs, elevation
-            ):
+            for exterior, holes in _boundaries_to_polygons(boundaries, ocs, elevation):
                 points = path_to_vertices(exterior)
                 polygons.append(
-                    polygon_mapping(
-                        points, [path_to_vertices(hole) for hole in holes]
-                    )
+                    polygon_mapping(points, [path_to_vertices(hole) for hole in holes])
                 )
             if len(polygons) > 1:
                 return join_multi_single_type_mappings(polygons)
             return polygons[0]
 
 
 def _boundaries_to_polygons(boundaries, ocs, elevation):
     paths = (
-        from_hatch_boundary_path(boundary, ocs, elevation)
-        for boundary in boundaries
+        from_hatch_boundary_path(boundary, ocs, elevation) for boundary in boundaries
     )
-    for polygon in fast_bbox_detection(paths):
+    for polygon in make_polygon_structure(paths):
         exterior = polygon[0]
         # only take exterior path of level 1 holes, nested holes are ignored
         yield exterior, [hole[0] for hole in polygon[1:]]
 
 
 def collection(
     entities: Iterable[DXFGraphic],
     distance: float = MAX_FLATTENING_DISTANCE,
     force_line_string: bool = False,
-) -> dict:
+) -> GeoMapping:
     """Create the ``__geo_interface__`` mapping as :class:`dict` for the
     given DXF `entities`, see https://gist.github.com/sgillies/2217756
 
     Returns a "MultiPoint", "MultiLineString" or "MultiPolygon" collection if
     all entities return the same GeoJSON type ("Point", "LineString", "Polygon")
     else a "GeometryCollection".
 
@@ -785,15 +855,15 @@
     types = set(g[TYPE] for g in m)
     if len(types) > 1:
         return geometry_collection_mapping(m)
     else:
         return join_multi_single_type_mappings(m)
 
 
-def line_string_mapping(points: list[Vec3]) -> dict:
+def line_string_mapping(points: list[Vec3]) -> GeoMapping:
     """Returns a "LineString" mapping.
 
     .. code::
 
         {
             "type": "LineString",
             "coordinates": [
@@ -830,15 +900,15 @@
     else:
         if not ccw:
             points.reverse()
 
     return points
 
 
-def polygon_mapping(points: list[Vec3], holes: list[list[Vec3]]) -> dict:
+def polygon_mapping(points: list[Vec3], holes: list[list[Vec3]]) -> GeoMapping:
     """Returns a "Polygon" mapping.
 
     .. code::
 
         {
             "type": "Polygon",
             "coordinates": [
@@ -868,15 +938,15 @@
         rings = exterior, []
     return {
         TYPE: POLYGON,
         COORDINATES: rings,
     }
 
 
-def join_multi_single_type_mappings(geometries: Iterable[dict]) -> dict:
+def join_multi_single_type_mappings(geometries: Iterable[GeoMapping]) -> GeoMapping:
     """Returns multiple geometries as a "MultiPoint", "MultiLineString" or
     "MultiPolygon" mapping.
     """
     types = set()
     data = list()
     for g in geometries:
         types.add(g[TYPE])
@@ -886,28 +956,28 @@
         raise TypeError(f"Type mismatch: {str(types)}")
     elif len(types) == 0:
         return dict()
     else:
         return {TYPE: "Multi" + tuple(types)[0], COORDINATES: data}
 
 
-def geometry_collection_mapping(geometries: Iterable[dict]) -> dict:
+def geometry_collection_mapping(geometries: Iterable[GeoMapping]) -> GeoMapping:
     """Returns multiple geometries as a "GeometryCollection" mapping."""
     return {TYPE: GEOMETRY_COLLECTION, GEOMETRIES: list(geometries)}
 
 
 # Values stored in GeoData RSS tag are not precise enough to match
 # control calculation at epsg.io:
 # Semi Major Axis: 6.37814e+06
 # Semi Minor Axis: 6.35675e+06
 
 WGS84_SEMI_MAJOR_AXIS = 6378137
 WGS84_SEMI_MINOR_AXIS = 6356752.3142
 WGS84_ELLIPSOID_ECCENTRIC = math.sqrt(
-    1.0 - WGS84_SEMI_MINOR_AXIS ** 2 / WGS84_SEMI_MAJOR_AXIS ** 2
+    1.0 - WGS84_SEMI_MINOR_AXIS**2 / WGS84_SEMI_MAJOR_AXIS**2
 )
 CONST_E2 = math.e / 2.0
 CONST_PI_2 = math.pi / 2.0
 CONST_PI_4 = math.pi / 4.0
 
 
 def wgs84_4326_to_3395(location: Vec3) -> Vec3:
@@ -980,7 +1050,23 @@
 
 
 def dd2dms(dd: float) -> tuple[float, float, float]:
     """Convert decimal degrees into degree, minutes, seconds."""
     m, s = divmod(dd * 3600, 60)
     d, m = divmod(m, 60)
     return d, m, s
+
+
+def assign_layers(entity: DXFGraphic, mapping: GeoMapping) -> None:
+    """Reference implementation for a :func:`post_process` function.
+
+    .. seealso::
+
+        :func:`dxf_entities`
+
+    """
+    properties = mapping.get(PROPERTIES)
+    if properties is None:
+        return
+    layer = properties.get("layer")
+    if layer:
+        entity.dxf.layer = layer
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/importer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/meshex.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/mtxpl.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/odafc.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/openscad.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/pycsg.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/r12export.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/r12writer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/text2path.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/text2path.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 def get_font(font: fonts.FontFace) -> fonts.AbstractFont:
     font_name = fonts.font_manager.find_font_name(font)
     return fonts.make_font(font_name, cap_height=1.0)
 
 
 def _str_to_path(s: str, render_engine: fonts.AbstractFont, size: float = 1.0) -> Path:
-    return render_engine.text_path_ex(s, cap_height=size).to_3d_path()
+    return render_engine.text_path_ex(s, cap_height=size).to_path()
 
 
 def alignment_transformation(
     fm: fonts.FontMeasurements,
     bbox: BoundingBox,
     align: TextEntityAlignment,
     length: float,
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/xplayer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/xplayer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 """xplayer = cross backend player."""
 from __future__ import annotations
 from typing import Callable
-from ezdxf import path
 from ezdxf.math import Vec2
 from ezdxf.colors import RGB
 
-from ezdxf.addons.drawing.backend import BackendInterface
+from ezdxf.addons.drawing.backend import BackendInterface, BkPath2d
 from ezdxf.addons.drawing.properties import BackendProperties
 from ezdxf.addons.hpgl2 import api as hpgl2
 from ezdxf.addons.hpgl2.backend import (
     Properties as HPGL2Properties,
     RecordType as HPGL2RecordType,
 )
 
@@ -33,46 +32,34 @@
             points: list[Vec2] = record_data.vertices()
             size = len(points)
             if size == 1:
                 backend.draw_point(points[0], backend_properties)
             elif size == 2:
                 backend.draw_line(points[0], points[1], backend_properties)
             else:
-                backend.draw_path(_from_2d_points(points), backend_properties)
+                backend.draw_path(BkPath2d.from_vertices(points), backend_properties)
         elif record_type == HPGL2RecordType.FILLED_PATHS:
-            # filled paths are stored as single paths! see: PolygonBuffer.get_paths()
-            external_paths, holes = path.winding_deconstruction(
-                path.fast_bbox_detection(p.to_path2d() for p in record_data)
-            )
-            backend.draw_filled_paths(external_paths, holes, backend_properties)  # type: ignore
+            backend.draw_filled_paths(record_data, backend_properties)  # type: ignore
         elif record_type == HPGL2RecordType.OUTLINE_PATHS:
             for p in record_data:
-                backend.draw_path(p.to_path2d(), backend_properties)
+                backend.draw_path(p, backend_properties)
     backend.finalize()
 
 
 def _make_drawing_backend_properties(properties: HPGL2Properties) -> BackendProperties:
     """Make BackendProperties() for the drawing add-on."""
     return BackendProperties(
         color=properties.pen_color.to_hex(),
         lineweight=properties.pen_width,
         layer="0",
         pen=properties.pen_index,
         handle="",
     )
 
 
-def _from_2d_points(points: list[Vec2]) -> path.Path2d:
-    """Returns points as 2D path."""
-    path2d = path.Path2d(points[0])
-    for point in points[1:]:
-        path2d.line_to(point)
-    return path2d
-
-
 def map_color(color: str) -> Callable[[BackendProperties], BackendProperties]:
     def _map_color(properties: BackendProperties) -> BackendProperties:
         return BackendProperties(
             color=color,
             lineweight=properties.lineweight,
             layer=properties.layer,
             pen=properties.pen,
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/xqt.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/browser/data.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/browser/model.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/browser/model.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/browser/views.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/clipper.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/clipper.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,104 +1,116 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Optional, Iterable, Iterator, Sequence
 
-from ezdxf.math import AnyVec, Matrix44, Vec2, BoundingBox2d
+from ezdxf.math import Matrix44, Vec2, BoundingBox2d
 from ezdxf.math.clipping import ClippingRect2d
-from ezdxf.path import Path, Path2d, bbox, from_vertices, single_paths
+from ezdxf.npshapes import NumpyPath2d, NumpyPoints2d, single_paths
+from ezdxf.protocols import SupportsBoundingBox
 
 __all__ = ["ClippingRect"]
 
 
 class ClippingRect:
     def __init__(self) -> None:
         self._stack: list[tuple[Optional[ClippingRect2d], Optional[Matrix44]]] = []
         self.view: Optional[ClippingRect2d] = None
         self.m: Optional[Matrix44] = None
 
     @property
     def is_active(self) -> bool:
         return self.view is not None
 
-    def push(self, path: Path | Path2d, m: Optional[Matrix44]) -> None:
+    def push(self, path: SupportsBoundingBox, m: Optional[Matrix44]) -> None:
         if self.view is not None:
             self._stack.append((self.view, self.m))
-        box = BoundingBox2d(path.control_vertices())
+        box = path.bbox()
         self.view = ClippingRect2d(box.extmin, box.extmax)
         self.m = m
 
     def pop(self) -> None:
         if self._stack:
             self.view, self.m = self._stack.pop()
         else:
             self.view = None
             self.m = None
 
-    def clip_point(self, point: AnyVec) -> Optional[AnyVec]:
+    def clip_point(self, point: Vec2) -> Optional[Vec2]:
+        # Expected points outside the view to be removed!
         if self.m is not None:
             point = self.m.transform(point)
         if self.view is not None and not self.view.is_inside(Vec2(point)):
             return None
         return point
 
-    def clip_line(self, start: AnyVec, end: AnyVec) -> Sequence[AnyVec]:
+    def clip_line(self, start: Vec2, end: Vec2) -> Sequence[Vec2]:
+        # Expected lines outside the view to be removed!
         # An arbitrary clipping polygon could return more than 1 line segment
         m = self.m
         if m is not None:
             start, end = m.fast_2d_transform((start, end))
         if self.view is not None:
             return self.view.clip_line(start, end)
         return start, end
 
     def clip_filled_paths(
-        self, paths: Iterable[Path | Path2d], max_sagitta: float
-    ) -> Iterator[Path | Path2d]:
+        self, paths: Iterable[NumpyPath2d], max_sagitta: float
+    ) -> Iterator[NumpyPath2d]:
+        # Expected overall paths outside the view to be removed!
+        view = self.view
+        assert view is not None
         m = self.m
         for path in paths:
             if m is not None:
-                path = path.transform(m)
+                path.transform_inplace(m)
             # path in paperspace units!
-            box = BoundingBox2d(path.control_vertices())
-            view = self.view
-            assert view is not None
+            box = path.bbox()
+            if not view.has_intersection(box):
+                # path is complete outside the view
+                continue
             if view.is_inside(box.extmin) and view.is_inside(box.extmax):
-                # no clipping needed
+                # path is complete inside the view, no clipping required
                 yield path
-            else:  # clipping is required, but only clipping of polygons is supported
-                yield from_vertices(
-                    view.clip_polygon(
-                        Vec2.list(path.flattening(max_sagitta, segments=16))
-                    ),
-                    close=True,
-                )
+            else:
+                # clipping is required, but only clipping of polygons is supported
+                if path.has_sub_paths:
+                    yield from self.clip_filled_paths(path.sub_paths(), max_sagitta)
+                else:
+                    yield NumpyPath2d.from_vertices(
+                        view.clip_polygon(
+                            Vec2.list(path.flattening(max_sagitta, segments=4))
+                        ),
+                        close=True,
+                    )
 
     def clip_paths(
-        self, paths: Iterable[Path | Path2d], max_sagitta: float
-    ) -> Iterator[Path | Path2d]:
+        self, paths: Iterable[NumpyPath2d], max_sagitta: float
+    ) -> Iterator[NumpyPath2d]:
+        # Expected paths outside the view to be removed!
         view = self.view
         assert view is not None
         m = self.m
 
         for path in paths:
             if m is not None:
-                path = path.transform(m)
+                path.transform_inplace(m)
             # path in paperspace units!
             box = BoundingBox2d(path.control_vertices())
             if view.is_inside(box.extmin) and view.is_inside(box.extmax):
                 yield path
-            for sub_path in single_paths([path]):  # type: ignore
-                polyline = Vec2.list(sub_path.flattening(max_sagitta, segments=16))
+            for sub_path in path.sub_paths():
+                polyline = Vec2.list(sub_path.flattening(max_sagitta, segments=4))
                 for part in view.clip_polyline(polyline):
-                    yield from_vertices(part, close=False)
+                    yield NumpyPath2d.from_vertices(part, close=False)
 
-    def clip_polygon(self, points: Iterable[AnyVec]) -> Sequence[Vec2]:
+    def clip_polygon(self, points: NumpyPoints2d) -> NumpyPoints2d:
+        # Expected polygons outside the view to be removed!
         if self.m is not None:
-            points = self.m.fast_2d_transform(points)
+            points.transform_inplace(self.m)
             # points in paperspace units!
-        points = list(points)
         view = self.view
         if view is not None:
-            box = BoundingBox2d(points)
-            if not view.is_inside(box.extmin) or not view.is_inside(box.extmax):
-                return view.clip_polygon(points)
+            extmin, extmax = points.extents()
+            if not view.is_inside(extmin) or not view.is_inside(extmax):
+                return NumpyPoints2d(view.clip_polygon(points.vertices()))
         return points
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/config.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,46 @@
-#  Copyright (c) 2021-2022, Manfred Moitzi
+#  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Iterable
-from ezdxf.math import AnyVec
-from ezdxf.path import Path, Path2d
+from ezdxf.math import Vec2
 from .properties import BackendProperties
-from .backend import Backend
+from .backend import Backend, BkPath2d, BkPoints2d
 from .config import Configuration
 
 
 class BasicBackend(Backend):
     """The basic backend has no draw_path() support and approximates all curves
     by lines.
     """
 
     def __init__(self):
         super().__init__()
         self.collector = []
         self.configure(Configuration())
 
-    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
+    def draw_point(self, pos: Vec2, properties: BackendProperties) -> None:
         self.collector.append(("point", pos, properties))
 
-    def draw_line(
-        self, start: AnyVec, end: AnyVec, properties: BackendProperties
-    ) -> None:
+    def draw_line(self, start: Vec2, end: Vec2, properties: BackendProperties) -> None:
         self.collector.append(("line", start, end, properties))
 
     def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: BackendProperties
+        self, points: BkPoints2d, properties: BackendProperties
     ) -> None:
-        self.collector.append(("filled_polygon", list(points), properties))
+        self.collector.append(("filled_polygon", points, properties))
 
     def set_background(self, color: str) -> None:
         self.collector.append(("bgcolor", color))
 
     def clear(self) -> None:
         self.collector = []
 
 
 class PathBackend(BasicBackend):
-    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
+    def draw_path(self, path: BkPath2d, properties: BackendProperties) -> None:
         self.collector.append(("path", path, properties))
 
     def draw_filled_paths(
-        self,
-        paths: Iterable[Path | Path2d],
-        holes: Iterable[Path | Path2d],
-        properties: BackendProperties,
+        self, paths: Iterable[BkPath2d], properties: BackendProperties
     ) -> None:
-        self.collector.append(("filled_path", (tuple(paths), tuple(holes)), properties))
+        self.collector.append(("filled_path", tuple(paths), properties))
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_utils.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/debug_utils.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/dxf.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/dxf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Iterable, TYPE_CHECKING, no_type_check
 from functools import lru_cache
-import itertools
 import enum
 
 
 from ezdxf import colors
 from ezdxf.lldxf.const import VALID_DXF_LINEWEIGHTS
-from ezdxf.math import AnyVec, BoundingBox2d
-from ezdxf.path import Path, Path2d, to_splines_and_polylines, to_hatches
+from ezdxf.math import Vec2, BoundingBox2d
+from ezdxf.path import to_splines_and_polylines, to_hatches
 from ezdxf.layouts import BaseLayout
 
 from .type_hints import Color
-from .backend import BackendInterface
+from .backend import BackendInterface, BkPath2d, BkPoints2d
 from .config import Configuration
 from .properties import BackendProperties
 
 if TYPE_CHECKING:
     from ezdxf.document import Drawing
     from ezdxf.entities import Solid
 
@@ -27,14 +26,15 @@
     """This enum is used to define the color output mode of the :class:`DXFBackend`.
 
     Attributes:
         ACI: the color is set as :ref:`ACI` and assigned by layer
         RGB: the color is set as RGB true color value
 
     """
+
     # Use color index as primary color
     ACI = enum.auto()
 
     # Use always the RGB value
     RGB = enum.auto()
 
 
@@ -119,56 +119,52 @@
         rgb: colors.RGB | None = None
         aci = BYLAYER
         if self.color_mode == ColorMode.RGB:
             rgb = properties.rgb
             aci = properties.pen
         hatch.set_solid_fill(color=aci, style=0, rgb=rgb)
 
-    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
+    def draw_point(self, pos: Vec2, properties: BackendProperties) -> None:
         self.layout.add_point(pos, dxfattribs=self.resolve_properties(properties))
 
-    def draw_line(
-        self, start: AnyVec, end: AnyVec, properties: BackendProperties
-    ) -> None:
+    def draw_line(self, start: Vec2, end: Vec2, properties: BackendProperties) -> None:
         self.layout.add_line(start, end, dxfattribs=self.resolve_properties(properties))
 
     def draw_solid_lines(
-        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: BackendProperties
+        self, lines: Iterable[tuple[Vec2, Vec2]], properties: BackendProperties
     ) -> None:
         lines = list(lines)
         if len(lines) == 0:
             return
         attribs = self.resolve_properties(properties)
         for start, end in lines:
             self.layout.add_line(start, end, dxfattribs=attribs)
 
-    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
+    def draw_path(self, path: BkPath2d, properties: BackendProperties) -> None:
         attribs = self.resolve_properties(properties)
         if path.has_curves:
             for entity in to_splines_and_polylines(path, dxfattribs=attribs):  # type: ignore
                 self.layout.add_entity(entity)
         else:
             self.layout.add_lwpolyline(path.control_vertices(), dxfattribs=attribs)
 
     def draw_filled_paths(
-        self,
-        paths: Iterable[Path | Path2d],
-        holes: Iterable[Path | Path2d],
-        properties: BackendProperties,
+        self, paths: Iterable[BkPath2d], properties: BackendProperties
     ) -> None:
         attribs = self.resolve_properties(properties)
-        for hatch in to_hatches(itertools.chain(paths, holes), dxfattribs=attribs):
+        py_paths = [p.to_path() for p in paths]
+        for hatch in to_hatches(py_paths, dxfattribs=attribs):
             self.layout.add_entity(hatch)
             self.set_solid_fill(hatch, properties)
 
     def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: BackendProperties
+        self, points: BkPoints2d, properties: BackendProperties
     ) -> None:
         hatch = self.layout.add_hatch(dxfattribs=self.resolve_properties(properties))
-        hatch.paths.add_polyline_path(points, is_closed=True)
+        hatch.paths.add_polyline_path(points.vertices(), is_closed=True)
         self.set_solid_fill(hatch, properties)
 
     def configure(self, config: Configuration) -> None:
         pass
 
     def clear(self) -> None:
         pass
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/frontend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,44 @@
 # Copyright (c) 2020-2023, Matthew Broadway
 # License: MIT License
 from __future__ import annotations
 import math
 from typing import (
     Iterable,
-    Iterator,
     cast,
     Union,
-    Sequence,
     Dict,
     Callable,
-    Tuple,
     Optional,
+    TYPE_CHECKING,
 )
 from typing_extensions import TypeAlias
 import logging
 import itertools
 import time
 
 import ezdxf.bbox
-from ezdxf.colors import RGB
 from ezdxf.addons.drawing.config import (
     Configuration,
     ProxyGraphicPolicy,
     HatchPolicy,
 )
 from ezdxf.addons.drawing.backend import BackendInterface
-from ezdxf.addons.drawing.clipper import ClippingRect
 from ezdxf.addons.drawing.properties import (
     RenderContext,
     OLE2FRAME_COLOR,
     Properties,
     Filling,
     LayoutProperties,
-    BackendProperties,
-)
-from ezdxf.addons.drawing.config import (
-    LinePolicy,
-    BackgroundPolicy,
-    ColorPolicy,
-    TextPolicy,
 )
+from ezdxf.addons.drawing.config import BackgroundPolicy, TextPolicy
 from ezdxf.addons.drawing.text import simplified_text_chunks
 from ezdxf.addons.drawing.type_hints import FilterFunc
 from ezdxf.addons.drawing.gfxproxy import DXFGraphicProxy
 from ezdxf.addons.drawing.mtext_complex import complex_mtext_renderer
-from ezdxf.addons.drawing.unified_text_renderer import UnifiedTextRenderer
 from ezdxf.entities import (
     DXFEntity,
     DXFGraphic,
     Insert,
     MText,
     Polyline,
     LWPolyline,
@@ -62,117 +51,110 @@
     Point,
     Viewport,
 )
 from ezdxf.entities.attrib import BaseAttrib
 from ezdxf.entities.polygon import DXFPolygon
 from ezdxf.entities.boundary_paths import AbstractBoundaryPath
 from ezdxf.layouts import Layout
-from ezdxf.math import Vec2, Vec3, OCS, NULLVEC, Matrix44, AnyVec, BoundingBox2d
+from ezdxf.math import Vec2, Vec3, OCS, NULLVEC
 from ezdxf.path import (
     Path,
-    Path2d,
     make_path,
     from_hatch_boundary_path,
-    fast_bbox_detection,
+    make_polygon_structure,
     winding_deconstruction,
     from_vertices,
-    single_paths,
 )
-from ezdxf.render import MeshBuilder, TraceBuilder, linetypes
+from ezdxf.render import MeshBuilder, TraceBuilder
 from ezdxf import reorder
 from ezdxf.proxygraphic import ProxyGraphic, ProxyGraphicError
 from ezdxf.protocols import SupportsVirtualEntities, virtual_entities
-from ezdxf.tools.text import (
-    has_inline_formatting_codes,
-    replace_non_printable_characters,
-)
+from ezdxf.tools.text import has_inline_formatting_codes
 from ezdxf.lldxf import const
 from ezdxf.render import hatching
 from ezdxf.fonts import fonts
 from .type_hints import Color
 
+if TYPE_CHECKING:
+    from .designer import Designer
 
-__all__ = ["Frontend"]
+__all__ = ["Frontend", "UniversalFrontend"]
 
 
 TDispatchTable: TypeAlias = Dict[str, Callable[[DXFGraphic, Properties], None]]
-PatternKey: TypeAlias = Tuple[str, float]
-
 POST_ISSUE_MSG = (
     "Please post sample DXF file at https://github.com/mozman/ezdxf/issues."
 )
 logger = logging.getLogger("ezdxf")
 
 
-class Frontend:
+class UniversalFrontend:
     """Drawing frontend, responsible for decomposing entities into graphic
-    primitives and resolving entity properties.
+    primitives and resolving entity properties. Supports 2D and 3D backends.
 
     By passing the bounding box cache of the modelspace entities can speed up
     paperspace rendering, because the frontend can filter entities which are not
     visible in the VIEWPORT. Even passing in an empty cache can speed up
     rendering time when multiple viewports need to be processed.
 
     Args:
         ctx: the properties relevant to rendering derived from a DXF document
-        out: the backend to draw to
+        designer: connection between frontend and backend
         config: settings to configure the drawing frontend and backend
         bbox_cache: bounding box cache of the modelspace entities or an empty
             cache which will be filled dynamically when rendering multiple
             viewports or ``None`` to disable bounding box caching at all
 
     """
 
     def __init__(
         self,
         ctx: RenderContext,
-        out: BackendInterface,
+        designer: Designer,
         config: Configuration = Configuration(),
         bbox_cache: Optional[ezdxf.bbox.Cache] = None,
     ):
         # RenderContext contains all information to resolve resources for a
         # specific DXF document.
         self.ctx = ctx
-        self.out = out
+        # the designer is the connection between frontend and backend
+        self.designer = designer
+        designer.set_draw_entities_callback(self.draw_entities_callback)
         self.config = ctx.update_configuration(config)
+        designer.set_config(self.config)
 
         if self.config.pdsize is None or self.config.pdsize <= 0:
             self.log_message("relative point size is not supported")
             self.config = self.config.with_changes(pdsize=1)
 
-        self.out.configure(self.config)
-
         # Parents entities of current entity/sub-entity
         self.parent_stack: list[DXFGraphic] = []
 
         self._dispatch = self._build_dispatch_table()
 
         # Supported DXF entities which use only proxy graphic for rendering:
         self._proxy_graphic_only_entities: set[str] = {
             "MLEADER",  # todo: remove if MLeader.virtual_entities() is implemented
             "MULTILEADER",
             "ACAD_PROXY_ENTITY",
         }
-        # connection link between frontend and backend, the frontend should not
-        # call the draw_...() methods of the backend directly:
-        self._designer = Designer(self, out)
 
         # Optional bounding box cache, which maybe was created by detecting the
         # modelspace extends. This cache is used when rendering VIEWPORT
         # entities in paperspace to detect if an entity is even visible,
         # this can speed up rendering time if multiple viewports are present.
         # If the bbox_cache is not ``None``, entities not in cache will be
         # added dynamically. This is only beneficial when rendering multiple
         # viewports, as the upfront bounding box calculation adds some rendering
         # time.
         self._bbox_cache = bbox_cache
 
     @property
     def text_engine(self):
-        return self._designer.text_engine
+        return self.designer.text_engine
 
     def _build_dispatch_table(self) -> TDispatchTable:
         dispatch_table: TDispatchTable = {
             "POINT": self.draw_point_entity,
             "HATCH": self.draw_hatch_entity,
             "MPOLYGON": self.draw_mpolygon_entity,
             "MESH": self.draw_mesh_entity,
@@ -255,15 +237,15 @@
             )
         else:
             self.draw_entities(
                 layout,
                 filter_func=filter_func,
             )
         if finalize:
-            self.out.finalize()
+            self.designer.finalize()
 
     def set_background(self, color: Color) -> None:
         policy = self.config.background_policy
         override = True
         if policy == BackgroundPolicy.DEFAULT:
             override = False
         elif policy == BackgroundPolicy.OFF:
@@ -272,40 +254,45 @@
             color = "#000000"
         elif policy == BackgroundPolicy.WHITE:
             color = "#ffffff"
         elif policy == BackgroundPolicy.CUSTOM:
             color = self.config.custom_bg_color
         if override:
             self.ctx.current_layout_properties.set_colors(color)
-        self.out.set_background(color)
+        self.designer.set_background(color)
 
     def draw_entities(
         self,
         entities: Iterable[DXFGraphic],
         *,
         filter_func: Optional[FilterFunc] = None,
     ) -> None:
         """Draw the given `entities`. The method skips invisible entities
         and entities for which the given filter function returns ``False``.
 
         """
         _draw_entities(self, self.ctx, entities, filter_func=filter_func)
 
+    def draw_entities_callback(
+        self, ctx: RenderContext, entities: Iterable[DXFGraphic]
+    ) -> None:
+        _draw_entities(self, ctx, entities)
+
     def draw_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         """Draw a single DXF entity.
 
         Args:
             entity: DXF entity inherited from DXFGraphic()
             properties: resolved entity properties
 
         """
-        self.out.enter_entity(entity, properties)
+        self.designer.enter_entity(entity, properties)
         if not entity.is_virtual:
             # top level entity
-            self._designer.set_current_entity_handle(entity.dxf.handle)
+            self.designer.set_current_entity_handle(entity.dxf.handle)
         if (
             entity.proxy_graphic
             and self.config.proxy_graphic_policy == ProxyGraphicPolicy.PREFER
         ):
             self.draw_proxy_graphic(entity.proxy_graphic, entity.doc)
         else:
             draw_method = self._dispatch.get(entity.dxftype(), None)
@@ -328,30 +315,30 @@
                     self.config.proxy_graphic_policy != ProxyGraphicPolicy.IGNORE
                     or entity.dxftype() not in self._proxy_graphic_only_entities
                 ):
                     self.draw_composite_entity(entity, properties)
             else:
                 self.skip_entity(entity, "unsupported")
 
-        self.out.exit_entity(entity)
+        self.designer.exit_entity(entity)
 
     def draw_line_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         d, dxftype = entity.dxf, entity.dxftype()
         if dxftype == "LINE":
-            self._designer.draw_line(d.start, d.end, properties)
+            self.designer.draw_line(d.start, d.end, properties)
 
         elif dxftype in ("XLINE", "RAY"):
             start = d.start
             delta = d.unit_vector * self.config.infinite_line_length
             if dxftype == "XLINE":
-                self._designer.draw_line(
+                self.designer.draw_line(
                     start - delta / 2, start + delta / 2, properties
                 )
             elif dxftype == "RAY":
-                self._designer.draw_line(start, start + delta, properties)
+                self.designer.draw_line(start, start + delta, properties)
         else:
             raise TypeError(dxftype)
 
     def draw_text_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         if self.config.text_policy == TextPolicy.IGNORE:
             return
         # Draw embedded MTEXT entity as virtual MTEXT entity:
@@ -361,23 +348,23 @@
             self.draw_text_entity_3d(entity, properties)
         else:
             self.draw_text_entity_2d(entity, properties)
 
     def get_font_face(self, properties: Properties) -> fonts.FontFace:
         font_face = properties.font
         if font_face is None:
-            return self._designer.default_font_face
+            return self.designer.default_font_face
         return font_face
 
     def draw_text_entity_2d(self, entity: DXFGraphic, properties: Properties) -> None:
         if isinstance(entity, Text):
             for line, transform, cap_height in simplified_text_chunks(
                 entity, self.text_engine, font_face=self.get_font_face(properties)
             ):
-                self._designer.draw_text(
+                self.designer.draw_text(
                     line, transform, properties, cap_height, entity.dxftype()
                 )
         else:
             raise TypeError(entity.dxftype())
 
     def draw_text_entity_3d(self, entity: DXFGraphic, properties: Properties) -> None:
         self.skip_entity(entity, "3D text not supported")
@@ -395,28 +382,28 @@
             self.draw_simple_mtext(mtext, properties)
 
     def draw_simple_mtext(self, mtext: MText, properties: Properties) -> None:
         """Draw the content of a MTEXT entity without inline formatting codes."""
         for line, transform, cap_height in simplified_text_chunks(
             mtext, self.text_engine, font_face=self.get_font_face(properties)
         ):
-            self._designer.draw_text(
+            self.designer.draw_text(
                 line, transform, properties, cap_height, mtext.dxftype()
             )
 
     def draw_complex_mtext(self, mtext: MText, properties: Properties) -> None:
         """Draw the content of a MTEXT entity including inline formatting codes."""
-        complex_mtext_renderer(self.ctx, self._designer, mtext, properties)
+        complex_mtext_renderer(self.ctx, self.designer, mtext, properties)
 
     def draw_curve_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         try:
             path = make_path(entity)
         except AttributeError:  # API usage error
             raise TypeError(f"Unsupported DXF type {entity.dxftype()}")
-        self._designer.draw_path(path, properties)
+        self.designer.draw_path(path, properties)
 
     def draw_point_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         point = cast(Point, entity)
         pdmode = self.config.pdmode
         pdsize = self.config.pdsize
         assert pdmode is not None
         assert pdsize is not None
@@ -425,25 +412,25 @@
         if properties.layer.lower() == "defpoints":
             if not self.config.show_defpoints:
                 return
             else:  # Render defpoints as dimensionless points:
                 pdmode = 0
 
         if pdmode == 0:
-            self._designer.draw_point(entity.dxf.location, properties)
+            self.designer.draw_point(entity.dxf.location, properties)
         else:
             for entity in point.virtual_entities(pdsize, pdmode):
                 dxftype = entity.dxftype()
                 if dxftype == "LINE":
-                    start = Vec3(entity.dxf.start)
+                    start = entity.dxf.start
                     end = entity.dxf.end
                     if start.isclose(end):
-                        self._designer.draw_point(start, properties)
+                        self.designer.draw_point(start, properties)
                     else:  # direct draw by backend is OK!
-                        self._designer.draw_line(start, end, properties)
+                        self.designer.draw_line(start, end, properties)
                     pass
                 elif dxftype == "CIRCLE":
                     self.draw_curve_entity(entity, properties)
                 else:
                     raise ValueError(dxftype)
 
     def draw_solid_entity(self, entity: DXFGraphic, properties: Properties) -> None:
@@ -458,27 +445,26 @@
             except AttributeError:
                 # all 4 vertices are required, otherwise the entity is invalid
                 # for AutoCAD
                 self.skip_entity(entity, "missing required vertex attribute")
                 return
             edge_visibility = entity.get_edges_visibility()
             if all(edge_visibility):
-                self._designer.draw_path(from_vertices(points), properties)
+                self.designer.draw_path(from_vertices(points), properties)
             else:
                 for a, b, visible in zip(points, points[1:], edge_visibility):
                     if visible:
-                        self._designer.draw_line(a, b, properties)
+                        self.designer.draw_line(a, b, properties)
 
         elif isinstance(entity, Solid):
             # set solid fill type for SOLID and TRACE
             properties.filling = Filling()
-            self._designer.draw_filled_polygon(
+            self.designer.draw_filled_polygon(
                 entity.wcs_vertices(close=False), properties
             )
-
         else:
             raise TypeError("API error, requires a SOLID, TRACE or 3DFACE entity")
 
     def draw_hatch_pattern(
         self, polygon: DXFPolygon, paths: list[Path], properties: Properties
     ):
         if polygon.pattern is None or len(polygon.pattern.lines) == 0:
@@ -504,15 +490,15 @@
                 line_pattern = baseline.pattern_renderer(line.distance)
                 for s, e in line_pattern.render(line.start, line.end):
                     if ocs.transform:
                         s, e = ocs.to_wcs((s.x, s.y, elevation)), ocs.to_wcs(
                             (e.x, e.y, elevation)
                         )
                     lines.append((s, e))
-        self._designer.draw_solid_lines(lines, properties)
+        self.designer.draw_solid_lines(lines, properties)
 
     def draw_hatch_entity(
         self,
         entity: DXFGraphic,
         properties: Properties,
         *,
         loops: Optional[list[Path]] = None,
@@ -540,42 +526,28 @@
             return
 
         # draw SOLID filling
         ocs = polygon.ocs()
         # all OCS coordinates have the same z-axis stored as vector (0, 0, z),
         # default (0, 0, 0)
         elevation = entity.dxf.elevation.z
-
-        external_paths: list[Path]
-        holes: list[Path]
-
+        paths: list[Path]
         if loops is not None:  # only MPOLYGON
-            external_paths, holes = winding_deconstruction(  # type: ignore
-                fast_bbox_detection(loops)
-            )
+            paths = loops
         else:  # only HATCH
-            paths = polygon.paths.rendering_paths(polygon.dxf.hatch_style)
-            polygons: list = fast_bbox_detection(
-                closed_loops(paths, ocs, elevation)  # type: ignore
+            boundary_paths = list(
+                polygon.paths.rendering_paths(polygon.dxf.hatch_style)
             )
-            external_paths, holes = winding_deconstruction(polygons)  # type: ignore
-
+            paths = closed_loops(boundary_paths, ocs, elevation)
         if show_only_outline:
-            for p in itertools.chain(ignore_text_boxes(external_paths), holes):
-                self._designer.draw_path(p, properties)
+            for p in ignore_text_boxes(paths):
+                self.designer.draw_path(p, properties)
             return
-
-        if external_paths:
-            self._designer.draw_filled_paths(
-                ignore_text_boxes(external_paths), holes, properties
-            )
-        elif holes:
-            # The first path is considered the exterior path, everything else are
-            # holes.
-            self._designer.draw_filled_paths([holes[0]], holes[1:], properties)
+        if paths:
+            self.designer.draw_filled_paths(ignore_text_boxes(paths), properties)
 
     def draw_mpolygon_entity(self, entity: DXFGraphic, properties: Properties):
         def resolve_fill_color() -> str:
             return self.ctx.resolve_aci_color(entity.dxf.fill_color, properties.layer)
 
         polygon = cast(DXFPolygon, entity)
         ocs = polygon.ocs()
@@ -602,33 +574,33 @@
             # line color is also pattern color: properties.color
             self.draw_hatch_entity(entity, properties, loops=loops)
 
         # 2. draw boundary paths
         properties.color = line_color
         # draw boundary paths as lines
         for loop in loops:
-            self._designer.draw_path(loop, properties)
+            self.designer.draw_path(loop, properties)
 
     def draw_wipeout_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         wipeout = cast(Wipeout, entity)
         properties.filling = Filling()
         properties.color = self.ctx.current_layout_properties.background_color
-        path = wipeout.boundary_path_wcs()
-        self._designer.draw_filled_polygon(path, properties)
+        clipping_polygon = wipeout.boundary_path_wcs()
+        self.designer.draw_filled_polygon(clipping_polygon, properties)
 
     def draw_viewport(self, vp: Viewport) -> None:
         # the "active" viewport and invisible viewports should be filtered at this
         # stage, see function _draw_viewports()
         if vp.dxf.status < 1:
             return
 
         if not vp.is_top_view:
             self.log_message("Cannot render non top-view viewports")
             return
-        self._designer.draw_viewport(vp, self.ctx, self._bbox_cache)
+        self.designer.draw_viewport(vp, self.ctx, self._bbox_cache)
 
     def draw_ole2frame_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         ole2frame = cast(OLE2Frame, entity)
         bbox = ole2frame.bbox()
         if not bbox.is_empty:
             self._draw_filled_rect(bbox.rect_vertices(), OLE2FRAME_COLOR)
 
@@ -637,25 +609,25 @@
         points: Iterable[Vec2],
         color: str,
     ) -> None:
         props = Properties()
         props.color = color
         # default SOLID filling
         props.filling = Filling()
-        self._designer.draw_filled_polygon(Vec3.list(points), props)
+        self.designer.draw_filled_polygon(points, props)
 
     def draw_mesh_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         builder = MeshBuilder.from_mesh(entity)  # type: ignore
         self.draw_mesh_builder_entity(builder, properties)
 
     def draw_mesh_builder_entity(
         self, builder: MeshBuilder, properties: Properties
     ) -> None:
         for face in builder.faces_as_vertices():
-            self._designer.draw_path(
+            self.designer.draw_path(
                 from_vertices(face, close=True), properties=properties
             )
 
     def draw_polyline_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         dxftype = entity.dxftype()
         if dxftype == "POLYLINE":
             e = cast(Polyface, entity)
@@ -685,22 +657,21 @@
             )
             for polygon in trace.polygons():  # polygon is a sequence of Vec2()
                 if transform:
                     points = ocs.points_to_wcs(
                         Vec3(v.x, v.y, elevation) for v in polygon
                     )
                 else:
-                    points = Vec3.generate(polygon)
+                    points = polygon
                 # Set default SOLID filling for LWPOLYLINE
                 properties.filling = Filling()
-                self._designer.draw_filled_polygon(points, properties)
+                self.designer.draw_filled_polygon(points, properties)
             return
 
-        path = make_path(entity)
-        self._designer.draw_path(path, properties)
+        self.designer.draw_path(make_path(entity), properties)
 
     def draw_composite_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         def draw_insert(insert: Insert):
             self.draw_entities(insert.attribs)
             # draw_entities() includes the visibility check:
             self.draw_entities(
                 insert.virtual_entities(
@@ -732,14 +703,45 @@
             try:
                 self.draw_entities(virtual_entities(ProxyGraphic(data, doc)))
             except ProxyGraphicError as e:
                 print(str(e))
                 print(POST_ISSUE_MSG)
 
 
+class Frontend(UniversalFrontend):
+    """Drawing frontend for 2D backends, responsible for decomposing entities into
+    graphic primitives and resolving entity properties.
+
+    By passing the bounding box cache of the modelspace entities can speed up
+    paperspace rendering, because the frontend can filter entities which are not
+    visible in the VIEWPORT. Even passing in an empty cache can speed up
+    rendering time when multiple viewports need to be processed.
+
+    Args:
+        ctx: the properties relevant to rendering derived from a DXF document
+        out: the 2D backend to draw to
+        config: settings to configure the drawing frontend and backend
+        bbox_cache: bounding box cache of the modelspace entities or an empty
+            cache which will be filled dynamically when rendering multiple
+            viewports or ``None`` to disable bounding box caching at all
+
+    """
+
+    def __init__(
+        self,
+        ctx: RenderContext,
+        out: BackendInterface,
+        config: Configuration = Configuration(),
+        bbox_cache: Optional[ezdxf.bbox.Cache] = None,
+    ):
+        from .designer import Designer2d
+
+        super().__init__(ctx, Designer2d(out), config, bbox_cache)
+
+
 def is_spatial_text(extrusion: Vec3) -> bool:
     # note: the magnitude of the extrusion vector has no effect on text scale
     return not math.isclose(extrusion.x, 0) or not math.isclose(extrusion.y, 0)
 
 
 def closed_loops(
     paths: list[AbstractBoundaryPath],
@@ -769,317 +771,16 @@
             isinstance(path.user_data, const.BoundaryPathState)
             and path.user_data.textbox
         ):
             continue  # skip text box paths
         yield path
 
 
-class Designer:
-    """The designer is placed between the frontend and the backend
-    and adds this features:
-
-        - automatically linetype rendering
-        - VIEWPORT rendering
-        - foreground color mapping according Frontend.config.color_policy
-
-    """
-
-    def __init__(self, frontend: Frontend, backend: BackendInterface):
-        self.frontend = frontend
-        self.backend = backend
-        self.config = frontend.config
-        self.pattern_cache: dict[PatternKey, Sequence[float]] = dict()
-        self.text_engine = UnifiedTextRenderer()
-        self.default_font_face = fonts.FontFace()
-        self.clipper = ClippingRect()
-        self.current_vp_scale = 1.0
-        self._current_entity_handle: str = ""
-        self._color_mapping: dict[str, str] = dict()
-
-    @property
-    def vp_ltype_scale(self) -> float:
-        """The linetype pattern should look the same in all viewports
-        regardless of the viewport scale.
-        """
-        return 1.0 / max(self.current_vp_scale, 0.0001)  # max out at 1:10000
-
-    def get_backend_properties(self, properties: Properties) -> BackendProperties:
-        try:
-            color = self._color_mapping[properties.color]
-        except KeyError:
-            color = apply_color_policy(
-                properties.color, self.config.color_policy, self.config.custom_fg_color
-            )
-            self._color_mapping[properties.color] = color
-        return BackendProperties(
-            color,
-            properties.lineweight,
-            properties.layer,
-            properties.pen,
-            self._current_entity_handle,
-        )
-
-    def set_current_entity_handle(self, handle: str) -> None:
-        assert handle is not None
-        self._current_entity_handle = handle
-
-    def draw_viewport(
-        self,
-        vp: Viewport,
-        layout_ctx: RenderContext,
-        bbox_cache: Optional[ezdxf.bbox.Cache] = None,
-    ) -> None:
-        """Draw the content of the given viewport current viewport."""
-        if vp.doc is None:
-            return
-        try:
-            msp_limits = vp.get_modelspace_limits()
-        except ValueError:  # modelspace limits not detectable
-            return
-        if self.enter_viewport(vp):
-            _draw_entities(
-                self.frontend,
-                layout_ctx.from_viewport(vp),
-                filter_vp_entities(vp.doc.modelspace(), msp_limits, bbox_cache),
-            )
-            self.exit_viewport()
-
-    def enter_viewport(self, vp: Viewport) -> bool:
-        """Set current viewport, returns ``True`` for valid viewports."""
-        self.current_vp_scale = vp.get_scale()
-        m = vp.get_transformation_matrix()
-        clipping_path = make_path(vp)
-        if len(clipping_path):
-            self.clipper.push(clipping_path, m)
-            return True
-        return False
-
-    def exit_viewport(self):
-        self.clipper.pop()
-        self.current_vp_scale = 1.0
-
-    def draw_point(self, pos: AnyVec, properties: Properties) -> None:
-        if self.clipper.is_active:
-            point = self.clipper.clip_point(pos)
-            if point is None:
-                return
-            pos = point
-        self.backend.draw_point(pos, self.get_backend_properties(properties))
-
-    def draw_line(self, start: AnyVec, end: AnyVec, properties: Properties):
-        if (
-            self.config.line_policy == LinePolicy.SOLID
-            or len(properties.linetype_pattern) < 2  # CONTINUOUS
-        ):
-            if self.clipper.is_active:
-                points = self.clipper.clip_line(start, end)
-                if len(points) != 2:
-                    return
-                start, end = points
-            self.backend.draw_line(start, end, self.get_backend_properties(properties))
-        else:
-            renderer = linetypes.LineTypeRenderer(self.pattern(properties))
-            self.draw_solid_lines(  # includes transformation
-                ((s, e) for s, e in renderer.line_segment(start, end)),
-                properties,
-            )
-
-    def draw_solid_lines(
-        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: Properties
-    ) -> None:
-        if self.clipper.is_active:
-            clipped_lines: list[Sequence[AnyVec]] = []
-            for start, end in lines:
-                points = self.clipper.clip_line(start, end)
-                if points:
-                    clipped_lines.append(points)
-            lines = clipped_lines  # type: ignore
-        self.backend.draw_solid_lines(lines, self.get_backend_properties(properties))
-
-    def draw_path(self, path: Path | Path2d, properties: Properties):
-        if (
-            self.config.line_policy == LinePolicy.SOLID
-            or len(properties.linetype_pattern) < 2  # CONTINUOUS
-        ):
-            if self.clipper.is_active:
-                for clipped_path in self.clipper.clip_paths(
-                    [path], self.config.max_flattening_distance
-                ):
-                    self.backend.draw_path(
-                        clipped_path, self.get_backend_properties(properties)
-                    )
-                return
-            self.backend.draw_path(path, self.get_backend_properties(properties))
-        else:
-            renderer = linetypes.LineTypeRenderer(self.pattern(properties))
-            vertices = path.flattening(self.config.max_flattening_distance, segments=16)
-            self.draw_solid_lines(
-                ((s, e) for s, e in renderer.line_segments(vertices)),
-                properties,
-            )
-
-    def draw_filled_paths(
-        self,
-        paths: Iterable[Path | Path2d],
-        holes: Iterable[Path | Path2d],
-        properties: Properties,
-    ) -> None:
-        if self.clipper.is_active:
-            max_sagitta = self.config.max_flattening_distance
-            paths = self.clipper.clip_filled_paths(paths, max_sagitta)
-            holes = self.clipper.clip_filled_paths(holes, max_sagitta)
-        self.backend.draw_filled_paths(
-            paths, holes, self.get_backend_properties(properties)
-        )
-
-    def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: Properties
-    ) -> None:
-        if self.clipper.is_active:
-            points = self.clipper.clip_polygon(points)
-        self.backend.draw_filled_polygon(
-            points, self.get_backend_properties(properties)
-        )
-
-    def pattern(self, properties: Properties) -> Sequence[float]:
-        """Get pattern - implements pattern caching."""
-        if self.config.line_policy == LinePolicy.SOLID:
-            scale = 0.0
-        else:
-            scale = properties.linetype_scale * self.vp_ltype_scale
-
-        key: PatternKey = (properties.linetype_name, scale)
-        pattern_ = self.pattern_cache.get(key)
-        if pattern_ is None:
-            pattern_ = self.create_pattern(properties, scale)
-            self.pattern_cache[key] = pattern_
-        return pattern_
-
-    def create_pattern(self, properties: Properties, scale: float) -> Sequence[float]:
-        """Returns simplified linetype tuple: on-off sequence"""
-        if len(properties.linetype_pattern) < 2:
-            # Do not return None -> None indicates: "not cached"
-            return tuple()
-        else:
-            min_dash_length = self.config.min_dash_length * self.vp_ltype_scale
-            pattern = [
-                max(e * scale, min_dash_length) for e in properties.linetype_pattern
-            ]
-            if len(pattern) % 2:
-                pattern.pop()
-            return pattern
-
-    def draw_text(
-        self,
-        text: str,
-        transform: Matrix44,
-        properties: Properties,
-        cap_height: float,
-        dxftype: str = "TEXT",
-    ) -> None:
-        text_policy = self.config.text_policy
-        if not text.strip() or text_policy == TextPolicy.IGNORE:
-            return  # no point rendering empty strings
-        text = prepare_string_for_rendering(text, dxftype)
-        font_face = properties.font
-        if font_face is None:
-            font_face = self.default_font_face
-        try:
-            text_path = self.text_engine.get_text_path(text, font_face, cap_height)
-        except (RuntimeError, ValueError):
-            return
-
-        transformed_path = text_path.transform(transform)
-        if text_policy == TextPolicy.REPLACE_RECT:
-            bbox = BoundingBox2d(transformed_path.control_vertices())
-            self.draw_path(from_vertices(bbox.rect_vertices(), close=True), properties)
-            return
-        if text_policy == TextPolicy.REPLACE_FILL:
-            bbox = BoundingBox2d(transformed_path.control_vertices())
-            if properties.filling is None:
-                properties.filling = Filling()
-            self.draw_filled_polygon(bbox.rect_vertices(), properties)
-            return
-        if (
-            self.text_engine.is_stroke_font(font_face)
-            or text_policy == TextPolicy.OUTLINE
-        ):
-            self.draw_path(transformed_path, properties)
-            return
-
-        polygons = fast_bbox_detection(single_paths([transformed_path]))  # type: ignore
-        external_paths, holes = winding_deconstruction(polygons)  # type: ignore
-        if properties.filling is None:
-            properties.filling = Filling()
-        self.draw_filled_paths(external_paths, holes, properties)  # type: ignore
-
-
-def filter_vp_entities(
-    msp: Layout,
-    limits: Sequence[float],
-    bbox_cache: Optional[ezdxf.bbox.Cache] = None,
-) -> Iterator[DXFGraphic]:
-    """Yields all DXF entities that need to be processed by the given viewport
-    `limits`. The entities may be partially of even complete outside the viewport.
-    By passing the bounding box cache of the modelspace entities,
-    the function can filter entities outside the viewport to speed up rendering
-    time.
-
-    There are two processing modes for the `bbox_cache`:
-
-        1. The `bbox_cache` is``None``: all entities must be processed,
-           pass through mode
-        2. If the `bbox_cache` is given but does not contain an entity,
-           the bounding box is computed and added to the cache.
-           Even passing in an empty cache can speed up rendering time when
-           multiple viewports need to be processed.
-
-    Args:
-        msp: modelspace layout
-        limits: modelspace limits of the viewport, as tuple (min_x, min_y, max_x, max_y)
-        bbox_cache: the bounding box cache of the modelspace entities
-
-    """
-
-    # WARNING: this works only with top-view viewports
-    # The current state of the drawing add-on supports only top-view viewports!
-    def is_visible(e):
-        entity_bbox = bbox_cache.get(e)
-        if entity_bbox is None:
-            # compute and add bounding box
-            entity_bbox = ezdxf.bbox.extents((e,), fast=True, cache=bbox_cache)
-        if not entity_bbox.has_data:
-            return True
-        # Check for separating axis:
-        if min_x >= entity_bbox.extmax.x:
-            return False
-        if max_x <= entity_bbox.extmin.x:
-            return False
-        if min_y >= entity_bbox.extmax.y:
-            return False
-        if max_y <= entity_bbox.extmin.y:
-            return False
-        return True
-
-    if bbox_cache is None:  # pass through all entities
-        yield from msp
-        return
-
-    min_x, min_y, max_x, max_y = limits
-    if not bbox_cache.has_data:
-        # fill cache at once
-        ezdxf.bbox.extents(msp, fast=True, cache=bbox_cache)
-
-    for entity in msp:
-        if is_visible(entity):
-            yield entity
-
-
 def _draw_entities(
-    frontend: Frontend,
+    frontend: UniversalFrontend,
     ctx: RenderContext,
     entities: Iterable[DXFGraphic],
     *,
     filter_func: Optional[FilterFunc] = None,
 ) -> None:
     if filter_func is not None:
         entities = filter(filter_func, entities)
@@ -1099,15 +800,15 @@
         if properties.is_visible:
             frontend.draw_entity(entity, properties)
         else:
             frontend.skip_entity(entity, "invisible")
     _draw_viewports(frontend, viewports)
 
 
-def _draw_viewports(frontend: Frontend, viewports: list[Viewport]) -> None:
+def _draw_viewports(frontend: UniversalFrontend, viewports: list[Viewport]) -> None:
     # The VIEWPORT attributes "id" and "status" are very unreliable, maybe because of
     # the "great" documentation by Autodesk.
     # Viewport status field: (according to the DXF Reference)
     # -1 = On, but is fully off-screen, or is one of the viewports that is not
     #      active because the $MAXACTVP count is currently being exceeded.
     #  0 = Off
     # <positive value> = On and active. The value indicates the order of
@@ -1125,68 +826,7 @@
     # is not reliable at all - but what else is there to do?  The "active" layout should
     # have the id "1", but this information is also not reliable.
     if viewports[0].dxf.get("status", 1) == 1:
         viewports.pop(0)
     # Draw viewports in order of "status"
     for viewport in viewports:
         frontend.draw_viewport(viewport)
-
-
-def prepare_string_for_rendering(text: str, dxftype: str) -> str:
-    assert "\n" not in text, "not a single line of text"
-    if dxftype in {"TEXT", "ATTRIB", "ATTDEF"}:
-        text = replace_non_printable_characters(text, replacement="?")
-        text = text.replace("\t", "?")
-    elif dxftype == "MTEXT":
-        text = replace_non_printable_characters(text, replacement="▯")
-        text = text.replace("\t", "        ")
-    else:
-        raise TypeError(dxftype)
-    return text
-
-
-def invert_color(color: Color) -> Color:
-    r, g, b = RGB.from_hex(color)
-    return RGB(255 - r, 255 - g, 255 - b).to_hex()
-
-
-def swap_bw(color: str) -> Color:
-    color = color.lower()
-    if color == "#000000":
-        return "#ffffff"
-    if color == "#ffffff":
-        return "#000000"
-    return color
-
-
-def color_to_monochrome(color: Color, scale: float = 1.0, offset: float = 0.0) -> Color:
-    lum = RGB.from_hex(color).luminance * scale + offset
-    if lum < 0.0:
-        lum = 0.0
-    elif lum > 1.0:
-        lum = 1.0
-    gray = round(lum * 255)
-    return RGB(gray, gray, gray).to_hex()
-
-
-def apply_color_policy(color: Color, policy: ColorPolicy, custom_color: Color) -> Color:
-    alpha = color[7:9]
-    color = color[:7]
-    if policy == ColorPolicy.COLOR_SWAP_BW:
-        color = swap_bw(color)
-    elif policy == ColorPolicy.COLOR_NEGATIVE:
-        color = invert_color(color)
-    elif policy == ColorPolicy.MONOCHROME_DARK_BG:  # [0.3, 1.0]
-        color = color_to_monochrome(color, scale=0.7, offset=0.3)
-    elif policy == ColorPolicy.MONOCHROME_LIGHT_BG:  # [0.0, 0.7]
-        color = color_to_monochrome(color, scale=0.7, offset=0.0)
-    elif policy == ColorPolicy.MONOCHROME:  # [0.0, 1.0]
-        color = color_to_monochrome(color)
-    elif policy == ColorPolicy.BLACK:
-        color = "#000000"
-    elif policy == ColorPolicy.WHITE:
-        color = "#ffffff"
-    elif policy == ColorPolicy.CUSTOM:
-        fg = custom_color
-        color = fg[:7]
-        alpha = fg[7:9]
-    return color + alpha
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/hpgl2.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/hpgl2.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Iterable, Sequence, no_type_check
-
 import copy
-import itertools
 
 from ezdxf import colors
-from ezdxf.math import AnyVec
-from ezdxf.path import Path, Path2d, Command
+from ezdxf.math import Vec2
+from ezdxf.path import Command
 
 from .type_hints import Color
-from .backend import BackendInterface
+from .backend import BackendInterface, BkPath2d, BkPoints2d
 from .config import Configuration, LineweightPolicy
 from .properties import BackendProperties
 from . import layout, recorder
 
 
 __all__ = ["PlotterBackend"]
 
@@ -25,14 +23,20 @@
 FLATTEN_MAX = 10  # plot units
 MM_TO_PLU = 40  # 40 plu = 1mm
 DEFAULT_PEN = 0
 WHITE = colors.RGB(255, 255, 255)
 BLACK = colors.RGB(0, 0, 0)
 MAX_FLATTEN = 10
 
+# comparing Command.<attrib> to ints is very slow
+CMD_MOVE_TO = int(Command.MOVE_TO)
+CMD_LINE_TO = int(Command.LINE_TO)
+CMD_CURVE3_TO = int(Command.CURVE3_TO)
+CMD_CURVE4_TO = int(Command.CURVE4_TO)
+
 
 class PlotterBackend(recorder.Recorder):
     """The :class:`PlotterBackend` creates HPGL/2 plot files for output on raster
     plotters. This backend does not need any additional packages.
     The plot files are tested by the plot file viewer `ViewCompanion Standard`_
     but not on real hardware - please use with care and give feedback.
 
@@ -250,15 +254,15 @@
 
     def set_pen_width(self, width: float) -> None:
         if self.current_pen_width == width:
             return
         self.data.append(f"PW{width:g};".encode())  # pen width in mm
         self.current_pen_width = width
 
-    def enter_polygon_mode(self, start_point: AnyVec) -> None:
+    def enter_polygon_mode(self, start_point: Vec2) -> None:
         x = round(start_point.x, self.decimal_places)
         y = round(start_point.y, self.decimal_places)
         self.data.append(f"PA;PU{x},{y};PM;".encode())
 
     def close_current_polygon(self) -> None:
         self.data.append(b"PM1;")
 
@@ -270,20 +274,20 @@
         pen_color, opacity = self.resolve_pen_color(properties.color)
         pen_width = self.resolve_pen_width(properties.lineweight)
         pen_number = self.switch_current_pen(pen_number, pen_color)
         self.set_pen(pen_number)
         self.set_pen_width(pen_width)
 
     def add_polyline_encoded(
-        self, vertices: Iterable[AnyVec], properties: BackendProperties
+        self, vertices: Iterable[Vec2], properties: BackendProperties
     ):
         self.set_properties(properties)
         self.data.append(polyline_encoder(vertices, self.factional_bits, self.base))
 
-    def add_path(self, path: Path | Path2d, properties: BackendProperties):
+    def add_path(self, path: BkPath2d, properties: BackendProperties):
         if self.curves and path.has_curves:
             self.set_properties(properties)
             self.data.append(path_encoder(path, self.decimal_places))
         else:
             points = list(path.flattening(MAX_FLATTEN, segments=4))
             self.add_polyline_encoded(points, properties)
 
@@ -317,62 +321,57 @@
         self._stroke_width_cache[width] = stroke_width
         return stroke_width
 
     def set_background(self, color: Color) -> None:
         # background is always a white paper
         pass
 
-    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
+    def draw_point(self, pos: Vec2, properties: BackendProperties) -> None:
         self.add_polyline_encoded([pos], properties)
 
-    def draw_line(
-        self, start: AnyVec, end: AnyVec, properties: BackendProperties
-    ) -> None:
+    def draw_line(self, start: Vec2, end: Vec2, properties: BackendProperties) -> None:
         self.add_polyline_encoded([start, end], properties)
 
     def draw_solid_lines(
-        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: BackendProperties
+        self, lines: Iterable[tuple[Vec2, Vec2]], properties: BackendProperties
     ) -> None:
         lines = list(lines)
         if len(lines) == 0:
             return
         for line in lines:
             self.add_polyline_encoded(line, properties)
 
-    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
+    def draw_path(self, path: BkPath2d, properties: BackendProperties) -> None:
         for sub_path in path.sub_paths():
             if len(sub_path) == 0:
                 continue
             self.add_path(sub_path, properties)
 
     def draw_filled_paths(
-        self,
-        paths: Iterable[Path | Path2d],
-        holes: Iterable[Path | Path2d],
-        properties: BackendProperties,
+        self, paths: Iterable[BkPath2d], properties: BackendProperties
     ) -> None:
-        all_paths = list(itertools.chain(paths, holes))
-        if len(all_paths) == 0:
+        paths = list(paths)
+        if len(paths) == 0:
             return
-        self.enter_polygon_mode(all_paths[0].start)
-        for p in all_paths:
+        self.enter_polygon_mode(paths[0].start)
+        for p in paths:
             for sub_path in p.sub_paths():
                 if len(sub_path) == 0:
                     continue
                 self.add_path(sub_path, properties)
                 self.close_current_polygon()
         self.fill_polygon()
 
     def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: BackendProperties
+        self, points: BkPoints2d, properties: BackendProperties
     ) -> None:
-        points = list(points)
-        if points:
-            self.enter_polygon_mode(points[0])
-            self.add_polyline_encoded(points, properties)
+        points2d: list[Vec2] = points.vertices()
+        if points2d:
+            self.enter_polygon_mode(points2d[0])
+            self.add_polyline_encoded(points2d, properties)
             self.fill_polygon()
 
     def configure(self, config: Configuration) -> None:
         self.lineweight_policy = config.lineweight_policy
         if config.min_lineweight:
             # config.min_lineweight in 1/300 inch!
             min_lineweight_mm = config.min_lineweight * 25.4 / 300
@@ -411,15 +410,15 @@
     max_lineweight=2.11,  # defined by DXF
 ) -> float:
     lineweight = max(min(lineweight, max_lineweight), min_lineweight) - min_lineweight
     factor = (max_stroke_width - min_stroke_width) / (max_lineweight - min_lineweight)
     return round(min_stroke_width + round(lineweight * factor), 2)
 
 
-def flatten_path(path: Path | Path2d) -> Sequence[AnyVec]:
+def flatten_path(path: BkPath2d) -> Sequence[Vec2]:
     points = list(path.flattening(distance=FLATTEN_MAX))
     return points
 
 
 def compile_hpgl2(header: Sequence[bytes], commands: Sequence[bytes]) -> bytes:
     output = bytearray(PRELUDE)
     output.extend(b"".join(header))
@@ -444,15 +443,15 @@
     if base == 64:
         chars.append(191 + x)
     else:
         chars.append(95 + x)
     return bytes(chars)
 
 
-def polyline_encoder(vertices: Iterable[AnyVec], frac_bits: int, base: int) -> bytes:
+def polyline_encoder(vertices: Iterable[Vec2], frac_bits: int, base: int) -> bytes:
     cmd = b"PE"
     if base == 32:
         cmd = b"PE7"
     if frac_bits:
         cmd += b">" + pe_encode(frac_bits, 0, base)
     data = [cmd + b"<="]
     vertices = list(vertices)
@@ -467,15 +466,15 @@
         data.append(pe_encode(delta.y, frac_bits, base))
         current = vertex
     data.append(b";")
     return b"".join(data)
 
 
 @no_type_check
-def path_encoder(path: Path2d, decimal_places: int | None) -> bytes:
+def path_encoder(path: BkPath2d, decimal_places: int | None) -> bytes:
     # first point as absolute coordinates
     current = path.start
     x = round(current.x, decimal_places)
     y = round(current.y, decimal_places)
     data = [f"PU;PA{x:g},{y:g};PD;".encode()]
     prev_command = Command.MOVE_TO
     if len(path):
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/layout.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 
 import matplotlib.pyplot as plt
 from matplotlib.collections import LineCollection
 from matplotlib.lines import Line2D
 from matplotlib.patches import PathPatch
 from matplotlib.path import Path
 
-import ezdxf.path
-from ezdxf.addons.drawing.backend import Backend
+from ezdxf.npshapes import to_matplotlib_path
+from ezdxf.addons.drawing.backend import Backend, BkPath2d, BkPoints2d
 from ezdxf.addons.drawing.properties import BackendProperties, LayoutProperties
 from ezdxf.addons.drawing.type_hints import FilterFunc
 from ezdxf.addons.drawing.type_hints import Color
-from ezdxf.math import Vec3, Matrix44, AnyVec
+from ezdxf.math import Vec2
 from ezdxf.layouts import Layout
-from .config import Configuration, HatchPolicy
+from .config import Configuration
 
 logger = logging.getLogger("ezdxf")
 # matplotlib docs: https://matplotlib.org/index.html
 
 # line style:
 # https://matplotlib.org/api/_as_gen/matplotlib.lines.Line2D.html#matplotlib.lines.Line2D.set_linestyle
 # https://matplotlib.org/gallery/lines_bars_and_markers/linestyles.html
@@ -79,15 +79,15 @@
         z = self._current_z
         self._current_z += 1
         return z
 
     def set_background(self, color: Color):
         self.ax.set_facecolor(color)
 
-    def draw_point(self, pos: AnyVec, properties: BackendProperties):
+    def draw_point(self, pos: Vec2, properties: BackendProperties):
         """Draw a real dimensionless point."""
         color = properties.color
         self.ax.scatter(
             [pos.x],
             [pos.y],
             s=SCATTER_POINT_SIZE,
             c=color,
@@ -98,15 +98,15 @@
         """Set lineweight_scaling=0 to use a constant minimal lineweight."""
         assert self.config.min_lineweight is not None
         return max(
             properties.lineweight * self.config.lineweight_scaling,
             self.config.min_lineweight,
         )
 
-    def draw_line(self, start: AnyVec, end: AnyVec, properties: BackendProperties):
+    def draw_line(self, start: Vec2, end: Vec2, properties: BackendProperties):
         """Draws a single solid line, line type rendering is done by the
         frontend since v0.18.1
         """
         if start.isclose(end):
             # matplotlib draws nothing for a zero-length line:
             self.draw_point(start, properties)
         else:
@@ -118,15 +118,15 @@
                     color=properties.color,
                     zorder=self._get_z(),
                 )
             )
 
     def draw_solid_lines(
         self,
-        lines: Iterable[tuple[AnyVec, AnyVec]],
+        lines: Iterable[tuple[Vec2, Vec2]],
         properties: BackendProperties,
     ):
         """Fast method to draw a bunch of solid lines with the same properties."""
         color = properties.color
         lineweight = self.get_lineweight(properties)
         _lines = []
         point_x = []
@@ -146,72 +146,53 @@
                 linewidths=lineweight,
                 color=color,
                 zorder=z,
                 capstyle="butt",
             )
         )
 
-    def draw_path(
-        self, path: ezdxf.path.Path | ezdxf.path.Path2d, properties: BackendProperties
-    ):
+    def draw_path(self, path: BkPath2d, properties: BackendProperties):
         """Draw a solid line path, line type rendering is done by the
         frontend since v0.18.1
         """
-        mpl_path = ezdxf.path.to_matplotlib_path([path])
+        mpl_path = to_matplotlib_path([path])
         try:
             patch = PathPatch(
                 mpl_path,
                 linewidth=self.get_lineweight(properties),
                 fill=False,
                 color=properties.color,
                 zorder=self._get_z(),
             )
         except ValueError as e:
             logger.info(f"ignored matplotlib error: {str(e)}")
         else:
             self.ax.add_patch(patch)
 
     def draw_filled_paths(
-        self,
-        paths: Iterable[ezdxf.path.Path | ezdxf.path.Path2d],
-        holes: Iterable[ezdxf.path.Path | ezdxf.path.Path2d],
-        properties: BackendProperties,
+        self, paths: Iterable[BkPath2d], properties: BackendProperties
     ):
         linewidth = 0
-        oriented_paths: list[ezdxf.path.Path | ezdxf.path.Path2d] = []
-        for path in paths:
-            try:
-                path = path.counter_clockwise()
-            except ValueError:  # cannot detect path orientation
-                continue
-            oriented_paths.append(path)
-
-        for hole in holes:
-            try:
-                hole = hole.clockwise()
-            except ValueError:  # cannot detect path orientation
-                continue
-            oriented_paths.append(hole)
 
         try:
             patch = PathPatch(
-                ezdxf.path.to_matplotlib_path(oriented_paths),
+                to_matplotlib_path(paths),
                 color=properties.color,
                 linewidth=linewidth,
                 fill=True,
                 zorder=self._get_z(),
             )
         except ValueError as e:
             logger.info(f"ignored matplotlib error in draw_filled_paths(): {str(e)}")
         else:
             self.ax.add_patch(patch)
 
-    def draw_filled_polygon(self, points: Iterable[AnyVec], properties: BackendProperties):
+    def draw_filled_polygon(self, points: BkPoints2d, properties: BackendProperties):
         self.ax.fill(
-            *zip(*((p.x, p.y) for p in points)),
+            *zip(*((p.x, p.y) for p in points.vertices())),
             color=properties.color,
             linewidth=0,
             zorder=self._get_z(),
         )
 
     def clear(self):
         self.ax.clear()
@@ -224,20 +205,14 @@
             miny, maxy = self.ax.get_ylim()
             data_width, data_height = maxx - minx, maxy - miny
             if not math.isclose(data_width, 0):
                 width, height = plt.figaspect(data_height / data_width)
                 self.ax.get_figure().set_size_inches(width, height, forward=True)
 
 
-def _transform_path(path: Path, transform: Matrix44) -> Path:
-    # raises ValueError for invalid TextPath objects
-    vertices = transform.transform_vertices([Vec3(x, y) for x, y in path.vertices])
-    return Path([(v.x, v.y) for v in vertices], path.codes)  # type: ignore
-
-
 def _get_aspect_ratio(ax: plt.Axes) -> float:
     minx, maxx = ax.get_xlim()
     miny, maxy = ax.get_ylim()
     data_width, data_height = maxx - minx, maxy - miny
     if abs(data_height) > 1e-9:
         return data_width / data_height
     return 1.0
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pymupdf.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pymupdf.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Iterable, no_type_check
 import copy
 
-from ezdxf.math import AnyVec, Vec2
+from ezdxf.math import Vec2
 from ezdxf.colors import RGB
-from ezdxf.path import Path, Path2d, Command
+from ezdxf.path import Command
 from ezdxf.version import __version__
 
 from .type_hints import Color
-from .backend import BackendInterface
+from .backend import BackendInterface, BkPath2d, BkPoints2d
 from .config import Configuration, LineweightPolicy
 from .properties import BackendProperties
 from . import layout, recorder
 
 is_pymupdf_installed = True
 try:
     import fitz
@@ -38,14 +38,15 @@
     Install package::
 
         pip install pymupdf
 
     .. _PyMuPdf: https://pypi.org/project/PyMuPDF/
 
     """
+
     def __init__(self) -> None:
         super().__init__()
         self._init_flip_y = True
 
     def _get_replay(
         self, page: layout.Page, settings: layout.Settings = layout.Settings()
     ) -> PyMuPdfRenderBackend:
@@ -264,64 +265,57 @@
             stroke_width = map_lineweight_to_stroke_width(
                 width, self.min_stroke_width, self.max_stroke_width
             )
         stroke_width = max(self.abs_min_stroke_width, stroke_width)
         self._stroke_width_cache[width] = stroke_width
         return stroke_width
 
-    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
+    def draw_point(self, pos: Vec2, properties: BackendProperties) -> None:
         shape = self.new_shape()
         pos = Vec2(pos)
         shape.drawLine(pos, pos)
         self.finish_line(shape, properties, close=False)
         shape.commit()
 
-    def draw_line(
-        self, start: AnyVec, end: AnyVec, properties: BackendProperties
-    ) -> None:
+    def draw_line(self, start: Vec2, end: Vec2, properties: BackendProperties) -> None:
         shape = self.new_shape()
         shape.drawLine(Vec2(start), Vec2(end))
         self.finish_line(shape, properties, close=False)
         shape.commit()
 
     def draw_solid_lines(
-        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: BackendProperties
+        self, lines: Iterable[tuple[Vec2, Vec2]], properties: BackendProperties
     ) -> None:
         shape = self.new_shape()
         for start, end in lines:
             shape.drawLine(start, end)
         self.finish_line(shape, properties, close=False)
         shape.commit()
 
-    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
+    def draw_path(self, path: BkPath2d, properties: BackendProperties) -> None:
         if len(path) == 0:
             return
         shape = self.new_shape()
         add_path_to_shape(shape, path, close=False)
         self.finish_line(shape, properties, close=False)
         shape.commit()
 
     def draw_filled_paths(
-        self,
-        paths: Iterable[Path | Path2d],
-        holes: Iterable[Path | Path2d],
-        properties: BackendProperties,
+        self, paths: Iterable[BkPath2d], properties: BackendProperties
     ) -> None:
         shape = self.new_shape()
         for p in paths:
             add_path_to_shape(shape, p, close=True)
-        for p in holes:
-            add_path_to_shape(shape, p, close=True)
         self.finish_filling(shape, properties)
         shape.commit()
 
     def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: BackendProperties
+        self, points: BkPoints2d, properties: BackendProperties
     ) -> None:
-        vertices = Vec2.list(points)
+        vertices = points.vertices()
         if len(vertices) < 3:
             return
         # input coordinates are page coordinates in pdf units
         shape = self.new_shape()
         shape.drawPolyline(vertices)
         self.finish_filling(shape, properties)
         shape.commit()
@@ -344,15 +338,15 @@
         pass
 
     def exit_entity(self, entity) -> None:
         pass
 
 
 @no_type_check
-def add_path_to_shape(shape, path: Path2d, close: bool) -> None:
+def add_path_to_shape(shape, path: BkPath2d, close: bool) -> None:
     start = path.start
     sub_path_start = start
     last_point = start
     for command in path.commands():
         end = command.end
         if command.type == Command.MOVE_TO:
             if close and not sub_path_start.isclose(end):
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/pyqt.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,20 @@
 # mypy: ignore_errors=True
 from __future__ import annotations
 from typing import Optional, Iterable
 import abc
 import math
 
 from ezdxf.addons.xqt import QtCore as qc, QtGui as qg, QtWidgets as qw
-from ezdxf.addons.drawing.backend import Backend
+from ezdxf.addons.drawing.backend import Backend, BkPath2d, BkPoints2d
 from ezdxf.addons.drawing.config import Configuration
 from ezdxf.addons.drawing.type_hints import Color
 from ezdxf.addons.drawing.properties import BackendProperties
-from ezdxf.math import Vec3, Matrix44
-from ezdxf.path import Path, to_qpainter_path
+from ezdxf.math import Vec2, Matrix44
+from ezdxf.npshapes import to_qpainter_path
 
 
 class _Point(qw.QAbstractGraphicsShapeItem):
     """A dimensionless point which is drawn 'cosmetically' (scale depends on
     view)
     """
 
@@ -108,83 +108,67 @@
 
     def _get_fill_brush(self, color: Color) -> qg.QBrush:
         return qg.QBrush(self._get_color(color), qc.Qt.SolidPattern)  # type: ignore
 
     def set_background(self, color: Color):
         self._scene.setBackgroundBrush(qg.QBrush(self._get_color(color)))
 
-    def draw_point(self, pos: Vec3, properties: BackendProperties) -> None:
+    def draw_point(self, pos: Vec2, properties: BackendProperties) -> None:
         """Draw a real dimensionless point."""
         brush = self._get_fill_brush(properties.color)
         item = _Point(pos.x, pos.y, brush)
         self._add_item(item, properties.handle)
 
-    def draw_line(self, start: Vec3, end: Vec3, properties: BackendProperties) -> None:
+    def draw_line(self, start: Vec2, end: Vec2, properties: BackendProperties) -> None:
         # PyQt draws a long line for a zero-length line:
         if start.isclose(end):
             self.draw_point(start, properties)
         else:
             item = qw.QGraphicsLineItem(start.x, start.y, end.x, end.y)
             item.setPen(self._get_pen(properties))
             self._add_item(item, properties.handle)
 
     def draw_solid_lines(
         self,
-        lines: Iterable[tuple[Vec3, Vec3]],
+        lines: Iterable[tuple[Vec2, Vec2]],
         properties: BackendProperties,
     ):
         """Fast method to draw a bunch of solid lines with the same properties."""
         pen = self._get_pen(properties)
         add_line = self._add_item
         for s, e in lines:
             if s.isclose(e):
                 self.draw_point(s, properties)
             else:
                 item = qw.QGraphicsLineItem(s.x, s.y, e.x, e.y)
                 item.setPen(pen)
                 add_line(item, properties.handle)
 
-    def draw_path(self, path: Path, properties: BackendProperties) -> None:
+    def draw_path(self, path: BkPath2d, properties: BackendProperties) -> None:
         item = qw.QGraphicsPathItem(to_qpainter_path([path]))
         item.setPen(self._get_pen(properties))
         item.setBrush(self._no_fill)
         self._add_item(item, properties.handle)
 
     def draw_filled_paths(
-        self,
-        paths: Iterable[Path],
-        holes: Iterable[Path],
-        properties: BackendProperties,
+        self, paths: Iterable[BkPath2d], properties: BackendProperties
     ) -> None:
-        oriented_paths: list[Path] = []
-        for path in paths:
-            try:
-                path = path.counter_clockwise()
-            except ValueError:  # cannot detect path orientation
-                continue
-            oriented_paths.append(path)
-        for path in holes:
-            try:
-                path = path.clockwise()
-            except ValueError:  # cannot detect path orientation
-                continue
-            oriented_paths.append(path)
-        if len(oriented_paths) == 0:
-            return
-        item = _CosmeticPath(to_qpainter_path(oriented_paths))
+        # Default fill rule is OddEvenFill! Detecting the path orientation is not
+        # necessary!
+        item = _CosmeticPath(to_qpainter_path(paths))
         item.setPen(self._get_pen(properties))
         item.setBrush(self._get_fill_brush(properties.color))
         self._add_item(item, properties.handle)
 
     def draw_filled_polygon(
-        self, points: Iterable[Vec3], properties: BackendProperties
+        self, points: BkPoints2d, properties: BackendProperties
     ) -> None:
         brush = self._get_fill_brush(properties.color)
         polygon = qg.QPolygonF()
-        for p in points:
+        for p in points.vertices():
             polygon.append(qc.QPointF(p.x, p.y))
         item = _CosmeticPolygon(polygon)
         item.setPen(self._no_line)
         item.setBrush(brush)
         self._add_item(item, properties.handle)
 
     def clear(self) -> None:
@@ -207,14 +191,15 @@
     """
 
     def __init__(
         self,
         scene: Optional[qw.QGraphicsScene] = None,
     ):
         super().__init__(scene or qw.QGraphicsScene())
+
     # This implementation keeps all virtual entities alive by attaching references
     # to entities to the graphic scene items.
 
     def set_item_data(self, item: qw.QGraphicsItem, entity_handle: str) -> None:
         parent_stack = tuple(e for e, props in self.entity_stack[:-1])
         current_entity = self.current_entity
         item.setData(CorrespondingDXFEntity, current_entity)
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/recorder.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/header.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,271 +1,371 @@
-#  Copyright (c) 2023, Manfred Moitzi
-#  License: MIT License
+# Copyright (c) 2011-2022, Manfred Moitzi
+# License: MIT License
 from __future__ import annotations
-from typing import Iterable, Any, Iterator, Callable, Optional, NamedTuple
-from typing_extensions import Self, TypeAlias
-import copy
-import enum
-import dataclasses
-
-from ezdxf.math import AnyVec, BoundingBox2d, Matrix44
-from ezdxf.path import Path, Path2d
-from ezdxf import npshapes
-from ezdxf.tools import take2
-
-from .backend import BackendInterface
-from .config import Configuration
-from .properties import BackendProperties
-from .type_hints import Color
-
-
-class RecordType(enum.Enum):
-    """Enum, determines the data record type.
-
-    Attributes:
-        POINTS:
-        SOLID_LINES:
-        PATH:
-        FILLED_PATHS:
-    """
-    POINTS = enum.auto()
-    SOLID_LINES = enum.auto()
-    PATH = enum.auto()
-    FILLED_PATHS = enum.auto()
-
-
-@dataclasses.dataclass
-class DataRecord:
-    type: RecordType
-    property_hash: int
-    handle: str  # top-level entity handle
-    data: Any
-
+from typing import (
+    Any,
+    Iterable,
+    Iterator,
+    KeysView,
+    Optional,
+    Sequence,
+    TYPE_CHECKING,
+    Union,
+)
+import logging
+from collections import OrderedDict
+
+from ezdxf.lldxf import const
+from ezdxf.lldxf.tags import group_tags, Tags, DXFTag
+from ezdxf.lldxf.types import strtag
+from ezdxf.lldxf.validator import header_validator
+from ezdxf.sections.headervars import (
+    HEADER_VAR_MAP,
+    version_specific_group_code,
+)
+
+if TYPE_CHECKING:
+    from ezdxf.lldxf.tagwriter import AbstractTagWriter
+
+logger = logging.getLogger("ezdxf")
+
+MIN_HEADER_TEXT = """  0
+SECTION
+  2
+HEADER
+  9
+$ACADVER
+  1
+AC1009
+  9
+$DWGCODEPAGE
+  3
+ANSI_1252
+  9
+$HANDSEED
+  5
+FF
+"""
+
+# Additional variables may be stored as DICTIONARYVAR in the OBJECTS
+# section in the DICTIONARY "AcDbVariableDictionary" of the root dict.
+# - CANNOSCALE
+# - CENTEREXE
+# - CENTERLTYPEFILE
+# - CETRANSPARENCY
+# - CMLEADERSTYLE
+# - CTABLESTYLE
+# - CVIEWDETAILSTYLE
+# - CVIEWSECTIONSTYLE
+# - LAYEREVAL
+# - LAYERNOTIFY
+# - LIGHTINGUNITS
+# - MSLTSCALE
+
+
+class CustomVars:
+    """The :class:`CustomVars` class stores custom properties in the DXF header as
+    $CUSTOMPROPERTYTAG and $CUSTOMPROPERTY values. Custom properties require DXF R2004
+    or later, `ezdxf` can create custom properties for older DXF versions as well, but
+    AutoCAD will not show that properties.
 
-class Recorder(BackendInterface):
-    """Records the output of the Frontend class."""
+    """
 
     def __init__(self) -> None:
-        self.config = Configuration()
-        self.background: Color = "#000000"
-        self.records: list[DataRecord] = []
-        self.properties: dict[int, BackendProperties] = dict()
-
-    def player(self) -> Player:
-        """Returns a :class:`Player` instance with the original recordings! Make a copy
-        of this player to protect the original recordings from being modified::
-
-            safe_player = recorder.player().copy()
-
-        """
-        player = Player()
-        player.config = self.config
-        player.background = self.background
-        player.records = self.records
-        player.properties = self.properties
-        player.has_shared_recordings = True
-        return player
-
-    def configure(self, config: Configuration) -> None:
-        self.config = config
-
-    def set_background(self, color: Color) -> None:
-        self.background = color
-
-    def store(
-        self, type_: RecordType, properties: BackendProperties, data: Any
-    ) -> None:
-        # exclude top-level entity handle to reduce the variance:
-        # color, lineweight, layer, pen
-        prop_hash = hash(properties[:4])
-        self.records.append(
-            DataRecord(
-                type=type_, property_hash=prop_hash, handle=properties.handle, data=data
-            )
-        )
-        self.properties[prop_hash] = properties
-
-    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
-        self.store(RecordType.POINTS, properties, npshapes.NumpyPoints2d((pos,)))
-
-    def draw_line(
-        self, start: AnyVec, end: AnyVec, properties: BackendProperties
-    ) -> None:
-        self.store(RecordType.POINTS, properties, npshapes.NumpyPoints2d((start, end)))
-
-    def draw_solid_lines(
-        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: BackendProperties
-    ) -> None:
-        def flatten() -> Iterator[AnyVec]:
-            for s, e in lines:
-                yield s
-                yield e
-
-        self.store(
-            RecordType.SOLID_LINES, properties, npshapes.NumpyPoints2d(flatten())
-        )
-
-    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
-        self.store(RecordType.PATH, properties, npshapes.NumpyPath2d(path))
-
-    def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: BackendProperties
-    ) -> None:
-        self.store(RecordType.POINTS, properties, npshapes.NumpyPoints2d(points))
-
-    def draw_filled_paths(
-        self,
-        paths: Iterable[Path | Path2d],
-        holes: Iterable[Path | Path2d],
-        properties: BackendProperties,
-    ) -> None:
-        _paths = tuple(npshapes.NumpyPath2d(p) for p in paths)
-        _holes = tuple(npshapes.NumpyPath2d(p) for p in holes)
-        self.store(RecordType.FILLED_PATHS, properties, (_paths, _holes))
+        self.properties: list[tuple[str, str]] = list()
 
-    def enter_entity(self, entity, properties) -> None:
-        pass
-
-    def exit_entity(self, entity) -> None:
-        pass
+    def __len__(self) -> int:
+        """Count of custom properties."""
+        return len(self.properties)
+
+    def __iter__(self) -> Iterator[tuple[str, str]]:
+        """Iterate over all custom properties as ``(tag, value)`` tuples."""
+        return iter(self.properties)
 
     def clear(self) -> None:
-        raise NotImplementedError()
+        """Remove all custom properties."""
+        self.properties.clear()
 
-    def finalize(self) -> None:
-        pass
+    def append(self, tag: str, value: str) -> None:
+        """Add custom property as ``(tag, value)`` tuple."""
+        # custom properties always stored as strings
+        self.properties.append((tag, str(value)))
+
+    def get(self, tag: str, default: Optional[str] = None):
+        """Returns the value of the first custom property `tag`."""
+        for key, value in self.properties:
+            if key == tag:
+                return value
+        else:
+            return default
+
+    def has_tag(self, tag: str) -> bool:
+        """Returns ``True`` if custom property `tag` exist."""
+        return self.get(tag) is not None
+
+    def remove(self, tag: str, all: bool = False) -> None:
+        """Removes the first occurrence of custom property `tag`, removes all
+        occurrences if `all` is ``True``.
 
+        Raises `:class:`DXFValueError` if `tag`  does not exist.
 
-class Override(NamedTuple):
-    """Represents the override state for a data record.
+        """
+        found_tag = False
+        for item in self.properties:
+            if item[0] == tag:
+                self.properties.remove(item)
+                found_tag = True
+                if not all:
+                    return
+        if not found_tag:
+            raise const.DXFValueError(f"Tag '{tag}' does not exist")
+
+    def replace(self, tag: str, value: str) -> None:
+        """Replaces the value of the first custom property `tag` by a new
+        `value`.
 
-    Attributes:
-        properties: original or modified :class:`BackendProperties`
-        is_visible: override visibility e.g. switch layers on/off
+        Raises :class:`DXFValueError` if `tag`  does not exist.
 
-    """
+        """
+        properties = self.properties
+        for index in range(len(properties)):
+            name = properties[index][0]
+            if name == tag:
+                properties[index] = (name, value)
+                return
+
+        raise const.DXFValueError(f"Tag '{tag}' does not exist")
+
+    def write(self, tagwriter: AbstractTagWriter) -> None:
+        """Export custom properties as DXF tags. (internal API)"""
+        for tag, value in self.properties:
+            s = f"  9\n$CUSTOMPROPERTYTAG\n  1\n{tag}\n  9\n$CUSTOMPROPERTY\n  1\n{value}\n"
+            tagwriter.write_str(s)
+
+
+def default_vars() -> OrderedDict:
+    vars = OrderedDict()
+    for vardef in HEADER_VAR_MAP.values():
+        vars[vardef.name] = HeaderVar(DXFTag(vardef.code, vardef.default))
+    return vars
+
+
+class HeaderSection:
+    MIN_HEADER_TAGS = Tags.from_text(MIN_HEADER_TEXT)
+    name = "HEADER"
 
-    properties: BackendProperties
-    is_visible: bool = True
+    def __init__(self) -> None:
+        self.hdrvars: dict[str, HeaderVar] = OrderedDict()
+        self.custom_vars = CustomVars()
 
+    @classmethod
+    def load(cls, tags: Optional[Iterable[DXFTag]] = None) -> HeaderSection:
+        """Constructor to generate header variables loaded from DXF files
+        (untrusted environment).
 
-OverrideFunc: TypeAlias = Callable[[BackendProperties], Override]
+        Args:
+            tags: DXF tags as Tags() or ExtendedTags()
 
+        (internal API)
+        """
+        if tags is None:  # create default header
+            # files without a header have the default version: R12
+            return cls.new(dxfversion=const.DXF12)
+        section = cls()
+        section.load_tags(iter(tags))
+        return section
+
+    @classmethod
+    def new(cls, dxfversion=const.LATEST_DXF_VERSION) -> HeaderSection:
+        section = HeaderSection()
+        section.hdrvars = default_vars()
+        section["$ACADVER"] = dxfversion
+        return section
+
+    def load_tags(self, tags: Iterable[DXFTag]) -> None:
+        """Constructor to generate header variables loaded from DXF files
+        (untrusted environment).
 
-class Player:
-    """Plays the recordings of the :class:`Recorder` backend on another backend."""
+        Args:
+            tags: DXF tags as Tags() or ExtendedTags()
 
-    def __init__(self) -> None:
-        self.config = Configuration()
-        self.background: Color = "#000000"
-        self.records: list[DataRecord] = []
-        self.properties: dict[int, BackendProperties] = dict()
-        self._bbox = BoundingBox2d()
-        self.has_shared_recordings: bool = False
-
-    def __copy__(self) -> Self:
-        """Returns a copy of the player with non-shared recordings."""
-        player = self.__class__()
-        # config is a frozen dataclass:
-        player.config = self.config
-        player.background = self.background
-        # recordings are mutable - transformed inplace:
-        player.records = copy.deepcopy(self.records)
-        # the properties dict may grow, but entries will never be removed:
-        player.properties = self.properties
-        player.has_shared_recordings = False
-        return player
-
-    copy = __copy__
-
-    def recordings(self) -> Iterator[tuple[RecordType, BackendProperties, Any]]:
-        """Yields all recordings as `(RecordType, BackendProperties, Data)` tuples.
-
-        The content of the `Data` field is determined by the enum :class:`RecordType`:
-
-        - :attr:`RecordType.POINTS` returns a :class:`NumpyPoints2d` instance,
-          len() == 1 is a point, len() == 2 is a line, len() > 2 is a filled polygon
-        - :attr:`RecordType.SOLID_LINES` returns a :class:`NumpyPoints2d` instance
-          where each pair (n, n+1) represents the start- and end point of a line
-        - :attr:`RecordType.PATH`: returns a :class:`NumpyPath2d` instance that
-          represents a linear 2D path
-        - :attr:`RecordType.FILLED_PATHS` returns a tuple (exterior_paths, holes),
-          where exterior_paths and holes are tuples of :class:`NumpyPath2d`.
+        """
+        _tags = iter(tags) or iter(self.MIN_HEADER_TAGS)
+        section_tag = next(_tags)
+        name_tag = next(_tags)
+
+        if section_tag != (0, "SECTION") or name_tag != (2, "HEADER"):
+            raise const.DXFStructureError("Critical structure error in HEADER section.")
+
+        groups = group_tags(header_validator(_tags), splitcode=9)
+        custom_property_stack = []  # collect $CUSTOMPROPERTY/TAG
+        for group in groups:
+            name = group[0].value
+            value = group[1]
+            if name in ("$CUSTOMPROPERTYTAG", "$CUSTOMPROPERTY"):
+                custom_property_stack.append(value.value)
+            else:
+                self.hdrvars[name] = HeaderVar(value)
+
+        custom_property_stack.reverse()
+        while len(custom_property_stack):
+            try:
+                self.custom_vars.append(
+                    tag=custom_property_stack.pop(),
+                    value=custom_property_stack.pop(),
+                )
+            except IndexError:  # internal exception
+                break
+
+    @classmethod
+    def from_text(cls, text: str) -> HeaderSection:
+        """Load constructor from text for testing"""
+        return cls.load(Tags.from_text(text))  # type: ignore
+
+    def _headervar_factory(self, key: str, value: Any) -> DXFTag:
+        if key in HEADER_VAR_MAP:
+            factory = HEADER_VAR_MAP[key].factory
+            return factory(value)
+        else:
+            raise const.DXFKeyError(f"Invalid header variable {key}.")
+
+    def __len__(self) -> int:
+        """Returns count of header variables."""
+        return len(self.hdrvars)
+
+    def __contains__(self, key) -> bool:
+        """Returns ``True`` if header variable `key` exist."""
+        return key in self.hdrvars
+
+    def varnames(self) -> KeysView:
+        """Returns an iterable of all header variable names."""
+        return self.hdrvars.keys()
+
+    def export_dxf(self, tagwriter: AbstractTagWriter) -> None:
+        """Exports header section as DXF tags. (internal API)"""
+
+        def _write(name: str, value: Any) -> None:
+            if value.value is None:
+                logger.info(f"did not write header var {name}, value is None.")
+                return
+            tagwriter.write_tag2(9, name)
+            group_code = version_specific_group_code(name, dxfversion)
+            # fix invalid group codes
+            if group_code != value.code:
+                value = HeaderVar((group_code, value.value))
+            tagwriter.write_str(str(value))
+
+        dxfversion: str = tagwriter.dxfversion
+        write_handles = tagwriter.write_handles
+
+        tagwriter.write_str("  0\nSECTION\n  2\nHEADER\n")
+        save = self["$ACADVER"]
+        self["$ACADVER"] = dxfversion
+        for name, value in header_vars_by_priority(self.hdrvars, dxfversion):
+            if not write_handles and name == "$HANDSEED":
+                continue  # skip $HANDSEED
+            _write(name, value)
+            if name == "$LASTSAVEDBY":  # ugly hack, but necessary for AutoCAD
+                self.custom_vars.write(tagwriter)
+        self["$ACADVER"] = save
+        tagwriter.write_str("  0\nENDSEC\n")
+
+    def get(self, key: str, default: Any = None) -> Any:
+        """Returns value of header variable `key` if exist, else the `default`
+        value.
 
         """
-        props = self.properties
-        for record in self.records:
-            properties = BackendProperties(
-                *props[record.property_hash][:4], record.handle
-            )
-            yield record.type, properties, record.data
-
-    def replay(
-        self, backend: BackendInterface, override: Optional[OverrideFunc] = None
-    ) -> None:
-        """Replay the recording on another backend that implements the
-        :class:`BackendInterface`. The optional `override` function can be used to
-        override the properties and state of data records, it gets the :class:`BackendProperties`
-        as input and must return an :class:`Override` instance.
+        if key in self.hdrvars:
+            return self.__getitem__(key)
+        else:
+            return default
+
+    def __getitem__(self, key: str) -> Any:
+        """Get header variable `key` by index operator like:
+        :code:`drawing.header['$ACADVER']`
+
         """
+        try:
+            return self.hdrvars[key].value
+        except KeyError:  # map exception
+            raise const.DXFKeyError(str(key))
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        """Set header variable `key` to `value` by index operator like:
+        :code:`drawing.header['$ANGDIR'] = 1`
 
-        backend.configure(self.config)
-        backend.set_background(self.background)
-        for record_type, properties, data in self.recordings():
-            if override:
-                state = override(properties)
-                if not state.is_visible:
-                    continue
-                properties = state.properties
-            if record_type == RecordType.POINTS:
-                vertices = data.vertices()
-                if len(vertices) == 1:
-                    backend.draw_point(vertices[0], properties)
-                elif len(vertices) == 2:
-                    backend.draw_line(vertices[0], vertices[1], properties)
-                else:
-                    backend.draw_filled_polygon(vertices, properties)
-            elif record_type == RecordType.SOLID_LINES:
-                backend.draw_solid_lines(take2(data.vertices()), properties)
-            elif record_type == RecordType.PATH:
-                backend.draw_path(data.to_path2d(), properties)
-            elif record_type == RecordType.FILLED_PATHS:
-                paths = [p.to_path2d() for p in data[0]]
-                holes = [p.to_path2d() for p in data[1]]
-                backend.draw_filled_paths(paths, holes, properties)
-        backend.finalize()
-
-    def transform(self, m: Matrix44) -> None:
-        """Transforms the recordings inplace by a transformation matrix `m` of type
-        :class:`~ezdxf.math.Matrix44`.
         """
-        for record in self.records:
-            if record.type == RecordType.FILLED_PATHS:
-                for p in record.data[0]:
-                    p.transform_inplace(m)
-                for p in record.data[1]:
-                    p.transform_inplace(m)
-            else:
-                record.data.transform_inplace(m)
+        try:
+            tags = self._headervar_factory(key, value)
+        except (IndexError, ValueError):
+            raise const.DXFValueError(str(value))
+        self.hdrvars[key] = HeaderVar(tags)
+
+    def __delitem__(self, key: str) -> None:
+        """Delete header variable `key` by index operator like:
+        :code:`del drawing.header['$ANGDIR']`
 
-        if self._bbox.has_data:
-            # works for 90-, 180- and 270-degree rotation
-            self._bbox = BoundingBox2d(m.fast_2d_transform(self._bbox.rect_vertices()))
-
-    def bbox(self) -> BoundingBox2d:
-        """Returns the bounding box of all records as :class:`~ezdxf.math.BoundingBox2d`."""
-        if not self._bbox.has_data:
-            self.update_bbox()
-        return self._bbox
-
-    def update_bbox(self) -> None:
-        points: list[AnyVec] = []
-        for record in self.records:
-            try:
-                if record.type == RecordType.FILLED_PATHS:
-                    for path in record.data[0]:  # only add paths, ignore holes
-                        points.extend(path.extents())
-                else:
-                    points.extend(record.data.extents())
-            except npshapes.EmptyShapeError:
-                pass
-        self._bbox = BoundingBox2d(points)
+        """
+        try:
+            del self.hdrvars[key]
+        except KeyError:  # map exception
+            raise const.DXFKeyError(str(key))
+
+    def reset_wcs(self):
+        """Reset the current UCS settings to the :ref:`WCS`."""
+        self["$UCSBASE"] = ""
+        self["$UCSNAME"] = ""
+        self["$UCSORG"] = (0, 0, 0)
+        self["$UCSXDIR"] = (1, 0, 0)
+        self["$UCSYDIR"] = (0, 1, 0)
+        self["$UCSORTHOREF"] = ""
+        self["$UCSORTHOVIEW"] = 0
+        self["$UCSORGTOP"] = (0, 0, 0)
+        self["$UCSORGBOTTOM"] = (0, 0, 0)
+        self["$UCSORGLEFT"] = (0, 0, 0)
+        self["$UCSORGRIGHT"] = (0, 0, 0)
+        self["$UCSORGFRONT"] = (0, 0, 0)
+        self["$UCSORGBACK"] = (0, 0, 0)
+
+
+def header_vars_by_priority(
+    header_vars: dict[str, HeaderVar], dxfversion: str
+) -> Iterable[tuple]:
+    order = []
+    for name, value in header_vars.items():
+        vardef = HEADER_VAR_MAP.get(name, None)
+        if vardef is None:
+            logger.info(f"Header variable {name} ignored, dxfversion={dxfversion}.")
+            continue
+        if vardef.mindxf <= dxfversion <= vardef.maxdxf:
+            order.append((vardef.priority, (name, value)))
+    order.sort()
+    for priority, tag in order:
+        yield tag
+
+
+class HeaderVar:
+    def __init__(self, tag: Union[DXFTag, Sequence]):
+        self.tag = tag
+
+    @property
+    def code(self) -> int:
+        return self.tag[0]
+
+    @property
+    def value(self) -> Any:
+        return self.tag[1]
+
+    @property
+    def ispoint(self) -> bool:
+        return self.code == 10
+
+    def __str__(self) -> str:
+        if self.ispoint:
+            code, value = self.tag
+            s = []
+            for coord in value:
+                s.append(strtag((code, coord)))
+                code += 10
+            return "".join(s)
+        else:
+            return strtag(self.tag)  # type: ignore
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/svg.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/svg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Iterable, Sequence, no_type_check
 
 import copy
-import itertools
 from xml.etree import ElementTree as ET
 
-from ezdxf.math import AnyVec, Vec2
-from ezdxf.path import Path, Path2d, Command
+from ezdxf.math import Vec2
+from ezdxf.path import Command
 
 
 from .type_hints import Color
-from .backend import BackendInterface
+from .backend import BackendInterface, BkPath2d, BkPoints2d
 from .config import Configuration, LineweightPolicy
 from .properties import BackendProperties
 from . import layout, recorder
 
 __all__ = ["SVGBackend"]
 
 
@@ -254,49 +253,46 @@
 
     def set_background(self, color: Color) -> None:
         color_str = color[:7]
         opacity = alpha_to_opacity(color[7:9])
         self.background.set("fill", color_str)
         self.background.set("fill-opacity", str(opacity))
 
-    def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
+    def draw_point(self, pos: Vec2, properties: BackendProperties) -> None:
         self.add_strokes(self.make_polyline_str([pos, pos]), properties)
 
-    def draw_line(
-        self, start: AnyVec, end: AnyVec, properties: BackendProperties
-    ) -> None:
+    def draw_line(self, start: Vec2, end: Vec2, properties: BackendProperties) -> None:
         self.add_strokes(self.make_polyline_str([start, end]), properties)
 
     def draw_solid_lines(
-        self, lines: Iterable[tuple[AnyVec, AnyVec]], properties: BackendProperties
+        self, lines: Iterable[tuple[Vec2, Vec2]], properties: BackendProperties
     ) -> None:
         lines = list(lines)
         if len(lines) == 0:
             return
         self.add_strokes(self.make_multi_line_str(lines), properties)
 
-    def draw_path(self, path: Path | Path2d, properties: BackendProperties) -> None:
+    def draw_path(self, path: BkPath2d, properties: BackendProperties) -> None:
         self.add_strokes(self.make_path_str(path), properties)
 
     def draw_filled_paths(
-        self,
-        paths: Iterable[Path | Path2d],
-        holes: Iterable[Path | Path2d],
-        properties: BackendProperties,
+        self, paths: Iterable[BkPath2d], properties: BackendProperties
     ) -> None:
         d = []
-        for path in itertools.chain(paths, holes):
+        for path in paths:
             if len(path):
                 d.append(self.make_path_str(path, close=True))
         self.add_filling(" ".join(d), properties)
 
     def draw_filled_polygon(
-        self, points: Iterable[AnyVec], properties: BackendProperties
+        self, points: BkPoints2d, properties: BackendProperties
     ) -> None:
-        self.add_filling(self.make_polyline_str(list(points), close=True), properties)
+        self.add_filling(
+            self.make_polyline_str(points.vertices(), close=True), properties
+        )
 
     @staticmethod
     def make_polyline_str(points: Sequence[Vec2], close=False) -> str:
         if len(points) < 2:
             return ""
         current = points[0]
         # first move is absolute, consecutive lines are relative:
@@ -320,15 +316,15 @@
             current = start
             d.append(CMD_L_REL.format(end - current))
             current = end
         return " ".join(d)
 
     @staticmethod
     @no_type_check
-    def make_path_str(path: Path | Path2d, close=False) -> str:
+    def make_path_str(path: BkPath2d, close=False) -> str:
         d: list[str] = [CMD_M_ABS.format(path.start)]
         if len(path) == 0:
             return ""
 
         current = path.start
         for cmd in path.commands():
             end = cmd.end
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #  Copyright (c) 2022-2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import TypeVar
+from typing import TypeVar, TYPE_CHECKING
 import abc
 from ezdxf.fonts import fonts
-from ezdxf.path import Path2d
+
+if TYPE_CHECKING:
+    from ezdxf.npshapes import NumpyPath2d
 
 T = TypeVar("T")
 
 
 class TextRenderer(abc.ABC):
     """Minimal requirement to be usable as a universal text renderer"""
 
@@ -26,13 +28,19 @@
         cap_height: float = 1.0,
     ) -> float:
         ...
 
     @abc.abstractmethod
     def get_text_path(
         self, text: str, font_face: fonts.FontFace, cap_height: float = 1.0
-    ) -> Path2d:
+    ) -> NumpyPath2d:
+        ...
+
+    @abc.abstractmethod
+    def get_text_glyph_paths(
+        self, text: str, font_face: fonts.FontFace, cap_height: float = 1.0
+    ) -> list[NumpyPath2d]:
         ...
 
     @abc.abstractmethod
     def is_stroke_font(self, font_face: fonts.FontFace) -> bool:
         ...
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/unified_text_renderer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/drawing/unified_text_renderer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # Copyright (c) 2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-import ezdxf.path
+from typing import TYPE_CHECKING
 from ezdxf.fonts import fonts
 from ezdxf.fonts.font_measurements import FontMeasurements
 
 from .text_renderer import TextRenderer
 
+if TYPE_CHECKING:
+    from ezdxf.npshapes import NumpyPath2d
+
 
 class UnifiedTextRenderer(TextRenderer):
     """This text renderer supports .ttf, .ttc, .otf, .shx, .shp and .lff fonts.
 
     The resolving order for .shx fonts is applied in the RenderContext.add_text_style()
     method.
 
@@ -45,18 +48,24 @@
         self, font_face: fonts.FontFace, cap_height: float = 1.0
     ) -> FontMeasurements:
         abstract_font = self.get_font(font_face)
         return abstract_font.measurements.scale(cap_height)
 
     def get_text_path(
         self, text: str, font_face: fonts.FontFace, cap_height: float = 1.0
-    ) -> ezdxf.path.Path2d:
+    ) -> NumpyPath2d:
         abstract_font = self.get_font(font_face)
         return abstract_font.text_path_ex(text, cap_height)
 
+    def get_text_glyph_paths(
+        self, text: str, font_face: fonts.FontFace, cap_height: float = 1.0
+    ) -> list[NumpyPath2d]:
+        abstract_font = self.get_font(font_face)
+        return abstract_font.text_glyph_paths(text, cap_height)
+
     def get_text_line_width(
         self,
         text: str,
         font_face: fonts.FontFace,
         cap_height: float = 1.0,
     ) -> float:
         abstract_font = self.get_font(font_face)
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/api.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/backend.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing_extensions import Self
 import abc
 import copy
 import enum
 import math
 from .deps import (
     Vec2,
-    Path2d,
+    Path,
     colors,
     Matrix44,
     BoundingBox2d,
 )
 from .properties import Properties, Pen
 from ezdxf.npshapes import NumpyPath2d, NumpyPoints2d
 
@@ -40,24 +40,24 @@
             points: sequence of :class:`ezdxf.math.Vec2` instances
 
         """
         ...
 
     @abc.abstractmethod
     def draw_paths(
-        self, properties: Properties, paths: Sequence[Path2d], filled: bool
+        self, properties: Properties, paths: Sequence[Path], filled: bool
     ) -> None:
         """Draws filled or outline paths from the sequence of `paths`. The input coordinates
         are page coordinates in plot units. The `paths` sequence can contain 0 or more
         single :class:`~ezdxf.path.Path` instances. Draws outline paths if
         Properties.FillType is NONE and filled paths otherwise.
 
         Args:
             properties: display :class:`Properties` for the filled polygon
-            paths: sequence of single :class:`ezdxf.path.Path2d` instances
+            paths: sequence of single :class:`ezdxf.path.Path` instances
             filled: draw filled paths if ``True`` otherwise outline paths
 
         """
         ...
 
 
 class RecordType(enum.Enum):
@@ -97,17 +97,17 @@
         """
         return Player(self._records, self._properties)
 
     def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
         self.store(RecordType.POLYLINE, properties, NumpyPoints2d(points))
 
     def draw_paths(
-        self, properties: Properties, paths: Sequence[Path2d], filled: bool
+        self, properties: Properties, paths: Sequence[Path], filled: bool
     ) -> None:
-        data = tuple(NumpyPath2d(p) for p in paths)
+        data = tuple(map(NumpyPath2d, paths))
         record_type = RecordType.FILLED_PATHS if filled else RecordType.OUTLINE_PATHS
         self.store(record_type, properties, data)
 
     def store(self, record_type: RecordType, properties: Properties, args) -> None:
         prop_hash = properties.hash()
         if prop_hash not in self._properties:
             self._properties[prop_hash] = properties.copy()
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/deps.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/deps.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,11 +3,11 @@
 #
 # Central import location of frontend dependencies.
 # To extract te hpgl2 add-on from the ezdxf package, the following tools have to be
 # implemented or extracted too. The dependencies of the implemented backends are not
 # listed here.
 
 from ezdxf.math import Vec2, ConstructionCircle, BoundingBox2d, Bezier4P, AnyVec, Matrix44
-from ezdxf.path import Path2d, bbox as path_bbox, transform_paths
+from ezdxf.path import Path, bbox as path_bbox, transform_paths
 from ezdxf.tools.standards import PAGE_SIZES
 from ezdxf import colors
 NULLVEC2 = Vec2(0, 0)
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/page.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #  License: MIT License
 from __future__ import annotations
 from typing import Sequence, Iterator
 import math
 
 from .deps import (
     Vec2,
-    Path2d,
+    Path,
     NULLVEC2,
     ConstructionCircle,
     Bezier4P,
 )
 from .properties import RGB, Properties, FillType
 from .backend import Backend
 from .polygon_buffer import PolygonBuffer
@@ -246,30 +246,30 @@
         # input coordinates are user coordinates
         current_page_location = self.page_location
         self.move_to_abs(end)  # user coordinates!
         if self.is_pen_down:
             # convert to page coordinates:
             ctrl1, ctrl2, end = self.page.page_points((ctrl1, ctrl2, end))
             # draw cubic bezier curve in absolute page coordinates:
-            p = Path2d(current_page_location)
+            p = Path(current_page_location)
             p.curve4_to(end, ctrl1, ctrl2)
             self.backend.draw_paths(self.properties, [p], filled=False)
 
     def plot_rel_cubic_bezier(self, ctrl1: Vec2, ctrl2: Vec2, end: Vec2):
         # input coordinates are user coordinates
         ctrl1, ctrl2, end = rel_to_abs_points_static(
             self.user_location, (ctrl1, ctrl2, end)
         )
         self.plot_abs_cubic_bezier(ctrl1, ctrl2, end)
 
-    def plot_filled_polygon_buffer(self, paths: Sequence[Path2d]):
+    def plot_filled_polygon_buffer(self, paths: Sequence[Path]):
         # input coordinates are page coordinates!
         self.backend.draw_paths(self.properties, paths, filled=True)
 
-    def plot_outline_polygon_buffer(self, paths: Sequence[Path2d]):
+    def plot_outline_polygon_buffer(self, paths: Sequence[Path]):
         # input coordinates are page coordinates!
         self.backend.draw_paths(self.properties, paths, filled=False)
 
 
 def rel_to_abs_points_dynamic(current: Vec2, points: Sequence[Vec2]) -> Iterator[Vec2]:
     """Returns the absolute location of increment points, each point is an increment
     of the previous point starting at the current pen location.
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Sequence
 from .backend import Backend
-from .deps import Vec2, Path2d
+from .deps import Vec2, Path
 from .properties import Properties
 
 
 class PolygonBuffer(Backend):
     def __init__(self):
-        self.path = Path2d()
+        self.path = Path()
         self.start_new_sub_polygon = False
 
     def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
         if len(points) == 0:
             return
         index = 0
         if self.start_new_sub_polygon:
@@ -24,30 +24,30 @@
                 if index == count:
                     return
             self.path.move_to(points[index])
         for p in points[index + 1 :]:
             self.path.line_to(p)
 
     def draw_paths(
-        self, properties: Properties, paths: Sequence[Path2d], filled: bool
+        self, properties: Properties, paths: Sequence[Path], filled: bool
     ) -> None:
         if filled:
             raise NotImplementedError()
         for p in paths:
             if len(p) == 0:
                 continue
             if self.start_new_sub_polygon:
                 self.start_new_sub_polygon = False
                 self.path.move_to(p.start)
             self.path.append_path(p)
 
-    def get_paths(self) -> Sequence[Path2d]:
+    def get_paths(self) -> Sequence[Path]:
         return list(self.path.sub_paths())
 
     def close_path(self):
         if len(self.path):
             self.path.close_sub_path()
             self.start_new_sub_polygon = True
 
     def reset(self, location: Vec2) -> None:
-        self.path = Path2d(location)
+        self.path = Path(location)
         self.start_new_sub_polygon = False
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/properties.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/tokenizer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/tokenizer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/viewer.py` & `ezdxf-1.1.0b4/src/ezdxf/addons/hpgl2/viewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/acad_table.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/acis.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/appdata.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/appid.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/arc.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/attrib.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/block.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/blockrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/circle.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dictionary.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dimension.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dxfns.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/ellipse.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/factory.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/geodata.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/gradient.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/gradient.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/hatch.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/helix.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/image.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/insert.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/layer.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/layout.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/leader.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/light.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/line.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/ltype.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/material.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/mesh.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/mleader.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/mline.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/mtext.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/oleframe.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/pattern.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/point.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/polygon.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/polygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/polyline.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/shape.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/solid.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/spline.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/subentity.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/sun.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/table.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/text.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/textstyle.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/textstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/tolerance.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/ucs.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/underlay.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/view.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/viewport.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/vport.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/xdata.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/xdict.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/xline.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/entities/__init__.py` & `ezdxf-1.1.0b4/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/fonts/fonts.py` & `ezdxf-1.1.0b4/src/ezdxf/fonts/fonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,24 +19,23 @@
 )
 from .font_measurements import FontMeasurements
 from .glyphs import GlyphPath, Glyphs
 
 if TYPE_CHECKING:
     from ezdxf.document import Drawing
     from ezdxf.entities import DXFEntity, Textstyle
-    from ezdxf.path import Path2d
 
 logger = logging.getLogger("ezdxf")
 FONT_MANAGER_CACHE_FILE = "font_manager_cache.json"
 CACHE_DIRECTORY = ".cache"
 font_manager = FontManager()
 
 SHX_FONTS = {
     # See examples in: CADKitSamples/Shapefont.dxf
-    # Shape file structure is not documented, therefore replace this fonts by
+    # Shape file structure is not documented, therefore, replace these fonts by
     # true type fonts.
     # `None` is for: use the default font.
     #
     # All these replacement TTF fonts have a copyright remark:
     # "(c) Copyright 1996 by Autodesk Inc., All rights reserved"
     # and therefore can not be included in ezdxf or the associated repository!
     # You got them if you install any Autodesk product, like the free available
@@ -370,14 +369,22 @@
     def text_path_ex(
         self, text: str, cap_height: float, width_factor: float = 1.0
     ) -> GlyphPath:
         """Returns the 2D text path for the given text, bypasses the stored `cap_height`
         and `width_factor`."""
         ...
 
+    @abc.abstractmethod
+    def text_glyph_paths(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> list[GlyphPath]:
+        """Returns a list of 2D glyph paths for the given text, bypasses the stored
+        `cap_height` and `width_factor`."""
+        ...
+
 
 class MonospaceFont(AbstractFont):
     """Represents a monospaced font where each letter has the same cap- and descender
     height and the same width. The given cap height and width factor are the default
     values for measurements and rendering. The extended methods can override these
     default values.
 
@@ -419,32 +426,38 @@
     ) -> float:
         """Returns the text width in drawing units, bypasses the stored `cap_height` and
         `width_factor`.
         """
         return len(text) * cap_height * width_factor
 
     def text_path(self, text: str) -> GlyphPath:
-        """Returns the rectangle text width x cap height as :class:`~ezdxf.path.Path2d` instance."""
+        """Returns the rectangle text width x cap height as :class:`NumpyPath2d` instance."""
         return self.text_path_ex(text, self.measurements.cap_height, self._width_factor)
 
     def text_path_ex(
         self, text: str, cap_height: float, width_factor: float = 1.0
     ) -> GlyphPath:
-        """Returns the rectangle text width x cap height as  :class:`~ezdxf.path.Path2d`
+        """Returns the rectangle text width x cap height as  :class:`NumpyPath2d`
         instance, bypasses the stored `cap_height` and `width_factor`.
         """
-        from ezdxf.path import Path2d
+        from ezdxf.path import Path
 
         text_width = self.text_width_ex(text, cap_height, width_factor)
-        p = Path2d((0, 0))
+        p = Path((0, 0))
         p.line_to((text_width, 0))
         p.line_to((text_width, cap_height))
         p.line_to((0, cap_height))
         p.close()
-        return p
+        return GlyphPath(p)
+
+    def text_glyph_paths(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> list[GlyphPath]:
+        """Returns the same rectangle as the method :meth:`text_path_ex` in a list."""
+        return [self.text_path_ex(text, cap_height, width_factor)]
 
     def space_width(self) -> float:
         """Returns the width of a "space" char."""
         return self._space_width
 
 
 class _CachedFont(AbstractFont, abc.ABC):
@@ -490,25 +503,25 @@
     def text_path_ex(
         self, text: str, cap_height: float, width_factor: float = 1.0
     ) -> GlyphPath:
         """Returns the 2D text path for the given text, bypasses the stored `cap_height`
         and `width_factor`."""
         return self.glyph_cache.get_text_path(text, cap_height, width_factor)
 
+    def text_glyph_paths(
+        self, text: str, cap_height: float, width_factor: float = 1.0
+    ) -> list[GlyphPath]:
+        """Returns a list of 2D glyph paths for the given text, bypasses the stored
+        `cap_height` and `width_factor`."""
+        return self.glyph_cache.get_text_glyph_paths(text, cap_height, width_factor)
+
     def space_width(self) -> float:
         """Returns the width of a "space" char."""
         return self._space_width
 
-# --------------------------------------------------------------------------------------
-# NOTES:
-# "romantic.ttf" uses the Private Use Area (PUA) codepoints (f000-e000) for its glyphs
-# and has no glyphs for the usual code points.
-# see example: "CADKitSamples\Proposed Townhouse.dxf"
-# I deleted this font from my system!
-
 
 class TrueTypeFont(_CachedFont):
     """Represents a TrueType font. Font measurement and glyph rendering is done by the
     `fontTools` package. The given cap height and width factor are the default values
     for measurements and glyph rendering. The extended methods can override these
     default values.
     """
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/fonts/font_face.py` & `ezdxf-1.1.0b4/src/ezdxf/fonts/font_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/fonts/font_manager.py` & `ezdxf-1.1.0b4/src/ezdxf/fonts/font_manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from __future__ import annotations
 
 import pathlib
 from typing import Iterable, NamedTuple, Optional, Sequence
 import os
 import platform
 import json
+import logging
 
 from pathlib import Path
 from fontTools.ttLib import TTFont, TTLibError
 from .font_face import FontFace
 from . import shapefile, lff
 
+logger = logging.getLogger("ezdxf")
 WINDOWS = "Windows"
 LINUX = "Linux"
 MACOS = "Darwin"
 
 
 WIN_SYSTEM_ROOT = os.environ.get("SystemRoot", "C:/Windows")
 WIN_FONT_DIRS = [
@@ -451,17 +453,23 @@
     for record in names:
         if record.nameID == 1:
             family = record.string.decode(record.getEncoding())
         elif record.nameID == 2:
             style = record.string.decode(record.getEncoding())
         if family and style:
             break
-    os2_table = ttf["OS/2"]
-    weight = os2_table.usWeightClass
-    width = os2_table.usWidthClass
+    try:
+        os2_table = ttf["OS/2"]
+    except Exception:  # e.g. ComickBook_Simple.ttf has an invalid "OS/2" table
+        logger.info(f"cannot load OS/2 table of font '{font_path.name}'")
+        weight = 400
+        width = 5
+    else:
+        weight = os2_table.usWeightClass
+        width = os2_table.usWidthClass
     return FontFace(
         filename=font_path.name,
         family=family,
         style=normalize_style(style),
         width=width,
         weight=weight,
     )
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/fonts/font_measurements.py` & `ezdxf-1.1.0b4/src/ezdxf/fonts/font_measurements.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/fonts/lff.py` & `ezdxf-1.1.0b4/src/ezdxf/fonts/lff.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         ocs = OCS()
         for polyline in self.polylines:
             p = path.Path()  # empty path is required
             path.add_2d_polyline(
                 p, convert_bulge_values(polyline), close=False, elevation=0, ocs=ocs
             )
             final_path.extend_multi_path(p)
-        return final_path.to_2d_path()
+        return GlyphPath(final_path)
 
 
 def convert_bulge_values(polyline: Polyline) -> Iterator[Sequence[float]]:
     # In DXF the bulge value is always stored at the start vertex of the arc.
     last_index = len(polyline) - 1
     for index, vertex in enumerate(polyline):
         bulge = 0.0
@@ -230,47 +230,47 @@
 
     def get_empty_box(self) -> GlyphPath:
         glyph_A = self.get_shape(65)
         box = BoundingBox2d(glyph_A.control_vertices())
         height = box.size.y
         width = box.size.x
         start = glyph_A.start
-        p = GlyphPath(start)
+        p = path.Path(start)
         p.line_to(start + Vec2(width, 0))
         p.line_to(start + Vec2(width, height))
         p.line_to(start + Vec2(0, height))
         p.close()
         p.move_to(glyph_A.end)
-        return p
+        return GlyphPath(p)
 
     def _render_shape(self, shape_number) -> GlyphPath:
         try:
             glyph = self.font[shape_number]
         except KeyError:
             if shape_number > 32:
                 return self.empty_box
             raise ValueError("space and non-printable characters are not glyphs")
         return glyph.to_path()
 
     def get_shape(self, shape_number: int) -> GlyphPath:
         if shape_number <= 32:
             raise ValueError("space and non-printable characters are not glyphs")
         try:
-            return self._glyph_cache[shape_number]
+            return self._glyph_cache[shape_number].clone()
         except KeyError:
             pass
         glyph = self._render_shape(shape_number)
         self._glyph_cache[shape_number] = glyph
         advance_width = 0.0
         if len(glyph):
-            box = BoundingBox2d(glyph.control_vertices())
+            box = glyph.bbox()
             assert box.extmax is not None
             advance_width = box.extmax.x + self.font.letter_spacing
         self._advance_width_cache[shape_number] = advance_width
-        return glyph
+        return glyph.clone()
 
     def get_advance_width(self, shape_number: int) -> float:
         if shape_number < 32:
             return 0.0
         if shape_number == 32:
             return self.space_width
         try:
@@ -301,25 +301,24 @@
 
     def get_text_length(
         self, text: str, cap_height: float, width_factor: float = 1.0
     ) -> float:
         scaling_factor = self.get_scaling_factor(cap_height) * width_factor
         return sum(self.get_advance_width(ord(c)) for c in text) * scaling_factor
 
-    def get_text_path(
+    def get_text_glyph_paths(
         self, text: str, cap_height: float, width_factor: float = 1.0
-    ) -> GlyphPath:
-        p = GlyphPath()
+    ) -> list[GlyphPath]:
+        glyph_paths: list[GlyphPath] = []
         sy = self.get_scaling_factor(cap_height)
         sx = sy * width_factor
         m = Matrix44.scale(sx, sy, 1)
         current_location = 0.0
         for c in text:
             shape_number = ord(c)
             if shape_number > 32:
                 glyph = self.get_shape(shape_number)
                 m[3, 0] = current_location
-                p.extend_multi_path(glyph.transform(m))
+                glyph.transform_inplace(m)
+                glyph_paths.append(glyph)
             current_location += self.get_advance_width(shape_number) * sx
-        if not p.end.isclose((current_location, 0)):
-            p.move_to((current_location, 0))
-        return p
+        return glyph_paths
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/fonts/shapefile.py` & `ezdxf-1.1.0b4/src/ezdxf/fonts/shapefile.py`

 * *Files 2% similar despite different names*

```diff
@@ -611,43 +611,43 @@
     get_codes: Callable[[int], Sequence[int]],
     stacked: bool,
     start: UVec = (0, 0),
     reset_to_baseline=False,
 ) -> GlyphPath:
     """Renders multiple shapes into a single glyph path."""
     ctx = ShapeRenderer(
-        GlyphPath(start),
+        path.Path(start),
         pen_down=True,
         stacked=stacked,
         get_codes=get_codes,
     )
     for shape_number in shape_numbers:
         try:
             ctx.render(shape_number, reset_to_baseline=reset_to_baseline)
         except UnsupportedShapeNumber:
             pass
         except StackUnderflow:
             raise StackUnderflow(
                 f"stack underflow while rendering shape number {shape_number}"
             )
         # move cursor to the start of the next char???
-    return ctx.p
+    return GlyphPath(ctx.p)
 
 
 #        0, 1, 2,   3, 4,    5,  6,  7,  8,  9,  A,    B, C,   D, E, F
 VEC_X = [1, 1, 1, 0.5, 0, -0.5, -1, -1, -1, -1, -1, -0.5, 0, 0.5, 1, 1]
 #        0,   1, 2, 3, 4, 5, 6,   7, 8,    9,  A,  B,  C,  D,  E,    F
 VEC_Y = [0, 0.5, 1, 1, 1, 1, 1, 0.5, 0, -0.5, -1, -1, -1, -1, -1, -0.5]
 
 
 class ShapeRenderer:
     """Low level glyph renderer for SHX/SHP fonts."""
     def __init__(
         self,
-        p: GlyphPath,
+        p: path.Path,
         get_codes: Callable[[int], Sequence[int]],
         *,
         vector_length: float = 1.0,
         pen_down: bool = True,
         stacked: bool = False,
     ):
         self.p = p
@@ -656,15 +656,15 @@
         self.stacked = stacked  # vertical stacked text
         self._location_stack: list[Vec2] = []
         self._get_codes = get_codes
         self._baseline_y = self.p.start.y
 
     @property
     def current_location(self) -> Vec2:
-        return self.p.end
+        return Vec2(self.p.end)
 
     def push(self) -> None:
         self._location_stack.append(self.current_location)
 
     def pop(self) -> None:
         self.p.move_to(self._location_stack.pop())
 
@@ -942,50 +942,54 @@
 
     def get_empty_box(self) -> GlyphPath:
         glyph_A = self.get_shape(65)
         box = BoundingBox2d(glyph_A.control_vertices())
         height = box.size.y
         width = box.size.x
         start = glyph_A.start
-        p = GlyphPath(start)
+        p = path.Path(start)
         p.line_to(start + Vec2(width, 0))
         p.line_to(start + Vec2(width, height))
         p.line_to(start + Vec2(0, height))
         p.close()
         p.move_to(glyph_A.end)
-        return p
+        return GlyphPath(p)
 
     def _render_shape(self, shape_number) -> GlyphPath:
         ctx = ShapeRenderer(
-            GlyphPath(),
+            path.Path(),
             pen_down=True,
             stacked=False,
             get_codes=self.font.get_codes,
         )
         try:
             ctx.render(shape_number, reset_to_baseline=False)
         except StackUnderflow:
             pass
-        return ctx.p
+        return GlyphPath(ctx.p)
 
     def get_shape(self, shape_number: int) -> GlyphPath:
         try:
-            return self._glyph_cache[shape_number]
+            return self._glyph_cache[shape_number].clone()
         except KeyError:
             pass
         try:
             glyph = self._render_shape(shape_number)
         except UnsupportedShapeNumber:
             if shape_number < 32:
-                glyph = GlyphPath()
+                glyph = GlyphPath(None)
             else:
                 glyph = self.empty_box
         self._glyph_cache[shape_number] = glyph
-        self._advance_width_cache[shape_number] = glyph.end.x
-        return glyph
+        try:
+            width = glyph.end.x
+        except IndexError:
+            width = self.space_width
+        self._advance_width_cache[shape_number] = width
+        return glyph.clone()
 
     def get_advance_width(self, shape_number: int) -> float:
         if shape_number == 32:
             return self.space_width
         try:
             return self._advance_width_cache[shape_number]
         except KeyError:
@@ -1017,25 +1021,25 @@
 
     def get_text_length(
         self, text: str, cap_height: float, width_factor: float = 1.0
     ) -> float:
         scaling_factor = self.get_scaling_factor(cap_height) * width_factor
         return sum(self.get_advance_width(ord(c)) for c in text) * scaling_factor
 
-    def get_text_path(
-        self, text: str, cap_height: float, width_factor: float = 1.0
-    ) -> GlyphPath:
-        p = GlyphPath()
+    def get_text_glyph_paths(
+        self, text: str, cap_height: float = 1.0, width_factor: float = 1.0
+    ) -> list[GlyphPath]:
+        """Returns the glyph paths of string `s` as a list, scaled to cap height."""
+        glyph_paths: list[GlyphPath] = []
         sy = self.get_scaling_factor(cap_height)
         sx = sy * width_factor
         m = Matrix44.scale(sx, sy, 1)
         current_location = 0.0
         for c in text:
             shape_number = ord(c)
             if shape_number > 32:
                 glyph = self.get_shape(shape_number)
                 m[3, 0] = current_location
-                p.extend_multi_path(glyph.transform(m))
+                glyph.transform_inplace(m)
+                glyph_paths.append(glyph)
             current_location += self.get_advance_width(shape_number) * sx
-        if not p.end.isclose((current_location, 0)):
-            p.move_to((current_location, 0))
-        return p
+        return glyph_paths
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/fonts/ttfonts.py` & `ezdxf-1.1.0b4/src/ezdxf/fonts/ttfonts.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,32 +2,33 @@
 #  License: MIT License
 from __future__ import annotations
 from typing import Any, no_type_check
 from fontTools.pens.basePen import BasePen
 from fontTools.ttLib import TTFont
 
 from ezdxf.math import Matrix44, UVec, BoundingBox2d
+from ezdxf.path import Path
 from .font_manager import FontManager, UnsupportedFont
 from .font_measurements import FontMeasurements
 from .glyphs import GlyphPath, Glyphs
 
 UNICODE_WHITE_SQUARE = 9633  # U+25A1
 UNICODE_REPLACEMENT_CHAR = 65533  # U+FFFD
 
 font_manager = FontManager()
 
 
 class PathPen(BasePen):
     def __init__(self, glyph_set) -> None:
         super().__init__(glyph_set)
-        self._path = GlyphPath()
+        self._path = Path()
 
     @property
     def path(self) -> GlyphPath:
-        return self._path
+        return GlyphPath(self._path)
 
     def _moveTo(self, pt: UVec) -> None:
         self._path.move_to(pt)
 
     def _lineTo(self, pt: UVec) -> None:
         self._path.line_to(pt)
 
@@ -122,22 +123,22 @@
             generic_glyph = self.undefined_generic_glyph
         self._generic_glyph_cache[char] = generic_glyph
         return generic_glyph
 
     def get_glyph_path(self, char: str) -> GlyphPath:
         """Returns the raw glyph path, without any scaling applied."""
         try:
-            return self._glyph_path_cache[char]
+            return self._glyph_path_cache[char].clone()
         except KeyError:
             pass
         pen = PathPen(self.glyph_set)
         self.get_generic_glyph(char).draw(pen)
         glyph_path = pen.path
         self._glyph_path_cache[char] = glyph_path
-        return glyph_path
+        return glyph_path.clone()
 
     def get_glyph_width(self, char: str) -> float:
         """Returns the raw glyph width, without any scaling applied."""
         try:
             return self._glyph_width_cache[char]
         except KeyError:
             pass
@@ -145,19 +146,19 @@
         try:
             width = self.get_generic_glyph(char).width
         except KeyError:
             pass
         self._glyph_width_cache[char] = width
         return width
 
-    def get_text_path(
+    def get_text_glyph_paths(
         self, s: str, cap_height: float = 1.0, width_factor: float = 1.0
-    ) -> GlyphPath:
-        """Returns the concatenated glyph paths of string s, scaled to cap height."""
-        text_path = GlyphPath()
+    ) -> list[GlyphPath]:
+        """Returns the glyph paths of string `s` as a list, scaled to cap height."""
+        glyph_paths: list[GlyphPath] = []
         x_offset: float = 0
         requires_kerning = isinstance(self.kerning, KerningTable)
         resize_factor = self.get_scaling_factor(cap_height)
         y_factor = resize_factor
         x_factor = resize_factor * width_factor
         # set scaling factor:
         m = Matrix44.scale(x_factor, y_factor, 1.0)
@@ -166,22 +167,21 @@
         prev_char = ""
 
         for char in s:
             if requires_kerning:
                 x_offset += self.kerning.get(prev_char, char) * x_factor
             # set horizontal offset:
             m[3, 0] = x_offset
-            glyph_path = self.get_glyph_path(char).transform(m)
-            if x_offset == 0:
-                text_path = glyph_path
-            elif len(glyph_path):
-                text_path.extend_multi_path(glyph_path)
+            glyph_path = self.get_glyph_path(char)
+            glyph_path.transform_inplace(m)
+            if len(glyph_path):
+                glyph_paths.append(glyph_path)
             x_offset += self.get_glyph_width(char) * x_factor
             prev_char = char
-        return text_path
+        return glyph_paths
 
     def detect_space_width(self) -> float:
         """Returns the space width for the raw (unscaled) font."""
         return self.get_glyph_width(" ")
 
     def _get_text_length_with_kerning(self, s: str, cap_height: float = 1.0) -> float:
         length = 0.0
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/layouts/base.py` & `ezdxf-1.1.0b4/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.1.0b4/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/layouts/layout.py` & `ezdxf-1.1.0b4/src/ezdxf/layouts/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/layouts/layouts.py` & `ezdxf-1.1.0b4/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/const.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/loader.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/repair.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/tags.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/types.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/lldxf/validator.py` & `ezdxf-1.1.0b4/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/arc.py` & `ezdxf-1.1.0b4/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/bbox.py` & `ezdxf-1.1.0b4/src/ezdxf/math/bbox.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,9 +485,9 @@
             elif x > maxx:
                 maxx = x
             if y < miny:
                 miny = y
             elif y > maxy:
                 maxy = y
     if minx is None:
-        raise ValueError("No vertices give.")
+        raise ValueError("no vertices given")
     return Vec2(minx, miny), Vec2(maxx, maxy)
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/bezier.py` & `ezdxf-1.1.0b4/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.1.0b4/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/box.py` & `ezdxf-1.1.0b4/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/bspline.py` & `ezdxf-1.1.0b4/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/bulge.py` & `ezdxf-1.1.0b4/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/circle.py` & `ezdxf-1.1.0b4/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/clipping.py` & `ezdxf-1.1.0b4/src/ezdxf/math/clipping.py`

 * *Files 1% similar despite different names*

```diff
@@ -206,14 +206,19 @@
             self._bbox.extmin, self._bbox.extmax, start, end
         )
 
     def is_inside(self, point: Vec2) -> bool:
         """Returns ``True`` if `point` is inside the clipping rectangle."""
         return self._bbox.inside(point)
 
+    def has_intersection(self, other: BoundingBox2d) -> bool:
+        """Returns ``True`` if `other` bounding box intersects the clipping rectangle.
+        """
+        return self._bbox.has_intersection(other)
+
 
 def clip_polygon_2d(
     clip: Iterable[UVec],
     subject: Iterable[UVec],
     ccw_check: bool = True,
 ) -> Sequence[Vec2]:
     """Clip the `subject` polygon by the **convex** clipping polygon `clip`.
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/clustering.py` & `ezdxf-1.1.0b4/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/construct2d.py` & `ezdxf-1.1.0b4/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/construct3d.py` & `ezdxf-1.1.0b4/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/cspline.py` & `ezdxf-1.1.0b4/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/curvetools.py` & `ezdxf-1.1.0b4/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/ellipse.py` & `ezdxf-1.1.0b4/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.1.0b4/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/linalg.py` & `ezdxf-1.1.0b4/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/line.py` & `ezdxf-1.1.0b4/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/offset2d.py` & `ezdxf-1.1.0b4/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/parametrize.py` & `ezdxf-1.1.0b4/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/perlin.py` & `ezdxf-1.1.0b4/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/polyline.py` & `ezdxf-1.1.0b4/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/rtree.py` & `ezdxf-1.1.0b4/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/surfaces.py` & `ezdxf-1.1.0b4/src/ezdxf/math/surfaces.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/transformtools.py` & `ezdxf-1.1.0b4/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/triangulation.py` & `ezdxf-1.1.0b4/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/ucs.py` & `ezdxf-1.1.0b4/src/ezdxf/math/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.1.0b4/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.1.0b4/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/_bspline.py` & `ezdxf-1.1.0b4/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/_construct.py` & `ezdxf-1.1.0b4/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/_ctypes.py` & `ezdxf-1.1.0b4/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.1.0b4/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/_matrix44.py` & `ezdxf-1.1.0b4/src/ezdxf/math/_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/_vector.py` & `ezdxf-1.1.0b4/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/math/__init__.py` & `ezdxf-1.1.0b4/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/path/commands.py` & `ezdxf-1.1.0b4/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/path/converter.py` & `ezdxf-1.1.0b4/src/ezdxf/path/converter.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,15 +9,14 @@
     Optional,
     Callable,
     Type,
     TypeVar,
 )
 from typing_extensions import TypeAlias
 from functools import singledispatch, partial
-import enum
 from ezdxf.math import (
     ABS_TOL,
     Vec2,
     Vec3,
     NULLVEC,
     Z_AXIS,
     OCS,
@@ -54,15 +53,15 @@
     EdgePath,
     LineEdge,
     ArcEdge,
     EllipseEdge,
     SplineEdge,
 )
 from ezdxf.entities.polygon import DXFPolygon
-from .path import Path, AbstractPath, Path2d
+from .path import Path
 from .commands import Command
 from . import tools
 from .nesting import group_paths
 
 __all__ = [
     "make_path",
     "to_lines",
@@ -75,20 +74,14 @@
     "to_splines_and_polylines",
     "from_hatch",
     "from_hatch_ocs",
     "from_hatch_boundary_path",
     "from_hatch_edge_path",
     "from_hatch_polyline_path",
     "from_vertices",
-    "from_matplotlib_path",
-    "from_qpainter_path",
-    "to_matplotlib_path",
-    "to_qpainter_path",
-    "multi_path_from_matplotlib_path",
-    "multi_path_from_qpainter_path",
 ]
 
 MAX_DISTANCE = 0.01
 MIN_SEGMENTS = 4
 G1_TOL = 1e-4
 TPolygon = TypeVar("TPolygon", Hatch, MPolygon)
 BoundaryFactory = Callable[[BoundaryPaths, Path, int], None]
@@ -498,40 +491,40 @@
             path.line_to(vertex)
     if close:
         path.close()
     return path
 
 
 def to_lwpolylines(
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> Iterator[LWPolyline]:
     """Convert the given `paths` into :class:`~ezdxf.entities.LWPolyline`
     entities.
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
-        paths: iterable of :class:`Path` or :class:`Path2d` objects
+        paths: iterable of :class:`Path` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         extrusion: extrusion vector for all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of :class:`~ezdxf.entities.LWPolyline` objects
 
     """
-    if isinstance(paths, AbstractPath):
+    if isinstance(paths, Path):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
         return []
     extrusion = Vec3(extrusion)
     reference_point = Vec3(paths[0].start)
@@ -554,40 +547,40 @@
 def _get_ocs(extrusion: Vec3, reference_point: Vec3) -> tuple[OCS, float]:
     ocs = OCS(extrusion)
     elevation = ocs.from_wcs(reference_point).z  # type: ignore
     return ocs, elevation
 
 
 def to_polylines2d(
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> Iterator[Polyline]:
     """Convert the given `paths` into 2D :class:`~ezdxf.entities.Polyline`
     entities.
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
-        paths: iterable of :class:`Path` or :class:`Path2d` objects
+        paths: iterable of :class:`Path` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         extrusion: extrusion vector for all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of 2D :class:`~ezdxf.entities.Polyline` objects
 
     """
-    if isinstance(paths, AbstractPath):
+    if isinstance(paths, Path):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
         return []
     extrusion = Vec3(extrusion)
     reference_point = Vec3(paths[0].start)
@@ -605,15 +598,15 @@
             p = Polyline.new(dxfattribs=dxfattribs)
             p.append_vertices(path.flattening(distance, segments))
             p.new_seqend()
             yield p
 
 
 def to_hatches(
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     edge_path: bool = True,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     g1_tol: float = G1_TOL,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
@@ -623,15 +616,15 @@
     of LINE and SPLINE edges, as boundary paths for boundaries including curves.
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
-        paths: iterable of :class:`Path` or :class:`Path2d` objects
+        paths: iterable of :class:`Path` objects
         edge_path: ``True`` for edge paths build of LINE and SPLINE edges,
             ``False`` for only LWPOLYLINE paths as boundary paths
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve to flatten LWPOLYLINE paths
         g1_tol: tolerance for G1 continuity check to separate SPLINE edges
         extrusion: extrusion vector to all paths
         dxfattribs: additional DXF attribs
@@ -649,20 +642,20 @@
     else:
         # noinspection PyTypeChecker
         boundary_factory = partial(
             build_poly_path, distance=distance, segments=segments
         )
 
     yield from _polygon_converter(
-        Hatch, tools.to_3d_paths(paths), boundary_factory, extrusion, dxfattribs
+        Hatch, paths, boundary_factory, extrusion, dxfattribs
     )
 
 
 def to_mpolygons(
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> Iterator[MPolygon]:
     """Convert the given `paths` into :class:`~ezdxf.entities.MPolygon` entities.
@@ -671,15 +664,15 @@
 
     The `extrusion` vector is applied to all paths, all vertices are projected
     onto the plane normal to this extrusion vector. The default extrusion vector
     is the WCS z-axis. The plane elevation is the distance from the WCS origin
     to the start point of the first path.
 
     Args:
-        paths: iterable of :class:`Path` or :class:`Path2d` objects
+        paths: iterable of :class:`Path` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve to flatten LWPOLYLINE paths
         extrusion: extrusion vector to all paths
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of :class:`~ezdxf.entities.MPolygon` objects
@@ -689,15 +682,15 @@
     boundary_factory: BoundaryFactory = partial(
         build_poly_path, distance=distance, segments=segments
     )
     dxfattribs = dict(dxfattribs or {})
     dxfattribs.setdefault("fill_color", const.BYLAYER)  # type: ignore
 
     yield from _polygon_converter(
-        MPolygon, tools.to_3d_paths(paths), boundary_factory, extrusion, dxfattribs
+        MPolygon, paths, boundary_factory, extrusion, dxfattribs
     )
 
 
 def build_edge_path(
     boundaries: BoundaryPaths,
     path: Path,
     flags: int,
@@ -742,15 +735,15 @@
 def _polygon_converter(
     cls: Type[TPolygon],
     paths: Iterable[Path],
     add_boundary: BoundaryFactory,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> Iterator[TPolygon]:
-    if isinstance(paths, AbstractPath):
+    if isinstance(paths, Path):
         paths = [paths]
     else:
         paths = list(paths)
     if len(paths) == 0:
         return []
 
     extrusion = Vec3(extrusion)
@@ -778,66 +771,66 @@
         for hole in group[1:]:
             hole.close()
             add_boundary(boundaries, hole, 0)  # type: ignore
         yield polygon
 
 
 def to_polylines3d(
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> Iterator[Polyline]:
     """Convert the given `paths` into 3D :class:`~ezdxf.entities.Polyline`
     entities.
 
     Args:
-        paths: iterable of :class:`Path` or :class:`Path2d` objects
+        paths: iterable of :class:`Path` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of 3D :class:`~ezdxf.entities.Polyline` objects
 
     """
-    if isinstance(paths, AbstractPath):
+    if isinstance(paths, Path):
         paths = [paths]
 
     dxfattribs = dict(dxfattribs or {})
     dxfattribs["flags"] = const.POLYLINE_3D_POLYLINE
     for path in tools.single_paths(paths):  # type: ignore
         if len(path) > 0:
             p = Polyline.new(dxfattribs=dxfattribs)
             p.append_vertices(path.flattening(distance, segments))
             p.new_seqend()
             yield p
 
 
 def to_lines(
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> Iterator[Line]:
     """Convert the given `paths` into :class:`~ezdxf.entities.Line` entities.
 
     Args:
-        paths: iterable of :class:`Path` or :class:`Path2d` objects
+        paths: iterable of :class:`Path` objects
         distance:  maximum distance, see :meth:`Path.flattening`
         segments: minimum segment count per Bézier curve
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of :class:`~ezdxf.entities.Line` objects
 
     """
-    if isinstance(paths, AbstractPath):
+    if isinstance(paths, Path):
         paths = [paths]
     dxfattribs = dict(dxfattribs or {})
     prev_vertex = None
     for path in tools.single_paths(paths):  # type: ignore
         if len(path) == 0:
             continue
         for vertex in path.flattening(distance, segments):
@@ -850,23 +843,21 @@
             prev_vertex = vertex
         prev_vertex = None
 
 
 PathParts: TypeAlias = Union[BSpline, List[Vec3]]
 
 
-def to_bsplines_and_vertices(
-    path: Path | Path2d, g1_tol: float = G1_TOL
-) -> Iterator[PathParts]:
+def to_bsplines_and_vertices(path: Path, g1_tol: float = G1_TOL) -> Iterator[PathParts]:
     """Convert a :class:`Path` object into multiple cubic B-splines and
     polylines as lists of vertices. Breaks adjacent Bèzier without G1
     continuity into separated B-splines.
 
     Args:
-        path: :class:`Path` or :class:`Path2d` objects
+        path: :class:`Path` objects
         g1_tol: tolerance for G1 continuity check
 
     Returns:
         :class:`~ezdxf.math.BSpline` and lists of :class:`~ezdxf.math.Vec3`
 
     """
     from ezdxf.math import bezier_to_bspline
@@ -923,15 +914,15 @@
     if bezier:
         yield from to_bspline()
     if polyline:
         yield to_vertices()
 
 
 def to_splines_and_polylines(
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     g1_tol: float = G1_TOL,
     dxfattribs=None,
 ) -> Iterator[Union[Spline, Polyline]]:
     """Convert the given `paths` into :class:`~ezdxf.entities.Spline` and 3D
     :class:`~ezdxf.entities.Polyline` entities.
 
@@ -940,15 +931,15 @@
         g1_tol: tolerance for G1 continuity check
         dxfattribs: additional DXF attribs
 
     Returns:
         iterable of :class:`~ezdxf.entities.Line` objects
 
     """
-    if isinstance(paths, AbstractPath):
+    if isinstance(paths, Path):
         paths = [paths]
     dxfattribs = dict(dxfattribs or {})
 
     for path in tools.single_paths(paths):  # type: ignore
         for data in to_bsplines_and_vertices(path, g1_tol):
             if isinstance(data, BSpline):
                 spline = Spline.new(dxfattribs=dxfattribs)
@@ -957,219 +948,7 @@
             else:
                 attribs = dict(dxfattribs)
                 attribs["flags"] = const.POLYLINE_3D_POLYLINE
                 polyline = Polyline.new(dxfattribs=dxfattribs)
                 polyline.append_vertices(data)
                 polyline.new_seqend()
                 yield polyline
-
-
-# Interface to Matplotlib.path.Path
-
-
-@enum.unique
-class MplCmd(enum.IntEnum):
-    CLOSEPOLY = 79
-    CURVE3 = 3
-    CURVE4 = 4
-    LINETO = 2
-    MOVETO = 1
-    STOP = 0
-
-
-# TODO: return Path2d
-def multi_path_from_matplotlib_path(mpath, curves=True) -> Path:
-    """Returns a :class:`Path` object from a Matplotlib `Path`_
-    (`TextPath`_)  object. (requires Matplotlib). Returns a multi-path object
-    if necessary.
-
-    .. _TextPath: https://matplotlib.org/3.1.1/api/textpath_api.html
-    .. _Path: https://matplotlib.org/3.1.1/api/path_api.html#matplotlib.path.Path
-
-    """
-    path = Path()
-    current_polyline_start = Vec3()
-    for vertices, cmd in mpath.iter_segments(curves=curves):
-        cmd = MplCmd(cmd)
-        if cmd == MplCmd.MOVETO:
-            # vertices = [x0, y0]
-            current_polyline_start = Vec3(vertices)
-            path.move_to(vertices)
-        elif cmd == MplCmd.LINETO:
-            # vertices = [x0, y0]
-            path.line_to(vertices)
-        elif cmd == MplCmd.CURVE3:
-            # vertices = [x0, y0, x1, y1]
-            path.curve3_to(vertices[2:], vertices[0:2])
-        elif cmd == MplCmd.CURVE4:
-            # vertices = [x0, y0, x1, y1, x2, y2]
-            path.curve4_to(vertices[4:], vertices[0:2], vertices[2:4])
-        elif cmd == MplCmd.CLOSEPOLY:
-            # vertices = [0, 0]
-            if not path.end.isclose(current_polyline_start):
-                path.line_to(current_polyline_start)
-        elif cmd == MplCmd.STOP:  # not used
-            pass
-    return path
-
-
-# TODO: not used in ezdxf, remove?
-def from_matplotlib_path(mpath, curves=True) -> Iterator[Path]:
-    """Yields multiple :class:`Path` objects from a Matplotlib `Path`_
-    (`TextPath`_)  object. (requires Matplotlib)
-
-    .. _TextPath: https://matplotlib.org/3.1.1/api/textpath_api.html
-    .. _Path: https://matplotlib.org/3.1.1/api/path_api.html#matplotlib.path.Path
-
-    """
-    path = multi_path_from_matplotlib_path(mpath, curves=curves)
-    if path.has_sub_paths:
-        return path.sub_paths()
-    else:
-        return iter([path])
-
-
-def to_matplotlib_path(paths: Iterable[Path | Path2d], extrusion: UVec = Z_AXIS):
-    """Convert the given `paths` into a single :class:`matplotlib.path.Path` object.
-
-    The `extrusion` vector is applied to all paths, all vertices are projected
-    onto the plane normal to this extrusion vector.The default extrusion vector
-    is the WCS z-axis. The Matplotlib :class:`Path` is a 2D object with
-    :ref:`OCS` coordinates and the z-elevation is lost. (requires Matplotlib)
-
-    Args:
-        paths: iterable of :class:`Path` or :class:`Path2d` objects
-        extrusion: extrusion vector for all paths
-
-    Returns:
-        matplotlib `Path`_ in OCS!
-
-    """
-    from matplotlib.path import Path as MatplotlibPath
-
-    if not Z_AXIS.isclose(extrusion):
-        paths = tools.transform_paths_to_ocs(paths, OCS(extrusion))
-    else:
-        paths = list(paths)
-    if len(paths) == 0:  # type: ignore
-        raise ValueError("one or more paths required")
-
-    def add_command(code: MplCmd, point: Vec2 | Vec3):
-        codes.append(code)
-        vertices.append((point.x, point.y))
-
-    vertices: list[tuple[float, float]] = []
-    codes: list[MplCmd] = []
-    for path in paths:
-        add_command(MplCmd.MOVETO, path.start)
-        for cmd in path.commands():
-            if cmd.type == Command.LINE_TO:
-                add_command(MplCmd.LINETO, cmd.end)
-            elif cmd.type == Command.MOVE_TO:
-                add_command(MplCmd.MOVETO, cmd.end)
-            elif cmd.type == Command.CURVE3_TO:
-                add_command(MplCmd.CURVE3, cmd.ctrl)  # type: ignore
-                add_command(MplCmd.CURVE3, cmd.end)
-            elif cmd.type == Command.CURVE4_TO:
-                add_command(MplCmd.CURVE4, cmd.ctrl1)  # type: ignore
-                add_command(MplCmd.CURVE4, cmd.ctrl2)  # type: ignore
-                add_command(MplCmd.CURVE4, cmd.end)
-
-    # STOP command is currently not required
-    assert len(vertices) == len(codes)
-    return MatplotlibPath(vertices, codes)
-
-
-# Interface to QtGui.QPainterPath
-
-
-# TODO: return Path2d
-def multi_path_from_qpainter_path(qpath) -> Path:
-    """Returns a :class:`Path` objects from a `QPainterPath`_.
-    Returns a multi-path object if necessary. (requires Qt bindings)
-
-    .. _QPainterPath: https://doc.qt.io/qt-5/qpainterpath.html
-
-    """
-    # QPainterPath stores only cubic Bèzier curves
-    path = Path()
-    vertices: list[Vec3] = []
-    for index in range(qpath.elementCount()):
-        element = qpath.elementAt(index)
-        cmd = element.type
-        v = Vec3(element.x, element.y)
-
-        if cmd == 0:  # MoveTo
-            assert len(vertices) == 0
-            path.move_to(v)
-        elif cmd == 1:  # LineTo
-            assert len(vertices) == 0
-            path.line_to(v)
-        elif cmd == 2:  # CurveTo
-            assert len(vertices) == 0
-            vertices.append(v)
-        elif cmd == 3:  # CurveToDataElement
-            if len(vertices) == 2:
-                path.curve4_to(v, vertices[0], vertices[1])
-                vertices.clear()
-            else:
-                vertices.append(v)
-    return path
-
-
-# TODO: not used in ezdxf, remove?
-def from_qpainter_path(qpath) -> Iterator[Path]:
-    """Yields multiple :class:`Path` objects from a `QPainterPath`_.
-    (requires Qt bindings)
-
-    .. _QPainterPath: https://doc.qt.io/qt-5/qpainterpath.html
-
-    """
-    # QPainterPath stores only cubic Bèzier curves
-    path = multi_path_from_qpainter_path(qpath)
-    if path.has_sub_paths:
-        return path.sub_paths()
-    else:
-        return iter([path])
-
-
-def to_qpainter_path(paths: Iterable[Path | Path2d], extrusion: UVec = Z_AXIS):
-    """Convert the given `paths` into a :class:`QtGui.QPainterPath` object.
-
-    The `extrusion` vector is applied to all paths, all vertices are projected
-    onto the plane normal to this extrusion vector. The default extrusion vector
-    is the WCS z-axis. The :class:`QPainterPath` is a 2D object with :ref:`OCS`
-    coordinates and the z-elevation is lost. (requires Qt bindings)
-
-    Args:
-        paths: iterable of :class:`Path` objects
-        extrusion: extrusion vector for all paths
-
-    Returns:
-        `QPainterPath`_ in OCS!
-
-    """
-    from ezdxf.addons.xqt import QPainterPath, QPointF
-
-    if not Z_AXIS.isclose(extrusion):
-        paths = tools.transform_paths_to_ocs(paths, OCS(extrusion))
-    else:
-        paths = list(paths)
-    if len(paths) == 0:  # type: ignore
-        raise ValueError("one or more paths required")
-
-    def qpnt(v: Vec2 | Vec3):
-        return QPointF(v.x, v.y)
-
-    qpath = QPainterPath()
-    for path in paths:
-        qpath.moveTo(qpnt(path.start))
-        for cmd in path.commands():
-            if cmd.type == Command.LINE_TO:
-                qpath.lineTo(qpnt(cmd.end))
-            elif cmd.type == Command.MOVE_TO:
-                qpath.moveTo(qpnt(cmd.end))
-            elif cmd.type == Command.CURVE3_TO:
-                qpath.quadTo(qpnt(cmd.ctrl), qpnt(cmd.end))  # type: ignore
-            elif cmd.type == Command.CURVE4_TO:
-                qpath.cubicTo(qpnt(cmd.ctrl1), qpnt(cmd.ctrl2), qpnt(cmd.end))  # type: ignore
-    return qpath
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/path/nesting.py` & `ezdxf-1.1.0b4/src/ezdxf/path/nesting.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,38 +3,37 @@
 """
 This module provides "nested Polygon" detection for multiple paths.
 
 Terminology
 -----------
 
 exterior
-    creates a filled area, has counter-clockwise (ccw) winding in matplotlib
+    creates a filled area, has counter-clockwise (ccw) winding
     exterior := Path
 
 hole
-    creates an unfilled area, has clockwise winding (cw) in matplotlib,
+    creates an unfilled area, has clockwise winding (cw),
     hole := Polygon
 
 polygon
     list of nested paths:
     polygon without a hole: [path]
     polygon with 1 hole: [path, [path]]
     polygon with 2 separated holes: [path, [path], [path]]
     polygon with 2 nested holes: [path, [path, [path]]]
 
-    polygon := [exterior, hole*]
+    polygon := [exterior, *hole]
 
 The result is a list of polygons:
 
 1 polygon returns: [[ext-path]]
 2 separated polygons returns: [[ext-path], [ext-path, [hole-path]]]
 
-A hole is just another polygon, for a correct visualisation in
-matplotlib the winding of the nested paths have to follow the alternating
-order ccw-cw-ccw-cw... :
+A hole is just another polygon, some render backends may require a distinct winding
+order for nested paths like: ccw-cw-ccw-cw...
 
 [Exterior-ccw,
     [Hole-Exterior-cw,
         [Sub-Hole-ccw],
         [Sub-Hole-ccw],
     ],
     [Hole-Exterior-cw],
@@ -44,103 +43,85 @@
 The implementation has to do some expensive tests, like check if a path is
 inside of another path or if paths do overlap. A goal is to reduce this costs
 by using proxy objects:
 
 Bounding Box Proxy
 ------------------
 
-Use the bounding box, this is very fast but not accurate, but could handle
-most of the real world scenarios, in the assumption that most HATCHES are
-created from non-overlapping boundary paths.
+This implementation uses the bounding box of the path as proxy object, this is very fast
+but not accurate, but can handle most of the real world scenarios, in the assumption
+that most HATCHES are created from non-overlapping boundary paths.
 Overlap detection and resolving is not possible.
 
-Bounding Box Construction:
-- Fast: use bounding box from control vertices
-- Accurate: use bounding box from flattened curve
-
-Inside Check:
-- Fast: center point of the bounding box
-- Slow: use all corner points of the bounding box
-
-
-Convex Hull Proxy
------------------
-
-Use the convex hull of the path, this is more accurate but also
-much slower. Overlap detection and resolving is not possible.
-
-Convex Hull construction:
-- Fast: use convex hull from control vertices
-- Accurate: use convex hull from flattened curve
-
-Inside Check:
-- Fast: center point of convex hull
-- Slow: use all points of the convex hull
-
-
-Flattened Curve
----------------
-
-Use the flattened curve vertices, this is the most accurate solution and also
-the slowest. Overlap detection and resolving is possible: exterior is the
-union of two overlapping paths, hole is the intersection of this two paths,
-the hole vertices have to be subtracted from the exterior vertices.
+The input paths have to implement the SupportsBoundingBox protocol, which requires
+only a method bbox() that returns a BoundingBox2d instance for the path.
 
 Sort by Area
 ------------
 
 It is not possible for a path to contain another path with a larger area.
 
 """
 from __future__ import annotations
-from typing import Tuple, Optional, List, Iterable
+from typing import (
+    Tuple,
+    Optional,
+    List,
+    Iterable,
+    Sequence,
+    Iterator,
+    TypeVar,
+)
 from typing_extensions import TypeAlias
 from collections import namedtuple
-from .path import AbstractPath
-from ezdxf.math import BoundingBox2d
+from ezdxf.math import AbstractBoundingBox
+from ezdxf.protocols import SupportsBoundingBox
+
 
 __all__ = [
-    "fast_bbox_detection",
+    "make_polygon_structure",
     "winding_deconstruction",
     "group_paths",
     "flatten_polygons",
 ]
 
-Exterior: TypeAlias = AbstractPath
-Polygon: TypeAlias = Tuple[Exterior, Optional[List["Polygon"]]]
+
+T = TypeVar("T", bound=SupportsBoundingBox)
+
+Polygon: TypeAlias = Tuple[T, Optional[List["Polygon"]]]
 BoxStruct = namedtuple("BoxStruct", "bbox, path")
 
 
-def fast_bbox_detection(paths: Iterable[AbstractPath]) -> list[Polygon]:
-    """Create a nested polygon structure from iterable `paths`, using 2D
+def make_polygon_structure(paths: Iterable[T]) -> list[Polygon]:
+    """Returns a recursive polygon structure from iterable `paths`, uses 2D
     bounding boxes as fast detection objects.
 
     """
 
     # Implements fast bounding box construction and fast inside check.
     def area(item: BoxStruct) -> float:
-        width, height = item.bbox.size
-        return width * height
+        size = item.bbox.size
+        return size.x * size.y
 
     def separate(
-        exterior: BoundingBox2d, candidates: list[BoxStruct]
+        exterior: AbstractBoundingBox, candidates: list[BoxStruct]
     ) -> tuple[list[BoxStruct], list[BoxStruct]]:
         holes: list[BoxStruct] = []
         outside: list[BoxStruct] = []
         for candidate in candidates:
             # Fast inside check:
             (holes if exterior.inside(candidate.bbox.center) else outside).append(
                 candidate
             )
         return holes, outside
 
     def polygon_structure(outside: list[BoxStruct]) -> list[list]:
         polygons = []
         while outside:
-            exterior = outside.pop()  # path with largest area
+            exterior = outside.pop()  # path with the largest area
             # Get holes inside of exterior and returns the remaining paths
             # outside of exterior:
             holes, outside = separate(exterior.bbox, outside)
             if holes:
                 # build nested hole structure:
                 # the largest hole could contain the smaller holes,
                 # and so on ...
@@ -150,56 +131,55 @@
 
     def as_nested_paths(polygons) -> list:
         return [
             polygon.path if isinstance(polygon, BoxStruct) else as_nested_paths(polygon)
             for polygon in polygons
         ]
 
-    boxed_paths = [
-        # Fast bounding box construction:
-        BoxStruct(BoundingBox2d(path.control_vertices()), path)
-        for path in paths
-        if len(path)
-    ]
+    boxed_paths = []
+    for path in paths:
+        bbox = path.bbox()
+        if bbox.has_data:
+            boxed_paths.append(BoxStruct(bbox, path))
     boxed_paths.sort(key=area)
     return as_nested_paths(polygon_structure(boxed_paths))
 
 
 def winding_deconstruction(
     polygons: list[Polygon],
-) -> tuple[list[AbstractPath], list[AbstractPath]]:
+) -> tuple[list[T], list[T]]:
     """Flatten the nested polygon structure in a tuple of two lists,
     the first list contains the paths which should be counter-clockwise oriented
     and the second list contains the paths which should be clockwise oriented.
 
     The paths are not converted to this orientation.
 
     """
 
     def deconstruct(polygons_, level):
         for polygon in polygons_:
-            if isinstance(polygon, AbstractPath):
+            if isinstance(polygon, Sequence):
+                deconstruct(polygon, level + 1)
+            else:
                 # level 0 is the list of polygons
                 # level 1 = ccw, 2 = cw, 3 = ccw, 4 = cw, ...
-                (ccw_paths if (level % 2) else cw_paths).append(polygon)  # type:ignore
-            else:
-                deconstruct(polygon, level + 1)
+                (ccw_paths if (level % 2) else cw_paths).append(polygon)
 
-    cw_paths: list[AbstractPath] = []
-    ccw_paths: list[AbstractPath] = []
+    cw_paths: list[T] = []
+    ccw_paths: list[T] = []
     deconstruct(polygons, 0)
     return ccw_paths, cw_paths
 
 
-def flatten_polygons(polygons: Polygon) -> Iterable[AbstractPath]:
+def flatten_polygons(polygons: Polygon) -> Iterator[T]:
     """Yield a flat representation of the given nested polygons."""
-    for polygon in polygons:  # type: ignore
-        if isinstance(polygon, AbstractPath):
-            yield polygon
-        else:
+    for polygon in polygons:
+        if isinstance(polygon, Sequence):
             yield from flatten_polygons(polygon)  # type: ignore
+        else:
+            yield polygon  # T
 
 
-def group_paths(paths: Iterable[AbstractPath]) -> list[list[AbstractPath]]:
+def group_paths(paths: Iterable[T]) -> list[list[T]]:
     """Group separated paths and their inner holes as flat lists."""
-    polygons = fast_bbox_detection(paths)  # type: ignore
+    polygons = make_polygon_structure(paths)
     return [list(flatten_polygons(polygon)) for polygon in polygons]
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/path/path.py` & `ezdxf-1.1.0b4/src/ezdxf/path/path.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,77 +1,93 @@
 # Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-import abc
 from typing import (
     Optional,
     Iterator,
+    Iterable,
     Any,
-    TypeVar,
-    Type,
-    Generic,
     Callable,
-    Sequence,
 )
 from typing_extensions import Self
 from ezdxf.math import (
     Vec3,
-    Vec2,
     NULLVEC,
     OCS,
     Bezier3P,
     Bezier4P,
     Matrix44,
     has_clockwise_orientation,
     UVec,
+    BoundingBox,
 )
 
 from .commands import (
     Command,
     LineTo,
     MoveTo,
     Curve3To,
     Curve4To,
-    AnyCurve,
     PathElement,
 )
 
-__all__ = ["AbstractPath", "Path", "Path2d"]
+__all__ = ["Path"]
 
 MAX_DISTANCE = 0.01
 MIN_SEGMENTS = 4
 G1_TOL = 1e-4
-
-T = TypeVar("T", Vec2, Vec3)
-
 _slots = ("_vertices", "_start_index", "_commands", "_has_sub_paths", "_user_data")
 
 
-class AbstractPath(Generic[T], abc.ABC):
+class Path:
     __slots__ = _slots
-    _pnt_class: Type[T]
 
     def __init__(self, start: UVec = NULLVEC):
         # stores all command vertices in a contiguous list:
-        self._vertices: list[T] = [self._pnt_class(start)]
+        self._vertices: list[Vec3] = [Vec3(start)]
         # start index of each command
         self._start_index: list[int] = []
         self._commands: list[Command] = []
         self._has_sub_paths = False
         self._user_data: Any = None  # should be immutable data!
 
-    @abc.abstractmethod
+    @classmethod
+    def from_vertices_and_commands(
+        cls, vertices: list[Vec3], command_codes: list[Command], user_data: Any = None
+    ) -> Self:
+        """Create path instances from a list of vertices and a list of commands."""
+        # Used for fast conversion from NumpyPath2d to Path.
+        # This is "hacky" but also 8x faster than the correct way using only public
+        # methods and properties.
+        new_path = cls()
+        if len(vertices) == 0:
+            return new_path
+        new_path._vertices = vertices
+        new_path._commands = command_codes
+        new_path._start_index = make_vertex_index(command_codes)
+        new_path._has_sub_paths = any(cmd == Command.MOVE_TO for cmd in command_codes)
+        new_path._user_data = user_data
+        return new_path
+
     def transform(self, m: Matrix44) -> Self:
         """Returns a new transformed path.
 
         Args:
              m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
 
         """
-        ...
+        new_path = self.clone()
+        new_path._vertices = list(m.transform_vertices(self._vertices))
+        return new_path
+
+    def bbox(self) -> BoundingBox:
+        """Returns the bounding box of all control vertices as
+        :class:`~ezdxf.math.BoundingBox` instance.
+        """
+        return BoundingBox(self.control_vertices())
 
     def __len__(self) -> int:
         """Returns count of path elements."""
         return len(self._commands)
 
     def __getitem__(self, item) -> PathElement:
         """Returns the path element at given index, slicing is not supported."""
@@ -105,15 +121,15 @@
         """Returns a new copy of :class:`Path` with shared immutable data."""
         copy = self.__class__()
         # vertices itself are immutable - no copying required
         copy._vertices = self._vertices.copy()
         self._copy_properties(copy)
         return copy
 
-    def _copy_properties(self, clone: AbstractPath) -> None:
+    def _copy_properties(self, clone: Path) -> None:
         assert len(self._vertices) == len(clone._vertices)
         clone._commands = self._commands.copy()
         clone._start_index = self._start_index.copy()
         clone._has_sub_paths = self._has_sub_paths
         # copy by reference: user data should be immutable data!
         clone._user_data = self._user_data
 
@@ -128,33 +144,33 @@
         return self._user_data
 
     @user_data.setter
     def user_data(self, data: Any):
         self._user_data = data
 
     @property
-    def start(self) -> T:
+    def start(self) -> Vec3:
         """:class:`Path` start point, resetting the start point of an empty
         path is possible.
         """
         return self._vertices[0]
 
     @start.setter
     def start(self, location: UVec) -> None:
         if self._commands:
             raise ValueError("Requires an empty path.")
         else:
-            self._vertices[0] = self._pnt_class(location)
+            self._vertices[0] = Vec3(location)
 
     @property
-    def end(self) -> T:
+    def end(self) -> Vec3:
         """:class:`Path` end point."""
         return self._vertices[-1]
 
-    def control_vertices(self) -> list[T]:
+    def control_vertices(self) -> list[Vec3]:
         """Yields all path control vertices in consecutive order."""
         if self._commands:
             return list(self._vertices)
         return []
 
     def command_codes(self) -> list[int]:
         """Internal API."""
@@ -167,24 +183,26 @@
         if len(vertices) > 1:
             return vertices[0].isclose(vertices[-1])
         return False
 
     @property
     def has_lines(self) -> bool:
         """Returns ``True`` if the path has any line segments."""
-        return any(cmd == Command.LINE_TO for cmd in self._commands)
+        return Command.LINE_TO in self._commands
 
     @property
     def has_curves(self) -> bool:
         """Returns ``True`` if the path has any curve segments."""
-        return any(cmd in AnyCurve for cmd in self._commands)
+        return (
+            Command.CURVE4_TO in self._commands or Command.CURVE3_TO in self._commands
+        )
 
     @property
     def has_sub_paths(self) -> bool:
-        """Returns ``True`` if the path is a :term:`Multi-Path` object which
+        """Returns ``True`` if the path is a :term:`Multi-Path` object that
         contains multiple sub-paths.
 
         """
         return self._has_sub_paths
 
     def has_clockwise_orientation(self) -> bool:
         """Returns ``True`` if 2D path has clockwise orientation, ignores
@@ -212,55 +230,54 @@
         else:
             raise ValueError(f"Invalid command: {t}")
 
     def line_to(self, location: UVec) -> None:
         """Add a line from actual path end point to `location`."""
         self._commands.append(Command.LINE_TO)
         self._start_index.append(len(self._vertices))
-        self._vertices.append(self._pnt_class(location))
+        self._vertices.append(Vec3(location))
 
     def move_to(self, location: UVec) -> None:
         """Start a new sub-path at `location`. This creates a gap between the
         current end-point and the start-point of the new sub-path. This converts
         the instance into a :term:`Multi-Path` object.
 
         If the :meth:`move_to` command is the first command, the start point of
         the path will be reset to `location`.
 
         """
         commands = self._commands
         if not commands:
-            self._vertices[0] = self._pnt_class(location)
+            self._vertices[0] = Vec3(location)
             return
         self._has_sub_paths = True
         if commands[-1] == Command.MOVE_TO:
             # replace last move to command
             commands.pop()
             self._vertices.pop()
             self._start_index.pop()
         commands.append(Command.MOVE_TO)
         self._start_index.append(len(self._vertices))
-        self._vertices.append(self._pnt_class(location))
+        self._vertices.append(Vec3(location))
 
     def curve3_to(self, location: UVec, ctrl: UVec) -> None:
         """Add a quadratic Bèzier-curve from actual path end point to
         `location`, `ctrl` is the control point for the quadratic Bèzier-curve.
         """
         self._commands.append(Command.CURVE3_TO)
         self._start_index.append(len(self._vertices))
-        self._vertices.extend((self._pnt_class(ctrl), self._pnt_class(location)))
+        self._vertices.extend((Vec3(ctrl), Vec3(location)))
 
     def curve4_to(self, location: UVec, ctrl1: UVec, ctrl2: UVec) -> None:
         """Add a cubic Bèzier-curve from actual path end point to `location`,
         `ctrl1` and `ctrl2` are the control points for the cubic Bèzier-curve.
         """
         self._commands.append(Command.CURVE4_TO)
         self._start_index.append(len(self._vertices))
-        pnt = self._pnt_class
-        self._vertices.extend((pnt(ctrl1), pnt(ctrl2), pnt(location)))
+        self._vertices.extend((Vec3(ctrl1), Vec3(ctrl2), Vec3(location)))
 
     def close(self) -> None:
         """Close path by adding a line segment from the end point to the start
         point.
         """
         if not self.is_closed:
             self.line_to(self.start)
@@ -276,27 +293,27 @@
                 start_point is not None
             ), "internal error: required MOVE_TO command not found"
             if not self.end.isclose(start_point):
                 self.line_to(start_point)
         else:
             self.close()
 
-    def _start_of_last_sub_path(self) -> Optional[T]:
+    def _start_of_last_sub_path(self) -> Optional[Vec3]:
         move_to = Command.MOVE_TO
         commands = self._commands
         index = len(commands) - 1
         # The first command at index 0 is never MOVE_TO!
         while index > 0:
             if commands[index] == move_to:
                 return self._vertices[self._start_index[index]]
             index -= 1
         return None
 
     def reversed(self) -> Self:
-        """Returns a new :class:`Path` with reversed segments and control
+        """Returns a new :class:`Path` with reversed commands and control
         vertices.
 
         """
         path = self.clone()
         if not path._commands:
             return path
         if path._commands[-1] == Command.MOVE_TO:
@@ -308,32 +325,17 @@
             path._vertices.pop()
             path._start_index.pop()
             path._has_sub_paths = any(  # is still a multi-path?
                 cmd == Command.MOVE_TO for cmd in path._commands
             )
         path._commands.reverse()
         path._vertices.reverse()
-        path._reindex()
+        path._start_index = make_vertex_index(path._commands)
         return path
 
-    def _reindex(self) -> None:
-        start = 1
-        start_index = self._start_index
-        for index, cmd in enumerate(self._commands):
-            start_index[index] = start
-            # ordered by common usage:
-            if cmd == Command.LINE_TO:
-                start += 1
-            elif cmd == Command.CURVE4_TO:
-                start += 3
-            elif cmd == Command.CURVE3_TO:
-                start += 2
-            elif cmd == Command.MOVE_TO:
-                start += 1
-
     def clockwise(self) -> Self:
         """Returns new :class:`Path` in clockwise orientation.
 
         Raises:
             TypeError: can't detect orientation of a :term:`Multi-Path` object
 
         """
@@ -351,30 +353,35 @@
         """
 
         if self.has_clockwise_orientation():
             return self.reversed()
         else:
             return self.clone()
 
-    @abc.abstractmethod
-    def approximate(self, segments: int = 20) -> Iterator[T]:
+    def approximate(self, segments: int = 20) -> Iterator[Vec3]:
         """Approximate path by vertices, `segments` is the count of
         approximation segments for each Bézier curve.
 
         Does not yield any vertices for empty paths, where only a start point
         is present!
 
         Approximation of :term:`Multi-Path` objects is possible, but gaps are
         indistinguishable from line segments.
 
         """
-        ...
 
-    @abc.abstractmethod
-    def flattening(self, distance: float, segments: int = 16) -> Iterator[T]:
+        def curve3(p0: Vec3, p1: Vec3, p2: Vec3) -> Iterator[Vec3]:
+            return iter(Bezier3P((p0, p1, p2)).approximate(segments))
+
+        def curve4(p0: Vec3, p1: Vec3, p2: Vec3, p3: Vec3) -> Iterator[Vec3]:
+            return iter(Bezier4P((p0, p1, p2, p3)).approximate(segments))
+
+        return self._approximate(curve3, curve4)
+
+    def flattening(self, distance: float, segments: int = 4) -> Iterator[Vec3]:
         """Approximate path by vertices and use adaptive recursive flattening
         to approximate Bèzier curves. The argument `segments` is the
         minimum count of approximation segments for each curve, if the distance
         from the center of the approximation segment to the curve is bigger than
         `distance` the segment will be subdivided.
 
         Does not yield any vertices for empty paths, where only a start point
@@ -386,17 +393,28 @@
         Args:
             distance: maximum distance from the center of the curve to the
                 center of the line segment between two approximation points to
                 determine if a segment should be subdivided.
             segments: minimum segment count per Bézier curve
 
         """
-        ...
 
-    def _approximate(self, curve3: Callable, curve4: Callable) -> Iterator[T]:
+        def curve3(p0: Vec3, p1: Vec3, p2: Vec3) -> Iterator[Vec3]:
+            if distance == 0.0:
+                raise ValueError(f"invalid max distance: 0.0")
+            return iter(Bezier3P((p0, p1, p2)).flattening(distance, segments))
+
+        def curve4(p0: Vec3, p1: Vec3, p2: Vec3, p3: Vec3) -> Iterator[Vec3]:
+            if distance == 0.0:
+                raise ValueError(f"invalid max distance: 0.0")
+            return iter(Bezier4P((p0, p1, p2, p3)).flattening(distance, segments))
+
+        return self._approximate(curve3, curve4)
+
+    def _approximate(self, curve3: Callable, curve4: Callable) -> Iterator[Vec3]:
         if not self._commands:
             return
 
         start = self._vertices[0]
         yield start
 
         vertices = self._vertices
@@ -416,25 +434,22 @@
                 yield from pts
             else:
                 raise ValueError(f"Invalid command: {cmd}")
             start = end_location
 
     def to_wcs(self, ocs: OCS, elevation: float) -> None:
         """Transform path from given `ocs` to WCS coordinates inplace."""
-        # Important: requires a 3D path otherwise would change the type of path
-        if self._pnt_class is not Vec3:
-            raise TypeError("Not supported by 2D paths.")
         self._vertices = list(
             ocs.to_wcs(v.replace(z=elevation)) for v in self._vertices
         )
 
     def sub_paths(self) -> Iterator[Self]:
-        """Yield sub-path as :term:`Single-Path` objects.
+        """Yield all sub-paths as :term:`Single-Path` objects.
 
-        It is safe to call :meth:`sub_paths` on any path-type:
+        It's safe to call :meth:`sub_paths` on any path-type:
         :term:`Single-Path`, :term:`Multi-Path` and :term:`Empty-Path`.
 
         """
         path = self.__class__(start=self.start)
         path._user_data = self._user_data
         move_to = Command.MOVE_TO
         for cmd in self.commands():
@@ -442,27 +457,27 @@
                 yield path
                 path = self.__class__(start=cmd.end)
                 path._user_data = self._user_data
             else:
                 path.append_path_element(cmd)
         yield path
 
-    def extend_multi_path(self, path: AbstractPath[T]) -> None:
+    def extend_multi_path(self, path: Path) -> None:
         """Extend the path by another path. The source path is automatically a
         :term:`Multi-Path` object, even if the previous end point matches the
         start point of the appended path. Ignores paths without any commands
         (empty paths).
 
         """
         if len(path):
             self.move_to(path.start)
             for cmd in path.commands():
                 self.append_path_element(cmd)
 
-    def append_path(self, path: AbstractPath[T]) -> None:
+    def append_path(self, path: Path) -> None:
         """Append another path to this path. Adds a :code:`self.line_to(path.start)`
         if the end of this path != the start of appended path.
 
         """
         if len(path) == 0:
             return  # do not append an empty path
         if self._commands:
@@ -470,104 +485,23 @@
                 self.line_to(path.start)
         else:
             self.start = path.start
         for cmd in path.commands():
             self.append_path_element(cmd)
 
 
-class Path(AbstractPath[Vec3]):
-    __slots__ = _slots
-    _pnt_class = Vec3
-
-    def approximate(self, segments: int = 20) -> Iterator[Vec3]:
-        def curve3(p0: T, p1: T, p2: T) -> Iterator[Vec3]:
-            return iter(Bezier3P((p0, p1, p2)).approximate(segments))
-
-        def curve4(p0: T, p1: T, p2: T, p3: T) -> Iterator[Vec3]:
-            return iter(Bezier4P((p0, p1, p2, p3)).approximate(segments))
-
-        return self._approximate(curve3, curve4)
-
-    def flattening(self, distance: float, segments: int = 16) -> Iterator[Vec3]:
-        def curve3(p0: T, p1: T, p2: T) -> Iterator[Vec3]:
-            if distance == 0.0:
-                raise ValueError(f"invalid max distance: 0.0")
-            return iter(Bezier3P((p0, p1, p2)).flattening(distance, segments))
-
-        def curve4(p0: T, p1: T, p2: T, p3: T) -> Iterator[Vec3]:
-            if distance == 0.0:
-                raise ValueError(f"invalid max distance: 0.0")
-            return iter(Bezier4P((p0, p1, p2, p3)).flattening(distance, segments))
-
-        return self._approximate(curve3, curve4)
-
-    def to_2d_path(self) -> Path2d:
-        """Returns a new 2D path. The conversion is almost as fast as a copy.
-
-        .. versionadded:: 1.1
-
-        """
-        path2d = Path2d()
-        path2d._vertices = Vec2.list(self._vertices)
-        self._copy_properties(path2d)
-        return path2d
-
-    def transform(self, m: Matrix44) -> Self:
-        """Returns a new transformed 3D path.
-
-        Args:
-             m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
-
-        """
-        new_path = self.clone()
-        new_path._vertices = list(m.transform_vertices(self._vertices))
-        return new_path
-
-
-class Path2d(AbstractPath[Vec2]):
-    __slots__ = _slots
-    _pnt_class = Vec2
-
-    def approximate(self, segments: int = 20) -> Iterator[Vec2]:
-        def curve3(p0: T, p1: T, p2: T) -> Iterator[Vec2]:
-            return Vec2.generate(Bezier3P((p0, p1, p2)).approximate(segments))
-
-        def curve4(p0: T, p1: T, p2: T, p3: T) -> Iterator[Vec2]:
-            return Vec2.generate(Bezier4P((p0, p1, p2, p3)).approximate(segments))
-
-        return self._approximate(curve3, curve4)
-
-    def flattening(self, distance: float, segments: int = 16) -> Iterator[Vec2]:
-        def curve3(p0: T, p1: T, p2: T) -> Iterator[Vec2]:
-            if distance == 0.0:
-                raise ValueError(f"invalid max distance: 0.0")
-            return Vec2.generate(Bezier3P((p0, p1, p2)).flattening(distance, segments))
-
-        def curve4(p0: T, p1: T, p2: T, p3: T) -> Iterator[Vec2]:
-            if distance == 0.0:
-                raise ValueError(f"invalid max distance: 0.0")
-            return Vec2.generate(
-                Bezier4P((p0, p1, p2, p3)).flattening(distance, segments)
-            )
-
-        return self._approximate(curve3, curve4)
-
-    def to_3d_path(self, elevation: float = 0.0) -> Path:
-        """Returns a new 3D path, the z-axis of all vertices is set to `elevation`.
-        The conversion is almost as fast as a copy.
-        """
-        path3d = Path()
-        elevation = float(elevation)
-        path3d._vertices = [Vec3(v.x, v.y, elevation) for v in self._vertices]
-        self._copy_properties(path3d)
-        return path3d
-
-    def transform(self, m: Matrix44) -> Self:
-        """Returns a new transformed 2D path.
-
-        Args:
-             m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
-
-        """
-        new_path = self.clone()
-        new_path._vertices = list(m.fast_2d_transform(self._vertices))
-        return new_path
+CMD_SIZE = {
+    Command.MOVE_TO: 1,
+    Command.LINE_TO: 1,
+    Command.CURVE3_TO: 2,
+    Command.CURVE4_TO: 3,
+}
+
+
+def make_vertex_index(command_codes: Iterable[Command]) -> list[int]:
+    cmd_size = CMD_SIZE
+    start: int = 1
+    start_index: list[int] = []
+    for code in command_codes:
+        start_index.append(start)
+        start += cmd_size[code]
+    return start_index
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/path/shapes.py` & `ezdxf-1.1.0b4/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/path/tools.py` & `ezdxf-1.1.0b4/src/ezdxf/path/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     cubic_bezier_arc_parameters,
     cubic_bezier_bbox,
     quadratic_bezier_bbox,
 )
 from ezdxf.math.triangulation import mapbox_earcut_2d
 from ezdxf.query import EntityQuery
 
-from .path import Path, Path2d, AbstractPath
+from .path import Path
 from .commands import Command
 from . import converter, nesting
 
 if TYPE_CHECKING:
     from ezdxf.query import EntityQuery
     from ezdxf.eztypes import GenericLayoutType
 
@@ -60,15 +60,14 @@
     "render_splines_and_polylines",
     "add_bezier4p",
     "add_bezier3p",
     "add_ellipse",
     "add_2d_polyline",
     "add_spline",
     "to_multi_path",
-    "to_3d_paths",
     "single_paths",
     "have_close_control_vertices",
     "lines_to_curve3",
     "lines_to_curve4",
     "fillet",
     "polygonal_fillet",
     "chamfer",
@@ -78,74 +77,61 @@
 ]
 
 MAX_DISTANCE = 0.01
 MIN_SEGMENTS = 4
 G1_TOL = 1e-4
 IS_CLOSE_TOL = 1e-10
 
-T = TypeVar("T", Path, Path2d)
-
 
 def to_multi_path(paths: Iterable[Path]) -> Path:
     """Returns a multi-path object from all given paths and their sub-paths.
     Ignores paths without any commands (empty paths).
     """
     multi_path = Path()
     for p in paths:
         multi_path.extend_multi_path(p)
     return multi_path
 
 
-def to_3d_paths(paths: Iterable[Path | Path2d]) -> Iterator[Path]:
-    """Yields all paths as 3D :class:`Path` instances."""
-    if isinstance(paths, AbstractPath):
-        paths = [paths]
-    for path in paths:
-        if isinstance(path, Path2d):
-            yield path.to_3d_path()
-        else:
-            yield path
-
-
-def single_paths(paths: Iterable[T]) -> Iterable[T]:
+def single_paths(paths: Iterable[Path]) -> Iterable[Path]:
     """Yields all given paths and their sub-paths as single path objects."""
     for p in paths:
         if p.has_sub_paths:
             yield from p.sub_paths()
         else:
             yield p
 
 
-def transform_paths(paths: Iterable[T], m: Matrix44) -> list[T]:
+def transform_paths(paths: Iterable[Path], m: Matrix44) -> list[Path]:
     """Transform multiple path objects at once by transformation
     matrix `m`. Returns a list of the transformed path objects.
 
     Args:
         paths: iterable of :class:`Path` or :class:`Path2d` objects
         m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
 
     """
     return [p.transform(m) for p in paths]
 
 
-def transform_paths_to_ocs(paths: Iterable[Path | Path2d], ocs: OCS) -> list[Path]:
+def transform_paths_to_ocs(paths: Iterable[Path], ocs: OCS) -> list[Path]:
     """Transform multiple :class:`Path` objects at once from WCS to OCS.
     Returns a list of the transformed :class:`Path` objects.
 
     Args:
         paths: iterable of :class:`Path` or :class:`Path2d` objects
         ocs: OCS transformation of type :class:`~ezdxf.math.OCS`
 
     """
     t = ocs.matrix.copy()
     t.transpose()
-    return transform_paths(to_3d_paths(paths), t)
+    return transform_paths(paths, t)
 
 
-def bbox(paths: Iterable[Path | Path2d], *, fast=False) -> BoundingBox:
+def bbox(paths: Iterable[Path], *, fast=False) -> BoundingBox:
     """Returns the :class:`~ezdxf.math.BoundingBox` for the given paths.
 
     Args:
         paths: iterable of :class:`Path` or :class:`Path2d` objects
         fast: calculates the precise bounding box of Bèzier curves if
             ``False``, otherwise uses the control points of Bézier curves to
             determine their bounding box.
@@ -158,21 +144,21 @@
         else:
             bb = precise_bbox(p)
             if bb.has_data:
                 box.extend((bb.extmin, bb.extmax))
     return box
 
 
-def precise_bbox(path: Path | Path2d) -> BoundingBox:
+def precise_bbox(path: Path) -> BoundingBox:
     """Returns the precise :class:`~ezdxf.math.BoundingBox` for the given paths."""
     if len(path) == 0:  # empty path
         return BoundingBox()
     start = path.start
     points: list[Vec3] = [start]
-    for cmd in path:
+    for cmd in path.commands():
         if cmd.type == Command.LINE_TO:
             points.append(cmd.end)
         elif cmd.type == Command.CURVE4_TO:
             bb = cubic_bezier_bbox(
                 Bezier4P((start, cmd.ctrl1, cmd.ctrl2, cmd.end))  # type: ignore
             )
             points.append(bb.extmin)
@@ -268,15 +254,15 @@
 
 
 # Path to entity converter and render utilities:
 
 
 def render_lwpolylines(
     layout: GenericLayoutType,
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
@@ -310,15 +296,15 @@
     for lwpolyline in lwpolylines:
         layout.add_entity(lwpolyline)
     return EntityQuery(lwpolylines)
 
 
 def render_polylines2d(
     layout: GenericLayoutType,
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = 0.01,
     segments: int = 4,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as 2D
@@ -352,15 +338,15 @@
     for polyline2d in polylines2d:
         layout.add_entity(polyline2d)
     return EntityQuery(polylines2d)
 
 
 def render_hatches(
     layout: GenericLayoutType,
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     edge_path: bool = True,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     g1_tol: float = G1_TOL,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
@@ -401,15 +387,15 @@
     for hatch in hatches:
         layout.add_entity(hatch)
     return EntityQuery(hatches)
 
 
 def render_mpolygons(
     layout: GenericLayoutType,
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
@@ -445,15 +431,15 @@
     for polygon in polygons:
         layout.add_entity(polygon)
     return EntityQuery(polygons)
 
 
 def render_polylines3d(
     layout: GenericLayoutType,
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as 3D
     :class:`~ezdxf.entities.Polyline` entities.
@@ -481,15 +467,15 @@
     for polyline3d in polylines3d:
         layout.add_entity(polyline3d)
     return EntityQuery(polylines3d)
 
 
 def render_lines(
     layout: GenericLayoutType,
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
     :class:`~ezdxf.entities.Line` entities.
@@ -516,15 +502,15 @@
     for line in lines:
         layout.add_entity(line)
     return EntityQuery(lines)
 
 
 def render_splines_and_polylines(
     layout: GenericLayoutType,
-    paths: Iterable[Path | Path2d],
+    paths: Iterable[Path],
     *,
     g1_tol: float = G1_TOL,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as :class:`~ezdxf.entities.Spline`
     and 3D :class:`~ezdxf.entities.Polyline` entities.
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.css` & `ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.html` & `ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.html`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.js` & `ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.js`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.py` & `ezdxf-1.1.0b4/src/ezdxf/pp/dxfpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/pp/pprint.py` & `ezdxf-1.1.0b4/src/ezdxf/pp/pprint.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.css` & `ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.py` & `ezdxf-1.1.0b4/src/ezdxf/pp/rawpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/pp/reflinks.py` & `ezdxf-1.1.0b4/src/ezdxf/pp/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.1.0b4/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/arrows.py` & `ezdxf-1.1.0b4/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/curves.py` & `ezdxf-1.1.0b4/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/dimension.py` & `ezdxf-1.1.0b4/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/dim_base.py` & `ezdxf-1.1.0b4/src/ezdxf/render/dim_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -369,15 +369,15 @@
             attribs["lineweight"] = self.lineweight
         return attribs
 
 
 class Arrows:
     def __init__(self, dim_style: DimStyleOverride, color: int, scale: float):
         get = dim_style.get
-        self.color: int = color
+        self.color: int = get("dimclrd", color)
         self.tick_size: float = get("dimtsz", 0.0) * scale
         self.arrow1_name: str = ""  # empty string is a closed filled arrow
         self.arrow2_name: str = ""  # empty string is a closed filled arrow
         self.arrow_size: float = get("dimasz", 0.25) * scale
         self.suppress1 = False  # ezdxf only
         self.suppress2 = False  # ezdxf only
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/dim_curved.py` & `ezdxf-1.1.0b4/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.1.0b4/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/dim_linear.py` & `ezdxf-1.1.0b4/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.1.0b4/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/dim_radius.py` & `ezdxf-1.1.0b4/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/forms.py` & `ezdxf-1.1.0b4/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/hatching.py` & `ezdxf-1.1.0b4/src/ezdxf/render/hatching.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     Vec3,
     Bezier3P,
     Bezier4P,
     intersection_ray_cubic_bezier_2d,
     quadratic_to_cubic_bezier,
 )
 from ezdxf import const
-from ezdxf.path import Path, Path2d, LineTo, MoveTo, Curve3To, Curve4To
+from ezdxf.path import Path, LineTo, MoveTo, Curve3To, Curve4To
 
 if TYPE_CHECKING:
     from ezdxf.entities.polygon import DXFPolygon
 
 MIN_HATCH_LINE_DISTANCE = 1e-4  # ??? what's a good choice
 NONE_VEC2 = Vec2(math.nan, math.nan)
 KEY_NDIGITS = 4
@@ -485,15 +485,15 @@
 
     if not path_start.isclose(start):  # close path
         yield start, path_start
 
 
 def hatch_paths(
     baseline: HatchBaseLine,
-    paths: Sequence[Path|Path2d],
+    paths: Sequence[Path],
     terminate: Optional[Callable[[], bool]] = None,
 ) -> Iterator[Line]:
     """Yields all pattern lines for all hatch lines generated by the given
     :class:`HatchBaseLine`, intersecting the given 2D :class:`~ezdxf.path.Path`
     instances as :class:`Line` instances. The paths are handled as projected
     into the xy-plane the z-axis of path vertices will be ignored if present.
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/leader.py` & `ezdxf-1.1.0b4/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/linetypes.py` & `ezdxf-1.1.0b4/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/mesh.py` & `ezdxf-1.1.0b4/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/mleader.py` & `ezdxf-1.1.0b4/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/mline.py` & `ezdxf-1.1.0b4/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/point.py` & `ezdxf-1.1.0b4/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/polyline.py` & `ezdxf-1.1.0b4/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/r12spline.py` & `ezdxf-1.1.0b4/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/trace.py` & `ezdxf-1.1.0b4/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/_linetypes.py` & `ezdxf-1.1.0b4/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/render/__init__.py` & `ezdxf-1.1.0b4/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/16x16.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/24x24.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/256x256.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/32x32.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/48x48.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/64x64.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.1.0b4/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/sections/blocks.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/sections/classes.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/sections/entities.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/sections/headervars.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/sections/objects.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/sections/table.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/sections/tables.py` & `ezdxf-1.1.0b4/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/analyze.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/binarydata.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/codepage.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/crypt.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/debug.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/difftags.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/handle.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/indexing.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/juliandate.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/pattern.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/rawloader.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/standards.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/strip.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/test.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/text.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/text_layout.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/text_size.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf/tools/__init__.py` & `ezdxf-1.1.0b4/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.1.0b4/src/ezdxf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b3
+Version: 1.1.0b4
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -211,24 +211,23 @@
 Feedback is greatly appreciated.
 
 Manfred
 
 News
 ====
 
-Version 1.1.0b2 - dev
----------------------
+Version 1.1.0 Beta
+------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-1.html
 - WARNING: The font support changed drastically in this version, if you use the 
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
-- NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
 - NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF, PNG
 - NEW: native `SVG`, `HPGL/2`  and `DXF` backends for the `drawing` add-on, these backends 
   do not need additional libraries to work
 - NEW: `PyMuPdf` backend for the `drawing` add-on, support for PDF, PNG, PPM and PBM export
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
@@ -245,19 +244,23 @@
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
+- CHANGED: `BackendInterface` and all derived backends support only 2D shapes
+- REMOVED: Matplotlib/Qt path converters from `ezdxf.path.converter`
 - REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
+- BUGFIX: [#898](https://github.com/mozman/ezdxf/issues/898)
+  use `dimclrd` color for dimension arrow blocks 
 
 Version 1.0.3 - 2023-03-26
 --------------------------
 
 - Release notes: https://ezdxf.mozman.at/release-v1-0.html
 - NEW: [#833](https://github.com/mozman/ezdxf/issues/833)
   logging non-unique entity handles when loading a DXF document as warnings, auditing
```

## Comparing `ezdxf-1.1.0b3/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.1.0b4/src/ezdxf.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -141,14 +141,15 @@
 src/ezdxf/acc/bspline.pyx
 src/ezdxf/acc/construct.pxd
 src/ezdxf/acc/construct.pyx
 src/ezdxf/acc/linetypes.pyx
 src/ezdxf/acc/mapbox_earcut.pyx
 src/ezdxf/acc/matrix44.pxd
 src/ezdxf/acc/matrix44.pyx
+src/ezdxf/acc/np_support.pyx
 src/ezdxf/acc/vector.pxd
 src/ezdxf/acc/vector.pyx
 src/ezdxf/acis/__init__.py
 src/ezdxf/acis/abstract.py
 src/ezdxf/acis/api.py
 src/ezdxf/acis/const.py
 src/ezdxf/acis/dbg.py
@@ -197,14 +198,15 @@
 src/ezdxf/addons/browser/views.py
 src/ezdxf/addons/drawing/__init__.py
 src/ezdxf/addons/drawing/backend.py
 src/ezdxf/addons/drawing/clipper.py
 src/ezdxf/addons/drawing/config.py
 src/ezdxf/addons/drawing/debug_backend.py
 src/ezdxf/addons/drawing/debug_utils.py
+src/ezdxf/addons/drawing/designer.py
 src/ezdxf/addons/drawing/dxf.py
 src/ezdxf/addons/drawing/frontend.py
 src/ezdxf/addons/drawing/gfxproxy.py
 src/ezdxf/addons/drawing/hpgl2.py
 src/ezdxf/addons/drawing/layout.py
 src/ezdxf/addons/drawing/matplotlib.py
 src/ezdxf/addons/drawing/mtext_complex.py
```

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.1.0b4/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.1.0b4/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis_2.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_acis_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_surface.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_232_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.1.0b4/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.1.0b4/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.1.0b4/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/conftest.py` & `ezdxf-1.1.0b4/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_500_units.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_507_dxf_pretty_printer.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_507_dxf_pretty_printer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_514_text.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_515a_fonts_truetype.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_515a_fonts_truetype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_515b_fonts_shapefiles.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_515b_fonts_shapefiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         return fonts.font_manager.get_shapefile_glyph_cache("txt.shx")
 
     def test_get_glyphs(self, cache):
         glyph = cache.get_shape(ord("A"))
         box = BoundingBox2d(glyph.control_vertices())
         assert box.size.x == 6
         assert box.size.y == 6
-        assert glyph is cache.get_shape(ord("A"))
+        assert glyph is not cache.get_shape(ord("A")), "expected a copy"
 
     def test_get_advance_width(self, cache):
         glyph = cache.get_shape(ord("A"))
         assert glyph.end.x == 6  # last move_to defines the advance width
         assert cache.get_advance_width(ord("A")) == 6
 
     def test_get_space_width(self, cache):
@@ -115,17 +115,17 @@
     def test_path_for_unsupported_glyphs(self, cache):
         box = cache.get_shape(1234)
         assert len(box) == 5
 
     def test_spaces_are_measured(self, cache):
         assert cache.get_text_length("   ", cache.font_measurements.cap_height) == 18
 
-    def test_spaces_are_rendered(self, cache):
-        p = cache.get_text_path("   ", cache.font_measurements.cap_height)
-        assert p.end.isclose((18, 0))
+    def test_spaces_are_not_rendered(self, cache):
+        p = cache.get_text_glyph_paths("   ", cache.font_measurements.cap_height)
+        assert len(p) == 0
 
 
 def test_resolve_shx_font_name():
     assert fonts.resolve_shx_font_name("txt", order="s") == "txt.shx"
     assert fonts.resolve_shx_font_name("txt.shx", order="s") == "txt.shx"
     # txt_____.ttf is not available under test
     # prefer LibreCAD fonts:
```

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_515c_fonts_lff.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_515c_fonts_lff.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 import pytest
 
-from ezdxf.math import BoundingBox2d
 from ezdxf import path
 from ezdxf.fonts import fonts
 
 FONT = "standard.lff"
 
 
 @pytest.fixture(scope="module", autouse=True)
@@ -40,26 +39,37 @@
 
     def test_text_width_ex(self, lff):
         assert lff.text_width_ex("1234", cap_height=3, width_factor=2) == pytest.approx(
             18.189556764069664, abs=TOL
         )
 
     def test_text_path(self, lff):
-        box = BoundingBox2d(lff.text_path("1234").control_vertices())
-        assert box.size.x == pytest.approx(7.578981985029027, abs=TOL)
+        text_path = lff.text_path("1234")
+
+        # fmt: off
+        assert text_path.command_codes() == [
+            1, 1, 4, 1, 3, 3, 1, 1, 4, 1, 3, 3, 4, 1, 3, 3, 1, 3, 3, 1, 4, 1, 1, 4, 1
+        ]
+        # fmt: on
+        box = text_path.bbox()
+        assert box.size.x > 6
         assert box.size.y == pytest.approx(2.5789819850290274, abs=TOL)
 
     def test_text_path_ex(self, lff):
-        box = path.bbox(  # get exact bounding box
-            [lff.text_path_ex("1234", cap_height=3, width_factor=2)], fast=False
-        )
-        assert box.size.x == pytest.approx(18.189556764069664, abs=TOL)
+        text_path = lff.text_path_ex("1234", cap_height=3, width_factor=2)
+        box = path.precise_bbox(text_path)
+        assert box.size.x > 16
         assert box.size.y == pytest.approx(3, abs=TOL)
 
 
+def test_low_level_glyph_cache_measures_spaces():
+    cache = fonts.font_manager.get_lff_glyph_cache(FONT)
+    assert cache.get_text_length("   ", cache.font_measurements.cap_height) == 20.25
+
+
 def test_map_shx_to_lff():
     assert fonts.map_shx_to_lff("txt") == "standard.lff"
     assert fonts.map_shx_to_lff("txt.shx") == "standard.lff"
     assert fonts.map_shx_to_lff("iso") == "iso.lff"
     assert fonts.map_shx_to_lff("iso.shx") == "iso.lff"
     assert fonts.map_shx_to_lff("unknown.shx") == "unknown.shx"
```

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_533_shapefiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,15 +144,15 @@
             path.Command.MOVE_TO,
         ]
         assert p.start.isclose((6, 2))
         assert p.end.isclose((36, 0))
 
     def test_render_bulges(self, shp):
         p = shp.render_shape(0x53)  # uppercase letter S
-        commands = p.commands()
+        commands = list(p.commands())
         assert [c.type for c in commands] == [
             path.Command.CURVE4_TO,
             path.Command.CURVE4_TO,
             path.Command.CURVE4_TO,
             path.Command.LINE_TO,
             path.Command.CURVE4_TO,
             path.Command.CURVE4_TO,
@@ -297,16 +297,16 @@
         cache = shapefile.GlyphCache(shp)
         p = cache.get_shape(10)
         assert len(p) == 0
 
     def test_unsupported_printable_shape_number_returns_empty_box(self, shp):
         cache = shapefile.GlyphCache(shp)
         box = cache.get_shape(1234)
-        assert box is cache.empty_box
-        assert box.end.x == cache.space_width
+        assert box is not cache.empty_box, "expected a copy"
+        assert box.command_codes() == cache.empty_box.command_codes()
 
     def test_empty_box_has_advance_width_like_glyph_A(self, shp):
         cache = shapefile.GlyphCache(shp)
         assert cache.get_advance_width(1234) == cache.get_advance_width(65)
 
 
 FILE_1 = b"""
```

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_535_xref_basic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_537_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_05_tools/test_540_lff_parser.py` & `ezdxf-1.1.0b4/tests/test_05_tools/test_540_lff_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/conftest.py` & `ezdxf-1.1.0b4/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_600_base.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_605_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_613_point_in_poygon.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_613_point_in_poygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_616_plane.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_620_knot.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_640_bbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,19 +20,24 @@
         assert bbox.extmin == (-1, -2, -3)
         assert bbox.extmax == (7, 8, 9)
 
     def test_init_none(self):
         bbox = BoundingBox()
         assert bbox.is_empty is True
         assert bbox.has_data is False
+
         bbox.extend([(0, 0, 0), (10, 10, 10)])
         assert bbox.size == (10, 10, 10)
         assert bbox.is_empty is False
         assert bbox.has_data is True
 
+    def test_init_empty_list(self):
+        bbox = BoundingBox([])
+        assert bbox.has_data is False
+
     @pytest.mark.parametrize("v", [
         [],
         [(0, 0, 0)],
         [(1, 0, 0), (2, 0, 0)],
         [(1, 1, 0), (2, 2, 0)],
         [(1, 1, 1), (1, 1, 1)],
     ])
```

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_651_construction_polyline.py`

 * *Files 1% similar despite different names*

```diff
@@ -245,15 +245,15 @@
         assert len(cp) > 20
         assert abs(cp.length - math.tau) < 0.02
 
     def test_unit_circle_by_path(self):
         from ezdxf import path
 
         p = path.unit_circle()
-        cp = ConstructionPolyline(p.flattening(0.01))
+        cp = ConstructionPolyline(p.flattening(0.01, segments=16))
         assert cp.is_closed is True
         assert len(cp) > 60
         assert abs(cp.length - math.tau) < 0.002
 
 
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_658_bevel_tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         assert points == list(p.flattening(0.1))
 
     def test_points_for_45_deg(self):
         p = fillet(Vec3.list([(-5, 0), (0, 0), (-5, -5)]), 1.0)
         # result is visually checked in CAD application
         assert (
             close_vectors(
-                p.flattening(1),
+                p.flattening(1, segments=16),
                 [
                     Vec3(-5.0, 0.0, 0.0),
                     Vec3(-2.414213562373095, 0.0, 0.0),
                     Vec3(-2.338885112974325, -0.0028274449650404843, 0.0),
                     Vec3(-2.2647391508495334, -0.011198832627437505, 0.0),
                     Vec3(-2.192024742400491, -0.02494774213810442, 0.0),
                     Vec3(-2.1209909540289686, -0.04390775264795457, 0.0),
@@ -197,15 +197,15 @@
         )
 
     def test_points_for_135_deg(self):
         p = fillet(Vec3.list([(-5, 0), (0, 0), (-5, 5)]), 1.0)
         # result is visually checked in CAD application
         assert (
             close_vectors(
-                p.flattening(1),
+                p.flattening(1, segments=16),
                 [
                     Vec3(-5.0, 0.0, 0.0),
                     Vec3(-2.414213562373095, 0.0, 0.0),
                     Vec3(-2.338885112974325, 0.0028274449650404843, 0.0),
                     Vec3(-2.2647391508495334, 0.011198832627437505, 0.0),
                     Vec3(-2.192024742400491, 0.02494774213810442, 0.0),
                     Vec3(-2.1209909540289686, 0.04390775264795457, 0.0),
```

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.1.0b4/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,17 @@
     style = DimStyleOverride(dimline.dimension, override)
     renderer = LinearDimension(dimline.dimension, override=style)
     assert renderer.measurement.text == "100"
     assert renderer.measurement.decimal_separator == "."
     assert renderer.tol.decimal_places == 2  # default value
     assert renderer.tol.text == "±0.01"
     assert renderer.tol.valign == 0
-    assert compile_mtext(renderer.measurement, renderer.tol) == r"\A0;100{\H0.50x;±0.01}"
+    assert (
+        compile_mtext(renderer.measurement, renderer.tol) == r"\A0;100{\H0.50x;±0.01}"
+    )
 
 
 def test_linear_dimension_with_two_tolerances(dwg):
     msp = dwg.modelspace()
     dimline = msp.add_linear_dim(base=(0, 10), p1=(0, 0), p2=(101, 0))
     override = {
         "dimlfac": 1,
@@ -50,15 +52,18 @@
     renderer = LinearDimension(dimline.dimension, override=style)
     assert renderer.measurement.text == "101"
     assert renderer.measurement.decimal_separator == "."
     assert renderer.tol.decimal_places == 2  # default value
     assert renderer.tol.text_upper == "+0.02"
     assert renderer.tol.text_lower == "-0.03"
     assert renderer.tol.valign == 1
-    assert compile_mtext(renderer.measurement, renderer.tol) == r"\A1;101{\H0.50x;\S+0.02^ -0.03;}"
+    assert (
+        compile_mtext(renderer.measurement, renderer.tol)
+        == r"\A1;101{\H0.50x;\S+0.02^ -0.03;}"
+    )
 
 
 def test_linear_dimension_with_limits(dwg):
     msp = dwg.modelspace()
     dimline = msp.add_linear_dim(base=(0, 10), p1=(0, 0), p2=(101, 0))
     override = {
         "dimlfac": 1,
@@ -70,38 +75,53 @@
     style = DimStyleOverride(dimline.dimension, override)
     renderer = LinearDimension(dimline.dimension, override=style)
     assert renderer.measurement.text == "101"
     assert renderer.measurement.decimal_separator == "."
     assert renderer.tol.decimal_places == 2  # default value
     assert renderer.tol.text_upper == "101.02"
     assert renderer.tol.text_lower == "100.97"
-    assert compile_mtext(renderer.measurement, renderer.tol) == r"{\H0.50x;\S101.02^ 100.97;}"
+    assert (
+        compile_mtext(renderer.measurement, renderer.tol)
+        == r"{\H0.50x;\S101.02^ 100.97;}"
+    )
 
 
 def test_dimension_insert_attribute_translates_the_block_content():
     doc = ezdxf.new()
     msp = doc.modelspace()
     dimline = msp.add_linear_dim(base=(0, 10), p1=(0, 0), p2=(100, 0))
     dimline.render()
     dim = dimline.dimension
     blk = dim.get_geometry_block()
 
     blk_points = blk.query("POINT")
-    virtual_points = [
-        e for e in dim.virtual_entities() if e.dxftype() == "POINT"
-    ]
+    virtual_points = [e for e in dim.virtual_entities() if e.dxftype() == "POINT"]
 
     # without the insert attribute, the virtual points should be located at the
     # original location:
     for vpoint, blk_point in zip(virtual_points, blk_points):
         assert vpoint.dxf.location.isclose(blk_point.dxf.location)
 
     # set an insertion point for this dimension ...
     INSERT = Vec3(10, 10, 0)
     dim.dxf.insert = Vec3(INSERT)
-    virtual_points = [
-        e for e in dim.virtual_entities() if e.dxftype() == "POINT"
-    ]
+    virtual_points = [e for e in dim.virtual_entities() if e.dxftype() == "POINT"]
 
     # ... and the virtual points should be translated by the insert vector
     for vpoint, blk_point in zip(virtual_points, blk_points):
         assert (vpoint.dxf.location - blk_point.dxf.location).isclose(INSERT)
+
+
+@pytest.mark.parametrize("color", [1, 7])
+def test_override_all_colors(color):
+    new_doc = ezdxf.new()
+    new_msp = new_doc.modelspace()
+    style_override = {"dimclrt": color, "dimclrd": color, "dimclre": color}
+    dim_renderer = new_msp.add_linear_dim(
+        base=(0, 10), p1=(0, 0), p2=(100, 0), override=style_override
+    ).render()
+    dimension = dim_renderer.dimension
+    blk = dimension.get_geometry_block()
+    for entity in blk:
+        if entity.dxftype() == "POINT":
+            continue
+        assert entity.dxf.color == color
```

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_705_shape.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_707_trace.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_708a_path.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_708a_path.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020, Manfred Moitzi
+# Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 import pytest
 import math
 
 from ezdxf.path import (
     Path,
     make_path,
@@ -498,15 +498,15 @@
     pline.closed = True
     pline.append_points([(0, 0, 1), (1, 0, 1)], format="xyb")
     path = make_path(pline)
     assert path.start.isclose((0, 0))
     assert path.end.isclose((0, 0))
     assert len(path) == 4
     assert any(cmd.type == Command.CURVE4_TO for cmd in path)
-    vertices = list(path.flattening(0.1))
+    vertices = list(path.flattening(0.1, segments=16))
     assert len(vertices) == 65
 
 
 def test_make_path_from_full_circle_lwpolyline_issue_424():
     pline = LWPolyline()
     pline.closed = True
     points = [
@@ -623,34 +623,30 @@
     assert len(vertices) == 41
     assert vertices[0] == (0, 0)
     assert vertices[-1] == (3, 0)
 
 
 def test_path_from_hatch_polyline_path_without_bulge():
     polyline_path = PolylinePath()
-    polyline_path.set_vertices(
-        [(0, 0), (0, 1), (1, 1), (1, 0)], is_closed=False
-    )
+    polyline_path.set_vertices([(0, 0), (0, 1), (1, 1), (1, 0)], is_closed=False)
     path = converter.from_hatch_polyline_path(polyline_path)
     assert len(path) == 3
     assert path.start == (0, 0)
     assert path.end == (1, 0)
 
     polyline_path.is_closed = True
     path = converter.from_hatch_polyline_path(polyline_path)
     assert len(path) == 4
     assert path.start == (0, 0)
     assert path.end == (0, 0)
 
 
 def test_path_from_hatch_polyline_path_with_bulge():
     polyline_path = PolylinePath()
-    polyline_path.set_vertices(
-        [(0, 0), (1, 0, 0.5), (2, 0), (3, 0)], is_closed=False
-    )
+    polyline_path.set_vertices([(0, 0), (1, 0, 0.5), (2, 0), (3, 0)], is_closed=False)
     path = converter.from_hatch_polyline_path(polyline_path)
     assert len(path) == 4
     assert path.start == (0, 0)
     assert path.end == (3, 0)
 
     assert path[1].type == Command.CURVE4_TO
     assert path[1].end.isclose((1.5, -0.25))
@@ -714,86 +710,80 @@
 
     path = Path()
     path.line_to((2, 0))
     path.curve4_to((4, 0), (2, 1), (4, 1))  # end, ctrl1, ctrl2
     assert path.has_clockwise_orientation() is True
 
 
-def test_reversing_empty_path():
-    p = Path()
-    assert len(p.reversed()) == 0
-
-
-def test_reversing_one_line():
-    p = Path()
-    p.line_to((1, 0))
-    p2 = list(p.reversed().control_vertices())
-    assert close_vectors(p2, [(1, 0), (0, 0)])
-
-
-def test_reversing_one_curve3():
-    p = Path()
-    p.curve3_to((3, 0), (1.5, 1))
-    p2 = list(p.reversed().control_vertices())
-    assert close_vectors(p2, [(3, 0), (1.5, 1), (0, 0)])
-
-
-def test_reversing_one_curve4():
-    p = Path()
-    p.curve4_to((3, 0), (1, 1), (2, 1))
-    p2 = list(p.reversed().control_vertices())
-    assert close_vectors(p2, [(3, 0), (2, 1), (1, 1), (0, 0)])
-
-
-def test_reversing_path_ctrl_vertices(p1):
-    p2 = p1.reversed()
-    assert close_vectors(
-        p2.control_vertices(), reversed(list(p1.control_vertices()))
-    )
-
+class TestReversePath:
+    def test_reversing_empty_path(self):
+        p = Path()
+        assert len(p.reversed()) == 0
+
+    def test_reversing_one_line(self):
+        p = Path()
+        p.line_to((1, 0))
+        p2 = list(p.reversed().control_vertices())
+        assert close_vectors(p2, [(1, 0), (0, 0)])
+
+    def test_reversing_one_curve3(self):
+        p = Path()
+        p.curve3_to((3, 0), (1.5, 1))
+        p2 = list(p.reversed().control_vertices())
+        assert close_vectors(p2, [(3, 0), (1.5, 1), (0, 0)])
+
+    def test_reversing_one_curve4(self):
+        p = Path()
+        p.curve4_to((3, 0), (1, 1), (2, 1))
+        p2 = list(p.reversed().control_vertices())
+        assert close_vectors(p2, [(3, 0), (2, 1), (1, 1), (0, 0)])
+
+    def test_reversing_path_ctrl_vertices(self, p1):
+        p2 = p1.reversed()
+        assert close_vectors(
+            p2.control_vertices(), reversed(list(p1.control_vertices()))
+        )
 
-def test_reversing_path_approx(p1):
-    p2 = p1.reversed()
-    v1 = list(p1.approximate())
-    v2 = list(p2.approximate())
-    assert close_vectors(v1, reversed(v2))
-
-
-def test_reversing_multi_path():
-    p = Path()
-    p.line_to((1, 0, 0))
-    p.move_to((2, 0, 0))
-    p.line_to((3, 0, 0))
-    r = p.reversed()
-    assert r.has_sub_paths is True
-    assert len(r) == 3
-    assert r.start == (3, 0, 0)
-    assert r.end == (0, 0, 0)
-
-    r0, r1 = r.sub_paths()
-    assert r0.start == (3, 0, 0)
-    assert r0.end == (2, 0, 0)
-    assert r1.start == (1, 0, 0)
-    assert r1.end == (0, 0, 0)
-
-
-def test_reversing_multi_path_with_a_move_to_cmd_at_the_end():
-    p = Path()
-    p.line_to((1, 0, 0))
-    p.move_to((2, 0, 0))
-    # The last move_to will become the first move_to.
-    # A move_to as first command just moves the start point.
-    r = p.reversed()
-    assert len(r) == 1
-    assert r.start == (1, 0, 0)
-    assert r.end == (0, 0, 0)
-    assert r.has_sub_paths is False
+    def test_reversing_path_approx(self, p1):
+        p2 = p1.reversed()
+        v1 = list(p1.approximate())
+        v2 = list(p2.approximate())
+        assert close_vectors(v1, reversed(v2))
+
+    def test_reversing_multi_path(self):
+        p = Path()
+        p.line_to((1, 0, 0))
+        p.move_to((2, 0, 0))
+        p.line_to((3, 0, 0))
+        r = p.reversed()
+        assert r.has_sub_paths is True
+        assert len(r) == 3
+        assert r.start == (3, 0, 0)
+        assert r.end == (0, 0, 0)
+
+        r0, r1 = r.sub_paths()
+        assert r0.start == (3, 0, 0)
+        assert r0.end == (2, 0, 0)
+        assert r1.start == (1, 0, 0)
+        assert r1.end == (0, 0, 0)
+
+    def test_reversing_multi_path_with_a_move_to_cmd_at_the_end(self):
+        p = Path()
+        p.line_to((1, 0, 0))
+        p.move_to((2, 0, 0))
+        # The last move_to will become the first move_to.
+        # A move_to as first command just moves the start point.
+        r = p.reversed()
+        assert len(r) == 1
+        assert r.start == (1, 0, 0)
+        assert r.end == (0, 0, 0)
+        assert r.has_sub_paths is False
 
 
-def test_clockwise(p1):
+def test_cw_and_ccw_orientation(p1):
     from ezdxf.math import has_clockwise_orientation
 
     cw_path = p1.clockwise()
     ccw_path = p1.counter_clockwise()
     assert has_clockwise_orientation(cw_path.control_vertices()) is True
     assert has_clockwise_orientation(ccw_path.control_vertices()) is False
 
@@ -967,17 +957,15 @@
 class TestPathFromEdgePathWithElevationAndFlippedExtrusion:
     def test_line_edge(self):
         ep = EdgePath()
         ep.add_line(A, B)
         ep.add_line(B, C)
         ep.add_line(C, D)
         ep.add_line(D, A)
-        path = converter.from_hatch_edge_path(
-            ep, ocs=OCS((0, 0, -1)), elevation=4
-        )
+        path = converter.from_hatch_edge_path(ep, ocs=OCS((0, 0, -1)), elevation=4)
         assert len(list(path.sub_paths())) == 1, "expected one closed loop"
         assert len(list(path.control_vertices())) == 5
         assert all(math.isclose(v.z, -4) for v in path.control_vertices())
         assert path.is_closed is True, "expected a closed loop"
 
     def test_arc_edge(self):
         ep = EdgePath()
@@ -985,44 +973,38 @@
             center=(5.0, 5.0),
             radius=5.0,
             start_angle=0,
             end_angle=90,
             ccw=True,
         )
         ep.add_line((5, 10), (10, 5))
-        path = converter.from_hatch_edge_path(
-            ep, ocs=OCS((0, 0, -1)), elevation=4
-        )
+        path = converter.from_hatch_edge_path(ep, ocs=OCS((0, 0, -1)), elevation=4)
         assert len(path) == 2
         assert all(math.isclose(v.z, -4) for v in path.control_vertices())
 
     def test_ellipse_edge(self):
         ep = EdgePath()
         ep.add_ellipse(
             center=(5.0, 5.0),
             major_axis=(5.0, 0.0),
             ratio=1,
             start_angle=0,
             end_angle=90,
             ccw=True,
         )
         ep.add_line((5, 10), (10, 5))
-        path = converter.from_hatch_edge_path(
-            ep, ocs=OCS((0, 0, -1)), elevation=4
-        )
+        path = converter.from_hatch_edge_path(ep, ocs=OCS((0, 0, -1)), elevation=4)
         assert len(path) == 2
         assert all(math.isclose(v.z, -4) for v in path.control_vertices())
 
     def test_spline_edge(self):
         ep = EdgePath()
         ep.add_spline(fit_points=[(10, 5), (8, 5), (6, 8), (5, 10)])
         ep.add_line((5, 10), (10, 5))
-        path = converter.from_hatch_edge_path(
-            ep, ocs=OCS((0, 0, -1)), elevation=4
-        )
+        path = converter.from_hatch_edge_path(ep, ocs=OCS((0, 0, -1)), elevation=4)
         assert len(path) > 2
         assert all(math.isclose(v.z, -4) for v in path.control_vertices())
 
     def test_from_complex_edge_path(self, edge_path):
         path = converter.from_hatch_edge_path(
             edge_path, ocs=OCS((0, 0, -1)), elevation=4
         )
```

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-#  Copyright (c) 2021, Manfred Moitzi
+#  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 
 import pytest
-import sys
 
 pytest.importorskip("PySide6")
 
-from ezdxf.addons.xqt import QPainterPath, QPointF
 from ezdxf import path
 from ezdxf.math import quadratic_to_cubic_bezier, Bezier3P
+from ezdxf import npshapes
 
 
-class TestToQPainterPath:
+class TestNumpyPath2dToQPainterPath:
     def test_no_paths(self):
         with pytest.raises(ValueError):
-            path.to_qpainter_path([])
+            npshapes.to_qpainter_path([])
 
     def test_line_to(self):
         p = path.Path()
         p.line_to((4, 5, 6))
         p.line_to((7, 8, 6))
-        qpath = path.to_qpainter_path([p])
+        qpath = npshapes.to_qpainter_path([npshapes.NumpyPath2d(p)])
         assert qpath.elementCount() == 3
 
         m = qpath.elementAt(0)
         assert m.isMoveTo() is True
         assert (m.x, m.y) == (0, 0)
 
         l1 = qpath.elementAt(1)
@@ -35,15 +34,15 @@
         assert l2.isLineTo() is True
         assert (l2.x, l2.y) == (7, 8)
 
     def test_curve3_to(self):
         bez3 = Bezier3P([(0, 0), (2, 1), (4, 0)])
         p = path.Path()
         p.curve3_to(bez3.control_points[2], bez3.control_points[1])
-        qpath = path.to_qpainter_path([p])
+        qpath = npshapes.to_qpainter_path([npshapes.NumpyPath2d(p)])
         # Qt converts quadratic bezier curves unto cubic bezier curves
         assert qpath.elementCount() == 4
         bez4 = quadratic_to_cubic_bezier(bez3)
 
         q1 = qpath.elementAt(1)
         assert q1.isCurveTo()  # start of cure
         assert q1.x, q1.y == bez4.control_points[1]
@@ -54,15 +53,15 @@
         q3 = qpath.elementAt(3)
         assert q3.x, q3.y == bez4.control_points[2]
 
     def test_curve4_to(self):
         bez4 = [(4, 0, 2), (1, 1, 7), (3, 1, 5)]
         p = path.Path()
         p.curve4_to(*bez4)
-        qpath = path.to_qpainter_path([p])
+        qpath = npshapes.to_qpainter_path([npshapes.NumpyPath2d(p)])
         assert qpath.elementCount() == 4
         q1 = qpath.elementAt(1)
         assert q1.isCurveTo()  # start of cure
         assert q1.x, q1.y == bez4[1]
 
         q2 = qpath.elementAt(2)
         assert q2.x, q2.y == bez4[2]
@@ -71,28 +70,31 @@
         assert q3.x, q3.y == bez4[0]
 
     def test_two_single_paths(self):
         p1 = path.Path()
         p1.line_to((4, 5, 6))
         p2 = path.Path()
         p2.line_to((7, 8, 6))
-        qpath = path.to_qpainter_path([p1, p2])
+        qpath = npshapes.to_qpainter_path(
+            [npshapes.NumpyPath2d(p1), npshapes.NumpyPath2d(p2)]
+        )
         assert qpath.elementCount() == 4
         assert qpath.elementAt(0).isMoveTo() is True
         assert qpath.elementAt(1).isLineTo() is True
         assert qpath.elementAt(2).isMoveTo() is True
         assert qpath.elementAt(3).isLineTo() is True
 
     def test_one_multi_paths(self):
         p = path.Path()
         p.line_to((4, 5, 6))
         p.move_to((0, 0, 0))
         p.line_to((7, 8, 6))
-        qpath = path.to_qpainter_path([p])
+        qpath = npshapes.to_qpainter_path([npshapes.NumpyPath2d(p)])
         assert qpath.elementCount() == 4
         assert qpath.elementAt(0).isMoveTo() is True
         assert qpath.elementAt(1).isLineTo() is True
         assert qpath.elementAt(2).isMoveTo() is True
         assert qpath.elementAt(3).isLineTo() is True
 
+
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_708f_path_nesting.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         id="2 separated sub-paths",
     ),
 ]
 
 
 @pytest.mark.parametrize("paths,polygons", DETECTION_DATA)
 def test_fast_bbox_detection(paths, polygons):
-    assert nesting.fast_bbox_detection(paths) == polygons
+    assert nesting.make_polygon_structure(paths) == polygons
 
 
 @pytest.mark.parametrize(
     "polygons,exp_ccw,exp_cw",
     [
         pytest.param(
             [[EXT1_PATH]],
```

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_711_points.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.1.0b4/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_811a_drawing_frontend.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_811a_drawing_frontend.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 
 import pytest
 import ezdxf
-from ezdxf.addons.drawing import Frontend, RenderContext
+from ezdxf.math import Vec2
+from ezdxf.addons.drawing import RenderContext, Frontend
 from ezdxf.addons.drawing.properties import BackendProperties
 
-from ezdxf.addons.drawing.backend import Backend
+from ezdxf.addons.drawing.backend import Backend, BkPath2d
 from ezdxf.addons.drawing.debug_backend import BasicBackend, PathBackend
 from ezdxf.entities import DXFGraphic
 from ezdxf.render.forms import cube
-from ezdxf.path import from_vertices
+
+
+class MyTestFrontend(Frontend):
+    def __init__(self, ctx, backend):
+        super().__init__(ctx, backend)
+        self.out = backend
 
 
 @pytest.fixture
 def doc():
     d = ezdxf.new()
     d.layers.new("Test1")
     d.styles.add("DEJAVU", font="DejaVuSans.ttf")
@@ -29,20 +35,20 @@
 @pytest.fixture
 def ctx(doc):
     return RenderContext(doc)
 
 
 @pytest.fixture
 def basic(doc, ctx):
-    return Frontend(ctx, BasicBackend())
+    return MyTestFrontend(ctx, BasicBackend())
 
 
 @pytest.fixture
 def path_backend(doc, ctx):
-    return Frontend(ctx, PathBackend())
+    return MyTestFrontend(ctx, PathBackend())
 
 
 def unique_types(result):
     return {e[0] for e in result}
 
 
 def get_result(frontend):
@@ -51,15 +57,15 @@
 
 def test_basic_frontend_init(basic):
     assert isinstance(basic.out, BasicBackend)
 
 
 def test_backend_default_draw_path():
     backend = BasicBackend()
-    path = from_vertices([(0, 0), (1, 0), (2, 0)])
+    path = BkPath2d.from_vertices(Vec2.list([(0, 0), (1, 0), (2, 0)]))
     backend.draw_path(path, BackendProperties())
     result = backend.collector
     assert len(result) == 2
     assert result[0][0] == "line"
 
 
 def test_draw_layout(msp, basic):
@@ -222,15 +228,15 @@
         radius=2,
         start_angle=30,
         end_angle=60,
         dxfattribs={"extrusion": (0, 1, 1)},
     )
     basic.draw_entities(msp)
     result = get_result(basic)
-    assert len(result) > 10
+    assert len(result) >= 4
     assert unique_types(result) == {"line"}
 
 
 def test_3d_arc_path(msp, path_backend):
     msp.add_arc(
         (0, 0),
         radius=2,
@@ -251,15 +257,15 @@
         ratio=0.5,
         start_param=1,
         end_param=2,
         dxfattribs={"extrusion": (0, 1, 1)},
     )
     basic.draw_entities(msp)
     result = get_result(basic)
-    assert len(result) > 10
+    assert len(result) >= 4
     assert unique_types(result) == {"line"}
 
 
 def test_3d_ellipse_path(msp, path_backend):
     msp.add_ellipse(
         (0, 0),
         major_axis=(1, 0, 0),
@@ -295,15 +301,15 @@
 
 def test_mtext(msp, basic):
     # since v1.0.4 the frontend does the text rendering and passes only filled
     # polygons to the backend
     msp.add_mtext("line1\nline2", dxfattribs={"style": "DEJAVU"})
     basic.draw_entities(msp)
     result = get_result(basic)
-    assert len(result) == 12
+    assert len(result) == 10  # each character is now one multi-path: changed in v1.1.0b4
     assert result[0][0] == "filled_polygon"
 
 
 def test_hatch(msp, path_backend):
     hatch = msp.add_hatch()
     hatch.paths.add_polyline_path([(0, 0), (1, 0), (1, 1), (0, 1)])
     path_backend.draw_entities(msp)
@@ -339,15 +345,15 @@
     result = get_result(basic)
     assert len(result) == 24
     entities = {e[0] for e in result}
     assert entities == {"line"}
 
 
 def test_override_filter(msp, ctx):
-    class FrontendWithOverride(Frontend):
+    class FrontendWithOverride(MyTestFrontend):
         def __init__(self, ctx: RenderContext, out: Backend):
             super().__init__(ctx, out)
             self.override_enabled = True
 
         def override_properties(
             self, entity: DXFGraphic, properties: BackendProperties
         ) -> None:
```

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_811c_viewport_processing.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_811c_viewport_processing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_813_geo_interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -61,14 +61,26 @@
 }
 
 FEATURE_COLLECTION = {
     "type": "FeatureCollection",
     "features": [FEATURE_1, FEATURE_2],
 }
 
+FEATURE_PROPERTIES = {
+    "type": "Feature",
+    "properties": {"layer": "GeoJSON"},
+    "geometry": LINE_STRING,
+}
+
+FEATURE_PROPERTIES_GC = {
+    "type": "Feature",
+    "properties": {"layer": "GeoJSON"},
+    "geometry": GEOMETRY_COLLECTION,
+}
+
 
 @pytest.mark.parametrize(
     "points",
     [
         [],
         [(0, 0)],
         [(0, 0), (1, 0)],
@@ -240,19 +252,33 @@
 
 
 def test_parse_feature():
     feature = geo.parse(FEATURE_1)
     assert feature["geometry"] == LINE_STRING
 
 
+def test_feature_with_geometry_collection():
+    feature = geo.parse(FEATURE_PROPERTIES_GC)
+    geometry_collection = feature["geometry"]
+    assert geometry_collection["type"] == "GeometryCollection"
+    geometries = geometry_collection["geometries"]
+    assert isinstance(geometries, list)
+
+
 def test_parse_feature_collection():
     feature_collection = geo.parse(FEATURE_COLLECTION)
     assert len(feature_collection["features"]) == 2
 
 
+def test_iter_feature_with_geometry_collection():
+    gp = geo.GeoProxy(FEATURE_PROPERTIES_GC)
+    entities = list(gp)
+    assert len(entities) == 3
+
+
 @pytest.mark.parametrize(
     "entity",
     [
         POINT,
         LINE_STRING,
         POLYGON_0,
         POLYGON_1,
@@ -279,29 +305,25 @@
     res = cast(LWPolyline, list(geo.dxf_entities(LINE_STRING))[0])
     assert res.dxftype() == "LWPOLYLINE"
     assert list(res.vertices()) == Vec3.list(EXTERIOR)
 
 
 @pytest.mark.parametrize("dxftype, polygon", [("HATCH", 1), ("MPOLYGON", 4)])
 def test_polygon_without_holes_to_dxf_polygon(dxftype, polygon):
-    entity = cast(
-        DXFPolygon, list(geo.dxf_entities(POLYGON_0, polygon=polygon))[0]
-    )
+    entity = cast(DXFPolygon, list(geo.dxf_entities(POLYGON_0, polygon=polygon))[0])
     assert entity.dxftype() == dxftype
     assert len(entity.paths) == 1
     p = entity.paths[0]
     assert p.type == BoundaryPathType.POLYLINE
     assert p.vertices == Vec3.list(EXTERIOR)
 
 
 @pytest.mark.parametrize("dxftype, polygon", [("HATCH", 1), ("MPOLYGON", 4)])
 def test_polygon_with_holes_to_dxf_polygon(dxftype, polygon):
-    entity = cast(
-        DXFPolygon, list(geo.dxf_entities(POLYGON_2, polygon=polygon))[0]
-    )
+    entity = cast(DXFPolygon, list(geo.dxf_entities(POLYGON_2, polygon=polygon))[0])
     assert entity.dxftype() == dxftype
     assert len(entity.paths) == 3
     p = entity.paths[1]
     assert p.type == BoundaryPathType.POLYLINE
     assert p.vertices == Vec3.list(HOLE1)
     p = entity.paths[2]
     assert p.type == BoundaryPathType.POLYLINE
@@ -331,14 +353,31 @@
 
 def test_feature_collection_to_dxf_entities():
     collection = list(geo.dxf_entities(FEATURE_COLLECTION))
     assert len(collection) == 2
     assert collection[0].dxftype() == "LWPOLYLINE"
 
 
+def test_dxf_entities_post_process_properties():
+    entities = list(
+        geo.dxf_entities(FEATURE_PROPERTIES, post_process=geo.assign_layers)
+    )
+    polyline = entities[0]
+    assert polyline.dxf.layer == "GeoJSON"
+
+
+def test_dxf_entities_from_geometry_collection_post_process_properties():
+    entities = list(
+        geo.dxf_entities(FEATURE_PROPERTIES_GC, post_process=geo.assign_layers)
+    )
+    assert len(entities) == 3
+    for e in entities:
+        assert e.dxf.layer == "GeoJSON"
+
+
 @pytest.mark.parametrize(
     "deg, coords",
     [
         [(15, 47), (1669792.36, 5910809.62)],
         [(-15, 47), (-1669792.36, 5910809.62)],
         [(15, -47), (1669792.36, -5910809.62)],
         [(-15, -47), (-1669792.36, -5910809.62)],
```

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_814_text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_822_clipper.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_822_clipper.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import pytest
 
 
 from ezdxf.addons.drawing.clipper import ClippingRect
 from ezdxf.math import Vec2
 from ezdxf.path import rect
+from ezdxf import npshapes
 
 
 def test_clipping_points():
     clipper = ClippingRect()
     clipper.push(rect(2, 2), None)
     assert clipper.clip_point(Vec2(3, 3)) is None
     assert clipper.clip_point(Vec2(0.5, 0.5)).isclose((0.5, 0.5))
@@ -25,14 +26,14 @@
     assert start.isclose((-1, 0))
     assert end.isclose((1, 0))
 
 
 def test_clip_polyline():
     clipper = ClippingRect()
     clipper.push(rect(4, 4), None)
-    polyline = Vec2.list([(0, 1), (3, 0), (0, -1)])
+    polyline = npshapes.NumpyPoints2d(Vec2.list([(0, 1), (3, 0), (0, -1)]))
     result = clipper.clip_polygon(polyline)
     assert len(result) == 4
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_823_drawing_layout.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_823_drawing_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_824_svg_drawing_backend.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_824_svg_drawing_backend.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 
 import pytest
 from xml.etree import ElementTree as ET
 
 from ezdxf.math import Vec2
+from ezdxf.npshapes import NumpyPoints2d
 from ezdxf.addons.drawing import svg, layout
 from ezdxf.addons.drawing.properties import BackendProperties
 
 
 class TestStyles:
     @pytest.fixture
     def xml(self):
@@ -60,15 +61,15 @@
 
 
 class TestSVGBackend:
     @pytest.fixture
     def backend(self):
         backend_ = svg.SVGBackend()
         properties = BackendProperties(color="#ff0000", lineweight=0.25)
-        points = Vec2.list([(0, 0), (100, 0), (100, 100), (0, 100)])
+        points = NumpyPoints2d(Vec2.list([(0, 0), (100, 0), (100, 100), (0, 100)]))
         backend_.draw_filled_polygon(points, properties)
         return backend_
 
     def test_get_xml_root_element(self, backend):
         xml = backend.get_xml_root_element(layout.Page(400, 300))
         assert xml.tag.endswith("svg") is True
         assert xml.attrib["width"] == "400mm"
```

## Comparing `ezdxf-1.1.0b3/tests/test_08_addons/test_825_hpgl2_drawing_backend.py` & `ezdxf-1.1.0b4/tests/test_08_addons/test_825_hpgl2_drawing_backend.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 
 import pytest
 
 from ezdxf.math import Vec2
-from ezdxf.path import Path2d
+from ezdxf.path import Path
+from ezdxf.npshapes import NumpyPath2d
 from ezdxf.addons.drawing import hpgl2, layout
 from ezdxf.addons.drawing.properties import BackendProperties
 
 
 def test_empty_page():
     backend = hpgl2.PlotterBackend()
     backend.draw_point(Vec2(0, 0), BackendProperties())
@@ -43,18 +44,18 @@
     def test_pen_width_command_exist(self, result1):
         assert b"PW0.25;" in result1
 
     def test_lines_are_7_bit_int_base_32_polyline_encoded(self, result1):
         assert b"PE7<=__?Yf?Yf;" in result1
 
     def test_curves_are_ascii_encoded_relative_bezier_curves(self, properties):
-        path = Path2d((0, 0))
+        path = Path((0, 0))
         path.curve4_to((100, 100), (25, 0), (75, 100))
         backend = hpgl2.PlotterBackend()
-        backend.draw_path(path, properties)
+        backend.draw_path(NumpyPath2d(path), properties)
         result = backend.high_quality(layout.Page(0, 0))
         assert b"PU;PA0,0;PD;BR1000,0,3000,4000,4000,4000;PU;" in result
 
 
 if __name__ == '__main__':
     pytest.main([__file__])
```

## Comparing `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.1.0b4/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_873_circle_inverted_normal.py` & `ezdxf-1.1.0b4/tests/test_10_issues/test_issue_873_circle_inverted_normal.py`

 * *Files identical despite different names*

