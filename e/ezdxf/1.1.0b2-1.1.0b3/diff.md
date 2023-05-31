# Comparing `tmp/ezdxf-1.1.0b2.zip` & `tmp/ezdxf-1.1.0b3.zip`

## zipinfo {}

```diff
@@ -1,840 +1,841 @@
-Zip file size: 2098898 bytes, number of entries: 838
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/
--rw-rw-rw-  2.0 fat     1092 b- defN 23-May-20 08:27 ezdxf-1.1.0b2/LICENSE
--rw-rw-rw-  2.0 fat      302 b- defN 23-May-20 08:27 ezdxf-1.1.0b2/MANIFEST.in
--rw-rw-rw-  2.0 fat   101467 b- defN 23-May-20 08:27 ezdxf-1.1.0b2/NEWS.md
--rw-rw-rw-  2.0 fat    69334 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/PKG-INFO
--rw-rw-rw-  2.0 fat     6142 b- defN 23-May-20 08:27 ezdxf-1.1.0b2/README.md
--rw-rw-rw-  2.0 fat       55 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/requirements.txt
--rw-rw-rw-  2.0 fat       74 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/setup.cfg
--rw-rw-rw-  2.0 fat     5402 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/setup.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/
--rw-rw-rw-  2.0 fat      567 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_config_file.py
--rw-rw-rw-  2.0 fat      541 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_env_var.py
--rw-rw-rw-  2.0 fat      410 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/conftest.py
--rw-rw-rw-  2.0 fat     1054 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_acad_table.py
--rw-rw-rw-  2.0 fat     4686 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_all_dimline_styles.py
--rw-rw-rw-  2.0 fat     4133 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_all_ellipse_transformations.py
--rw-rw-rw-  2.0 fat     1064 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_anonymous_blocks.py
--rw-rw-rw-  2.0 fat      871 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_audit_critical_dxf_files.py
--rw-rw-rw-  2.0 fat     1603 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_audit_layouts.py
--rw-rw-rw-  2.0 fat     1726 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_complex_line_type_2.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_create_basic_graphics.py
--rw-rw-rw-  2.0 fat     1921 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_document_guid.py
--rw-rw-rw-  2.0 fat     1832 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_document_page_setup.py
--rw-rw-rw-  2.0 fat      998 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_dxf_info_scanning.py
--rw-rw-rw-  2.0 fat     1558 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_entities_iterator.py
--rw-rw-rw-  2.0 fat      934 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_fix_dulicate_handles.py
--rw-rw-rw-  2.0 fat     1901 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_geo.py
--rw-rw-rw-  2.0 fat     1250 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_groups.py
--rw-rw-rw-  2.0 fat      901 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_hpgl2_addon.py
--rw-rw-rw-  2.0 fat      630 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_ignore_junk_beyond_EOF.py
--rw-rw-rw-  2.0 fat     1155 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_launcher.py
--rw-rw-rw-  2.0 fat      631 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_leica_disto_r12.py
--rw-rw-rw-  2.0 fat      737 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_load_dxf_unicode_notation.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_mapbox_earcut.py
--rw-rw-rw-  2.0 fat     2230 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_mtext_columns.py
--rw-rw-rw-  2.0 fat     2392 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_mtext_explode_addon.py
--rw-rw-rw-  2.0 fat     1846 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_mtext_text_frame.py
--rw-rw-rw-  2.0 fat     1053 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_new_table_entries.py
--rw-rw-rw-  2.0 fat      887 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_none_ascii_read_write.py
--rw-rw-rw-  2.0 fat     3435 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_odafc.py
--rw-rw-rw-  2.0 fat     1737 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_open_binary_DXF_files.py
--rw-rw-rw-  2.0 fat      751 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_open_coord_order_issue.py
--rw-rw-rw-  2.0 fat     3842 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_open_exotic_dxf_files.py
--rw-rw-rw-  2.0 fat      879 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_open_R13_R14.py
--rw-rw-rw-  2.0 fat     3152 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_polyline_entity.py
--rw-rw-rw-  2.0 fat     1749 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_preserve_binary_data_in_xrecords.py
--rw-rw-rw-  2.0 fat     6944 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_r12export.py
--rw-rw-rw-  2.0 fat     6256 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_r12strict.py
--rw-rw-rw-  2.0 fat     3410 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_r12writer.py
--rw-rw-rw-  2.0 fat      567 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_read_file_without_handles.py
--rw-rw-rw-  2.0 fat     1121 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_read_write_modern_entites.py
--rw-rw-rw-  2.0 fat     5375 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_recover.py
--rw-rw-rw-  2.0 fat     1959 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_redraw_order.py
--rw-rw-rw-  2.0 fat     1819 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_rotated_block_attributes.py
--rw-rw-rw-  2.0 fat      774 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_surface_entities.py
--rw-rw-rw-  2.0 fat      928 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_write_fixed_meta_data.py
--rw-rw-rw-  2.0 fat     1806 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_write_without_handles.py
--rw-rw-rw-  2.0 fat     3638 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/test_xref_detach.py
--rw-rw-rw-  2.0 fat     3060 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/AC1003_LINE_Example.dxf
--rw-rw-rw-  2.0 fat   179505 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/acad_table_with_blk_ref.dxf
--rw-rw-rw-  2.0 fat     7956 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/ASCII_R12.dxf
--rw-rw-rw-  2.0 fat     3761 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r12.dxf
--rw-rw-rw-  2.0 fat    20914 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r13.dxf
--rw-rw-rw-  2.0 fat    21137 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r14.dxf
--rw-rw-rw-  2.0 fat    11564 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r2000.dxf
--rw-rw-rw-  2.0 fat     6424 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/cc_dxflib.dxf
--rw-rw-rw-  2.0 fat   173753 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/custom_blocks.dxf
--rw-rw-rw-  2.0 fat    32203 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/duplicate_handles.dxf
--rw-rw-rw-  2.0 fat    18554 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/dxf_unicode.dxf
--rw-rw-rw-  2.0 fat     1592 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/empty_handles.dxf
--rw-rw-rw-  2.0 fat    97103 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/groups.dxf
--rw-rw-rw-  2.0 fat     9146 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/Leica_Disto_S910.dxf
--rw-rw-rw-  2.0 fat    17986 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/MODEL.dxf
--rw-rw-rw-  2.0 fat    25799 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2007.dxf
--rw-rw-rw-  2.0 fat    23927 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2018.dxf
--rw-rw-rw-  2.0 fat    98230 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/mtext_framed_columns.dxf
--rw-rw-rw-  2.0 fat   106574 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/mtext_text_frame.dxf
--rw-rw-rw-  2.0 fat    12001 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/no_layouts.dxf
--rw-rw-rw-  2.0 fat    16295 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/PLOTFILE.plt
--rw-rw-rw-  2.0 fat    28788 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/POLI-ALL210_12.DXF
--rw-rw-rw-  2.0 fat      144 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/R12_with_trash_beyond_EOF.dxf
--rw-rw-rw-  2.0 fat   212407 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/recover01.dxf
--rw-rw-rw-  2.0 fat   115423 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/recover02.dxf
--rw-rw-rw-  2.0 fat    21178 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/small_r13.dxf
--rw-rw-rw-  2.0 fat    10326 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/small_r14.dxf
--rw-rw-rw-  2.0 fat    11286 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/XRECORD_0.bin
--rw-rw-rw-  2.0 fat    11662 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/XRECORD_1.bin
--rw-rw-rw-  2.0 fat    15337 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/integration_tests/data/XRECORD_2.bin
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/
--rw-rw-rw-  2.0 fat     4710 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/appsettings.py
--rw-rw-rw-  2.0 fat    19818 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/audit.py
--rw-rw-rw-  2.0 fat     5324 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/bbox.py
--rw-rw-rw-  2.0 fat     7888 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/blkrefs.py
--rw-rw-rw-  2.0 fat    13157 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/colors.py
--rw-rw-rw-  2.0 fat    32340 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/commands.py
--rw-rw-rw-  2.0 fat     1549 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/comments.py
--rw-rw-rw-  2.0 fat    22100 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/disassemble.py
--rw-rw-rw-  2.0 fat    52708 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/document.py
--rw-rw-rw-  2.0 fat      832 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/dwginfo.py
--rw-rw-rw-  2.0 fat    16248 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entitydb.py
--rw-rw-rw-  2.0 fat     7495 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/enums.py
--rw-rw-rw-  2.0 fat    13948 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/explode.py
--rw-rw-rw-  2.0 fat     1653 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/eztypes.py
--rw-rw-rw-  2.0 fat    10333 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/filemanagement.py
--rw-rw-rw-  2.0 fat    12157 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/gfxattribs.py
--rw-rw-rw-  2.0 fat   107500 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/graphicsfactory.py
--rw-rw-rw-  2.0 fat     3416 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/groupby.py
--rw-rw-rw-  2.0 fat     3241 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/npshapes.py
--rw-rw-rw-  2.0 fat     2567 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/protocols.py
--rw-rw-rw-  2.0 fat    33129 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/proxygraphic.py
--rw-rw-rw-  2.0 fat       95 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/py.typed
--rw-rw-rw-  2.0 fat    22499 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/query.py
--rw-rw-rw-  2.0 fat     2780 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/queryparser.py
--rw-rw-rw-  2.0 fat     9580 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/r12strict.py
--rw-rw-rw-  2.0 fat    30769 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/recover.py
--rw-rw-rw-  2.0 fat     3515 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/reorder.py
--rw-rw-rw-  2.0 fat    10364 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/transform.py
--rw-rw-rw-  2.0 fat     5750 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/units.py
--rw-rw-rw-  2.0 fat     8280 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/upright.py
--rw-rw-rw-  2.0 fat     9875 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/urecord.py
--rw-rw-rw-  2.0 fat     1024 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/version.py
--rw-rw-rw-  2.0 fat    63359 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/xref.py
--rw-rw-rw-  2.0 fat     2853 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/zoom.py
--rw-rw-rw-  2.0 fat    10986 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/_options.py
--rw-rw-rw-  2.0 fat     2566 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/__init__.py
--rw-rw-rw-  2.0 fat     3259 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/__main__.py
--rw-rw-rw-  2.0 fat     6072 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/bezier3p.pyx
--rw-rw-rw-  2.0 fat     9983 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/bezier4p.pyx
--rw-rw-rw-  2.0 fat    12964 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/bspline.pyx
--rw-rw-rw-  2.0 fat       90 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/construct.pxd
--rw-rw-rw-  2.0 fat     6584 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/construct.pyx
--rw-rw-rw-  2.0 fat     3113 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/linetypes.pyx
--rw-rw-rw-  2.0 fat    23989 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/mapbox_earcut.pyx
--rw-rw-rw-  2.0 fat      386 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pxd
--rw-rw-rw-  2.0 fat    23742 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pyx
--rw-rw-rw-  2.0 fat     2014 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/vector.pxd
--rw-rw-rw-  2.0 fat    23705 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/vector.pyx
--rw-rw-rw-  2.0 fat     1784 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.cpp
--rw-rw-rw-  2.0 fat      599 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.hpp
--rw-rw-rw-  2.0 fat      424 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.pxd
--rw-rw-rw-  2.0 fat      960 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.cpp
--rw-rw-rw-  2.0 fat      464 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.hpp
--rw-rw-rw-  2.0 fat      407 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.pxd
--rw-rw-rw-  2.0 fat     2135 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.hpp
--rw-rw-rw-  2.0 fat      572 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.pxd
--rw-rw-rw-  2.0 fat     1265 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acc/__init__.py
--rw-rw-rw-  2.0 fat     6393 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/abstract.py
--rw-rw-rw-  2.0 fat      884 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/api.py
--rw-rw-rw-  2.0 fat     5484 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/const.py
--rw-rw-rw-  2.0 fat     6726 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/dbg.py
--rw-rw-rw-  2.0 fat     2980 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/dxf.py
--rw-rw-rw-  2.0 fat    28991 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/entities.py
--rw-rw-rw-  2.0 fat     4088 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/hdr.py
--rw-rw-rw-  2.0 fat    12823 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/mesh.py
--rw-rw-rw-  2.0 fat    18690 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/sab.py
--rw-rw-rw-  2.0 fat    13184 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/sat.py
--rw-rw-rw-  2.0 fat      115 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/acis/__init__.py
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/
--rw-rw-rw-  2.0 fat    26415 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acadctb.py
--rw-rw-rw-  2.0 fat    22229 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/binpacking.py
--rw-rw-rw-  2.0 fat    27692 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dimlines.py
--rw-rw-rw-  2.0 fat    31371 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dxf2code.py
--rw-rw-rw-  2.0 fat    22037 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/genetic_algorithm.py
--rw-rw-rw-  2.0 fat    36445 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/geo.py
--rw-rw-rw-  2.0 fat     2674 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/gerber_D6673.py
--rw-rw-rw-  2.0 fat    25472 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/importer.py
--rw-rw-rw-  2.0 fat    17355 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/iterdxf.py
--rw-rw-rw-  2.0 fat     8940 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/menger_sponge.py
--rw-rw-rw-  2.0 fat    24787 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/meshex.py
--rw-rw-rw-  2.0 fat      492 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/mixins.py
--rw-rw-rw-  2.0 fat     6203 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/mtextsurrogate.py
--rw-rw-rw-  2.0 fat    13528 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/mtxpl.py
--rw-rw-rw-  2.0 fat    16400 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/odafc.py
--rw-rw-rw-  2.0 fat     9456 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/openscad.py
--rw-rw-rw-  2.0 fat    15878 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/pycsg.py
--rw-rw-rw-  2.0 fat    22496 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/r12export.py
--rw-rw-rw-  2.0 fat    27198 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/r12writer.py
--rw-rw-rw-  2.0 fat     7615 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/sierpinski_pyramid.py
--rw-rw-rw-  2.0 fat    33167 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/tablepainter.py
--rw-rw-rw-  2.0 fat    12789 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/text2path.py
--rw-rw-rw-  2.0 fat     3623 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/xplayer.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/xqt.py
--rw-rw-rw-  2.0 fat      453 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/__init__.py
--rw-rw-rw-  2.0 fat    10023 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/browser.py
--rw-rw-rw-  2.0 fat     1907 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/data.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/__init__.py
--rw-rw-rw-  2.0 fat      820 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/bookmarks.py
--rw-rw-rw-  2.0 fat    29367 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/browser.py
--rw-rw-rw-  2.0 fat    14891 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/data.py
--rw-rw-rw-  2.0 fat    10993 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/find_dialog.py
--rw-rw-rw-  2.0 fat     1281 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/loader.py
--rw-rw-rw-  2.0 fat    20974 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/model.py
--rw-rw-rw-  2.0 fat     2214 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/tags.py
--rw-rw-rw-  2.0 fat     1382 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/views.py
--rw-rw-rw-  2.0 fat      133 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/browser/__init__.py
--rw-rw-rw-  2.0 fat     7319 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/backend.py
--rw-rw-rw-  2.0 fat     3960 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/clipper.py
--rw-rw-rw-  2.0 fat     8991 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/config.py
--rw-rw-rw-  2.0 fat     1707 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_backend.py
--rw-rw-rw-  2.0 fat      514 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_utils.py
--rw-rw-rw-  2.0 fat    44702 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/frontend.py
--rw-rw-rw-  2.0 fat     1823 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/gfxproxy.py
--rw-rw-rw-  2.0 fat    14228 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/layout.py
--rw-rw-rw-  2.0 fat    12660 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/matplotlib.py
--rw-rw-rw-  2.0 fat     9878 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/mtext_complex.py
--rw-rw-rw-  2.0 fat    39035 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/properties.py
--rw-rw-rw-  2.0 fat    11034 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/pyqt.py
--rw-rw-rw-  2.0 fat    22624 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/qtviewer.py
--rw-rw-rw-  2.0 fat     8944 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/recorder.py
--rw-rw-rw-  2.0 fat    14774 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/svg.py
--rw-rw-rw-  2.0 fat    13023 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text.py
--rw-rw-rw-  2.0 fat      963 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text_renderer.py
--rw-rw-rw-  2.0 fat      344 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/type_hints.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/unified_text_renderer.py
--rw-rw-rw-  2.0 fat      171 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/drawing/__init__.py
--rw-rw-rw-  2.0 fat     3112 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/classes_section.py
--rw-rw-rw-  2.0 fat      763 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/const.py
--rw-rw-rw-  2.0 fat     6091 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/crc.py
--rw-rw-rw-  2.0 fat     3160 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/fileheader.py
--rw-rw-rw-  2.0 fat    14851 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/header_section.py
--rw-rw-rw-  2.0 fat     2976 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/loader.py
--rw-rw-rw-  2.0 fat      141 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/dwg/__init__.py
--rw-rw-rw-  2.0 fat     9537 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/api.py
--rw-rw-rw-  2.0 fat     8208 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/backend.py
--rw-rw-rw-  2.0 fat      513 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/compiler.py
--rw-rw-rw-  2.0 fat      571 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/deps.py
--rw-rw-rw-  2.0 fat     4720 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/dxf_backend.py
--rw-rw-rw-  2.0 fat    16087 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/interpreter.py
--rw-rw-rw-  2.0 fat     4836 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/page.py
--rw-rw-rw-  2.0 fat     3527 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/pdf_backend.py
--rw-rw-rw-  2.0 fat    11957 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/plotter.py
--rw-rw-rw-  2.0 fat     1411 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/polygon_buffer.py
--rw-rw-rw-  2.0 fat     5953 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/properties.py
--rw-rw-rw-  2.0 fat     3731 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/svg_backend.py
--rw-rw-rw-  2.0 fat     6258 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/tokenizer.py
--rw-rw-rw-  2.0 fat    14190 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/viewer.py
--rw-rw-rw-  2.0 fat      164 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/__init__.py
--rw-rw-rw-  2.0 fat     4757 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/acad_proxy_entity.py
--rw-rw-rw-  2.0 fat    18315 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/acad_table.py
--rw-rw-rw-  2.0 fat    25923 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/acis.py
--rw-rw-rw-  2.0 fat     4890 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/appdata.py
--rw-rw-rw-  2.0 fat     1954 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/appid.py
--rw-rw-rw-  2.0 fat     4942 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/arc.py
--rw-rw-rw-  2.0 fat    26138 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/attrib.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/block.py
--rw-rw-rw-  2.0 fat    10536 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/blockrecord.py
--rw-rw-rw-  2.0 fat    50143 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/boundary_paths.py
--rw-rw-rw-  2.0 fat     7961 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/circle.py
--rw-rw-rw-  2.0 fat    23664 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dictionary.py
--rw-rw-rw-  2.0 fat    48743 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dimension.py
--rw-rw-rw-  2.0 fat    35012 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dimstyle.py
--rw-rw-rw-  2.0 fat    23829 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dimstyleoverride.py
--rw-rw-rw-  2.0 fat     4399 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfclass.py
--rw-rw-rw-  2.0 fat    42404 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfentity.py
--rw-rw-rw-  2.0 fat    26923 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfgfx.py
--rw-rw-rw-  2.0 fat    15279 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfgroups.py
--rw-rw-rw-  2.0 fat    23699 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfns.py
--rw-rw-rw-  2.0 fat    13746 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/dxfobj.py
--rw-rw-rw-  2.0 fat    11186 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/ellipse.py
--rw-rw-rw-  2.0 fat     4170 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/factory.py
--rw-rw-rw-  2.0 fat    23785 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/geodata.py
--rw-rw-rw-  2.0 fat     4020 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/gradient.py
--rw-rw-rw-  2.0 fat    12263 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/hatch.py
--rw-rw-rw-  2.0 fat     3944 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/helix.py
--rw-rw-rw-  2.0 fat     4747 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/idbuffer.py
--rw-rw-rw-  2.0 fat    26057 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/image.py
--rw-rw-rw-  2.0 fat    27932 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/insert.py
--rw-rw-rw-  2.0 fat    27834 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/layer.py
--rw-rw-rw-  2.0 fat    14252 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/layout.py
--rw-rw-rw-  2.0 fat    12978 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/leader.py
--rw-rw-rw-  2.0 fat     4718 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/light.py
--rw-rw-rw-  2.0 fat     3718 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/line.py
--rw-rw-rw-  2.0 fat     9677 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/ltype.py
--rw-rw-rw-  2.0 fat    18878 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/lwpolyline.py
--rw-rw-rw-  2.0 fat    19653 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/material.py
--rw-rw-rw-  2.0 fat    18435 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mesh.py
--rw-rw-rw-  2.0 fat    57367 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mleader.py
--rw-rw-rw-  2.0 fat    37144 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mline.py
--rw-rw-rw-  2.0 fat     8385 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mpolygon.py
--rw-rw-rw-  2.0 fat    48153 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mtext.py
--rw-rw-rw-  2.0 fat     4351 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/mtext_columns.py
--rw-rw-rw-  2.0 fat     6284 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/objectcollection.py
--rw-rw-rw-  2.0 fat     2111 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/oleframe.py
--rw-rw-rw-  2.0 fat     4332 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/pattern.py
--rw-rw-rw-  2.0 fat     5238 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/point.py
--rw-rw-rw-  2.0 fat    16416 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/polygon.py
--rw-rw-rw-  2.0 fat    40087 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/polyline.py
--rw-rw-rw-  2.0 fat     4822 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/shape.py
--rw-rw-rw-  2.0 fat    10443 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/solid.py
--rw-rw-rw-  2.0 fat    24085 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/spline.py
--rw-rw-rw-  2.0 fat     8246 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/subentity.py
--rw-rw-rw-  2.0 fat     5196 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/sun.py
--rw-rw-rw-  2.0 fat     2449 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/table.py
--rw-rw-rw-  2.0 fat    17602 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/text.py
--rw-rw-rw-  2.0 fat     9035 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/textstyle.py
--rw-rw-rw-  2.0 fat     3597 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/tolerance.py
--rw-rw-rw-  2.0 fat     2703 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/ucs.py
--rw-rw-rw-  2.0 fat    14366 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/underlay.py
--rw-rw-rw-  2.0 fat     6040 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/view.py
--rw-rw-rw-  2.0 fat    28177 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/viewport.py
--rw-rw-rw-  2.0 fat     7867 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/visualstyle.py
--rw-rw-rw-  2.0 fat     9970 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/vport.py
--rw-rw-rw-  2.0 fat    17024 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/xdata.py
--rw-rw-rw-  2.0 fat     8495 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/xdict.py
--rw-rw-rw-  2.0 fat     3062 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/xline.py
--rw-rw-rw-  2.0 fat     3127 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/entities/__init__.py
--rw-rw-rw-  2.0 fat    23474 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/fonts.py
--rw-rw-rw-  2.0 fat     2242 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/font_face.py
--rw-rw-rw-  2.0 fat    17004 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/font_manager.py
--rw-rw-rw-  2.0 fat     1702 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/font_measurements.py
--rw-rw-rw-  2.0 fat      825 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/glyphs.py
--rw-rw-rw-  2.0 fat    10794 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/lff.py
--rw-rw-rw-  2.0 fat    35217 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/shapefile.py
--rw-rw-rw-  2.0 fat     7219 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/ttfonts.py
--rw-rw-rw-  2.0 fat       64 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/fonts/__init__.py
--rw-rw-rw-  2.0 fat    16696 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/base.py
--rw-rw-rw-  2.0 fat     4343 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/blocklayout.py
--rw-rw-rw-  2.0 fat    29369 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/layout.py
--rw-rw-rw-  2.0 fat    15314 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/layouts.py
--rw-rw-rw-  2.0 fat      232 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/layouts/__init__.py
--rw-rw-rw-  2.0 fat     8327 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/attributes.py
--rw-rw-rw-  2.0 fat    16500 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/const.py
--rw-rw-rw-  2.0 fat     1614 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/encoding.py
--rw-rw-rw-  2.0 fat    17013 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/extendedtags.py
--rw-rw-rw-  2.0 fat     5363 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/fileindex.py
--rw-rw-rw-  2.0 fat      727 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/hdrvars.py
--rw-rw-rw-  2.0 fat     5469 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/loader.py
--rw-rw-rw-  2.0 fat     7447 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/packedtags.py
--rw-rw-rw-  2.0 fat     6355 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/repair.py
--rw-rw-rw-  2.0 fat    13058 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/tagger.py
--rw-rw-rw-  2.0 fat    14336 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/tags.py
--rw-rw-rw-  2.0 fat     8952 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/tagwriter.py
--rw-rw-rw-  2.0 fat    12064 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/types.py
--rw-rw-rw-  2.0 fat    17069 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/validator.py
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/lldxf/__init__.py
--rw-rw-rw-  2.0 fat    19193 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/arc.py
--rw-rw-rw-  2.0 fat    16270 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bbox.py
--rw-rw-rw-  2.0 fat     9318 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bezier.py
--rw-rw-rw-  2.0 fat     2452 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bezier_interpolation.py
--rw-rw-rw-  2.0 fat     8730 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/box.py
--rw-rw-rw-  2.0 fat    52916 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bspline.py
--rw-rw-rw-  2.0 fat     5608 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/bulge.py
--rw-rw-rw-  2.0 fat     9002 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/circle.py
--rw-rw-rw-  2.0 fat    24003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/clipping.py
--rw-rw-rw-  2.0 fat     4319 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/clustering.py
--rw-rw-rw-  2.0 fat    12236 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/construct2d.py
--rw-rw-rw-  2.0 fat    26265 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/construct3d.py
--rw-rw-rw-  2.0 fat     1283 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/cspline.py
--rw-rw-rw-  2.0 fat     9114 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/curvetools.py
--rw-rw-rw-  2.0 fat    22048 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/ellipse.py
--rw-rw-rw-  2.0 fat     4406 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/eulerspiral.py
--rw-rw-rw-  2.0 fat    38883 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/linalg.py
--rw-rw-rw-  2.0 fat    10231 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/line.py
--rw-rw-rw-  2.0 fat     3053 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/offset2d.py
--rw-rw-rw-  2.0 fat     8256 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/parametrize.py
--rw-rw-rw-  2.0 fat    15602 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/perlin.py
--rw-rw-rw-  2.0 fat    15921 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/polyline.py
--rw-rw-rw-  2.0 fat    11867 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/rtree.py
--rw-rw-rw-  2.0 fat     3910 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/shape.py
--rw-rw-rw-  2.0 fat     2568 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/surfaces.py
--rw-rw-rw-  2.0 fat    12155 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/transformtools.py
--rw-rw-rw-  2.0 fat     3631 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/triangulation.py
--rw-rw-rw-  2.0 fat    16971 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/ucs.py
--rw-rw-rw-  2.0 fat     7213 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_bezier3p.py
--rw-rw-rw-  2.0 fat    12967 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_bezier4p.py
--rw-rw-rw-  2.0 fat     9440 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_bspline.py
--rw-rw-rw-  2.0 fat     7272 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_construct.py
--rw-rw-rw-  2.0 fat     2261 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_ctypes.py
--rw-rw-rw-  2.0 fat    24954 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    27606 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_matrix44.py
--rw-rw-rw-  2.0 fat    25912 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/_vector.py
--rw-rw-rw-  2.0 fat     2003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/math/__init__.py
--rw-rw-rw-  2.0 fat     1306 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/commands.py
--rw-rw-rw-  2.0 fat    39194 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/converter.py
--rw-rw-rw-  2.0 fat     6748 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/nesting.py
--rw-rw-rw-  2.0 fat    20453 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/path.py
--rw-rw-rw-  2.0 fat    10140 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/shapes.py
--rw-rw-rw-  2.0 fat    34692 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/tools.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/path/__init__.py
--rw-rw-rw-  2.0 fat     2987 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.css
--rw-rw-rw-  2.0 fat     1148 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.html
--rw-rw-rw-  2.0 fat    11304 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.js
--rw-rw-rw-  2.0 fat    17144 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.py
--rw-rw-rw-  2.0 fat     3770 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/pprint.py
--rw-rw-rw-  2.0 fat      812 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.css
--rw-rw-rw-  2.0 fat      316 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.html
--rw-rw-rw-  2.0 fat     2545 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.py
--rw-rw-rw-  2.0 fat     6896 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/reflinks.py
--rw-rw-rw-  2.0 fat      123 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/pp/__init__.py
--rw-rw-rw-  2.0 fat    10039 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/abstract_mtext_renderer.py
--rw-rw-rw-  2.0 fat    20495 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/arrows.py
--rw-rw-rw-  2.0 fat    17749 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/curves.py
--rw-rw-rw-  2.0 fat     4041 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dimension.py
--rw-rw-rw-  2.0 fat    52028 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_base.py
--rw-rw-rw-  2.0 fat    35702 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_curved.py
--rw-rw-rw-  2.0 fat     6894 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_diameter.py
--rw-rw-rw-  2.0 fat    24751 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_linear.py
--rw-rw-rw-  2.0 fat     8084 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_ordinate.py
--rw-rw-rw-  2.0 fat    20295 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/dim_radius.py
--rw-rw-rw-  2.0 fat    47170 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/forms.py
--rw-rw-rw-  2.0 fat    24213 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/hatching.py
--rw-rw-rw-  2.0 fat     4728 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/leader.py
--rw-rw-rw-  2.0 fat      664 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/linetypes.py
--rw-rw-rw-  2.0 fat    64121 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/mesh.py
--rw-rw-rw-  2.0 fat    60923 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/mleader.py
--rw-rw-rw-  2.0 fat     8437 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/mline.py
--rw-rw-rw-  2.0 fat     2964 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/point.py
--rw-rw-rw-  2.0 fat     8736 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/polyline.py
--rw-rw-rw-  2.0 fat     7886 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/r12spline.py
--rw-rw-rw-  2.0 fat    22541 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/trace.py
--rw-rw-rw-  2.0 fat     2881 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/_linetypes.py
--rw-rw-rw-  2.0 fat      778 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/render/__init__.py
--rw-rw-rw-  2.0 fat     1050 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/16x16.png
--rw-rw-rw-  2.0 fat     1420 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/24x24.png
--rw-rw-rw-  2.0 fat    10638 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/256x256.png
--rw-rw-rw-  2.0 fat     1758 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/32x32.png
--rw-rw-rw-  2.0 fat     2335 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/48x48.png
--rw-rw-rw-  2.0 fat     3050 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/64x64.png
--rw-rw-rw-  2.0 fat     2090 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-copy-64px.png
--rw-rw-rw-  2.0 fat     3109 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-find-64px.png
--rw-rw-rw-  2.0 fat     2388 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-bookmark-64px.png
--rw-rw-rw-  2.0 fat     2519 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-handle-64px.png
--rw-rw-rw-  2.0 fat     2409 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-line-64px.png
--rw-rw-rw-  2.0 fat     2231 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-left-arrow-64px.png
--rw-rw-rw-  2.0 fat     2322 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-next-entity-64px.png
--rw-rw-rw-  2.0 fat     2320 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-prev-entity-64px.png
--rw-rw-rw-  2.0 fat     2244 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-right-arrow-64px.png
--rw-rw-rw-  2.0 fat     2553 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-show-in-tree-64px.png
--rw-rw-rw-  2.0 fat     2373 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/resources/icon-store-bookmark-64px.png
--rw-rw-rw-  2.0 fat    10650 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/acdsdata.py
--rw-rw-rw-  2.0 fat    16508 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/blocks.py
--rw-rw-rw-  2.0 fat    11639 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/classes.py
--rw-rw-rw-  2.0 fat     4137 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/entities.py
--rw-rw-rw-  2.0 fat    11953 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/header.py
--rw-rw-rw-  2.0 fat    60696 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/headervars.py
--rw-rw-rw-  2.0 fat    27009 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/objects.py
--rw-rw-rw-  2.0 fat    26581 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/table.py
--rw-rw-rw-  2.0 fat     5270 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/tables.py
--rw-rw-rw-  2.0 fat       67 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/sections/__init__.py
--rw-rw-rw-  2.0 fat    19711 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/analyze.py
--rw-rw-rw-  2.0 fat    20434 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/binarydata.py
--rw-rw-rw-  2.0 fat     2931 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/codepage.py
--rw-rw-rw-  2.0 fat     7645 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/complex_ltype.py
--rw-rw-rw-  2.0 fat     1782 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/crypt.py
--rw-rw-rw-  2.0 fat     1511 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/debug.py
--rw-rw-rw-  2.0 fat     2341 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/difftags.py
--rw-rw-rw-  2.0 fat     1235 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/handle.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/indexing.py
--rw-rw-rw-  2.0 fat     2145 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/juliandate.py
--rw-rw-rw-  2.0 fat     6166 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/pattern.py
--rw-rw-rw-  2.0 fat     1256 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/rawloader.py
--rw-rw-rw-  2.0 fat   129174 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/standards.py
--rw-rw-rw-  2.0 fat     6049 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/strip.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/test.py
--rw-rw-rw-  2.0 fat    65518 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/text.py
--rw-rw-rw-  2.0 fat    54234 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/text_layout.py
--rw-rw-rw-  2.0 fat     6893 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/text_size.py
--rw-rw-rw-  2.0 fat     3077 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/zipmanager.py
--rw-rw-rw-  2.0 fat   142734 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/_iso_pattern.py
--rw-rw-rw-  2.0 fat     3564 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf/tools/__init__.py
--rw-rw-rw-  2.0 fat        1 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/dependency_links.txt
--rw-rw-rw-  2.0 fat       47 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/entry_points.txt
--rw-rw-rw-  2.0 fat        2 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/not-zip-safe
--rw-rw-rw-  2.0 fat    69334 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/PKG-INFO
--rw-rw-rw-  2.0 fat      302 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/requires.txt
--rw-rw-rw-  2.0 fat    31795 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/SOURCES.txt
--rw-rw-rw-  2.0 fat        6 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/src/ezdxf.egg-info/top_level.txt
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/
-drwxrwxrwx  2.0 fat        0 b- stor 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/
--rw-rw-rw-  2.0 fat      410 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/conftest.py
--rw-rw-rw-  2.0 fat     2336 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
--rw-rw-rw-  2.0 fat      780 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
--rw-rw-rw-  2.0 fat     2599 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
--rw-rw-rw-  2.0 fat     1124 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
--rw-rw-rw-  2.0 fat     5456 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
--rw-rw-rw-  2.0 fat      582 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
--rw-rw-rw-  2.0 fat      473 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_011_codepage.py
--rw-rw-rw-  2.0 fat    11593 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_012_crypt.py
--rw-rw-rw-  2.0 fat     1191 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
--rw-rw-rw-  2.0 fat     1033 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
--rw-rw-rw-  2.0 fat     4792 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
--rw-rw-rw-  2.0 fat      989 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_016_encoding.py
--rw-rw-rw-  2.0 fat     1383 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_018_handle.py
--rw-rw-rw-  2.0 fat     5518 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
--rw-rw-rw-  2.0 fat     8168 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
--rw-rw-rw-  2.0 fat     3787 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
--rw-rw-rw-  2.0 fat      401 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
--rw-rw-rw-  2.0 fat      539 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
--rw-rw-rw-  2.0 fat     2092 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_040_tags.py
--rw-rw-rw-  2.0 fat     3073 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
--rw-rw-rw-  2.0 fat     6419 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
--rw-rw-rw-  2.0 fat     1632 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
--rw-rw-rw-  2.0 fat    11265 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
--rw-rw-rw-  2.0 fat     3363 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
--rw-rw-rw-  2.0 fat     1974 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
--rw-rw-rw-  2.0 fat     2321 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
--rw-rw-rw-  2.0 fat      568 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
--rw-rw-rw-  2.0 fat     8682 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
--rw-rw-rw-  2.0 fat     1051 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
--rw-rw-rw-  2.0 fat     1500 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
--rw-rw-rw-  2.0 fat    11689 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_101_dxfnamespace.py
--rw-rw-rw-  2.0 fat     2893 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_102_appdata.py
--rw-rw-rw-  2.0 fat     2312 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_103_reactors.py
--rw-rw-rw-  2.0 fat     4001 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_104_extension_dict.py
--rw-rw-rw-  2.0 fat    20860 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_105_xdata.py
--rw-rw-rw-  2.0 fat    14169 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_110_dxfentity.py
--rw-rw-rw-  2.0 fat     2433 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
--rw-rw-rw-  2.0 fat     6781 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112a_dxfgfx.py
--rw-rw-rw-  2.0 fat      695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112b_dxfobj.py
--rw-rw-rw-  2.0 fat     2431 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_113_dxfclass.py
--rw-rw-rw-  2.0 fat     4044 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_114_factory.py
--rw-rw-rw-  2.0 fat     2256 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
--rw-rw-rw-  2.0 fat    15794 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_116_dictionary.py
--rw-rw-rw-  2.0 fat     4999 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_117_layer_table_entry.py
--rw-rw-rw-  2.0 fat      385 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_118_appid_table_entry.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
--rw-rw-rw-  2.0 fat     3003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_120_style_table_entry.py
--rw-rw-rw-  2.0 fat     2943 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
--rw-rw-rw-  2.0 fat      379 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_122_vport_table_entry.py
--rw-rw-rw-  2.0 fat     1113 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_123_view_table_entry.py
--rw-rw-rw-  2.0 fat     8757 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
--rw-rw-rw-  2.0 fat     1698 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_125_image_def.py
--rw-rw-rw-  2.0 fat     1312 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_126_image_def_reactor.py
--rw-rw-rw-  2.0 fat     1430 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_127_raster_variables.py
--rw-rw-rw-  2.0 fat     1540 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_128_pdf_definition.py
--rw-rw-rw-  2.0 fat     2778 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_129_xrecord.py
--rw-rw-rw-  2.0 fat     2423 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_130_id_buffer.py
--rw-rw-rw-  2.0 fat     2470 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_131_field_list.py
--rw-rw-rw-  2.0 fat     2435 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_132_layer_filter.py
--rw-rw-rw-  2.0 fat     2153 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_133_sun.py
--rw-rw-rw-  2.0 fat      852 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_134_material.py
--rw-rw-rw-  2.0 fat    11497 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_135_geo_data.py
--rw-rw-rw-  2.0 fat     1087 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_136_vba_project.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_137_sortentstable.py
--rw-rw-rw-  2.0 fat      704 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
--rw-rw-rw-  2.0 fat     7570 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_139_user_record.py
--rw-rw-rw-  2.0 fat      714 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_140_block_record.py
--rw-rw-rw-  2.0 fat     9153 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_141_layer_vp_override.py
--rw-rw-rw-  2.0 fat     2231 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/conftest.py
--rw-rw-rw-  2.0 fat     6532 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_200_line.py
--rw-rw-rw-  2.0 fat     4273 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_201_point.py
--rw-rw-rw-  2.0 fat     6827 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_202_circle.py
--rw-rw-rw-  2.0 fat     8949 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_203_arc.py
--rw-rw-rw-  2.0 fat     2852 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_204_shape.py
--rw-rw-rw-  2.0 fat     8242 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_205_solid.py
--rw-rw-rw-  2.0 fat     8476 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_206_text.py
--rw-rw-rw-  2.0 fat     4947 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_207_attdef.py
--rw-rw-rw-  2.0 fat     6312 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_208_attrib.py
--rw-rw-rw-  2.0 fat     2671 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_209_vertex.py
--rw-rw-rw-  2.0 fat     5930 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_1.py
--rw-rw-rw-  2.0 fat    13489 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_2.py
--rw-rw-rw-  2.0 fat     6650 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_explode.py
--rw-rw-rw-  2.0 fat     1780 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
--rw-rw-rw-  2.0 fat     7847 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_211_viewport.py
--rw-rw-rw-  2.0 fat    12629 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_212_insert.py
--rw-rw-rw-  2.0 fat     6024 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_213_minsert.py
--rw-rw-rw-  2.0 fat     3284 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_214_block.py
--rw-rw-rw-  2.0 fat     6882 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_215_dimension.py
--rw-rw-rw-  2.0 fat     4907 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
--rw-rw-rw-  2.0 fat    13186 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
--rw-rw-rw-  2.0 fat     6471 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
--rw-rw-rw-  2.0 fat     5535 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
--rw-rw-rw-  2.0 fat     3056 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
--rw-rw-rw-  2.0 fat     7181 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
--rw-rw-rw-  2.0 fat     2066 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
--rw-rw-rw-  2.0 fat     3615 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
--rw-rw-rw-  2.0 fat     6919 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_221_ellipse.py
--rw-rw-rw-  2.0 fat     2223 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_222_xline.py
--rw-rw-rw-  2.0 fat     1493 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_223_ray.py
--rw-rw-rw-  2.0 fat     2176 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_224_group.py
--rw-rw-rw-  2.0 fat    10917 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_225_mtext.py
--rw-rw-rw-  2.0 fat    12020 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline.py
--rw-rw-rw-  2.0 fat     5529 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
--rw-rw-rw-  2.0 fat    10893 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
--rw-rw-rw-  2.0 fat    15116 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_228_mesh.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
--rw-rw-rw-  2.0 fat    21421 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
--rw-rw-rw-  2.0 fat     6587 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
--rw-rw-rw-  2.0 fat     3140 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
--rw-rw-rw-  2.0 fat    12486 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
--rw-rw-rw-  2.0 fat     2274 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay.py
--rw-rw-rw-  2.0 fat     5243 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay_2.py
--rw-rw-rw-  2.0 fat     2294 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis.py
--rw-rw-rw-  2.0 fat     6799 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis_2.py
--rw-rw-rw-  2.0 fat     1854 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_surface.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_233_helix.py
--rw-rw-rw-  2.0 fat     2040 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_234_light.py
--rw-rw-rw-  2.0 fat     3806 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_235_leader.py
--rw-rw-rw-  2.0 fat    20392 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_236_multileader.py
--rw-rw-rw-  2.0 fat    10992 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_237_mline.py
--rw-rw-rw-  2.0 fat     2356 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_238_tolerance.py
--rw-rw-rw-  2.0 fat    27392 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
--rw-rw-rw-  2.0 fat     4347 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_240_arc_dimension.py
--rw-rw-rw-  2.0 fat     1069 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_241_hyperlink.py
--rw-rw-rw-  2.0 fat    11313 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_242_random_transform.py
--rw-rw-rw-  2.0 fat     3725 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_243_replace_entity.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
--rw-rw-rw-  2.0 fat     4456 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_245_wipeout.py
--rw-rw-rw-  2.0 fat     6175 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_246_spline_audit.py
--rw-rw-rw-  2.0 fat     8165 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
--rw-rw-rw-  2.0 fat     6003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mpolygon.py
--rw-rw-rw-  2.0 fat    13682 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
--rw-rw-rw-  2.0 fat     5713 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_249_boundary_paths.py
--rw-rw-rw-  2.0 fat     8331 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
--rw-rw-rw-  2.0 fat     7331 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_251_upright.py
--rw-rw-rw-  2.0 fat     4795 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
--rw-rw-rw-  2.0 fat     2082 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_253_ole2frame.py
--rw-rw-rw-  2.0 fat      821 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_254_get_font_name.py
--rw-rw-rw-  2.0 fat     5149 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_300_layout.py
--rw-rw-rw-  2.0 fat     4274 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
--rw-rw-rw-  2.0 fat     5582 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_302_block_references.py
--rw-rw-rw-  2.0 fat     2695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_303_auto_block_references.py
--rw-rw-rw-  2.0 fat      913 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_304_new_entity_space.py
--rw-rw-rw-  2.0 fat     3279 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
--rw-rw-rw-  2.0 fat     2609 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
--rw-rw-rw-  2.0 fat     2343 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_307_groupby.py
--rw-rw-rw-  2.0 fat    17748 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_308_query.py
--rw-rw-rw-  2.0 fat     6382 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_309_query_parser.py
--rw-rw-rw-  2.0 fat     5031 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
--rw-rw-rw-  2.0 fat     5782 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_312_virtual_layout.py
--rw-rw-rw-  2.0 fat      647 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_313_redraw_order.py
--rw-rw-rw-  2.0 fat     6128 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_401_headersection.py
--rw-rw-rw-  2.0 fat     2750 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_402_classessection.py
--rw-rw-rw-  2.0 fat     5208 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
--rw-rw-rw-  2.0 fat     6795 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404a_tables.py
--rw-rw-rw-  2.0 fat     4981 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
--rw-rw-rw-  2.0 fat     2450 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_405_classes.py
--rw-rw-rw-  2.0 fat     9094 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
--rw-rw-rw-  2.0 fat      848 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
--rw-rw-rw-  2.0 fat     3375 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
--rw-rw-rw-  2.0 fat     1433 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
--rw-rw-rw-  2.0 fat     5736 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_410_table.py
--rw-rw-rw-  2.0 fat     6607 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
--rw-rw-rw-  2.0 fat     1058 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
--rw-rw-rw-  2.0 fat    18072 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
--rw-rw-rw-  2.0 fat     4638 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
--rw-rw-rw-  2.0 fat    12327 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
--rw-rw-rw-  2.0 fat     6509 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
--rw-rw-rw-  2.0 fat     5656 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_417_bbox.py
--rw-rw-rw-  2.0 fat     5434 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
--rw-rw-rw-  2.0 fat      733 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
--rw-rw-rw-  2.0 fat     1240 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
--rw-rw-rw-  2.0 fat     5007 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
--rw-rw-rw-  2.0 fat      769 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
--rw-rw-rw-  2.0 fat     7289 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_424_audit.py
--rw-rw-rw-  2.0 fat     3737 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
--rw-rw-rw-  2.0 fat     2981 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
--rw-rw-rw-  2.0 fat     2416 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
--rw-rw-rw-  2.0 fat     2533 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
--rw-rw-rw-  2.0 fat   112800 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/conftest.py
--rw-rw-rw-  2.0 fat     5510 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_500_units.py
--rw-rw-rw-  2.0 fat     1052 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_501_truecolor.py
--rw-rw-rw-  2.0 fat     1021 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_502_raw_color.py
--rw-rw-rw-  2.0 fat     1695 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_503_indexing.py
--rw-rw-rw-  2.0 fat     1442 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_504_suppress_zeros.py
--rw-rw-rw-  2.0 fat      216 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_506_version.py
--rw-rw-rw-  2.0 fat      579 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_507_dxf_pretty_printer.py
--rw-rw-rw-  2.0 fat      657 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_508_read_zip.py
--rw-rw-rw-  2.0 fat     1445 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_509_comments.py
--rw-rw-rw-  2.0 fat     1185 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_510_byte_stream.py
--rw-rw-rw-  2.0 fat     4239 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_511_bit_stream.py
--rw-rw-rw-  2.0 fat     5595 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_512_pattern.py
--rw-rw-rw-  2.0 fat     2372 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_513_reorder_entities.py
--rw-rw-rw-  2.0 fat    17710 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_514_text.py
--rw-rw-rw-  2.0 fat     9269 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_515a_fonts_truetype.py
--rw-rw-rw-  2.0 fat     4729 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_515b_fonts_shapefiles.py
--rw-rw-rw-  2.0 fat     2225 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_515c_fonts_lff.py
--rw-rw-rw-  2.0 fat     4002 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_516_zoom.py
--rw-rw-rw-  2.0 fat    34209 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_517_text_layout.py
--rw-rw-rw-  2.0 fat      474 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_518_header_guid.py
--rw-rw-rw-  2.0 fat     3716 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_519_mtext_editor.py
--rw-rw-rw-  2.0 fat     3205 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_520_mtext_context.py
--rw-rw-rw-  2.0 fat    24496 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_521_mtext_parser.py
--rw-rw-rw-  2.0 fat     3863 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_522_text_scanner.py
--rw-rw-rw-  2.0 fat     5207 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_523_text_size.py
--rw-rw-rw-  2.0 fat     5063 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_524_block_reference_manager.py
--rw-rw-rw-  2.0 fat      773 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_525_transparency.py
--rw-rw-rw-  2.0 fat     2133 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_526_explode.py
--rw-rw-rw-  2.0 fat    13521 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_527_gfxattribs.py
--rw-rw-rw-  2.0 fat     2748 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_528_difftags.py
--rw-rw-rw-  2.0 fat     6700 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_529_acis_sat.py
--rw-rw-rw-  2.0 fat     2062 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_530_acis_sab.py
--rw-rw-rw-  2.0 fat    12366 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_531_acis_entities.py
--rw-rw-rw-  2.0 fat     7533 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_532_acis_mesh.py
--rw-rw-rw-  2.0 fat    43206 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_533_shapefiles.py
--rw-rw-rw-  2.0 fat     1034 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_534_dwg_info.py
--rw-rw-rw-  2.0 fat    47915 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_535_xref_basic.py
--rw-rw-rw-  2.0 fat    27614 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_536_xref_conflict.py
--rw-rw-rw-  2.0 fat     6887 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_537_transform.py
--rw-rw-rw-  2.0 fat     2246 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
--rw-rw-rw-  2.0 fat     3159 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_539_npshapes.py
--rw-rw-rw-  2.0 fat     2605 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_05_tools/test_540_lff_parser.py
--rw-rw-rw-  2.0 fat     4026 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/conftest.py
--rw-rw-rw-  2.0 fat     7460 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_600_base.py
--rw-rw-rw-  2.0 fat     2098 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_601_bulge.py
--rw-rw-rw-  2.0 fat    14651 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_602_vec3.py
--rw-rw-rw-  2.0 fat     8956 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_603_vec2.py
--rw-rw-rw-  2.0 fat     2801 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_604_banded_matrix.py
--rw-rw-rw-  2.0 fat     9738 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_604_linalg.py
--rw-rw-rw-  2.0 fat    13943 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_605_matrix44.py
--rw-rw-rw-  2.0 fat     5888 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_606_convexhull.py
--rw-rw-rw-  2.0 fat     1010 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_607_perlin_noise.py
--rw-rw-rw-  2.0 fat     3833 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_608_intersection_line_line_2d.py
--rw-rw-rw-  2.0 fat     1676 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_609_point_on_line.py
--rw-rw-rw-  2.0 fat     3171 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_610_ocs.py
--rw-rw-rw-  2.0 fat     7529 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_611_ucs.py
--rw-rw-rw-  2.0 fat     1831 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_612_ucs_pass_trough.py
--rw-rw-rw-  2.0 fat     2586 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_613_point_in_poygon.py
--rw-rw-rw-  2.0 fat    10913 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_614_construct_3d.py
--rw-rw-rw-  2.0 fat      602 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_615_rytz_axis.py
--rw-rw-rw-  2.0 fat     5215 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_616_plane.py
--rw-rw-rw-  2.0 fat      772 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_617_clockwise_orientation.py
--rw-rw-rw-  2.0 fat     6384 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_618_clipping.py
--rw-rw-rw-  2.0 fat    10108 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_619_greiner_hormann.py
--rw-rw-rw-  2.0 fat     2669 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_620_knot.py
--rw-rw-rw-  2.0 fat    18821 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_621_bspline.py
--rw-rw-rw-  2.0 fat     7652 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_622_bsplineu.py
--rw-rw-rw-  2.0 fat    11327 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_623_rbspline.py
--rw-rw-rw-  2.0 fat    10809 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_624_global_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1247 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_626_local_bspline_interpolation.py
--rw-rw-rw-  2.0 fat     1967 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_627_bspline_basis.py
--rw-rw-rw-  2.0 fat    10545 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_629_bezier.py
--rw-rw-rw-  2.0 fat    10714 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_630a_bezier4p_base.py
--rw-rw-rw-  2.0 fat    10204 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_630b_bezier4p_functions.py
--rw-rw-rw-  2.0 fat     1683 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_631_euler_spiral.py
--rw-rw-rw-  2.0 fat     4021 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_632_bezier3p.py
--rw-rw-rw-  2.0 fat    19463 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_640_bbox.py
--rw-rw-rw-  2.0 fat     5393 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_641_construction_ray.py
--rw-rw-rw-  2.0 fat     3673 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_642_construction_line.py
--rw-rw-rw-  2.0 fat     9459 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_643_construction_box.py
--rw-rw-rw-  2.0 fat    10941 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_644_construction_circle.py
--rw-rw-rw-  2.0 fat    10988 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_645_construction_arc.py
--rw-rw-rw-  2.0 fat     3422 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_646_offset_vertices_2d.py
--rw-rw-rw-  2.0 fat     7672 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_647_transform_tools.py
--rw-rw-rw-  2.0 fat     8993 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_648_construction_ellipse.py
--rw-rw-rw-  2.0 fat     4243 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_650_elliptic_arc_span.py
--rw-rw-rw-  2.0 fat     9011 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_651_construction_polyline.py
--rw-rw-rw-  2.0 fat     3168 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_652_approx_param_t.py
--rw-rw-rw-  2.0 fat     5806 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_653_polyline_intersection.py
--rw-rw-rw-  2.0 fat     5193 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_654_rtree.py
--rw-rw-rw-  2.0 fat      788 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_655_dbscan.py
--rw-rw-rw-  2.0 fat      834 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_656_k_means.py
--rw-rw-rw-  2.0 fat     4654 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_657_mapbox_earcut.py
--rw-rw-rw-  2.0 fat    11628 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_658_bevel_tools.py
--rw-rw-rw-  2.0 fat     1875 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_659_intersection_line_polygon_3d.py
--rw-rw-rw-  2.0 fat     1428 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
--rw-rw-rw-  2.0 fat     1741 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
--rw-rw-rw-  2.0 fat     3307 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_06_math/test_662_is_convex_polygon_2d.py
--rw-rw-rw-  2.0 fat     1466 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_701_arrows.py
--rw-rw-rw-  2.0 fat    17245 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_702_render_forms.py
--rw-rw-rw-  2.0 fat    34220 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_703_mesh_builder.py
--rw-rw-rw-  2.0 fat     3852 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_704_render_linear_dimension.py
--rw-rw-rw-  2.0 fat     1345 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_705_shape.py
--rw-rw-rw-  2.0 fat      483 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_706_random_path.py
--rw-rw-rw-  2.0 fat     5603 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_707_trace.py
--rw-rw-rw-  2.0 fat    33834 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708a_path.py
--rw-rw-rw-  2.0 fat    27351 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708b_path_tools.py
--rw-rw-rw-  2.0 fat     3633 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708c_matplotlib_path_tools.py
--rw-rw-rw-  2.0 fat     3099 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708d_qpainter_path_tools.py
--rw-rw-rw-  2.0 fat     4589 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708e_path_shapes.py
--rw-rw-rw-  2.0 fat     4118 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_708f_path_nesting.py
--rw-rw-rw-  2.0 fat     1308 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_709_linetype_renderer.py
--rw-rw-rw-  2.0 fat     2815 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_711_points.py
--rw-rw-rw-  2.0 fat     6594 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_712_render_curved_dimension.py
--rw-rw-rw-  2.0 fat     1472 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_713_mleader_builder.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_714_mleader_render_engine.py
--rw-rw-rw-  2.0 fat    11778 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_715_hatching.py
--rw-rw-rw-  2.0 fat     2626 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
--rw-rw-rw-  2.0 fat     4771 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_800_mtext_surrogate.py
--rw-rw-rw-  2.0 fat     1352 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_801_r12spline.py
--rw-rw-rw-  2.0 fat     7881 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_802_table_painter.py
--rw-rw-rw-  2.0 fat    12386 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_803_entities_to_code.py
--rw-rw-rw-  2.0 fat     6844 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_804_importer.py
--rw-rw-rw-  2.0 fat     2362 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_805_pycsg.py
--rw-rw-rw-  2.0 fat    15467 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_806_acadctb.py
--rw-rw-rw-  2.0 fat     4860 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_807_dwg_loader_basics.py
--rw-rw-rw-  2.0 fat    10862 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_810_drawing_properties.py
--rw-rw-rw-  2.0 fat    11353 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_811a_drawing_frontend.py
--rw-rw-rw-  2.0 fat     4304 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_811b_drawing_recorder.py
--rw-rw-rw-  2.0 fat     4157 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_812_drawing_graphic_proxy.py
--rw-rw-rw-  2.0 fat    12547 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_813_geo_interface.py
--rw-rw-rw-  2.0 fat    14853 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_814_text2path.py
--rw-rw-rw-  2.0 fat    16239 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_815_dxf_browser.py
--rw-rw-rw-  2.0 fat    11275 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_816_bin_packing.py
--rw-rw-rw-  2.0 fat    12554 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_817_genetic_algorithm.py
--rw-rw-rw-  2.0 fat     9008 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_818_meshex.py
--rw-rw-rw-  2.0 fat     1003 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_819_menger_sponge.py
--rw-rw-rw-  2.0 fat     4433 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_820_openscad.py
--rw-rw-rw-  2.0 fat    15527 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2.py
--rw-rw-rw-  2.0 fat     1322 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
--rw-rw-rw-  2.0 fat      976 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_822_clipper.py
--rw-rw-rw-  2.0 fat     5284 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_823_drawing_layout.py
--rw-rw-rw-  2.0 fat     3030 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_08_addons/test_824_svg_drawing_backend.py
--rw-rw-rw-  2.0 fat     2527 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_901_acc_vec2.py
--rw-rw-rw-  2.0 fat     2199 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_902_acc_vec3.py
--rw-rw-rw-  2.0 fat     2142 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
--rw-rw-rw-  2.0 fat     3158 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
--rw-rw-rw-  2.0 fat     1452 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
--rw-rw-rw-  2.0 fat     4755 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_906_acc_bspline.py
--rw-rw-rw-  2.0 fat     2656 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_414_bbox_calculation.py
--rw-rw-rw-  2.0 fat     1213 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
--rw-rw-rw-  2.0 fat     2268 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_574_flattening_error.py
--rw-rw-rw-  2.0 fat     1754 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
--rw-rw-rw-  2.0 fat      682 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_749_text_layout.py
--rw-rw-rw-  2.0 fat    11094 b- defN 23-May-20 08:28 ezdxf-1.1.0b2/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
-838 files, 8647859 bytes uncompressed, 1948272 bytes compressed:  77.5%
+Zip file size: 2111295 bytes, number of entries: 839
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/
+-rw-rw-rw-  2.0 fat     1092 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/LICENSE
+-rw-rw-rw-  2.0 fat      302 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/MANIFEST.in
+-rw-rw-rw-  2.0 fat   101826 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/NEWS.md
+-rw-rw-rw-  2.0 fat    69693 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/PKG-INFO
+-rw-rw-rw-  2.0 fat     6142 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/README.md
+-rw-rw-rw-  2.0 fat       55 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/requirements.txt
+-rw-rw-rw-  2.0 fat       74 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/setup.cfg
+-rw-rw-rw-  2.0 fat     5402 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/setup.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/
+-rw-rw-rw-  2.0 fat      567 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_config_file.py
+-rw-rw-rw-  2.0 fat      541 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_env_var.py
+-rw-rw-rw-  2.0 fat      410 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/conftest.py
+-rw-rw-rw-  2.0 fat     1054 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_acad_table.py
+-rw-rw-rw-  2.0 fat     4686 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_all_dimline_styles.py
+-rw-rw-rw-  2.0 fat     4133 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_all_ellipse_transformations.py
+-rw-rw-rw-  2.0 fat     1064 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_anonymous_blocks.py
+-rw-rw-rw-  2.0 fat      871 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_audit_critical_dxf_files.py
+-rw-rw-rw-  2.0 fat     1603 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_audit_layouts.py
+-rw-rw-rw-  2.0 fat     1726 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_complex_line_type_2.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_create_basic_graphics.py
+-rw-rw-rw-  2.0 fat     1921 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_document_guid.py
+-rw-rw-rw-  2.0 fat     1832 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_document_page_setup.py
+-rw-rw-rw-  2.0 fat      998 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_dxf_info_scanning.py
+-rw-rw-rw-  2.0 fat     1558 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_entities_iterator.py
+-rw-rw-rw-  2.0 fat      934 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_fix_dulicate_handles.py
+-rw-rw-rw-  2.0 fat     1901 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_geo.py
+-rw-rw-rw-  2.0 fat     1250 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_groups.py
+-rw-rw-rw-  2.0 fat      905 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_hpgl2_addon.py
+-rw-rw-rw-  2.0 fat      630 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_ignore_junk_beyond_EOF.py
+-rw-rw-rw-  2.0 fat     1155 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_launcher.py
+-rw-rw-rw-  2.0 fat      631 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_leica_disto_r12.py
+-rw-rw-rw-  2.0 fat      737 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_load_dxf_unicode_notation.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat     2230 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_mtext_columns.py
+-rw-rw-rw-  2.0 fat     2392 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_mtext_explode_addon.py
+-rw-rw-rw-  2.0 fat     1846 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_mtext_text_frame.py
+-rw-rw-rw-  2.0 fat     1053 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_new_table_entries.py
+-rw-rw-rw-  2.0 fat      887 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_none_ascii_read_write.py
+-rw-rw-rw-  2.0 fat     3435 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_odafc.py
+-rw-rw-rw-  2.0 fat     1737 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_open_binary_DXF_files.py
+-rw-rw-rw-  2.0 fat      751 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_open_coord_order_issue.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_open_exotic_dxf_files.py
+-rw-rw-rw-  2.0 fat      879 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_open_R13_R14.py
+-rw-rw-rw-  2.0 fat     3152 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_polyline_entity.py
+-rw-rw-rw-  2.0 fat     1749 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_preserve_binary_data_in_xrecords.py
+-rw-rw-rw-  2.0 fat     6944 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_r12export.py
+-rw-rw-rw-  2.0 fat     6256 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_r12strict.py
+-rw-rw-rw-  2.0 fat     3410 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_r12writer.py
+-rw-rw-rw-  2.0 fat      567 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_read_file_without_handles.py
+-rw-rw-rw-  2.0 fat     1121 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_read_write_modern_entites.py
+-rw-rw-rw-  2.0 fat     5375 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_recover.py
+-rw-rw-rw-  2.0 fat     1959 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_redraw_order.py
+-rw-rw-rw-  2.0 fat     1819 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_rotated_block_attributes.py
+-rw-rw-rw-  2.0 fat      774 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_surface_entities.py
+-rw-rw-rw-  2.0 fat      928 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_write_fixed_meta_data.py
+-rw-rw-rw-  2.0 fat     1806 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_write_without_handles.py
+-rw-rw-rw-  2.0 fat     3638 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/test_xref_detach.py
+-rw-rw-rw-  2.0 fat     3060 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/AC1003_LINE_Example.dxf
+-rw-rw-rw-  2.0 fat   179505 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/acad_table_with_blk_ref.dxf
+-rw-rw-rw-  2.0 fat     7956 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/ASCII_R12.dxf
+-rw-rw-rw-  2.0 fat     3761 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r12.dxf
+-rw-rw-rw-  2.0 fat    20914 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r13.dxf
+-rw-rw-rw-  2.0 fat    21137 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r14.dxf
+-rw-rw-rw-  2.0 fat    11564 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r2000.dxf
+-rw-rw-rw-  2.0 fat     6424 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/cc_dxflib.dxf
+-rw-rw-rw-  2.0 fat   173753 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/custom_blocks.dxf
+-rw-rw-rw-  2.0 fat    32203 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/duplicate_handles.dxf
+-rw-rw-rw-  2.0 fat    18554 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/dxf_unicode.dxf
+-rw-rw-rw-  2.0 fat     1592 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/empty_handles.dxf
+-rw-rw-rw-  2.0 fat    97103 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/groups.dxf
+-rw-rw-rw-  2.0 fat     9146 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/Leica_Disto_S910.dxf
+-rw-rw-rw-  2.0 fat    17986 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/MODEL.dxf
+-rw-rw-rw-  2.0 fat    25799 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2007.dxf
+-rw-rw-rw-  2.0 fat    23927 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2018.dxf
+-rw-rw-rw-  2.0 fat    98230 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/mtext_framed_columns.dxf
+-rw-rw-rw-  2.0 fat   106574 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/mtext_text_frame.dxf
+-rw-rw-rw-  2.0 fat    12001 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/no_layouts.dxf
+-rw-rw-rw-  2.0 fat    16295 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/PLOTFILE.plt
+-rw-rw-rw-  2.0 fat    28788 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/POLI-ALL210_12.DXF
+-rw-rw-rw-  2.0 fat      144 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+-rw-rw-rw-  2.0 fat   212407 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/recover01.dxf
+-rw-rw-rw-  2.0 fat   115423 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/recover02.dxf
+-rw-rw-rw-  2.0 fat    21178 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/small_r13.dxf
+-rw-rw-rw-  2.0 fat    10326 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/small_r14.dxf
+-rw-rw-rw-  2.0 fat    11286 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/XRECORD_0.bin
+-rw-rw-rw-  2.0 fat    11662 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/XRECORD_1.bin
+-rw-rw-rw-  2.0 fat    15337 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/integration_tests/data/XRECORD_2.bin
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/
+-rw-rw-rw-  2.0 fat     4710 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/appsettings.py
+-rw-rw-rw-  2.0 fat    19818 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/audit.py
+-rw-rw-rw-  2.0 fat     5324 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/bbox.py
+-rw-rw-rw-  2.0 fat     7888 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/blkrefs.py
+-rw-rw-rw-  2.0 fat    14858 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/colors.py
+-rw-rw-rw-  2.0 fat    31103 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/commands.py
+-rw-rw-rw-  2.0 fat     1549 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/comments.py
+-rw-rw-rw-  2.0 fat    22100 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/disassemble.py
+-rw-rw-rw-  2.0 fat    52708 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/document.py
+-rw-rw-rw-  2.0 fat      832 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/dwginfo.py
+-rw-rw-rw-  2.0 fat    16248 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entitydb.py
+-rw-rw-rw-  2.0 fat     7495 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/enums.py
+-rw-rw-rw-  2.0 fat    13948 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/explode.py
+-rw-rw-rw-  2.0 fat     1653 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/eztypes.py
+-rw-rw-rw-  2.0 fat    10333 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/filemanagement.py
+-rw-rw-rw-  2.0 fat    12157 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/gfxattribs.py
+-rw-rw-rw-  2.0 fat   107500 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/graphicsfactory.py
+-rw-rw-rw-  2.0 fat     3416 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/groupby.py
+-rw-rw-rw-  2.0 fat     3241 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/npshapes.py
+-rw-rw-rw-  2.0 fat     2567 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/protocols.py
+-rw-rw-rw-  2.0 fat    33129 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/proxygraphic.py
+-rw-rw-rw-  2.0 fat       95 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/py.typed
+-rw-rw-rw-  2.0 fat    22499 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/query.py
+-rw-rw-rw-  2.0 fat     2780 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/queryparser.py
+-rw-rw-rw-  2.0 fat     9580 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/r12strict.py
+-rw-rw-rw-  2.0 fat    30769 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/recover.py
+-rw-rw-rw-  2.0 fat     3515 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/reorder.py
+-rw-rw-rw-  2.0 fat    10364 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/transform.py
+-rw-rw-rw-  2.0 fat     5750 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/units.py
+-rw-rw-rw-  2.0 fat     8280 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/upright.py
+-rw-rw-rw-  2.0 fat     9875 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/urecord.py
+-rw-rw-rw-  2.0 fat     1024 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/version.py
+-rw-rw-rw-  2.0 fat    63359 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/xref.py
+-rw-rw-rw-  2.0 fat     2853 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/zoom.py
+-rw-rw-rw-  2.0 fat    10898 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/_options.py
+-rw-rw-rw-  2.0 fat     2566 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/__init__.py
+-rw-rw-rw-  2.0 fat     3259 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/__main__.py
+-rw-rw-rw-  2.0 fat     6072 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/bezier3p.pyx
+-rw-rw-rw-  2.0 fat     9983 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/bezier4p.pyx
+-rw-rw-rw-  2.0 fat    12964 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/bspline.pyx
+-rw-rw-rw-  2.0 fat       90 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/construct.pxd
+-rw-rw-rw-  2.0 fat     6584 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/construct.pyx
+-rw-rw-rw-  2.0 fat     3113 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/linetypes.pyx
+-rw-rw-rw-  2.0 fat    23989 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/mapbox_earcut.pyx
+-rw-rw-rw-  2.0 fat      386 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pxd
+-rw-rw-rw-  2.0 fat    23742 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pyx
+-rw-rw-rw-  2.0 fat     2014 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/vector.pxd
+-rw-rw-rw-  2.0 fat    23705 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/vector.pyx
+-rw-rw-rw-  2.0 fat     1784 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+-rw-rw-rw-  2.0 fat      599 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+-rw-rw-rw-  2.0 fat      424 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+-rw-rw-rw-  2.0 fat      960 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.cpp
+-rw-rw-rw-  2.0 fat      464 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.hpp
+-rw-rw-rw-  2.0 fat      407 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.pxd
+-rw-rw-rw-  2.0 fat     2135 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.hpp
+-rw-rw-rw-  2.0 fat      572 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.pxd
+-rw-rw-rw-  2.0 fat     1265 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acc/__init__.py
+-rw-rw-rw-  2.0 fat     6393 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/abstract.py
+-rw-rw-rw-  2.0 fat      884 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/api.py
+-rw-rw-rw-  2.0 fat     5484 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/const.py
+-rw-rw-rw-  2.0 fat     6726 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/dbg.py
+-rw-rw-rw-  2.0 fat     2980 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/dxf.py
+-rw-rw-rw-  2.0 fat    28991 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/entities.py
+-rw-rw-rw-  2.0 fat     4088 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/hdr.py
+-rw-rw-rw-  2.0 fat    12823 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/mesh.py
+-rw-rw-rw-  2.0 fat    18690 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/sab.py
+-rw-rw-rw-  2.0 fat    13184 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/sat.py
+-rw-rw-rw-  2.0 fat      115 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/acis/__init__.py
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/
+-rw-rw-rw-  2.0 fat    26415 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acadctb.py
+-rw-rw-rw-  2.0 fat    22229 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/binpacking.py
+-rw-rw-rw-  2.0 fat    27692 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dimlines.py
+-rw-rw-rw-  2.0 fat    31371 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dxf2code.py
+-rw-rw-rw-  2.0 fat    22037 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/genetic_algorithm.py
+-rw-rw-rw-  2.0 fat    36445 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/geo.py
+-rw-rw-rw-  2.0 fat     2674 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/gerber_D6673.py
+-rw-rw-rw-  2.0 fat    25472 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/importer.py
+-rw-rw-rw-  2.0 fat    17355 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/iterdxf.py
+-rw-rw-rw-  2.0 fat     8940 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/menger_sponge.py
+-rw-rw-rw-  2.0 fat    24787 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/meshex.py
+-rw-rw-rw-  2.0 fat      492 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/mixins.py
+-rw-rw-rw-  2.0 fat     6203 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/mtextsurrogate.py
+-rw-rw-rw-  2.0 fat    13528 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/mtxpl.py
+-rw-rw-rw-  2.0 fat    16400 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/odafc.py
+-rw-rw-rw-  2.0 fat     9456 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/openscad.py
+-rw-rw-rw-  2.0 fat    15878 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/pycsg.py
+-rw-rw-rw-  2.0 fat    22496 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/r12export.py
+-rw-rw-rw-  2.0 fat    27198 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/r12writer.py
+-rw-rw-rw-  2.0 fat     7615 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/sierpinski_pyramid.py
+-rw-rw-rw-  2.0 fat    33167 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/tablepainter.py
+-rw-rw-rw-  2.0 fat    12789 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/text2path.py
+-rw-rw-rw-  2.0 fat     3842 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/xplayer.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/xqt.py
+-rw-rw-rw-  2.0 fat      453 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/__init__.py
+-rw-rw-rw-  2.0 fat    10023 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/browser.py
+-rw-rw-rw-  2.0 fat     1907 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/data.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/__init__.py
+-rw-rw-rw-  2.0 fat      820 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/bookmarks.py
+-rw-rw-rw-  2.0 fat    29367 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/browser.py
+-rw-rw-rw-  2.0 fat    14891 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/data.py
+-rw-rw-rw-  2.0 fat    10993 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/find_dialog.py
+-rw-rw-rw-  2.0 fat     1281 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/loader.py
+-rw-rw-rw-  2.0 fat    21111 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/model.py
+-rw-rw-rw-  2.0 fat     2214 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/tags.py
+-rw-rw-rw-  2.0 fat     1382 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/views.py
+-rw-rw-rw-  2.0 fat      133 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/browser/__init__.py
+-rw-rw-rw-  2.0 fat     7319 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/backend.py
+-rw-rw-rw-  2.0 fat     3960 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/clipper.py
+-rw-rw-rw-  2.0 fat     9824 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/config.py
+-rw-rw-rw-  2.0 fat     1707 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_backend.py
+-rw-rw-rw-  2.0 fat      514 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_utils.py
+-rw-rw-rw-  2.0 fat     7295 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/dxf.py
+-rw-rw-rw-  2.0 fat    47447 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/frontend.py
+-rw-rw-rw-  2.0 fat     1823 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/gfxproxy.py
+-rw-rw-rw-  2.0 fat    19510 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/hpgl2.py
+-rw-rw-rw-  2.0 fat    14662 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/layout.py
+-rw-rw-rw-  2.0 fat    12506 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/matplotlib.py
+-rw-rw-rw-  2.0 fat     9878 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/mtext_complex.py
+-rw-rw-rw-  2.0 fat    38974 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/properties.py
+-rw-rw-rw-  2.0 fat    14612 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pymupdf.py
+-rw-rw-rw-  2.0 fat    11034 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pyqt.py
+-rw-rw-rw-  2.0 fat    22624 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/qtviewer.py
+-rw-rw-rw-  2.0 fat     9998 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/recorder.py
+-rw-rw-rw-  2.0 fat    14923 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/svg.py
+-rw-rw-rw-  2.0 fat    13023 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text.py
+-rw-rw-rw-  2.0 fat      963 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text_renderer.py
+-rw-rw-rw-  2.0 fat      314 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/type_hints.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/unified_text_renderer.py
+-rw-rw-rw-  2.0 fat      171 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/drawing/__init__.py
+-rw-rw-rw-  2.0 fat     3112 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/classes_section.py
+-rw-rw-rw-  2.0 fat      763 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/const.py
+-rw-rw-rw-  2.0 fat     6091 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/crc.py
+-rw-rw-rw-  2.0 fat     3160 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/fileheader.py
+-rw-rw-rw-  2.0 fat    14851 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/header_section.py
+-rw-rw-rw-  2.0 fat     2976 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/loader.py
+-rw-rw-rw-  2.0 fat      141 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/dwg/__init__.py
+-rw-rw-rw-  2.0 fat    13459 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/api.py
+-rw-rw-rw-  2.0 fat     8584 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/backend.py
+-rw-rw-rw-  2.0 fat      563 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/deps.py
+-rw-rw-rw-  2.0 fat    16079 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/interpreter.py
+-rw-rw-rw-  2.0 fat     4836 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/page.py
+-rw-rw-rw-  2.0 fat    11774 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/plotter.py
+-rw-rw-rw-  2.0 fat     1708 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/polygon_buffer.py
+-rw-rw-rw-  2.0 fat     5615 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/properties.py
+-rw-rw-rw-  2.0 fat     6222 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/tokenizer.py
+-rw-rw-rw-  2.0 fat    19451 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/viewer.py
+-rw-rw-rw-  2.0 fat      164 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/__init__.py
+-rw-rw-rw-  2.0 fat     4757 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat    18315 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/acad_table.py
+-rw-rw-rw-  2.0 fat    25923 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/acis.py
+-rw-rw-rw-  2.0 fat     4890 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/appdata.py
+-rw-rw-rw-  2.0 fat     1954 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/appid.py
+-rw-rw-rw-  2.0 fat     4942 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/arc.py
+-rw-rw-rw-  2.0 fat    26138 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/attrib.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/block.py
+-rw-rw-rw-  2.0 fat    10536 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/blockrecord.py
+-rw-rw-rw-  2.0 fat    50143 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/boundary_paths.py
+-rw-rw-rw-  2.0 fat     7961 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/circle.py
+-rw-rw-rw-  2.0 fat    23664 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dictionary.py
+-rw-rw-rw-  2.0 fat    48743 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dimension.py
+-rw-rw-rw-  2.0 fat    35012 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dimstyle.py
+-rw-rw-rw-  2.0 fat    23829 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dimstyleoverride.py
+-rw-rw-rw-  2.0 fat     4399 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfclass.py
+-rw-rw-rw-  2.0 fat    42404 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfentity.py
+-rw-rw-rw-  2.0 fat    26923 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfgfx.py
+-rw-rw-rw-  2.0 fat    15279 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfgroups.py
+-rw-rw-rw-  2.0 fat    23699 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfns.py
+-rw-rw-rw-  2.0 fat    13746 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/dxfobj.py
+-rw-rw-rw-  2.0 fat    11186 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/ellipse.py
+-rw-rw-rw-  2.0 fat     4170 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/factory.py
+-rw-rw-rw-  2.0 fat    23785 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/geodata.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/gradient.py
+-rw-rw-rw-  2.0 fat    12263 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/hatch.py
+-rw-rw-rw-  2.0 fat     3944 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/helix.py
+-rw-rw-rw-  2.0 fat     4747 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/idbuffer.py
+-rw-rw-rw-  2.0 fat    26057 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/image.py
+-rw-rw-rw-  2.0 fat    27932 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/insert.py
+-rw-rw-rw-  2.0 fat    27834 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/layer.py
+-rw-rw-rw-  2.0 fat    14252 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/layout.py
+-rw-rw-rw-  2.0 fat    12978 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/leader.py
+-rw-rw-rw-  2.0 fat     4718 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/light.py
+-rw-rw-rw-  2.0 fat     3718 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/line.py
+-rw-rw-rw-  2.0 fat     9677 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/ltype.py
+-rw-rw-rw-  2.0 fat    18878 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/lwpolyline.py
+-rw-rw-rw-  2.0 fat    19653 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/material.py
+-rw-rw-rw-  2.0 fat    18435 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mesh.py
+-rw-rw-rw-  2.0 fat    57367 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mleader.py
+-rw-rw-rw-  2.0 fat    37144 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mline.py
+-rw-rw-rw-  2.0 fat     8385 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mpolygon.py
+-rw-rw-rw-  2.0 fat    48153 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mtext.py
+-rw-rw-rw-  2.0 fat     4351 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/mtext_columns.py
+-rw-rw-rw-  2.0 fat     6284 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/objectcollection.py
+-rw-rw-rw-  2.0 fat     2111 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/oleframe.py
+-rw-rw-rw-  2.0 fat     4332 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/pattern.py
+-rw-rw-rw-  2.0 fat     5238 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/point.py
+-rw-rw-rw-  2.0 fat    16427 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/polygon.py
+-rw-rw-rw-  2.0 fat    40087 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/polyline.py
+-rw-rw-rw-  2.0 fat     4822 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/shape.py
+-rw-rw-rw-  2.0 fat    10443 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/solid.py
+-rw-rw-rw-  2.0 fat    24085 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/spline.py
+-rw-rw-rw-  2.0 fat     8246 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/subentity.py
+-rw-rw-rw-  2.0 fat     5196 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/sun.py
+-rw-rw-rw-  2.0 fat     2449 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/table.py
+-rw-rw-rw-  2.0 fat    17602 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/text.py
+-rw-rw-rw-  2.0 fat     9035 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/textstyle.py
+-rw-rw-rw-  2.0 fat     3597 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/tolerance.py
+-rw-rw-rw-  2.0 fat     2703 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/ucs.py
+-rw-rw-rw-  2.0 fat    14366 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/underlay.py
+-rw-rw-rw-  2.0 fat     6040 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/view.py
+-rw-rw-rw-  2.0 fat    28300 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/viewport.py
+-rw-rw-rw-  2.0 fat     7867 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/visualstyle.py
+-rw-rw-rw-  2.0 fat     9970 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/vport.py
+-rw-rw-rw-  2.0 fat    17024 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/xdata.py
+-rw-rw-rw-  2.0 fat     8495 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/xdict.py
+-rw-rw-rw-  2.0 fat     3062 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/xline.py
+-rw-rw-rw-  2.0 fat     3127 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/entities/__init__.py
+-rw-rw-rw-  2.0 fat    24773 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/fonts.py
+-rw-rw-rw-  2.0 fat     2242 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/font_face.py
+-rw-rw-rw-  2.0 fat    17004 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/font_manager.py
+-rw-rw-rw-  2.0 fat     1702 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/font_measurements.py
+-rw-rw-rw-  2.0 fat      825 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/glyphs.py
+-rw-rw-rw-  2.0 fat    10794 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/lff.py
+-rw-rw-rw-  2.0 fat    35217 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/shapefile.py
+-rw-rw-rw-  2.0 fat     7219 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/ttfonts.py
+-rw-rw-rw-  2.0 fat       64 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/fonts/__init__.py
+-rw-rw-rw-  2.0 fat    16696 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/base.py
+-rw-rw-rw-  2.0 fat     4343 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/blocklayout.py
+-rw-rw-rw-  2.0 fat    29785 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/layout.py
+-rw-rw-rw-  2.0 fat    15314 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/layouts.py
+-rw-rw-rw-  2.0 fat      232 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/layouts/__init__.py
+-rw-rw-rw-  2.0 fat     8327 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/attributes.py
+-rw-rw-rw-  2.0 fat    16500 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/const.py
+-rw-rw-rw-  2.0 fat     1614 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/encoding.py
+-rw-rw-rw-  2.0 fat    17013 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/extendedtags.py
+-rw-rw-rw-  2.0 fat     5363 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/fileindex.py
+-rw-rw-rw-  2.0 fat      727 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/hdrvars.py
+-rw-rw-rw-  2.0 fat     5469 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/loader.py
+-rw-rw-rw-  2.0 fat     7447 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/packedtags.py
+-rw-rw-rw-  2.0 fat     6355 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/repair.py
+-rw-rw-rw-  2.0 fat    13058 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/tagger.py
+-rw-rw-rw-  2.0 fat    14336 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/tags.py
+-rw-rw-rw-  2.0 fat     8952 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/tagwriter.py
+-rw-rw-rw-  2.0 fat    12064 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/types.py
+-rw-rw-rw-  2.0 fat    17069 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/validator.py
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/lldxf/__init__.py
+-rw-rw-rw-  2.0 fat    19193 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/arc.py
+-rw-rw-rw-  2.0 fat    16270 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bbox.py
+-rw-rw-rw-  2.0 fat     9318 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bezier.py
+-rw-rw-rw-  2.0 fat     2452 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bezier_interpolation.py
+-rw-rw-rw-  2.0 fat     8730 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/box.py
+-rw-rw-rw-  2.0 fat    52916 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bspline.py
+-rw-rw-rw-  2.0 fat     5608 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/bulge.py
+-rw-rw-rw-  2.0 fat     9002 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/circle.py
+-rw-rw-rw-  2.0 fat    24003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/clipping.py
+-rw-rw-rw-  2.0 fat     4319 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/clustering.py
+-rw-rw-rw-  2.0 fat    12236 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/construct2d.py
+-rw-rw-rw-  2.0 fat    26265 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/construct3d.py
+-rw-rw-rw-  2.0 fat     1283 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/cspline.py
+-rw-rw-rw-  2.0 fat     9114 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/curvetools.py
+-rw-rw-rw-  2.0 fat    22048 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/ellipse.py
+-rw-rw-rw-  2.0 fat     4406 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/eulerspiral.py
+-rw-rw-rw-  2.0 fat    38883 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/linalg.py
+-rw-rw-rw-  2.0 fat    10231 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/line.py
+-rw-rw-rw-  2.0 fat     3053 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/offset2d.py
+-rw-rw-rw-  2.0 fat     8256 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/parametrize.py
+-rw-rw-rw-  2.0 fat    15602 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/perlin.py
+-rw-rw-rw-  2.0 fat    15921 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/polyline.py
+-rw-rw-rw-  2.0 fat    11867 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/rtree.py
+-rw-rw-rw-  2.0 fat     3910 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/shape.py
+-rw-rw-rw-  2.0 fat     2568 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/surfaces.py
+-rw-rw-rw-  2.0 fat    12155 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/transformtools.py
+-rw-rw-rw-  2.0 fat     3631 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/triangulation.py
+-rw-rw-rw-  2.0 fat    16976 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/ucs.py
+-rw-rw-rw-  2.0 fat     7213 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_bezier3p.py
+-rw-rw-rw-  2.0 fat    12967 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_bezier4p.py
+-rw-rw-rw-  2.0 fat     9440 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_bspline.py
+-rw-rw-rw-  2.0 fat     7272 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_construct.py
+-rw-rw-rw-  2.0 fat     2261 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_ctypes.py
+-rw-rw-rw-  2.0 fat    24954 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    27606 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_matrix44.py
+-rw-rw-rw-  2.0 fat    25912 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/_vector.py
+-rw-rw-rw-  2.0 fat     2003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/math/__init__.py
+-rw-rw-rw-  2.0 fat     1306 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/commands.py
+-rw-rw-rw-  2.0 fat    39194 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/converter.py
+-rw-rw-rw-  2.0 fat     6748 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/nesting.py
+-rw-rw-rw-  2.0 fat    20453 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/path.py
+-rw-rw-rw-  2.0 fat    10140 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/shapes.py
+-rw-rw-rw-  2.0 fat    34708 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/tools.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/path/__init__.py
+-rw-rw-rw-  2.0 fat     2987 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.css
+-rw-rw-rw-  2.0 fat     1148 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.html
+-rw-rw-rw-  2.0 fat    11304 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.js
+-rw-rw-rw-  2.0 fat    17144 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.py
+-rw-rw-rw-  2.0 fat     3770 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/pprint.py
+-rw-rw-rw-  2.0 fat      812 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.css
+-rw-rw-rw-  2.0 fat      316 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.html
+-rw-rw-rw-  2.0 fat     2545 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.py
+-rw-rw-rw-  2.0 fat     6896 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/reflinks.py
+-rw-rw-rw-  2.0 fat      123 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/pp/__init__.py
+-rw-rw-rw-  2.0 fat    10039 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/abstract_mtext_renderer.py
+-rw-rw-rw-  2.0 fat    20495 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/arrows.py
+-rw-rw-rw-  2.0 fat    17749 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/curves.py
+-rw-rw-rw-  2.0 fat     4041 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dimension.py
+-rw-rw-rw-  2.0 fat    52028 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_base.py
+-rw-rw-rw-  2.0 fat    35702 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_curved.py
+-rw-rw-rw-  2.0 fat     6894 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_diameter.py
+-rw-rw-rw-  2.0 fat    24751 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_linear.py
+-rw-rw-rw-  2.0 fat     8084 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_ordinate.py
+-rw-rw-rw-  2.0 fat    20295 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/dim_radius.py
+-rw-rw-rw-  2.0 fat    47170 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/forms.py
+-rw-rw-rw-  2.0 fat    24213 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/hatching.py
+-rw-rw-rw-  2.0 fat     4728 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/leader.py
+-rw-rw-rw-  2.0 fat      664 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/linetypes.py
+-rw-rw-rw-  2.0 fat    64121 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/mesh.py
+-rw-rw-rw-  2.0 fat    60923 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/mleader.py
+-rw-rw-rw-  2.0 fat     8437 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/mline.py
+-rw-rw-rw-  2.0 fat     2964 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/point.py
+-rw-rw-rw-  2.0 fat     8736 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/polyline.py
+-rw-rw-rw-  2.0 fat     7886 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/r12spline.py
+-rw-rw-rw-  2.0 fat    22541 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/trace.py
+-rw-rw-rw-  2.0 fat     2881 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/_linetypes.py
+-rw-rw-rw-  2.0 fat      778 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/render/__init__.py
+-rw-rw-rw-  2.0 fat     1050 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/16x16.png
+-rw-rw-rw-  2.0 fat     1420 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/24x24.png
+-rw-rw-rw-  2.0 fat    10638 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/256x256.png
+-rw-rw-rw-  2.0 fat     1758 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/32x32.png
+-rw-rw-rw-  2.0 fat     2335 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/48x48.png
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/64x64.png
+-rw-rw-rw-  2.0 fat     2090 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-copy-64px.png
+-rw-rw-rw-  2.0 fat     3109 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-find-64px.png
+-rw-rw-rw-  2.0 fat     2388 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-bookmark-64px.png
+-rw-rw-rw-  2.0 fat     2519 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-handle-64px.png
+-rw-rw-rw-  2.0 fat     2409 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-line-64px.png
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-left-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2322 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-next-entity-64px.png
+-rw-rw-rw-  2.0 fat     2320 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-prev-entity-64px.png
+-rw-rw-rw-  2.0 fat     2244 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-right-arrow-64px.png
+-rw-rw-rw-  2.0 fat     2553 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-show-in-tree-64px.png
+-rw-rw-rw-  2.0 fat     2373 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/resources/icon-store-bookmark-64px.png
+-rw-rw-rw-  2.0 fat    10650 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/acdsdata.py
+-rw-rw-rw-  2.0 fat    16508 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/blocks.py
+-rw-rw-rw-  2.0 fat    11639 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/classes.py
+-rw-rw-rw-  2.0 fat     4137 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/entities.py
+-rw-rw-rw-  2.0 fat    11953 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/header.py
+-rw-rw-rw-  2.0 fat    60696 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/headervars.py
+-rw-rw-rw-  2.0 fat    27009 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/objects.py
+-rw-rw-rw-  2.0 fat    26581 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/table.py
+-rw-rw-rw-  2.0 fat     5270 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/tables.py
+-rw-rw-rw-  2.0 fat       67 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/sections/__init__.py
+-rw-rw-rw-  2.0 fat    19711 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/analyze.py
+-rw-rw-rw-  2.0 fat    20434 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/binarydata.py
+-rw-rw-rw-  2.0 fat     2931 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/codepage.py
+-rw-rw-rw-  2.0 fat     7645 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/complex_ltype.py
+-rw-rw-rw-  2.0 fat     1782 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/crypt.py
+-rw-rw-rw-  2.0 fat     1511 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/debug.py
+-rw-rw-rw-  2.0 fat     2341 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/difftags.py
+-rw-rw-rw-  2.0 fat     1235 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/handle.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/indexing.py
+-rw-rw-rw-  2.0 fat     2145 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/juliandate.py
+-rw-rw-rw-  2.0 fat     6166 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/pattern.py
+-rw-rw-rw-  2.0 fat     1256 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/rawloader.py
+-rw-rw-rw-  2.0 fat   129174 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/standards.py
+-rw-rw-rw-  2.0 fat     6049 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/strip.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/test.py
+-rw-rw-rw-  2.0 fat    65523 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/text.py
+-rw-rw-rw-  2.0 fat    54234 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/text_layout.py
+-rw-rw-rw-  2.0 fat     6893 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/text_size.py
+-rw-rw-rw-  2.0 fat     3077 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/zipmanager.py
+-rw-rw-rw-  2.0 fat   142734 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/_iso_pattern.py
+-rw-rw-rw-  2.0 fat     3564 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf/tools/__init__.py
+-rw-rw-rw-  2.0 fat        1 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/dependency_links.txt
+-rw-rw-rw-  2.0 fat       47 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        2 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/not-zip-safe
+-rw-rw-rw-  2.0 fat    69693 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/PKG-INFO
+-rw-rw-rw-  2.0 fat      302 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/requires.txt
+-rw-rw-rw-  2.0 fat    31857 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/SOURCES.txt
+-rw-rw-rw-  2.0 fat        6 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/src/ezdxf.egg-info/top_level.txt
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/
+drwxrwxrwx  2.0 fat        0 b- stor 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/
+-rw-rw-rw-  2.0 fat      410 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/conftest.py
+-rw-rw-rw-  2.0 fat     2336 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+-rw-rw-rw-  2.0 fat      780 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+-rw-rw-rw-  2.0 fat     2599 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+-rw-rw-rw-  2.0 fat     1124 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+-rw-rw-rw-  2.0 fat     5456 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+-rw-rw-rw-  2.0 fat      582 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+-rw-rw-rw-  2.0 fat      473 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+-rw-rw-rw-  2.0 fat    11593 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+-rw-rw-rw-  2.0 fat     1191 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+-rw-rw-rw-  2.0 fat     1033 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+-rw-rw-rw-  2.0 fat     4792 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+-rw-rw-rw-  2.0 fat      989 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+-rw-rw-rw-  2.0 fat     1383 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_018_handle.py
+-rw-rw-rw-  2.0 fat     5518 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+-rw-rw-rw-  2.0 fat     8168 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+-rw-rw-rw-  2.0 fat     3787 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+-rw-rw-rw-  2.0 fat      401 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+-rw-rw-rw-  2.0 fat      539 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+-rw-rw-rw-  2.0 fat     2092 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_040_tags.py
+-rw-rw-rw-  2.0 fat     3073 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+-rw-rw-rw-  2.0 fat     6419 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+-rw-rw-rw-  2.0 fat     1632 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+-rw-rw-rw-  2.0 fat    11265 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+-rw-rw-rw-  2.0 fat     3363 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+-rw-rw-rw-  2.0 fat     1974 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+-rw-rw-rw-  2.0 fat     2321 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+-rw-rw-rw-  2.0 fat      568 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+-rw-rw-rw-  2.0 fat     8682 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+-rw-rw-rw-  2.0 fat     1051 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+-rw-rw-rw-  2.0 fat     1500 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+-rw-rw-rw-  2.0 fat    11689 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+-rw-rw-rw-  2.0 fat     2893 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_102_appdata.py
+-rw-rw-rw-  2.0 fat     2312 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_103_reactors.py
+-rw-rw-rw-  2.0 fat     4001 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_104_extension_dict.py
+-rw-rw-rw-  2.0 fat    20860 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_105_xdata.py
+-rw-rw-rw-  2.0 fat    14169 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_110_dxfentity.py
+-rw-rw-rw-  2.0 fat     2433 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+-rw-rw-rw-  2.0 fat     6781 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+-rw-rw-rw-  2.0 fat      695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112b_dxfobj.py
+-rw-rw-rw-  2.0 fat     2431 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_113_dxfclass.py
+-rw-rw-rw-  2.0 fat     4044 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_114_factory.py
+-rw-rw-rw-  2.0 fat     2256 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+-rw-rw-rw-  2.0 fat    15794 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_116_dictionary.py
+-rw-rw-rw-  2.0 fat     4999 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+-rw-rw-rw-  2.0 fat      385 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+-rw-rw-rw-  2.0 fat     3003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_120_style_table_entry.py
+-rw-rw-rw-  2.0 fat     2943 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+-rw-rw-rw-  2.0 fat      379 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+-rw-rw-rw-  2.0 fat     1113 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_123_view_table_entry.py
+-rw-rw-rw-  2.0 fat     8757 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+-rw-rw-rw-  2.0 fat     1698 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_125_image_def.py
+-rw-rw-rw-  2.0 fat     1312 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+-rw-rw-rw-  2.0 fat     1430 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_127_raster_variables.py
+-rw-rw-rw-  2.0 fat     1540 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_128_pdf_definition.py
+-rw-rw-rw-  2.0 fat     2778 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_129_xrecord.py
+-rw-rw-rw-  2.0 fat     2423 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_130_id_buffer.py
+-rw-rw-rw-  2.0 fat     2470 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_131_field_list.py
+-rw-rw-rw-  2.0 fat     2435 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_132_layer_filter.py
+-rw-rw-rw-  2.0 fat     2153 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_133_sun.py
+-rw-rw-rw-  2.0 fat      852 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_134_material.py
+-rw-rw-rw-  2.0 fat    11497 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_135_geo_data.py
+-rw-rw-rw-  2.0 fat     1087 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_136_vba_project.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_137_sortentstable.py
+-rw-rw-rw-  2.0 fat      704 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+-rw-rw-rw-  2.0 fat     7570 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_139_user_record.py
+-rw-rw-rw-  2.0 fat      714 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_140_block_record.py
+-rw-rw-rw-  2.0 fat     9199 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+-rw-rw-rw-  2.0 fat     2231 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/conftest.py
+-rw-rw-rw-  2.0 fat     6532 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_200_line.py
+-rw-rw-rw-  2.0 fat     4273 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_201_point.py
+-rw-rw-rw-  2.0 fat     6827 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_202_circle.py
+-rw-rw-rw-  2.0 fat     8949 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_203_arc.py
+-rw-rw-rw-  2.0 fat     2852 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_204_shape.py
+-rw-rw-rw-  2.0 fat     8242 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_205_solid.py
+-rw-rw-rw-  2.0 fat     8476 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_206_text.py
+-rw-rw-rw-  2.0 fat     4947 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_207_attdef.py
+-rw-rw-rw-  2.0 fat     6312 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_208_attrib.py
+-rw-rw-rw-  2.0 fat     2671 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_209_vertex.py
+-rw-rw-rw-  2.0 fat     5930 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_1.py
+-rw-rw-rw-  2.0 fat    13489 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_2.py
+-rw-rw-rw-  2.0 fat     6650 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+-rw-rw-rw-  2.0 fat     1780 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+-rw-rw-rw-  2.0 fat     7847 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_211_viewport.py
+-rw-rw-rw-  2.0 fat    12629 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_212_insert.py
+-rw-rw-rw-  2.0 fat     6024 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_213_minsert.py
+-rw-rw-rw-  2.0 fat     3284 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_214_block.py
+-rw-rw-rw-  2.0 fat     6882 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_215_dimension.py
+-rw-rw-rw-  2.0 fat     4907 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+-rw-rw-rw-  2.0 fat    13186 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+-rw-rw-rw-  2.0 fat     6471 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+-rw-rw-rw-  2.0 fat     5535 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+-rw-rw-rw-  2.0 fat     3056 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+-rw-rw-rw-  2.0 fat     7181 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+-rw-rw-rw-  2.0 fat     2066 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+-rw-rw-rw-  2.0 fat     3615 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+-rw-rw-rw-  2.0 fat     6919 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_221_ellipse.py
+-rw-rw-rw-  2.0 fat     2223 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_222_xline.py
+-rw-rw-rw-  2.0 fat     1493 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_223_ray.py
+-rw-rw-rw-  2.0 fat     2176 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_224_group.py
+-rw-rw-rw-  2.0 fat    10917 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_225_mtext.py
+-rw-rw-rw-  2.0 fat    12020 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline.py
+-rw-rw-rw-  2.0 fat     5529 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+-rw-rw-rw-  2.0 fat    10893 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+-rw-rw-rw-  2.0 fat    15116 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_228_mesh.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+-rw-rw-rw-  2.0 fat    21421 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+-rw-rw-rw-  2.0 fat     6587 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+-rw-rw-rw-  2.0 fat     3140 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+-rw-rw-rw-  2.0 fat    12486 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+-rw-rw-rw-  2.0 fat     2274 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay.py
+-rw-rw-rw-  2.0 fat     5243 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay_2.py
+-rw-rw-rw-  2.0 fat     2294 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis.py
+-rw-rw-rw-  2.0 fat     6799 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis_2.py
+-rw-rw-rw-  2.0 fat     1854 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_surface.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_233_helix.py
+-rw-rw-rw-  2.0 fat     2040 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_234_light.py
+-rw-rw-rw-  2.0 fat     3806 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_235_leader.py
+-rw-rw-rw-  2.0 fat    20392 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_236_multileader.py
+-rw-rw-rw-  2.0 fat    10992 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_237_mline.py
+-rw-rw-rw-  2.0 fat     2356 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_238_tolerance.py
+-rw-rw-rw-  2.0 fat    27392 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+-rw-rw-rw-  2.0 fat     4347 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+-rw-rw-rw-  2.0 fat     1069 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_241_hyperlink.py
+-rw-rw-rw-  2.0 fat    11313 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_242_random_transform.py
+-rw-rw-rw-  2.0 fat     3725 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_243_replace_entity.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+-rw-rw-rw-  2.0 fat     4456 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_245_wipeout.py
+-rw-rw-rw-  2.0 fat     6175 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_246_spline_audit.py
+-rw-rw-rw-  2.0 fat     8165 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+-rw-rw-rw-  2.0 fat     6003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mpolygon.py
+-rw-rw-rw-  2.0 fat    13682 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+-rw-rw-rw-  2.0 fat     5713 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+-rw-rw-rw-  2.0 fat     8331 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+-rw-rw-rw-  2.0 fat     7331 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_251_upright.py
+-rw-rw-rw-  2.0 fat     4795 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+-rw-rw-rw-  2.0 fat     2082 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_253_ole2frame.py
+-rw-rw-rw-  2.0 fat      821 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_254_get_font_name.py
+-rw-rw-rw-  2.0 fat     5149 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_300_layout.py
+-rw-rw-rw-  2.0 fat     4274 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+-rw-rw-rw-  2.0 fat     5582 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_302_block_references.py
+-rw-rw-rw-  2.0 fat     2695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+-rw-rw-rw-  2.0 fat      913 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+-rw-rw-rw-  2.0 fat     3279 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+-rw-rw-rw-  2.0 fat     2609 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+-rw-rw-rw-  2.0 fat     2343 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_307_groupby.py
+-rw-rw-rw-  2.0 fat    17748 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_308_query.py
+-rw-rw-rw-  2.0 fat     6382 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_309_query_parser.py
+-rw-rw-rw-  2.0 fat     5031 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+-rw-rw-rw-  2.0 fat     5782 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+-rw-rw-rw-  2.0 fat      647 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_313_redraw_order.py
+-rw-rw-rw-  2.0 fat     6128 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+-rw-rw-rw-  2.0 fat     2750 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+-rw-rw-rw-  2.0 fat     5208 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+-rw-rw-rw-  2.0 fat     6795 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+-rw-rw-rw-  2.0 fat     4981 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+-rw-rw-rw-  2.0 fat     2450 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_405_classes.py
+-rw-rw-rw-  2.0 fat     9094 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+-rw-rw-rw-  2.0 fat      848 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+-rw-rw-rw-  2.0 fat     3375 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+-rw-rw-rw-  2.0 fat     1433 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+-rw-rw-rw-  2.0 fat     5736 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_410_table.py
+-rw-rw-rw-  2.0 fat     6607 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+-rw-rw-rw-  2.0 fat     1058 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+-rw-rw-rw-  2.0 fat    18072 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+-rw-rw-rw-  2.0 fat     4638 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+-rw-rw-rw-  2.0 fat    12327 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+-rw-rw-rw-  2.0 fat     6509 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+-rw-rw-rw-  2.0 fat     5656 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+-rw-rw-rw-  2.0 fat     5434 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+-rw-rw-rw-  2.0 fat      733 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+-rw-rw-rw-  2.0 fat     1240 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+-rw-rw-rw-  2.0 fat     5007 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+-rw-rw-rw-  2.0 fat      769 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+-rw-rw-rw-  2.0 fat     7289 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_424_audit.py
+-rw-rw-rw-  2.0 fat     3737 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+-rw-rw-rw-  2.0 fat     2981 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+-rw-rw-rw-  2.0 fat     2416 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+-rw-rw-rw-  2.0 fat     2533 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+-rw-rw-rw-  2.0 fat   112800 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/conftest.py
+-rw-rw-rw-  2.0 fat     5510 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_500_units.py
+-rw-rw-rw-  2.0 fat     1052 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_501_truecolor.py
+-rw-rw-rw-  2.0 fat     1021 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_502_raw_color.py
+-rw-rw-rw-  2.0 fat     1695 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_503_indexing.py
+-rw-rw-rw-  2.0 fat     1442 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_504_suppress_zeros.py
+-rw-rw-rw-  2.0 fat      216 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_506_version.py
+-rw-rw-rw-  2.0 fat      579 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_507_dxf_pretty_printer.py
+-rw-rw-rw-  2.0 fat      657 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_508_read_zip.py
+-rw-rw-rw-  2.0 fat     1445 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_509_comments.py
+-rw-rw-rw-  2.0 fat     1185 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_510_byte_stream.py
+-rw-rw-rw-  2.0 fat     4239 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_511_bit_stream.py
+-rw-rw-rw-  2.0 fat     5595 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_512_pattern.py
+-rw-rw-rw-  2.0 fat     2372 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_513_reorder_entities.py
+-rw-rw-rw-  2.0 fat    17710 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_514_text.py
+-rw-rw-rw-  2.0 fat     9269 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_515a_fonts_truetype.py
+-rw-rw-rw-  2.0 fat     4729 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_515b_fonts_shapefiles.py
+-rw-rw-rw-  2.0 fat     2225 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_515c_fonts_lff.py
+-rw-rw-rw-  2.0 fat     4002 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_516_zoom.py
+-rw-rw-rw-  2.0 fat    34209 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_517_text_layout.py
+-rw-rw-rw-  2.0 fat      474 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_518_header_guid.py
+-rw-rw-rw-  2.0 fat     3716 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_519_mtext_editor.py
+-rw-rw-rw-  2.0 fat     3205 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_520_mtext_context.py
+-rw-rw-rw-  2.0 fat    24496 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_521_mtext_parser.py
+-rw-rw-rw-  2.0 fat     3863 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_522_text_scanner.py
+-rw-rw-rw-  2.0 fat     5207 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_523_text_size.py
+-rw-rw-rw-  2.0 fat     5063 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_524_block_reference_manager.py
+-rw-rw-rw-  2.0 fat      773 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_525_transparency.py
+-rw-rw-rw-  2.0 fat     2133 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_526_explode.py
+-rw-rw-rw-  2.0 fat    13521 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_527_gfxattribs.py
+-rw-rw-rw-  2.0 fat     2748 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_528_difftags.py
+-rw-rw-rw-  2.0 fat     6700 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_529_acis_sat.py
+-rw-rw-rw-  2.0 fat     2062 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_530_acis_sab.py
+-rw-rw-rw-  2.0 fat    12366 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_531_acis_entities.py
+-rw-rw-rw-  2.0 fat     7533 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_532_acis_mesh.py
+-rw-rw-rw-  2.0 fat    43206 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_533_shapefiles.py
+-rw-rw-rw-  2.0 fat     1034 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_534_dwg_info.py
+-rw-rw-rw-  2.0 fat    47978 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_535_xref_basic.py
+-rw-rw-rw-  2.0 fat    27614 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_536_xref_conflict.py
+-rw-rw-rw-  2.0 fat     6887 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_537_transform.py
+-rw-rw-rw-  2.0 fat     2246 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+-rw-rw-rw-  2.0 fat     3159 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_539_npshapes.py
+-rw-rw-rw-  2.0 fat     2605 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_05_tools/test_540_lff_parser.py
+-rw-rw-rw-  2.0 fat     4026 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/conftest.py
+-rw-rw-rw-  2.0 fat     7460 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_600_base.py
+-rw-rw-rw-  2.0 fat     2098 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_601_bulge.py
+-rw-rw-rw-  2.0 fat    14651 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_602_vec3.py
+-rw-rw-rw-  2.0 fat     8956 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_603_vec2.py
+-rw-rw-rw-  2.0 fat     2801 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_604_banded_matrix.py
+-rw-rw-rw-  2.0 fat     9738 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_604_linalg.py
+-rw-rw-rw-  2.0 fat    13943 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_605_matrix44.py
+-rw-rw-rw-  2.0 fat     5888 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_606_convexhull.py
+-rw-rw-rw-  2.0 fat     1010 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_607_perlin_noise.py
+-rw-rw-rw-  2.0 fat     3833 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_608_intersection_line_line_2d.py
+-rw-rw-rw-  2.0 fat     1676 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_609_point_on_line.py
+-rw-rw-rw-  2.0 fat     3171 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_610_ocs.py
+-rw-rw-rw-  2.0 fat     7529 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_611_ucs.py
+-rw-rw-rw-  2.0 fat     1831 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_612_ucs_pass_trough.py
+-rw-rw-rw-  2.0 fat     2586 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_613_point_in_poygon.py
+-rw-rw-rw-  2.0 fat    10913 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_614_construct_3d.py
+-rw-rw-rw-  2.0 fat      602 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_615_rytz_axis.py
+-rw-rw-rw-  2.0 fat     5215 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_616_plane.py
+-rw-rw-rw-  2.0 fat      772 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_617_clockwise_orientation.py
+-rw-rw-rw-  2.0 fat     6384 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_618_clipping.py
+-rw-rw-rw-  2.0 fat    10108 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_619_greiner_hormann.py
+-rw-rw-rw-  2.0 fat     2669 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_620_knot.py
+-rw-rw-rw-  2.0 fat    18821 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_621_bspline.py
+-rw-rw-rw-  2.0 fat     7652 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_622_bsplineu.py
+-rw-rw-rw-  2.0 fat    11327 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_623_rbspline.py
+-rw-rw-rw-  2.0 fat    10809 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_624_global_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1247 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_626_local_bspline_interpolation.py
+-rw-rw-rw-  2.0 fat     1967 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_627_bspline_basis.py
+-rw-rw-rw-  2.0 fat    10545 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_629_bezier.py
+-rw-rw-rw-  2.0 fat    10714 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_630a_bezier4p_base.py
+-rw-rw-rw-  2.0 fat    10204 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_630b_bezier4p_functions.py
+-rw-rw-rw-  2.0 fat     1683 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_631_euler_spiral.py
+-rw-rw-rw-  2.0 fat     4021 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_632_bezier3p.py
+-rw-rw-rw-  2.0 fat    19463 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_640_bbox.py
+-rw-rw-rw-  2.0 fat     5393 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_641_construction_ray.py
+-rw-rw-rw-  2.0 fat     3673 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_642_construction_line.py
+-rw-rw-rw-  2.0 fat     9459 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_643_construction_box.py
+-rw-rw-rw-  2.0 fat    10941 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_644_construction_circle.py
+-rw-rw-rw-  2.0 fat    10988 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_645_construction_arc.py
+-rw-rw-rw-  2.0 fat     3422 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_646_offset_vertices_2d.py
+-rw-rw-rw-  2.0 fat     7672 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_647_transform_tools.py
+-rw-rw-rw-  2.0 fat     8993 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_648_construction_ellipse.py
+-rw-rw-rw-  2.0 fat     4243 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_650_elliptic_arc_span.py
+-rw-rw-rw-  2.0 fat     9011 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_651_construction_polyline.py
+-rw-rw-rw-  2.0 fat     3168 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_652_approx_param_t.py
+-rw-rw-rw-  2.0 fat     5806 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_653_polyline_intersection.py
+-rw-rw-rw-  2.0 fat     5193 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_654_rtree.py
+-rw-rw-rw-  2.0 fat      788 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_655_dbscan.py
+-rw-rw-rw-  2.0 fat      834 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_656_k_means.py
+-rw-rw-rw-  2.0 fat     4654 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_657_mapbox_earcut.py
+-rw-rw-rw-  2.0 fat    11628 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_658_bevel_tools.py
+-rw-rw-rw-  2.0 fat     1875 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1428 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+-rw-rw-rw-  2.0 fat     1741 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+-rw-rw-rw-  2.0 fat     3307 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_06_math/test_662_is_convex_polygon_2d.py
+-rw-rw-rw-  2.0 fat     1466 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_701_arrows.py
+-rw-rw-rw-  2.0 fat    17245 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_702_render_forms.py
+-rw-rw-rw-  2.0 fat    34220 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_703_mesh_builder.py
+-rw-rw-rw-  2.0 fat     3852 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_704_render_linear_dimension.py
+-rw-rw-rw-  2.0 fat     1345 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_705_shape.py
+-rw-rw-rw-  2.0 fat      483 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_706_random_path.py
+-rw-rw-rw-  2.0 fat     5603 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_707_trace.py
+-rw-rw-rw-  2.0 fat    33834 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708a_path.py
+-rw-rw-rw-  2.0 fat    27351 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708b_path_tools.py
+-rw-rw-rw-  2.0 fat     3633 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708c_matplotlib_path_tools.py
+-rw-rw-rw-  2.0 fat     3099 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708d_qpainter_path_tools.py
+-rw-rw-rw-  2.0 fat     4589 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708e_path_shapes.py
+-rw-rw-rw-  2.0 fat     4118 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_708f_path_nesting.py
+-rw-rw-rw-  2.0 fat     1308 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_709_linetype_renderer.py
+-rw-rw-rw-  2.0 fat     2815 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_711_points.py
+-rw-rw-rw-  2.0 fat     6594 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_712_render_curved_dimension.py
+-rw-rw-rw-  2.0 fat     1472 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_713_mleader_builder.py
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_714_mleader_render_engine.py
+-rw-rw-rw-  2.0 fat    11778 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_715_hatching.py
+-rw-rw-rw-  2.0 fat     2626 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+-rw-rw-rw-  2.0 fat     4771 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_800_mtext_surrogate.py
+-rw-rw-rw-  2.0 fat     1352 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_801_r12spline.py
+-rw-rw-rw-  2.0 fat     7881 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_802_table_painter.py
+-rw-rw-rw-  2.0 fat    12386 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_803_entities_to_code.py
+-rw-rw-rw-  2.0 fat     6844 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_804_importer.py
+-rw-rw-rw-  2.0 fat     2362 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_805_pycsg.py
+-rw-rw-rw-  2.0 fat    15467 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_806_acadctb.py
+-rw-rw-rw-  2.0 fat     4860 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_807_dwg_loader_basics.py
+-rw-rw-rw-  2.0 fat    10862 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_810_drawing_properties.py
+-rw-rw-rw-  2.0 fat    11353 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_811a_drawing_frontend.py
+-rw-rw-rw-  2.0 fat     4310 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_811b_drawing_recorder.py
+-rw-rw-rw-  2.0 fat     2898 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_811c_viewport_processing.py
+-rw-rw-rw-  2.0 fat     4157 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+-rw-rw-rw-  2.0 fat    12547 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_813_geo_interface.py
+-rw-rw-rw-  2.0 fat    14853 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_814_text2path.py
+-rw-rw-rw-  2.0 fat    16239 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_815_dxf_browser.py
+-rw-rw-rw-  2.0 fat    11275 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_816_bin_packing.py
+-rw-rw-rw-  2.0 fat    12554 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_817_genetic_algorithm.py
+-rw-rw-rw-  2.0 fat     9008 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_818_meshex.py
+-rw-rw-rw-  2.0 fat     1003 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_819_menger_sponge.py
+-rw-rw-rw-  2.0 fat     4433 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_820_openscad.py
+-rw-rw-rw-  2.0 fat    15655 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2.py
+-rw-rw-rw-  2.0 fat     1376 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+-rw-rw-rw-  2.0 fat      976 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_822_clipper.py
+-rw-rw-rw-  2.0 fat     5284 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_823_drawing_layout.py
+-rw-rw-rw-  2.0 fat     3255 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_824_svg_drawing_backend.py
+-rw-rw-rw-  2.0 fat     1965 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
+-rw-rw-rw-  2.0 fat     2527 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+-rw-rw-rw-  2.0 fat     2199 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+-rw-rw-rw-  2.0 fat     2142 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+-rw-rw-rw-  2.0 fat     3158 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+-rw-rw-rw-  2.0 fat     1452 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+-rw-rw-rw-  2.0 fat     4755 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+-rw-rw-rw-  2.0 fat     2656 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_414_bbox_calculation.py
+-rw-rw-rw-  2.0 fat     1213 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+-rw-rw-rw-  2.0 fat     2268 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_574_flattening_error.py
+-rw-rw-rw-  2.0 fat     1754 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+-rw-rw-rw-  2.0 fat      682 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_749_text_layout.py
+-rw-rw-rw-  2.0 fat    11094 b- defN 23-May-31 05:23 ezdxf-1.1.0b3/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+839 files, 8700179 bytes uncompressed, 1960443 bytes compressed:  77.5%
```

## zipnote {}

```diff
@@ -1,2515 +1,2518 @@
-Filename: ezdxf-1.1.0b2/
+Filename: ezdxf-1.1.0b3/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/
+Filename: ezdxf-1.1.0b3/integration_tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/
+Filename: ezdxf-1.1.0b3/src/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/
+Filename: ezdxf-1.1.0b3/tests/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/LICENSE
+Filename: ezdxf-1.1.0b3/LICENSE
 Comment: 
 
-Filename: ezdxf-1.1.0b2/MANIFEST.in
+Filename: ezdxf-1.1.0b3/MANIFEST.in
 Comment: 
 
-Filename: ezdxf-1.1.0b2/NEWS.md
+Filename: ezdxf-1.1.0b3/NEWS.md
 Comment: 
 
-Filename: ezdxf-1.1.0b2/PKG-INFO
+Filename: ezdxf-1.1.0b3/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b2/README.md
+Filename: ezdxf-1.1.0b3/README.md
 Comment: 
 
-Filename: ezdxf-1.1.0b2/requirements.txt
+Filename: ezdxf-1.1.0b3/requirements.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b2/setup.cfg
+Filename: ezdxf-1.1.0b3/setup.cfg
 Comment: 
 
-Filename: ezdxf-1.1.0b2/setup.py
+Filename: ezdxf-1.1.0b3/setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/
+Filename: ezdxf-1.1.0b3/integration_tests/data/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_config_file.py
+Filename: ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_config_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_env_var.py
+Filename: ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_env_var.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/conftest.py
+Filename: ezdxf-1.1.0b3/integration_tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_acad_table.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_all_dimline_styles.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_all_dimline_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_all_ellipse_transformations.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_all_ellipse_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_anonymous_blocks.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_anonymous_blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_audit_critical_dxf_files.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_audit_critical_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_audit_layouts.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_audit_layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_complex_line_type_2.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_complex_line_type_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_create_basic_graphics.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_create_basic_graphics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_document_guid.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_document_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_document_page_setup.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_document_page_setup.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_dxf_info_scanning.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_dxf_info_scanning.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_entities_iterator.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_entities_iterator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_fix_dulicate_handles.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_fix_dulicate_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_geo.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_groups.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_groups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_hpgl2_addon.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_hpgl2_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_ignore_junk_beyond_EOF.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_ignore_junk_beyond_EOF.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_launcher.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_launcher.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_leica_disto_r12.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_leica_disto_r12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_load_dxf_unicode_notation.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_load_dxf_unicode_notation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_mapbox_earcut.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_mtext_columns.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_mtext_explode_addon.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_mtext_explode_addon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_mtext_text_frame.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_mtext_text_frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_new_table_entries.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_new_table_entries.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_none_ascii_read_write.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_none_ascii_read_write.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_odafc.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_open_binary_DXF_files.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_open_binary_DXF_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_open_coord_order_issue.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_open_coord_order_issue.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_open_exotic_dxf_files.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_open_exotic_dxf_files.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_open_R13_R14.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_open_R13_R14.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_polyline_entity.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_polyline_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_preserve_binary_data_in_xrecords.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_preserve_binary_data_in_xrecords.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_r12export.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_r12strict.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_r12writer.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_read_file_without_handles.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_read_file_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_read_write_modern_entites.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_read_write_modern_entites.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_recover.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_redraw_order.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_rotated_block_attributes.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_rotated_block_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_surface_entities.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_surface_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_write_fixed_meta_data.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_write_fixed_meta_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_write_without_handles.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_write_without_handles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/test_xref_detach.py
+Filename: ezdxf-1.1.0b3/integration_tests/test_xref_detach.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/AC1003_LINE_Example.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/AC1003_LINE_Example.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/acad_table_with_blk_ref.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/acad_table_with_blk_ref.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/ASCII_R12.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/ASCII_R12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r12.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r12.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r13.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r14.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r2000.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r2000.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/cc_dxflib.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/cc_dxflib.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/custom_blocks.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/custom_blocks.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/duplicate_handles.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/duplicate_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/dxf_unicode.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/dxf_unicode.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/empty_handles.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/empty_handles.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/groups.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/groups.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/Leica_Disto_S910.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/Leica_Disto_S910.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/MODEL.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/MODEL.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2007.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2007.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2018.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2018.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/mtext_framed_columns.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/mtext_framed_columns.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/mtext_text_frame.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/mtext_text_frame.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/no_layouts.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/no_layouts.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/PLOTFILE.plt
+Filename: ezdxf-1.1.0b3/integration_tests/data/PLOTFILE.plt
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/POLI-ALL210_12.DXF
+Filename: ezdxf-1.1.0b3/integration_tests/data/POLI-ALL210_12.DXF
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/R12_with_trash_beyond_EOF.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/R12_with_trash_beyond_EOF.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/recover01.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/recover01.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/recover02.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/recover02.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/small_r13.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/small_r13.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/small_r14.dxf
+Filename: ezdxf-1.1.0b3/integration_tests/data/small_r14.dxf
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/XRECORD_0.bin
+Filename: ezdxf-1.1.0b3/integration_tests/data/XRECORD_0.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/XRECORD_1.bin
+Filename: ezdxf-1.1.0b3/integration_tests/data/XRECORD_1.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b2/integration_tests/data/XRECORD_2.bin
+Filename: ezdxf-1.1.0b3/integration_tests/data/XRECORD_2.bin
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/
+Filename: ezdxf-1.1.0b3/src/ezdxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/
+Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/
+Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/path/
+Filename: ezdxf-1.1.0b3/src/ezdxf/path/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/appsettings.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/audit.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/bbox.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/blkrefs.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/blkrefs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/colors.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/colors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/commands.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/comments.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/disassemble.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/document.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/document.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/dwginfo.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/dwginfo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entitydb.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entitydb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/enums.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/enums.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/explode.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/eztypes.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/eztypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/filemanagement.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/filemanagement.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/gfxattribs.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/graphicsfactory.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/graphicsfactory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/groupby.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/npshapes.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/protocols.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/protocols.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/proxygraphic.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/proxygraphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/py.typed
+Filename: ezdxf-1.1.0b3/src/ezdxf/py.typed
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/query.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/queryparser.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/queryparser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/r12strict.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/r12strict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/recover.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/recover.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/reorder.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/reorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/transform.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/units.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/upright.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/urecord.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/urecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/version.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/xref.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/xref.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/zoom.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/_options.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/_options.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/__main__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/__main__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/bezier3p.pyx
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/bezier3p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/bezier4p.pyx
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/bezier4p.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/bspline.pyx
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/bspline.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/construct.pxd
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/construct.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/construct.pyx
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/construct.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/linetypes.pyx
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/linetypes.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/mapbox_earcut.pyx
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/mapbox_earcut.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pxd
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pyx
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/vector.pxd
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/vector.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/vector.pyx
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/vector.pyx
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.cpp
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.hpp
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.pxd
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.cpp
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.cpp
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.hpp
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.pxd
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.hpp
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.hpp
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.pxd
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.pxd
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acc/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acc/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/abstract.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/abstract.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/api.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/const.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/dbg.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/dbg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/dxf.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/dxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/entities.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/hdr.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/hdr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/mesh.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/sab.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/sat.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/acis/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/acis/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acadctb.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/binpacking.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/binpacking.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dimlines.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dimlines.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dxf2code.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dxf2code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/genetic_algorithm.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/geo.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/geo.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/gerber_D6673.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/gerber_D6673.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/importer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/iterdxf.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/iterdxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/menger_sponge.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/meshex.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/mixins.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/mixins.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/mtextsurrogate.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/mtextsurrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/mtxpl.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/mtxpl.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/odafc.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/odafc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/openscad.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/pycsg.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/r12export.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/r12export.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/r12writer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/r12writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/sierpinski_pyramid.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/sierpinski_pyramid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/tablepainter.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/tablepainter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/text2path.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/xplayer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/xplayer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/xqt.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/xqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/browser.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/data.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/bookmarks.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/bookmarks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/browser.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/data.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/find_dialog.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/find_dialog.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/loader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/model.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/model.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/tags.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/views.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/views.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/browser/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/browser/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/backend.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/clipper.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/config.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/config.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_backend.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_utils.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_utils.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/frontend.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/dxf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/gfxproxy.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/layout.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/gfxproxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/matplotlib.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/mtext_complex.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/properties.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/matplotlib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/pyqt.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/mtext_complex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/qtviewer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/recorder.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pymupdf.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/svg.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pyqt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/qtviewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text_renderer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/type_hints.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/svg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/unified_text_renderer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/drawing/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/classes_section.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/type_hints.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/const.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/unified_text_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/crc.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/drawing/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/fileheader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/classes_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/header_section.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/loader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/crc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/dwg/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/fileheader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/api.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/header_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/backend.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/compiler.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/dwg/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/deps.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/api.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/dxf_backend.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/interpreter.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/deps.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/page.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/interpreter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/pdf_backend.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/page.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/plotter.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/plotter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/polygon_buffer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/polygon_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/properties.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/svg_backend.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/tokenizer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/tokenizer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/viewer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/viewer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/acad_proxy_entity.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/acad_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/acad_table.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/acis.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/appdata.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/appid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/appid.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/arc.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/attrib.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/block.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/blockrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/blockrecord.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/boundary_paths.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/circle.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dictionary.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dimension.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dimstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dimstyle.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dimstyleoverride.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dimstyleoverride.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfclass.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfentity.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfgfx.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfgroups.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfns.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/dxfobj.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/ellipse.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/factory.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/geodata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/geodata.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/gradient.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/gradient.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/hatch.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/hatch.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/helix.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/idbuffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/idbuffer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/image.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/image.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/insert.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/layer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/layout.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/leader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/light.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/line.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/ltype.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/lwpolyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/lwpolyline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/material.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mesh.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mleader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mpolygon.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mtext.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/mtext_columns.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/mtext_columns.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/objectcollection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/objectcollection.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/oleframe.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/oleframe.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/pattern.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/point.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/polygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/polygon.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/polyline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/shape.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/solid.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/spline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/subentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/subentity.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/sun.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/table.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/text.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/textstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/textstyle.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/tolerance.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/ucs.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/underlay.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/view.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/view.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/viewport.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/visualstyle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/visualstyle.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/vport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/vport.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/xdata.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/xdict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/xdict.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/xline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/entities/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/entities/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/fonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/fonts.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/font_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/font_face.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/font_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/font_manager.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/font_measurements.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/font_measurements.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/glyphs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/glyphs.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/lff.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/shapefile.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/shapefile.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/ttfonts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/ttfonts.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/fonts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/fonts/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/base.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/blocklayout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/blocklayout.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/layout.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/layouts.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/layouts.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/layouts/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/layouts/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/attributes.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/const.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/const.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/encoding.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/extendedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/extendedtags.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/fileindex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/fileindex.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/hdrvars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/hdrvars.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/loader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/packedtags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/packedtags.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/repair.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/repair.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/tagger.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/tagger.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/tags.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/tagwriter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/tagwriter.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/types.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/validator.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/lldxf/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/lldxf/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/arc.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/bbox.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/bezier.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/bezier_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/bezier_interpolation.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/box.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/bspline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/bulge.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/circle.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/clipping.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/clustering.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/clustering.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/construct2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/construct2d.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/construct3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/construct3d.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/cspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/cspline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/curvetools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/curvetools.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/ellipse.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/eulerspiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/eulerspiral.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/linalg.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/line.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/offset2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/offset2d.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/parametrize.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/parametrize.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/perlin.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/perlin.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/polyline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/rtree.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/shape.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/surfaces.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/surfaces.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/transformtools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/transformtools.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/triangulation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/triangulation.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/ucs.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/_bezier3p.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/_bezier4p.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/_bspline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/_construct.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/_construct.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/_ctypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/_ctypes.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/_mapbox_earcut.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/_matrix44.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/_vector.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/_vector.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/math/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/math/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/path/commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/path/commands.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/path/converter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/path/converter.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/path/nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/path/nesting.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/path/path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/path/path.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/path/shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/path/shapes.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/path/tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/path/tools.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/path/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/path/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.css
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.html
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.js
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.js
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/pprint.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/pprint.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.css
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.css
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.html
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.html
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/reflinks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/reflinks.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/pp/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/pp/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/abstract_mtext_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/abstract_mtext_renderer.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/arrows.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/curves.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/curves.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/dimension.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_base.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_curved.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_curved.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_diameter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_diameter.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_linear.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_linear.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_ordinate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_ordinate.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/dim_radius.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/dim_radius.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/forms.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/hatching.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/leader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/linetypes.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/mesh.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/mleader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/mleader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/mline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/point.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/polyline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/r12spline.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/trace.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/_linetypes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/_linetypes.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/render/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/render/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/16x16.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/16x16.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/24x24.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/24x24.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/256x256.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/256x256.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/32x32.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/32x32.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/48x48.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/48x48.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/64x64.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/64x64.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-copy-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-copy-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-find-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-find-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-bookmark-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-handle-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-handle-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-line-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-line-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-left-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-left-arrow-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-next-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-next-entity-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-prev-entity-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-prev-entity-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-right-arrow-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-right-arrow-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-show-in-tree-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-show-in-tree-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/resources/icon-store-bookmark-64px.png
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/resources/icon-store-bookmark-64px.png
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/acdsdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/acdsdata.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/blocks.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/blocks.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/classes.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/entities.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/header.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/header.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/headervars.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/headervars.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/objects.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/table.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/tables.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/sections/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/sections/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/analyze.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/analyze.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/binarydata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/binarydata.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/codepage.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/complex_ltype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/complex_ltype.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/crypt.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/debug.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/debug.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/difftags.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/handle.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/indexing.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/juliandate.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/pattern.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/rawloader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/rawloader.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/standards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/standards.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/strip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/strip.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/test.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/test.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/text.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/text_layout.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/text_size.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/zipmanager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/zipmanager.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/_iso_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/_iso_pattern.py
+Filename: ezdxf-1.1.0b3/src/ezdxf/tools/__init__.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf/tools/__init__.py
+Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/dependency_links.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/dependency_links.txt
+Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/entry_points.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/entry_points.txt
+Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/not-zip-safe
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/not-zip-safe
+Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/PKG-INFO
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/PKG-INFO
+Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/requires.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/requires.txt
+Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/SOURCES.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/SOURCES.txt
+Filename: ezdxf-1.1.0b3/src/ezdxf.egg-info/top_level.txt
 Comment: 
 
-Filename: ezdxf-1.1.0b2/src/ezdxf.egg-info/top_level.txt
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/
+Filename: ezdxf-1.1.0b3/tests/test_06_math/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/
+Filename: ezdxf-1.1.0b3/tests/test_07_render/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/
+Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/
+Filename: ezdxf-1.1.0b3/tests/test_10_issues/
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_10_issues/
+Filename: ezdxf-1.1.0b3/tests/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/conftest.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_010_binary_data.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_011_codepage.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_011_codepage.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_012_crypt.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_012_crypt.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_013_juliandate.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_016_encoding.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_016_encoding.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_018_handle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_018_handle.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_022_set_flag_state.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_024_render_tag.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_040_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_040_tags.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_041_group_tags.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py
+Filename: ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_101_dxfnamespace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_101_dxfnamespace.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_102_appdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_102_appdata.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_103_reactors.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_103_reactors.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_104_extension_dict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_104_extension_dict.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_105_xdata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_105_xdata.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_110_dxfentity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_110_dxfentity.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112a_dxfgfx.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112a_dxfgfx.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112b_dxfobj.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112b_dxfobj.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_113_dxfclass.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_113_dxfclass.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_114_factory.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_114_factory.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_115_new_empty_drawing.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_116_dictionary.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_116_dictionary.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_117_layer_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_117_layer_table_entry.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_118_appid_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_118_appid_table_entry.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_119_ucs_table_entry.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_120_style_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_120_style_table_entry.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_121_ltype_table_entry.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_122_vport_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_122_vport_table_entry.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_123_view_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_123_view_table_entry.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_125_image_def.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_125_image_def.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_126_image_def_reactor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_126_image_def_reactor.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_127_raster_variables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_127_raster_variables.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_128_pdf_definition.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_128_pdf_definition.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_129_xrecord.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_129_xrecord.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_130_id_buffer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_130_id_buffer.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_131_field_list.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_131_field_list.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_132_layer_filter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_132_layer_filter.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_133_sun.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_133_sun.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_134_material.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_134_material.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_135_geo_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_135_geo_data.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_136_vba_project.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_136_vba_project.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_137_sortentstable.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_137_sortentstable.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_138_setup_visual_styles.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_139_user_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_139_user_record.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_140_block_record.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_140_block_record.py
+Filename: ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_141_layer_vp_override.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_141_layer_vp_override.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/conftest.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_200_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_200_line.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_201_point.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_201_point.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_202_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_202_circle.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_203_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_203_arc.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_204_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_204_shape.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_205_solid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_205_solid.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_206_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_206_text.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_207_attdef.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_207_attdef.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_208_attrib.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_208_attrib.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_209_vertex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_209_vertex.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_1.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_2.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_explode.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_211_viewport.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_211_viewport.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_212_insert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_212_insert.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_213_minsert.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_213_minsert.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_214_block.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_214_block.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_215_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_215_dimension.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_216_dimlines_R12.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_221_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_221_ellipse.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_222_xline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_222_xline.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_223_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_223_ray.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_224_group.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_224_group.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_225_mtext.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_225_mtext.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_228_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_228_mesh.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229b_hatch_extended.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay_2.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis_2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis_2.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_surface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_surface.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_233_helix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_233_helix.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_234_light.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_234_light.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_235_leader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_235_leader.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_236_multileader.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_236_multileader.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_237_mline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_237_mline.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_238_tolerance.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_238_tolerance.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_239_proxy_graphic.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_240_arc_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_240_arc_dimension.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_241_hyperlink.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_241_hyperlink.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_242_random_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_242_random_transform.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_243_replace_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_243_replace_entity.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_245_wipeout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_245_wipeout.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_246_spline_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_246_spline_audit.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mpolygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mpolygon.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_249_boundary_paths.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_249_boundary_paths.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_251_upright.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_251_upright.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_253_ole2frame.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_253_ole2frame.py
+Filename: ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_254_get_font_name.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_254_get_font_name.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_300_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_300_layout.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_302_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_302_block_references.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_303_auto_block_references.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_303_auto_block_references.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_304_new_entity_space.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_304_new_entity_space.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_307_groupby.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_307_groupby.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_308_query.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_308_query.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_309_query_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_309_query_parser.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_312_virtual_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_312_virtual_layout.py
+Filename: ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_313_redraw_order.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_313_redraw_order.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_401_headersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_401_headersection.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_402_classessection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_402_classessection.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_403_entity_database.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404a_tables.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404a_tables.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_405_classes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_405_classes.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_407_entity_section.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_408_objects_section.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_409_create_objects.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_410_table.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_410_table.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_411_acds_data.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_415_layout_management.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_417_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_417_bbox.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_424_audit.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_424_audit.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_427_appsettings.py
+Filename: ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/conftest.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_500_units.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_500_units.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_501_truecolor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_501_truecolor.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_502_raw_color.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_502_raw_color.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_503_indexing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_503_indexing.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_504_suppress_zeros.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_504_suppress_zeros.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_506_version.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_506_version.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_507_dxf_pretty_printer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_507_dxf_pretty_printer.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_508_read_zip.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_508_read_zip.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_509_comments.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_509_comments.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_510_byte_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_510_byte_stream.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_511_bit_stream.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_511_bit_stream.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_512_pattern.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_512_pattern.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_513_reorder_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_513_reorder_entities.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_514_text.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_514_text.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_515a_fonts_truetype.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_515a_fonts_truetype.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_515b_fonts_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_515b_fonts_shapefiles.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_515c_fonts_lff.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_515c_fonts_lff.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_516_zoom.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_516_zoom.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_517_text_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_517_text_layout.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_518_header_guid.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_518_header_guid.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_519_mtext_editor.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_519_mtext_editor.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_520_mtext_context.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_520_mtext_context.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_521_mtext_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_521_mtext_parser.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_522_text_scanner.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_522_text_scanner.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_523_text_size.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_523_text_size.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_524_block_reference_manager.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_524_block_reference_manager.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_525_transparency.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_525_transparency.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_526_explode.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_526_explode.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_527_gfxattribs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_527_gfxattribs.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_528_difftags.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_528_difftags.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_529_acis_sat.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_529_acis_sat.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_530_acis_sab.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_530_acis_sab.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_531_acis_entities.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_531_acis_entities.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_532_acis_mesh.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_532_acis_mesh.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_533_shapefiles.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_533_shapefiles.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_534_dwg_info.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_534_dwg_info.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_535_xref_basic.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_535_xref_basic.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_536_xref_conflict.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_536_xref_conflict.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_537_transform.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_537_transform.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_538_scale_mtext_inline_commands.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_539_npshapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_539_npshapes.py
+Filename: ezdxf-1.1.0b3/tests/test_05_tools/test_540_lff_parser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_05_tools/test_540_lff_parser.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/conftest.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/conftest.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_600_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_600_base.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_601_bulge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_601_bulge.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_602_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_602_vec3.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_603_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_603_vec2.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_604_banded_matrix.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_604_banded_matrix.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_604_linalg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_604_linalg.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_605_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_605_matrix44.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_606_convexhull.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_606_convexhull.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_607_perlin_noise.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_607_perlin_noise.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_608_intersection_line_line_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_608_intersection_line_line_2d.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_609_point_on_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_609_point_on_line.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_610_ocs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_610_ocs.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_611_ucs.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_611_ucs.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_612_ucs_pass_trough.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_612_ucs_pass_trough.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_613_point_in_poygon.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_613_point_in_poygon.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_614_construct_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_614_construct_3d.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_615_rytz_axis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_615_rytz_axis.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_616_plane.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_616_plane.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_617_clockwise_orientation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_617_clockwise_orientation.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_618_clipping.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_618_clipping.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_619_greiner_hormann.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_619_greiner_hormann.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_620_knot.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_620_knot.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_621_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_621_bspline.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_622_bsplineu.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_622_bsplineu.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_623_rbspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_623_rbspline.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_624_global_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_624_global_bspline_interpolation.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_626_local_bspline_interpolation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_626_local_bspline_interpolation.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_627_bspline_basis.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_627_bspline_basis.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_629_bezier.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_629_bezier.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_630a_bezier4p_base.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_630a_bezier4p_base.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_630b_bezier4p_functions.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_630b_bezier4p_functions.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_631_euler_spiral.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_631_euler_spiral.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_632_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_632_bezier3p.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_640_bbox.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_640_bbox.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_641_construction_ray.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_641_construction_ray.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_642_construction_line.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_642_construction_line.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_643_construction_box.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_643_construction_box.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_644_construction_circle.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_644_construction_circle.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_645_construction_arc.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_645_construction_arc.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_646_offset_vertices_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_646_offset_vertices_2d.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_647_transform_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_647_transform_tools.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_648_construction_ellipse.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_648_construction_ellipse.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_650_elliptic_arc_span.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_650_elliptic_arc_span.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_651_construction_polyline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_651_construction_polyline.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_652_approx_param_t.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_652_approx_param_t.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_653_polyline_intersection.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_653_polyline_intersection.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_654_rtree.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_654_rtree.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_655_dbscan.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_655_dbscan.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_656_k_means.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_656_k_means.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_657_mapbox_earcut.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_657_mapbox_earcut.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_658_bevel_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_658_bevel_tools.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_659_intersection_line_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_659_intersection_line_polygon_3d.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_660_intersection_ray_polygon_3d.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py
+Filename: ezdxf-1.1.0b3/tests/test_06_math/test_662_is_convex_polygon_2d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_06_math/test_662_is_convex_polygon_2d.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_701_arrows.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_701_arrows.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_702_render_forms.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_702_render_forms.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_703_mesh_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_703_mesh_builder.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_704_render_linear_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_704_render_linear_dimension.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_705_shape.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_705_shape.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_706_random_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_706_random_path.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_707_trace.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_707_trace.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708a_path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708a_path.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708b_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708b_path_tools.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708c_matplotlib_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708c_matplotlib_path_tools.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708d_qpainter_path_tools.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708d_qpainter_path_tools.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708e_path_shapes.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708e_path_shapes.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_708f_path_nesting.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_708f_path_nesting.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_709_linetype_renderer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_709_linetype_renderer.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_711_points.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_711_points.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_712_render_curved_dimension.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_712_render_curved_dimension.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_713_mleader_builder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_713_mleader_builder.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_714_mleader_render_engine.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_714_mleader_render_engine.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_715_hatching.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_715_hatching.py
+Filename: ezdxf-1.1.0b3/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_07_render/test_715_issue_747_explode_3d_dim.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_800_mtext_surrogate.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_800_mtext_surrogate.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_801_r12spline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_801_r12spline.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_802_table_painter.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_802_table_painter.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_803_entities_to_code.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_803_entities_to_code.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_804_importer.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_804_importer.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_805_pycsg.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_805_pycsg.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_806_acadctb.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_806_acadctb.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_807_dwg_loader_basics.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_807_dwg_loader_basics.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_810_drawing_properties.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_810_drawing_properties.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_811a_drawing_frontend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_811a_drawing_frontend.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_811b_drawing_recorder.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_811b_drawing_recorder.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_811c_viewport_processing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_812_drawing_graphic_proxy.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_812_drawing_graphic_proxy.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_813_geo_interface.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_813_geo_interface.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_814_text2path.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_814_text2path.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_815_dxf_browser.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_815_dxf_browser.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_816_bin_packing.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_816_bin_packing.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_817_genetic_algorithm.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_817_genetic_algorithm.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_818_meshex.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_818_meshex.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_819_menger_sponge.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_819_menger_sponge.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_820_openscad.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_820_openscad.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_822_clipper.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_822_clipper.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_823_drawing_layout.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_823_drawing_layout.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_08_addons/test_824_svg_drawing_backend.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_824_svg_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_901_acc_vec2.py
+Filename: ezdxf-1.1.0b3/tests/test_08_addons/test_825_hpgl2_drawing_backend.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_902_acc_vec3.py
+Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_901_acc_vec2.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
+Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_902_acc_vec3.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
+Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
+Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_906_acc_bspline.py
+Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_414_bbox_calculation.py
+Filename: ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_906_acc_bspline.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
+Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_414_bbox_calculation.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_574_flattening_error.py
+Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
+Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_574_flattening_error.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_749_text_layout.py
+Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py
 Comment: 
 
-Filename: ezdxf-1.1.0b2/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
+Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_749_text_layout.py
+Comment: 
+
+Filename: ezdxf-1.1.0b3/tests/test_10_issues/test_issue_873_circle_inverted_normal.py
 Comment: 
 
 Zip file comment:
```

## Comparing `ezdxf-1.1.0b2/LICENSE` & `ezdxf-1.1.0b3/LICENSE`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/NEWS.md` & `ezdxf-1.1.0b3/NEWS.md`

 * *Files 0% similar despite different names*

```diff
@@ -10,33 +10,37 @@
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
 - NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
-- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF
-- NEW: native `SVG` backend for the `drawing` add-on
+- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF, PNG
+- NEW: native `SVG`, `HPGL/2`  and `DXF` backends for the `drawing` add-on, these backends 
+  do not need additional libraries to work
+- NEW: `PyMuPdf` backend for the `drawing` add-on, support for PDF, PNG, PPM and PBM export
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
   add-on to change/override foreground- and background color by the frontend 
+- NEW: `TextPolicy` configuration settings for the `drawing` add-on, render text as 
+  solid filling, outline path, replace text by (filled) rectangles or ignore text at all 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
-- REMOVED: `PillowBackend` and the `pillow` command
+- REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
 
 Version 1.0.3 - 2023-03-26
 --------------------------
```

## Comparing `ezdxf-1.1.0b2/PKG-INFO` & `ezdxf-1.1.0b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -223,33 +223,37 @@
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
 - NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
-- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF
-- NEW: native `SVG` backend for the `drawing` add-on
+- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF, PNG
+- NEW: native `SVG`, `HPGL/2`  and `DXF` backends for the `drawing` add-on, these backends 
+  do not need additional libraries to work
+- NEW: `PyMuPdf` backend for the `drawing` add-on, support for PDF, PNG, PPM and PBM export
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
   add-on to change/override foreground- and background color by the frontend 
+- NEW: `TextPolicy` configuration settings for the `drawing` add-on, render text as 
+  solid filling, outline path, replace text by (filled) rectangles or ignore text at all 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
-- REMOVED: `PillowBackend` and the `pillow` command
+- REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
 
 Version 1.0.3 - 2023-03-26
 --------------------------
```

## Comparing `ezdxf-1.1.0b2/README.md` & `ezdxf-1.1.0b3/README.md`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/setup.py` & `ezdxf-1.1.0b3/setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_config_file.py` & `ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_config_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/check_disable_c_ext_by_env_var.py` & `ezdxf-1.1.0b3/integration_tests/check_disable_c_ext_by_env_var.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_acad_table.py` & `ezdxf-1.1.0b3/integration_tests/test_acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_all_dimline_styles.py` & `ezdxf-1.1.0b3/integration_tests/test_all_dimline_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_all_ellipse_transformations.py` & `ezdxf-1.1.0b3/integration_tests/test_all_ellipse_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_anonymous_blocks.py` & `ezdxf-1.1.0b3/integration_tests/test_anonymous_blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_audit_critical_dxf_files.py` & `ezdxf-1.1.0b3/integration_tests/test_audit_critical_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_audit_layouts.py` & `ezdxf-1.1.0b3/integration_tests/test_audit_layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_complex_line_type_2.py` & `ezdxf-1.1.0b3/integration_tests/test_complex_line_type_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_create_basic_graphics.py` & `ezdxf-1.1.0b3/integration_tests/test_create_basic_graphics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_document_guid.py` & `ezdxf-1.1.0b3/integration_tests/test_document_guid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_document_page_setup.py` & `ezdxf-1.1.0b3/integration_tests/test_document_page_setup.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_dxf_info_scanning.py` & `ezdxf-1.1.0b3/integration_tests/test_dxf_info_scanning.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_entities_iterator.py` & `ezdxf-1.1.0b3/integration_tests/test_entities_iterator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_fix_dulicate_handles.py` & `ezdxf-1.1.0b3/integration_tests/test_fix_dulicate_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_geo.py` & `ezdxf-1.1.0b3/integration_tests/test_geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_groups.py` & `ezdxf-1.1.0b3/integration_tests/test_groups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_hpgl2_addon.py` & `ezdxf-1.1.0b3/integration_tests/test_hpgl2_addon.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 @pytest.fixture(scope="module")
 def svg_str():
     data = PLOTFILE.read_bytes()
     return hpgl2.to_svg(data)
 
 
 def test_svg_was_created(svg_str):
-    assert len(svg_str) > 80000
+    assert len(svg_str) > 70000
 
 
 def test_basic_svg_attributes(svg_str):
     root = ET.fromstring(svg_str)
     assert root.tag.endswith("svg")
-    assert root.attrib["width"] == "594mm"
-    assert root.attrib["height"] == "420mm"
+    assert root.attrib["width"] == "593.8mm"
+    assert root.attrib["height"] == "419.9mm"
     assert root.attrib["viewBox"] == "0 0 23752 16794"
 
 
 if __name__ == '__main__':
     pytest.main([__file__])
```

## Comparing `ezdxf-1.1.0b2/integration_tests/test_ignore_junk_beyond_EOF.py` & `ezdxf-1.1.0b3/integration_tests/test_ignore_junk_beyond_EOF.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_launcher.py` & `ezdxf-1.1.0b3/integration_tests/test_launcher.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_leica_disto_r12.py` & `ezdxf-1.1.0b3/integration_tests/test_leica_disto_r12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_load_dxf_unicode_notation.py` & `ezdxf-1.1.0b3/integration_tests/test_load_dxf_unicode_notation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_mapbox_earcut.py` & `ezdxf-1.1.0b3/integration_tests/test_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_mtext_columns.py` & `ezdxf-1.1.0b3/integration_tests/test_mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_mtext_explode_addon.py` & `ezdxf-1.1.0b3/integration_tests/test_mtext_explode_addon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_mtext_text_frame.py` & `ezdxf-1.1.0b3/integration_tests/test_mtext_text_frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_new_table_entries.py` & `ezdxf-1.1.0b3/integration_tests/test_new_table_entries.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_none_ascii_read_write.py` & `ezdxf-1.1.0b3/integration_tests/test_none_ascii_read_write.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_odafc.py` & `ezdxf-1.1.0b3/integration_tests/test_odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_open_binary_DXF_files.py` & `ezdxf-1.1.0b3/integration_tests/test_open_binary_DXF_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_open_coord_order_issue.py` & `ezdxf-1.1.0b3/integration_tests/test_open_coord_order_issue.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_open_exotic_dxf_files.py` & `ezdxf-1.1.0b3/integration_tests/test_open_exotic_dxf_files.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_open_R13_R14.py` & `ezdxf-1.1.0b3/integration_tests/test_open_R13_R14.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_polyline_entity.py` & `ezdxf-1.1.0b3/integration_tests/test_polyline_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_preserve_binary_data_in_xrecords.py` & `ezdxf-1.1.0b3/integration_tests/test_preserve_binary_data_in_xrecords.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_r12export.py` & `ezdxf-1.1.0b3/integration_tests/test_r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_r12strict.py` & `ezdxf-1.1.0b3/integration_tests/test_r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_r12writer.py` & `ezdxf-1.1.0b3/integration_tests/test_r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_read_file_without_handles.py` & `ezdxf-1.1.0b3/integration_tests/test_read_file_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_read_write_modern_entites.py` & `ezdxf-1.1.0b3/integration_tests/test_read_write_modern_entites.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_recover.py` & `ezdxf-1.1.0b3/integration_tests/test_recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_redraw_order.py` & `ezdxf-1.1.0b3/integration_tests/test_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_rotated_block_attributes.py` & `ezdxf-1.1.0b3/integration_tests/test_rotated_block_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_surface_entities.py` & `ezdxf-1.1.0b3/integration_tests/test_surface_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_write_fixed_meta_data.py` & `ezdxf-1.1.0b3/integration_tests/test_write_fixed_meta_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_write_without_handles.py` & `ezdxf-1.1.0b3/integration_tests/test_write_without_handles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/test_xref_detach.py` & `ezdxf-1.1.0b3/integration_tests/test_xref_detach.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/AC1003_LINE_Example.dxf` & `ezdxf-1.1.0b3/integration_tests/data/AC1003_LINE_Example.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/acad_table_with_blk_ref.dxf` & `ezdxf-1.1.0b3/integration_tests/data/acad_table_with_blk_ref.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/ASCII_R12.dxf` & `ezdxf-1.1.0b3/integration_tests/data/ASCII_R12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r12.dxf` & `ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r12.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r13.dxf` & `ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r14.dxf` & `ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/bin_dxf_r2000.dxf` & `ezdxf-1.1.0b3/integration_tests/data/bin_dxf_r2000.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/cc_dxflib.dxf` & `ezdxf-1.1.0b3/integration_tests/data/cc_dxflib.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/custom_blocks.dxf` & `ezdxf-1.1.0b3/integration_tests/data/custom_blocks.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/duplicate_handles.dxf` & `ezdxf-1.1.0b3/integration_tests/data/duplicate_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/dxf_unicode.dxf` & `ezdxf-1.1.0b3/integration_tests/data/dxf_unicode.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/empty_handles.dxf` & `ezdxf-1.1.0b3/integration_tests/data/empty_handles.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/groups.dxf` & `ezdxf-1.1.0b3/integration_tests/data/groups.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/Leica_Disto_S910.dxf` & `ezdxf-1.1.0b3/integration_tests/data/Leica_Disto_S910.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/MODEL.dxf` & `ezdxf-1.1.0b3/integration_tests/data/MODEL.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2007.dxf` & `ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2007.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/mtext_columns_R2018.dxf` & `ezdxf-1.1.0b3/integration_tests/data/mtext_columns_R2018.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/mtext_framed_columns.dxf` & `ezdxf-1.1.0b3/integration_tests/data/mtext_framed_columns.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/mtext_text_frame.dxf` & `ezdxf-1.1.0b3/integration_tests/data/mtext_text_frame.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/no_layouts.dxf` & `ezdxf-1.1.0b3/integration_tests/data/no_layouts.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/PLOTFILE.plt` & `ezdxf-1.1.0b3/integration_tests/data/PLOTFILE.plt`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/POLI-ALL210_12.DXF` & `ezdxf-1.1.0b3/integration_tests/data/POLI-ALL210_12.DXF`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/recover01.dxf` & `ezdxf-1.1.0b3/integration_tests/data/recover01.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/recover02.dxf` & `ezdxf-1.1.0b3/integration_tests/data/recover02.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/small_r13.dxf` & `ezdxf-1.1.0b3/integration_tests/data/small_r13.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/small_r14.dxf` & `ezdxf-1.1.0b3/integration_tests/data/small_r14.dxf`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/XRECORD_0.bin` & `ezdxf-1.1.0b3/integration_tests/data/XRECORD_0.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/XRECORD_1.bin` & `ezdxf-1.1.0b3/integration_tests/data/XRECORD_1.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/integration_tests/data/XRECORD_2.bin` & `ezdxf-1.1.0b3/integration_tests/data/XRECORD_2.bin`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/appsettings.py` & `ezdxf-1.1.0b3/src/ezdxf/appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/audit.py` & `ezdxf-1.1.0b3/src/ezdxf/audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/bbox.py` & `ezdxf-1.1.0b3/src/ezdxf/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/blkrefs.py` & `ezdxf-1.1.0b3/src/ezdxf/blkrefs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/commands.py` & `ezdxf-1.1.0b3/src/ezdxf/commands.py`

 * *Files 6% similar despite different names*

```diff
@@ -450,14 +450,15 @@
 
         config = Configuration(
             lineweight_scaling=args.lwscale,
         )
 
         signal.signal(signal.SIGINT, signal.SIG_DFL)  # handle Ctrl+C properly
         app = QtWidgets.QApplication(sys.argv)
+        app.setStyle("Fusion")
         set_app_icon(app)
         viewer = CADViewer.from_config(config)
         filename = args.file
         if filename:
             doc, auditor = load_document(filename)
             viewer.set_document(
                 doc,
@@ -500,14 +501,15 @@
         except ImportError as e:
             print(str(e))
             sys.exit(1)
         from ezdxf.addons import browser
 
         signal.signal(signal.SIGINT, signal.SIG_DFL)  # handle Ctrl+C properly
         app = QtWidgets.QApplication(sys.argv)
+        app.setStyle("Fusion")
         set_app_icon(app)
         main_window = browser.DXFStructureBrowser(
             args.file,
             line=args.line,
             handle=args.handle,
             resource_path=resources_path(),
         )
@@ -547,14 +549,15 @@
         except ImportError as e:
             print(str(e))
             sys.exit(1)
         from ezdxf.addons.acisbrowser.browser import AcisStructureBrowser
 
         signal.signal(signal.SIGINT, signal.SIG_DFL)  # handle Ctrl+C properly
         app = QtWidgets.QApplication(sys.argv)
+        app.setStyle("Fusion")
         set_app_icon(app)
         main_window = AcisStructureBrowser(
             args.file,
             handle=args.handle,
         )
         main_window.show()
         sys.exit(app.exec())
@@ -787,71 +790,14 @@
                     process(filename)
                     file_count += 1
 
             if file_count == 0:
                 sys.stderr.write(f'No matching files for pattern: "{pattern}"\n')
 
 
-def make_plt2fmt_parser(subparsers, name, fmt):
-    parser = subparsers.add_parser(name, help=f"convert HPGL/2 plot files to {fmt}")
-    parser.add_argument(
-        "files",
-        metavar="FILE",
-        nargs="+",
-        help=f"convert HPGL/2 plot files to {fmt}, wildcards (*, ?) supported",
-    )
-    parser.add_argument(
-        "-r",
-        "--rotate",
-        type=int,
-        choices=(0, 90, 180, 270),
-        default=0,
-        required=False,
-        help="rotate page about 90, 180 or 270 degrees",
-    )
-    parser.add_argument(
-        "-x",
-        "--scale_x",
-        type=float,
-        metavar="SX",
-        default=1.0,
-        required=False,
-        help="scale page in x-axis direction, use negative values to mirror page",
-    )
-    parser.add_argument(
-        "-y",
-        "--scale_y",
-        type=float,
-        metavar="SY",
-        default=1.0,
-        required=False,
-        help="scale page in y-axis direction, use negative values to mirror page",
-    )
-    parser.add_argument(
-        "-m",
-        "--merge_control",
-        type=int,
-        required=False,
-        default=2,
-        choices=(0, 1, 2),
-        help="provides control over the order of filled polygons, 0=off (print order), "
-        "1=luminance (order by luminance), 2=auto (default)",
-    )
-    parser.add_argument(
-        "-f",
-        "--force",
-        action="store_true",
-        required=False,
-        help="inserts the mandatory 'enter HPGL/2 mode' escape sequence into the data "
-        "stream; use this flag when no HPGL/2 data was found and you are sure the "
-        "file is a HPGL/2 plot file",
-    )
-    return parser
-
-
 @register
 class HPGL(Command):
     """Launcher sub-command: hpgl"""
 
     NAME = "hpgl"
 
     @staticmethod
@@ -880,29 +826,25 @@
             choices=(0, 90, 180, 270),
             default=0,
             required=False,
             help="rotate page about 90, 180 or 270 degrees (no gui)",
         )
         parser.add_argument(
             "-x",
-            "--scale_x",
-            type=float,
-            metavar="SX",
-            default=1.0,
+            "--mirror_x",
+            action="store_true",
             required=False,
-            help="scale page in x-axis direction, use negative values to mirror page, (no gui)",
+            help="mirror page in x-axis direction, (no gui)",
         )
         parser.add_argument(
             "-y",
-            "--scale_y",
-            type=float,
-            metavar="SY",
-            default=1.0,
+            "--mirror_y",
+            action="store_true",
             required=False,
-            help="scale page in y-axis direction, use negative values to mirror page (no gui)",
+            help="mirror page in y-axis direction, (no gui)",
         )
         parser.add_argument(
             "-m",
             "--merge_control",
             type=int,
             required=False,
             default=2,
@@ -919,43 +861,46 @@
             "stream; use this flag when no HPGL/2 data was found and you are sure the "
             "file is a HPGL/2 plot file",
         )
         parser.add_argument(
             "--aci",
             action="store_true",
             required=False,
-            help="use pen numbers as ACI colors (DXF only)",
+            help="use pen numbers as ACI colors and assign colors by layer (DXF only)",
+        )
+        parser.epilog = (
+            "Note that plot files are intended to be plotted on white paper."
         )
         parser.add_argument(
-            "--map_black_to_white",
-            action="store_true",
+            "--dpi",
+            type=int,
             required=False,
-            help="map black RGB plot colors to white RGB, does not affect ACI colors (DXF only)",
+            default=96,
+            help="pixel density in dots per inch (PNG only)",
         )
         parser.epilog = (
             "Note that plot files are intended to be plotted on white paper."
         )
 
     @staticmethod
     def run(args):
         if args.export:
-            for filename in glob.glob(args.file):
+            if os.path.exists(args.file):
+                filenames = [args.file]
+            else:
+                filenames = glob.glob(args.file)
+            for filename in filenames:
                 export_hpgl2(Path(filename), args)
         else:
-            filename = ""
-            if args.file:
-                names = list(glob.glob(args.file))
-                if len(names):
-                    filename = names[0]
-            launch_hpgl2_viewer(filename, args.force)
+            launch_hpgl2_viewer(args.file, args.force)
 
 
 def export_hpgl2(filepath: Path, args) -> None:
     from ezdxf.addons.hpgl2 import api as hpgl2
-    from ezdxf.addons.hpgl2.dxf_backend import ColorMode
+    from ezdxf.addons.drawing.dxf import ColorMode
 
     fmt = args.export.upper()
     start_msg = f"converting HPGL/2 plot file '{filepath.name}' to {fmt}"
     try:
         data = filepath.read_bytes()
     except IOError as e:
         print(str(e), file=sys.stderr)
@@ -965,51 +910,65 @@
     export_path = filepath.with_suffix(f".{fmt.lower()}")
     if fmt == "DXF":
         print(start_msg)
         color_mode = ColorMode.ACI if args.aci else ColorMode.RGB
         doc = hpgl2.to_dxf(
             data,
             rotation=args.rotate,
-            sx=args.scale_x,
-            sy=args.scale_y,
+            mirror_x=args.mirror_x,
+            mirror_y=args.mirror_y,
             color_mode=color_mode,
-            map_black_rgb_to_white_rgb=args.map_black_to_white,
             merge_control=args.merge_control,
         )
         try:
             doc.saveas(export_path)
         except IOError as e:
             print(str(e), file=sys.stderr)
 
     elif fmt == "SVG":
         print(start_msg)
         svg_string = hpgl2.to_svg(
             data,
             rotation=args.rotate,
-            sx=args.scale_x,
-            sy=args.scale_y,
+            mirror_x=args.mirror_x,
+            mirror_y=args.mirror_y,
             merge_control=args.merge_control,
         )
         try:
             export_path.write_text(svg_string)
         except IOError as e:
             print(str(e), file=sys.stderr)
     elif fmt == "PDF":
         print(start_msg)
         pdf_bytes = hpgl2.to_pdf(
             data,
             rotation=args.rotate,
-            sx=args.scale_x,
-            sy=args.scale_y,
+            mirror_x=args.mirror_x,
+            mirror_y=args.mirror_y,
             merge_control=args.merge_control,
         )
         try:
             export_path.write_bytes(pdf_bytes)
         except IOError as e:
             print(str(e), file=sys.stderr)
+    elif fmt == "PNG":
+        print(start_msg)
+        png_bytes = hpgl2.to_pixmap(
+            data,
+            rotation=args.rotate,
+            mirror_x=args.mirror_x,
+            mirror_y=args.mirror_y,
+            merge_control=args.merge_control,
+            fmt="png",
+            dpi=args.dpi,
+        )
+        try:
+            export_path.write_bytes(png_bytes)
+        except IOError as e:
+            print(str(e), file=sys.stderr)
     else:
         print(f"invalid export format: {fmt}")
         exit(1)
     print(f"file '{export_path.name}' successfully written")
 
 
 def launch_hpgl2_viewer(filename: str, force: bool) -> None:
@@ -1018,14 +977,15 @@
     except ImportError as e:
         print(str(e))
         exit(1)
     from ezdxf.addons.hpgl2.viewer import HPGL2Viewer
 
     signal.signal(signal.SIGINT, signal.SIG_DFL)  # handle Ctrl+C properly
     app = QtWidgets.QApplication(sys.argv)
+    app.setStyle("Fusion")
     set_app_icon(app)
     viewer = HPGL2Viewer()
     viewer.show()
     if filename and os.path.exists(filename):
         viewer.load_plot_file(filename, force=force)
     sys.exit(app.exec())
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/comments.py` & `ezdxf-1.1.0b3/src/ezdxf/comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/disassemble.py` & `ezdxf-1.1.0b3/src/ezdxf/disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/document.py` & `ezdxf-1.1.0b3/src/ezdxf/document.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/dwginfo.py` & `ezdxf-1.1.0b3/src/ezdxf/dwginfo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entitydb.py` & `ezdxf-1.1.0b3/src/ezdxf/entitydb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/enums.py` & `ezdxf-1.1.0b3/src/ezdxf/enums.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/explode.py` & `ezdxf-1.1.0b3/src/ezdxf/explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/eztypes.py` & `ezdxf-1.1.0b3/src/ezdxf/eztypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/filemanagement.py` & `ezdxf-1.1.0b3/src/ezdxf/filemanagement.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/gfxattribs.py` & `ezdxf-1.1.0b3/src/ezdxf/gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/graphicsfactory.py` & `ezdxf-1.1.0b3/src/ezdxf/graphicsfactory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/groupby.py` & `ezdxf-1.1.0b3/src/ezdxf/groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/npshapes.py` & `ezdxf-1.1.0b3/src/ezdxf/npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/protocols.py` & `ezdxf-1.1.0b3/src/ezdxf/protocols.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/proxygraphic.py` & `ezdxf-1.1.0b3/src/ezdxf/proxygraphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/query.py` & `ezdxf-1.1.0b3/src/ezdxf/query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/queryparser.py` & `ezdxf-1.1.0b3/src/ezdxf/queryparser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/r12strict.py` & `ezdxf-1.1.0b3/src/ezdxf/r12strict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/recover.py` & `ezdxf-1.1.0b3/src/ezdxf/recover.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/reorder.py` & `ezdxf-1.1.0b3/src/ezdxf/reorder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/transform.py` & `ezdxf-1.1.0b3/src/ezdxf/transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/units.py` & `ezdxf-1.1.0b3/src/ezdxf/units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/upright.py` & `ezdxf-1.1.0b3/src/ezdxf/upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/urecord.py` & `ezdxf-1.1.0b3/src/ezdxf/urecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/version.py` & `ezdxf-1.1.0b3/src/ezdxf/version.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,9 +20,9 @@
 # examples:
 #   major pre-release alpha 2: VERSION = "0.9.0a2"; version = (0, 9, 0, 'a2')
 #   major release candidate 0: VERSION = "0.9.0rc0"; version = (0, 9, 0, 'rc0')
 #   major release: VERSION = "0.9.0"; version = (0, 9, 0, 'release')
 #   1. bug fix release beta0: VERSION = "0.9.1b0"; version = (0, 9, 1, 'b0')
 #   2. bug fix release: VERSION = "0.9.2"; version = (0, 9, 2, 'release')
 
-version = (1, 1, 0, "b2")
-__version__ = "1.1.0b2"
+version = (1, 1, 0, "b3")
+__version__ = "1.1.0b3"
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/xref.py` & `ezdxf-1.1.0b3/src/ezdxf/xref.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/zoom.py` & `ezdxf-1.1.0b3/src/ezdxf/zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/_options.py` & `ezdxf-1.1.0b3/src/ezdxf/_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,17 @@
 from pathlib import Path
 from configparser import ConfigParser
 
 # Recommended uses of the global object "options":
 # import ezdxf
 # value = ezdxf.options.<attribute>
 #
-# If the import of "ezdxf" is not wanted:
+# alternative:
 # from ezdxf._options import options
 
-# The MATPLOTLIB global shows that Matplotlib is installed:
 TRUE_STATE = {"True", "true", "On", "on", "1"}
 CORE = "core"
 BROWSE_COMMAND = "browse-command"
 VIEW_COMMAND = "view-command"
 DRAW_COMMAND = "draw-command"
 EZDXF_INI = "ezdxf.ini"
 EZDXF = "ezdxf"
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/__init__.py` & `ezdxf-1.1.0b3/src/ezdxf/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/__main__.py` & `ezdxf-1.1.0b3/src/ezdxf/__main__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/bezier3p.pyx` & `ezdxf-1.1.0b3/src/ezdxf/acc/bezier3p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/bezier4p.pyx` & `ezdxf-1.1.0b3/src/ezdxf/acc/bezier4p.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/bspline.pyx` & `ezdxf-1.1.0b3/src/ezdxf/acc/bspline.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/construct.pyx` & `ezdxf-1.1.0b3/src/ezdxf/acc/construct.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/linetypes.pyx` & `ezdxf-1.1.0b3/src/ezdxf/acc/linetypes.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/mapbox_earcut.pyx` & `ezdxf-1.1.0b3/src/ezdxf/acc/mapbox_earcut.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/matrix44.pyx` & `ezdxf-1.1.0b3/src/ezdxf/acc/matrix44.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/vector.pxd` & `ezdxf-1.1.0b3/src/ezdxf/acc/vector.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/vector.pyx` & `ezdxf-1.1.0b3/src/ezdxf/acc/vector.pyx`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.cpp` & `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_cubic_bezier.hpp` & `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_cubic_bezier.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_quad_bezier.cpp` & `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_quad_bezier.cpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.hpp` & `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.hpp`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/_cpp_vec3.pxd` & `ezdxf-1.1.0b3/src/ezdxf/acc/_cpp_vec3.pxd`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acc/__init__.py` & `ezdxf-1.1.0b3/src/ezdxf/acc/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/abstract.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/abstract.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/api.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/api.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/const.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/dbg.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/dbg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/dxf.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/dxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/entities.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/hdr.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/hdr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/mesh.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/sab.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/acis/sat.py` & `ezdxf-1.1.0b3/src/ezdxf/acis/sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/acadctb.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/binpacking.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/binpacking.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/dimlines.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/dimlines.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/dxf2code.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/dxf2code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/genetic_algorithm.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/geo.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/geo.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/gerber_D6673.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/gerber_D6673.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/importer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/iterdxf.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/iterdxf.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/menger_sponge.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/meshex.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/mtextsurrogate.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/mtextsurrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/mtxpl.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/mtxpl.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/odafc.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/odafc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/openscad.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/pycsg.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/r12export.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/r12export.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/r12writer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/r12writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/sierpinski_pyramid.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/sierpinski_pyramid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/tablepainter.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/tablepainter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/text2path.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/xplayer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/xplayer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,63 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 """xplayer = cross backend player."""
 from __future__ import annotations
 from typing import Callable
 from ezdxf import path
 from ezdxf.math import Vec2
+from ezdxf.colors import RGB
 
 from ezdxf.addons.drawing.backend import BackendInterface
-from ezdxf.addons.drawing.properties import BackendProperties, rgb_to_hex, hex_to_rgb, luminance
+from ezdxf.addons.drawing.properties import BackendProperties
 from ezdxf.addons.hpgl2 import api as hpgl2
 from ezdxf.addons.hpgl2.backend import (
     Properties as HPGL2Properties,
     RecordType as HPGL2RecordType,
 )
 
 
 def hpgl2_to_drawing(
     player: hpgl2.Player,
     backend: BackendInterface,
     bg_color: str = "#ffffff",
     override: Callable[[BackendProperties], BackendProperties] | None = None,
 ) -> None:
     """Replays the recordings of the HPGL2 Recorder on a backend of the drawing add-on."""
-    backend.set_background(bg_color)  # plotting on white paper
+    if bg_color:
+        backend.set_background(bg_color)
     for record_type, properties, record_data in player.recordings():
         backend_properties = _make_drawing_backend_properties(properties)
         if override:
             backend_properties = override(backend_properties)
         if record_type == HPGL2RecordType.POLYLINE:
             points: list[Vec2] = record_data.vertices()
             size = len(points)
             if size == 1:
                 backend.draw_point(points[0], backend_properties)
             elif size == 2:
                 backend.draw_line(points[0], points[1], backend_properties)
             else:
                 backend.draw_path(_from_2d_points(points), backend_properties)
-        elif record_type == HPGL2RecordType.FILLED_POLYGON:
-            # filled polygons are stored as single paths! see: PolygonBuffer.get_paths()
+        elif record_type == HPGL2RecordType.FILLED_PATHS:
+            # filled paths are stored as single paths! see: PolygonBuffer.get_paths()
             external_paths, holes = path.winding_deconstruction(
                 path.fast_bbox_detection(p.to_path2d() for p in record_data)
             )
             backend.draw_filled_paths(external_paths, holes, backend_properties)  # type: ignore
+        elif record_type == HPGL2RecordType.OUTLINE_PATHS:
+            for p in record_data:
+                backend.draw_path(p.to_path2d(), backend_properties)
     backend.finalize()
 
 
 def _make_drawing_backend_properties(properties: HPGL2Properties) -> BackendProperties:
     """Make BackendProperties() for the drawing add-on."""
     return BackendProperties(
-        color=rgb_to_hex(properties.pen_color),
+        color=properties.pen_color.to_hex(),
         lineweight=properties.pen_width,
         layer="0",
         pen=properties.pen_index,
         handle="",
     )
 
 
@@ -74,23 +79,25 @@
             handle=properties.handle,
         )
 
     return _map_color
 
 
 def map_monochrome(dark_mode=True) -> Callable[[BackendProperties], BackendProperties]:
-    def to_grey(c: str) -> str:
-        grey = round(luminance(hex_to_rgb(c)) * 255)
+    def to_gray(color: str) -> str:
+        gray = round(RGB.from_hex(color).luminance * 255)
         if dark_mode:
-            grey = 255 - grey
-        return rgb_to_hex((grey, grey, grey))
+            gray = 255 - gray
+        return RGB(gray, gray, gray).to_hex()
 
     def _map_color(properties: BackendProperties) -> BackendProperties:
+        color = properties.color
+        alpha = color[7:9]
         return BackendProperties(
-            color=to_grey(properties.color),
+            color=to_gray(color[:7]) + alpha,
             lineweight=properties.lineweight,
             layer=properties.layer,
             pen=properties.pen,
             handle=properties.handle,
         )
 
     return _map_color
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/xqt.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/xqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/browser.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/acisbrowser/data.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/acisbrowser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/browser/bookmarks.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/browser/bookmarks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/browser/browser.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/browser/browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/browser/data.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/browser/data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/browser/find_dialog.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/browser/find_dialog.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/browser/loader.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/browser/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/browser/model.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/browser/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import textwrap
 from ezdxf.lldxf.types import (
     render_tag,
     DXFVertex,
     GROUP_MARKERS,
     POINTER_CODES,
 )
-from ezdxf.addons.xqt import QModelIndex, QAbstractTableModel, Qt
+from ezdxf.addons.xqt import QModelIndex, QAbstractTableModel, Qt, QtWidgets
 from ezdxf.addons.xqt import QStandardItemModel, QStandardItem, QColor
 from .tags import compile_tags, Tags
 
 __all__ = [
     "DXFTagsModel",
     "DXFStructureModel",
     "EntityContainer",
@@ -51,14 +51,16 @@
     def __init__(
         self, tags: Tags, start_line_number: int = 1, valid_handles=None
     ):
         super().__init__()
         self._tags = compile_tags(tags)
         self._line_numbers = calc_line_numbers(start_line_number, self._tags)
         self._valid_handles = valid_handles or set()
+        palette = QtWidgets.QApplication.palette()
+        self._group_marker_color = palette.highlight().color()
 
     def data(self, index: QModelIndex, role: int = ...) -> Any:  # type: ignore
         def is_invalid_handle(tag):
             if (
                 tag.code in POINTER_CODES
                 and not tag.value.upper() in self._valid_handles
             ):
@@ -67,15 +69,15 @@
 
         if role == Qt.DisplayRole:
             tag = self._tags[index.row()]
             return render_tag(tag, index.column())
         elif role == Qt.ForegroundRole:
             tag = self._tags[index.row()]
             if tag.code in GROUP_MARKERS:
-                return QColor("blue")
+                return self._group_marker_color
             elif is_invalid_handle(tag):
                 return QColor("red")
         elif role == DXFTagsRole:
             return self._tags[index.row()]
         elif role == Qt.ToolTipRole:
             code, value = self._tags[index.row()]
             if index.column() == 0:  # group code column
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/browser/tags.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/browser/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/browser/views.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/browser/views.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/backend.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/clipper.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/clipper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/config.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,39 +35,40 @@
         ``True``, which is the default value.
 
         This can not prevent drawing proxy graphic inside of blocks,
         because this is beyond the domain of the drawing add-on!
 
     Attributes:
         IGNORE: do not display proxy graphics (skip_entity will be called instead)
-        SHOW: if the entity cannot be rendered directly (eg if not implemented)
+        SHOW: if the entity cannot be rendered directly (e.g. if not implemented)
             but a proxy is present: display the proxy
         PREFER: display proxy graphics even for entities where direct rendering
             is available
     """
 
     IGNORE = auto()
     SHOW = auto()
     PREFER = auto()
 
 
 class HatchPolicy(Enum):
     """The action to take when a HATCH entity is encountered
 
     Attributes:
+        NORMAL: render pattern and solid fillings
         IGNORE: do not show HATCH entities at all
         SHOW_OUTLINE: show only the outline of HATCH entities
-        SHOW_SOLID: show HATCH entities but draw with solid fill
-            regardless of the pattern
-    """
+        SHOW_SOLID: show HATCH entities as solid filling regardless of the pattern
 
+    """
+    NORMAL = auto()
     IGNORE = auto()
     SHOW_OUTLINE = auto()
     SHOW_SOLID = auto()
-    SHOW_APPROXIMATE_PATTERN = auto()  # ignored since v0.18.1
+    SHOW_APPROXIMATE_PATTERN = auto()  # ignored since v0.18.1 == NORMAL
 
 
 class LineweightPolicy(Enum):
     """This enum is used to define how to determine the lineweight.
 
     Attributes:
         ABSOLUTE: in mm as resolved by the :class:`Frontend` class
@@ -88,28 +89,32 @@
 
 class ColorPolicy(Enum):
     """This enum is used to define how to determine the line/fill color.
 
     Attributes:
         COLOR: as resolved by the :class:`Frontend` class
         COLOR_SWAP_BW: as resolved by the :class:`Frontend` class but swaps black and white
-        COLOR_NEGATIVE: invert colors
-        MONOCHROME_BLACK_BG: all colors to gray scale for black background
-        MONOCHROME_WHITE_BG:  all colors to gray scale for white background
-        BLACK: all colors to black
-        WHITE: all colors to white
-        CUSTOM: all colors to custom color by :attr:`Configuration.custom_fg_color`
+        COLOR_NEGATIVE: invert all colors
+        MONOCHROME: maps all colors to gray scale in range [0%, 100%]
+        MONOCHROME_DARK_BG: maps all colors to gray scale in range [30%, 100%], brightens
+            colors for dark backgrounds
+        MONOCHROME_LIGHT_BG:  maps all colors to gray scale in range [0%, 70%], darkens
+            colors for light backgrounds
+        BLACK: maps all colors to black
+        WHITE: maps all colors to white
+        CUSTOM: maps all colors to custom color :attr:`Configuration.custom_fg_color`
 
     """
 
     COLOR = auto()
     COLOR_SWAP_BW = auto()
     COLOR_NEGATIVE = auto()
-    MONOCHROME_BLACK_BG = auto()
-    MONOCHROME_WHITE_BG = auto()
+    MONOCHROME = auto()
+    MONOCHROME_DARK_BG = auto()
+    MONOCHROME_LIGHT_BG = auto()
     BLACK = auto()
     WHITE = auto()
     CUSTOM = auto()
 
 
 class BackgroundPolicy(Enum):
     """This enum is used to define the background color.
@@ -126,14 +131,33 @@
     DEFAULT = auto()
     WHITE = auto()
     BLACK = auto()
     OFF = auto()
     CUSTOM = auto()
 
 
+class TextPolicy(Enum):
+    """This enum is used to define the text rendering.
+
+    Attributes:
+        FILLING: text is rendered as solid filling (default)
+        OUTLINE: text is rendered as outline paths
+        REPLACE_RECT: replace text by a rectangle
+        REPLACE_FILL: replace text by a filled rectangle
+        IGNORE: ignore text at all
+
+    """
+
+    FILLING = auto()
+    OUTLINE = auto()
+    REPLACE_RECT = auto()
+    REPLACE_FILL = auto()
+    IGNORE = auto()
+
+
 @dataclass(frozen=True)
 class Configuration:
     """Configuration options for the :mod:`drawing` add-on.
 
     Attributes:
         pdsize: the size to draw POINT entities (in drawing units)
             set to None to use the $PDSIZE value from the dxf document header
@@ -187,36 +211,38 @@
         color_policy:
         custom_fg_color: Used for :class:`ColorPolicy.custom` policy, custom foreground
             color as "#RRGGBBAA" color string (RGB+alpha)
         background_policy:
         custom_bg_color: Used for :class:`BackgroundPolicy.custom` policy, custom
             background color as "#RRGGBBAA" color string (RGB+alpha)
         lineweight_policy:
+        text_policy:
 
     """
 
     pdsize: Optional[int] = None  # use $PDSIZE from HEADER section
     pdmode: Optional[int] = None  # use $PDMODE from HEADER section
     measurement: Optional[Measurement] = None
     show_defpoints: bool = False
     proxy_graphic_policy: ProxyGraphicPolicy = ProxyGraphicPolicy.SHOW
     line_policy: LinePolicy = LinePolicy.ACCURATE
-    hatch_policy: HatchPolicy = HatchPolicy.SHOW_APPROXIMATE_PATTERN
+    hatch_policy: HatchPolicy = HatchPolicy.NORMAL
     infinite_line_length: float = 20
     lineweight_scaling: float = 1.0
     min_lineweight: Optional[float] = None
     min_dash_length: float = 0.1
     max_flattening_distance: float = disassemble.Primitive.max_flattening_distance
     circle_approximation_count: int = 128
     hatching_timeout: float = 30.0
     color_policy: ColorPolicy = ColorPolicy.COLOR
     custom_fg_color: Color = "#000000"
     background_policy: BackgroundPolicy = BackgroundPolicy.DEFAULT
     custom_bg_color: Color = "#ffffff"
     lineweight_policy: LineweightPolicy = LineweightPolicy.ABSOLUTE
+    text_policy: TextPolicy = TextPolicy.FILLING
 
     @staticmethod
     def defaults() -> Configuration:
         warnings.warn(
             "use Configuration() instead of Configuration.defaults()",
             DeprecationWarning,
         )
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_backend.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_backend.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/debug_utils.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/debug_utils.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/frontend.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/frontend.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,33 +15,36 @@
 )
 from typing_extensions import TypeAlias
 import logging
 import itertools
 import time
 
 import ezdxf.bbox
+from ezdxf.colors import RGB
 from ezdxf.addons.drawing.config import (
     Configuration,
     ProxyGraphicPolicy,
     HatchPolicy,
 )
 from ezdxf.addons.drawing.backend import BackendInterface
 from ezdxf.addons.drawing.clipper import ClippingRect
 from ezdxf.addons.drawing.properties import (
     RenderContext,
-    VIEWPORT_COLOR,
     OLE2FRAME_COLOR,
     Properties,
     Filling,
     LayoutProperties,
     BackendProperties,
-    hex_to_rgb,
-    rgb_to_hex,
 )
-from ezdxf.addons.drawing.config import LinePolicy, BackgroundPolicy, ColorPolicy
+from ezdxf.addons.drawing.config import (
+    LinePolicy,
+    BackgroundPolicy,
+    ColorPolicy,
+    TextPolicy,
+)
 from ezdxf.addons.drawing.text import simplified_text_chunks
 from ezdxf.addons.drawing.type_hints import FilterFunc
 from ezdxf.addons.drawing.gfxproxy import DXFGraphicProxy
 from ezdxf.addons.drawing.mtext_complex import complex_mtext_renderer
 from ezdxf.addons.drawing.unified_text_renderer import UnifiedTextRenderer
 from ezdxf.entities import (
     DXFEntity,
@@ -59,15 +62,15 @@
     Point,
     Viewport,
 )
 from ezdxf.entities.attrib import BaseAttrib
 from ezdxf.entities.polygon import DXFPolygon
 from ezdxf.entities.boundary_paths import AbstractBoundaryPath
 from ezdxf.layouts import Layout
-from ezdxf.math import Vec2, Vec3, OCS, NULLVEC, Matrix44, AnyVec
+from ezdxf.math import Vec2, Vec3, OCS, NULLVEC, Matrix44, AnyVec, BoundingBox2d
 from ezdxf.path import (
     Path,
     Path2d,
     make_path,
     from_hatch_boundary_path,
     fast_bbox_detection,
     winding_deconstruction,
@@ -81,15 +84,14 @@
 from ezdxf.tools.text import (
     has_inline_formatting_codes,
     replace_non_printable_characters,
 )
 from ezdxf.lldxf import const
 from ezdxf.render import hatching
 from ezdxf.fonts import fonts
-from ezdxf.colors import luminance
 from .type_hints import Color
 
 
 __all__ = ["Frontend"]
 
 
 TDispatchTable: TypeAlias = Dict[str, Callable[[DXFGraphic, Properties], None]]
@@ -170,15 +172,14 @@
 
     def _build_dispatch_table(self) -> TDispatchTable:
         dispatch_table: TDispatchTable = {
             "POINT": self.draw_point_entity,
             "HATCH": self.draw_hatch_entity,
             "MPOLYGON": self.draw_mpolygon_entity,
             "MESH": self.draw_mesh_entity,
-            "VIEWPORT": self.draw_viewport_entity,
             "WIPEOUT": self.draw_wipeout_entity,
             "MTEXT": self.draw_mtext_entity,
             "OLE2FRAME": self.draw_ole2frame_entity,
         }
         for dxftype in ("LINE", "XLINE", "RAY"):
             dispatch_table[dxftype] = self.draw_line_entity
         for dxftype in ("TEXT", "ATTRIB", "ATTDEF"):
@@ -258,24 +259,27 @@
                 filter_func=filter_func,
             )
         if finalize:
             self.out.finalize()
 
     def set_background(self, color: Color) -> None:
         policy = self.config.background_policy
+        override = True
         if policy == BackgroundPolicy.DEFAULT:
-            pass
+            override = False
         elif policy == BackgroundPolicy.OFF:
             color = "#ffffff00"  # white, fully transparent
         elif policy == BackgroundPolicy.BLACK:
             color = "#000000"
         elif policy == BackgroundPolicy.WHITE:
             color = "#ffffff"
         elif policy == BackgroundPolicy.CUSTOM:
             color = self.config.custom_bg_color
+        if override:
+            self.ctx.current_layout_properties.set_colors(color)
         self.out.set_background(color)
 
     def draw_entities(
         self,
         entities: Iterable[DXFGraphic],
         *,
         filter_func: Optional[FilterFunc] = None,
@@ -344,14 +348,16 @@
                 )
             elif dxftype == "RAY":
                 self._designer.draw_line(start, start + delta, properties)
         else:
             raise TypeError(dxftype)
 
     def draw_text_entity(self, entity: DXFGraphic, properties: Properties) -> None:
+        if self.config.text_policy == TextPolicy.IGNORE:
+            return
         # Draw embedded MTEXT entity as virtual MTEXT entity:
         if isinstance(entity, BaseAttrib) and entity.has_embedded_mtext_entity:
             self.draw_mtext_entity(entity.virtual_mtext_entity(), properties)
         elif is_spatial_text(Vec3(entity.dxf.extrusion)):
             self.draw_text_entity_3d(entity, properties)
         else:
             self.draw_text_entity_2d(entity, properties)
@@ -373,14 +379,16 @@
         else:
             raise TypeError(entity.dxftype())
 
     def draw_text_entity_3d(self, entity: DXFGraphic, properties: Properties) -> None:
         self.skip_entity(entity, "3D text not supported")
 
     def draw_mtext_entity(self, entity: DXFGraphic, properties: Properties) -> None:
+        if self.config.text_policy == TextPolicy.IGNORE:
+            return
         mtext = cast(MText, entity)
         if is_spatial_text(Vec3(mtext.dxf.extrusion)):
             self.skip_entity(mtext, "3D MTEXT not supported")
             return
         if mtext.has_columns or has_inline_formatting_codes(mtext.text):
             self.draw_complex_mtext(mtext, properties)
         else:
@@ -509,19 +517,22 @@
         *,
         loops: Optional[list[Path]] = None,
     ) -> None:
         if properties.filling is None:
             return
         filling = properties.filling
         show_only_outline = False
-        if self.config.hatch_policy == HatchPolicy.IGNORE:
+        hatch_policy = self.config.hatch_policy
+        if hatch_policy == HatchPolicy.NORMAL:
+            pass
+        elif hatch_policy == HatchPolicy.IGNORE:
             return
-        elif self.config.hatch_policy == HatchPolicy.SHOW_SOLID:
+        elif hatch_policy == HatchPolicy.SHOW_SOLID:
             filling = Filling()  # solid filling
-        elif self.config.hatch_policy == HatchPolicy.SHOW_OUTLINE:
+        elif hatch_policy == HatchPolicy.SHOW_OUTLINE:
             filling = Filling()  # solid filling
             show_only_outline = True
 
         polygon = cast(DXFPolygon, entity)
         if filling.type == Filling.PATTERN:
             if loops is None:
                 loops = hatching.hatch_boundary_paths(polygon, filter_text_boxes=True)
@@ -600,18 +611,18 @@
     def draw_wipeout_entity(self, entity: DXFGraphic, properties: Properties) -> None:
         wipeout = cast(Wipeout, entity)
         properties.filling = Filling()
         properties.color = self.ctx.current_layout_properties.background_color
         path = wipeout.boundary_path_wcs()
         self._designer.draw_filled_polygon(path, properties)
 
-    def draw_viewport_entity(self, entity: DXFGraphic, properties: Properties) -> None:
-        assert isinstance(entity, Viewport)
-        vp = entity
-        if vp.dxf.get("status", 0) < 2:  # 0= off; 1= "active viewport"
+    def draw_viewport(self, vp: Viewport) -> None:
+        # the "active" viewport and invisible viewports should be filtered at this
+        # stage, see function _draw_viewports()
+        if vp.dxf.status < 1:
             return
 
         if not vp.is_top_view:
             self.log_message("Cannot render non top-view viewports")
             return
         self._designer.draw_viewport(vp, self.ctx, self._bbox_cache)
 
@@ -813,17 +824,15 @@
 
     def draw_viewport(
         self,
         vp: Viewport,
         layout_ctx: RenderContext,
         bbox_cache: Optional[ezdxf.bbox.Cache] = None,
     ) -> None:
-        """Draw the content of the given viewport current viewport.
-        Returns ``False`` if the backend doesn't support viewports.
-        """
+        """Draw the content of the given viewport current viewport."""
         if vp.doc is None:
             return
         try:
             msp_limits = vp.get_modelspace_limits()
         except ValueError:  # modelspace limits not detectable
             return
         if self.enter_viewport(vp):
@@ -963,29 +972,44 @@
         self,
         text: str,
         transform: Matrix44,
         properties: Properties,
         cap_height: float,
         dxftype: str = "TEXT",
     ) -> None:
-        if not text.strip():
+        text_policy = self.config.text_policy
+        if not text.strip() or text_policy == TextPolicy.IGNORE:
             return  # no point rendering empty strings
         text = prepare_string_for_rendering(text, dxftype)
         font_face = properties.font
         if font_face is None:
             font_face = self.default_font_face
         try:
             text_path = self.text_engine.get_text_path(text, font_face, cap_height)
         except (RuntimeError, ValueError):
             return
 
         transformed_path = text_path.transform(transform)
-        if self.text_engine.is_stroke_font(font_face):
+        if text_policy == TextPolicy.REPLACE_RECT:
+            bbox = BoundingBox2d(transformed_path.control_vertices())
+            self.draw_path(from_vertices(bbox.rect_vertices(), close=True), properties)
+            return
+        if text_policy == TextPolicy.REPLACE_FILL:
+            bbox = BoundingBox2d(transformed_path.control_vertices())
+            if properties.filling is None:
+                properties.filling = Filling()
+            self.draw_filled_polygon(bbox.rect_vertices(), properties)
+            return
+        if (
+            self.text_engine.is_stroke_font(font_face)
+            or text_policy == TextPolicy.OUTLINE
+        ):
             self.draw_path(transformed_path, properties)
             return
+
         polygons = fast_bbox_detection(single_paths([transformed_path]))  # type: ignore
         external_paths, holes = winding_deconstruction(polygons)  # type: ignore
         if properties.filling is None:
             properties.filling = Filling()
         self.draw_filled_paths(external_paths, holes, properties)  # type: ignore
 
 
@@ -1055,27 +1079,60 @@
     ctx: RenderContext,
     entities: Iterable[DXFGraphic],
     *,
     filter_func: Optional[FilterFunc] = None,
 ) -> None:
     if filter_func is not None:
         entities = filter(filter_func, entities)
+    viewports: list[Viewport] = []
     for entity in entities:
+        if isinstance(entity, Viewport):
+            viewports.append(entity)
+            continue
         if not isinstance(entity, DXFGraphic):
             if frontend.config.proxy_graphic_policy != ProxyGraphicPolicy.IGNORE:
                 entity = DXFGraphicProxy(entity)
             else:
                 frontend.skip_entity(entity, "Cannot parse DXF entity")
                 continue
         properties = ctx.resolve_all(entity)
         frontend.override_properties(entity, properties)
         if properties.is_visible:
             frontend.draw_entity(entity, properties)
         else:
             frontend.skip_entity(entity, "invisible")
+    _draw_viewports(frontend, viewports)
+
+
+def _draw_viewports(frontend: Frontend, viewports: list[Viewport]) -> None:
+    # The VIEWPORT attributes "id" and "status" are very unreliable, maybe because of
+    # the "great" documentation by Autodesk.
+    # Viewport status field: (according to the DXF Reference)
+    # -1 = On, but is fully off-screen, or is one of the viewports that is not
+    #      active because the $MAXACTVP count is currently being exceeded.
+    #  0 = Off
+    # <positive value> = On and active. The value indicates the order of
+    # stacking for the viewports, where 1 is the "active" viewport, 2 is the
+    # next, and so on.
+    viewports.sort(key=lambda e: e.dxf.status)
+    # Remove all invisible viewports:
+    viewports = [vp for vp in viewports if vp.dxf.status > 0]
+    if not viewports:
+        return
+    # The "active" viewport determines how the paperspace layout is presented as a
+    # whole (location & zoom state).
+    # Maybe there are more than one "active" viewports, just remove the first one,
+    # or there is no "active" viewport at all - in this case the "status" attribute
+    # is not reliable at all - but what else is there to do?  The "active" layout should
+    # have the id "1", but this information is also not reliable.
+    if viewports[0].dxf.get("status", 1) == 1:
+        viewports.pop(0)
+    # Draw viewports in order of "status"
+    for viewport in viewports:
+        frontend.draw_viewport(viewport)
 
 
 def prepare_string_for_rendering(text: str, dxftype: str) -> str:
     assert "\n" not in text, "not a single line of text"
     if dxftype in {"TEXT", "ATTRIB", "ATTDEF"}:
         text = replace_non_printable_characters(text, replacement="?")
         text = text.replace("\t", "?")
@@ -1084,47 +1141,50 @@
         text = text.replace("\t", "        ")
     else:
         raise TypeError(dxftype)
     return text
 
 
 def invert_color(color: Color) -> Color:
-    r, g, b = hex_to_rgb(color)
-    return rgb_to_hex((255 - r, 255 - g, 255 - b))
+    r, g, b = RGB.from_hex(color)
+    return RGB(255 - r, 255 - g, 255 - b).to_hex()
 
 
 def swap_bw(color: str) -> Color:
     color = color.lower()
     if color == "#000000":
         return "#ffffff"
     if color == "#ffffff":
         return "#000000"
     return color
 
 
-def color_to_monochrome(color: Color, invert=False) -> Color:
-    lum = luminance(hex_to_rgb(color))
-    if invert:
-        gray = round((1.0 - lum) * 255)
-    else:
-        gray = round(lum * 255)
-    return rgb_to_hex((gray, gray, gray))
+def color_to_monochrome(color: Color, scale: float = 1.0, offset: float = 0.0) -> Color:
+    lum = RGB.from_hex(color).luminance * scale + offset
+    if lum < 0.0:
+        lum = 0.0
+    elif lum > 1.0:
+        lum = 1.0
+    gray = round(lum * 255)
+    return RGB(gray, gray, gray).to_hex()
 
 
 def apply_color_policy(color: Color, policy: ColorPolicy, custom_color: Color) -> Color:
     alpha = color[7:9]
     color = color[:7]
     if policy == ColorPolicy.COLOR_SWAP_BW:
         color = swap_bw(color)
     elif policy == ColorPolicy.COLOR_NEGATIVE:
         color = invert_color(color)
-    elif policy == ColorPolicy.MONOCHROME_WHITE_BG:
-        color = color_to_monochrome(color, invert=True)
-    elif policy == ColorPolicy.MONOCHROME_BLACK_BG:
-        color = color_to_monochrome(color, invert=False)
+    elif policy == ColorPolicy.MONOCHROME_DARK_BG:  # [0.3, 1.0]
+        color = color_to_monochrome(color, scale=0.7, offset=0.3)
+    elif policy == ColorPolicy.MONOCHROME_LIGHT_BG:  # [0.0, 0.7]
+        color = color_to_monochrome(color, scale=0.7, offset=0.0)
+    elif policy == ColorPolicy.MONOCHROME:  # [0.0, 1.0]
+        color = color_to_monochrome(color)
     elif policy == ColorPolicy.BLACK:
         color = "#000000"
     elif policy == ColorPolicy.WHITE:
         color = "#ffffff"
     elif policy == ColorPolicy.CUSTOM:
         fg = custom_color
         color = fg[:7]
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/gfxproxy.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/gfxproxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/layout.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,16 +14,16 @@
 
 
 class Units(enum.IntEnum):
     """Page units as enum.
 
     Attributes:
         inch: 25.4 mm
-        px: 1/72 inch
-        pt: 1/96 inch
+        px: 1/96 inch
+        pt: 1/72 inch
         mm:
         cm:
 
     """
 
     # equivalent to ezdxf.units if possible
     inch = 1
@@ -302,26 +302,31 @@
     def get_final_page(self, page: Page, settings: Settings) -> Page:
         rotation = self.get_rotation(settings)
         content_size = self.get_content_size(rotation)
         return final_page_size(content_size, page, settings)
 
     def get_placement_matrix(self, page: Page, settings=Settings()) -> Matrix44:
         # Argument `page` has to be the resolved final page size!
-
         rotation = self.get_rotation(settings)
 
         content_size = self.get_content_size(rotation)
         content_size_mm = content_size * settings.scale
         if settings.fit_page:
             content_size_mm *= fit_to_page(content_size_mm, page)
-        scale_dxf_to_mm = content_size_mm.x / content_size.x
+        try:
+            scale_dxf_to_mm = content_size_mm.x / content_size.x
+        except ZeroDivisionError:
+            scale_dxf_to_mm = 1.0
         # map output coordinates to range [0, output_coordinate_space]
-        scale_mm_to_output_space = settings.output_coordinate_space / max(
-            page.width_in_mm, page.height_in_mm
-        )
+        try:
+            scale_mm_to_output_space = settings.output_coordinate_space / max(
+                page.width_in_mm, page.height_in_mm
+            )
+        except ZeroDivisionError:
+            scale_mm_to_output_space = 1.0
 
         scale = scale_dxf_to_mm * scale_mm_to_output_space
         m = placement_matrix(
             self.dxf_bbox,
             sx=scale,
             sy=scale * self.flip_y,
             rotation=rotation,
@@ -346,43 +351,54 @@
     )
     return Page(round(width, 1), round(height, 1), Units.mm, margins)
 
 
 def limit_page_size(
     width: float, height: float, max_width: float, max_height: float
 ) -> tuple[float, float]:
-    ar = width / height
+    try:
+        ar = width / height
+    except ZeroDivisionError:
+        return width, height
     if max_height:
         height = min(max_height, height)
         width = height * ar
     if max_width and width > max_width:
         width = min(max_width, width)
         height = width / ar
     return width, height
 
 
 def fit_to_page(content_size_mm: Vec2, page: Page) -> float:
     margins = page.margins_in_mm
-    sx = (page.width_in_mm - margins.left - margins.right) / content_size_mm.x
-    sy = (page.height_in_mm - margins.top - margins.bottom) / content_size_mm.y
+    try:
+        sx = (page.width_in_mm - margins.left - margins.right) / content_size_mm.x
+        sy = (page.height_in_mm - margins.top - margins.bottom) / content_size_mm.y
+    except ZeroDivisionError:
+        return 1.0
     return min(sx, sy)
 
 
 def placement_matrix(
     bbox: BoundingBox2d,
     sx: float,
     sy: float,
     rotation: float,
     page: Page,
     output_coordinate_space: float,
 ) -> Matrix44:
     """Returns a matrix to place the bbox in the first quadrant of the coordinate
     system (+x, +y).
     """
-    scale_mm_to_vb = output_coordinate_space / max(page.width_in_mm, page.height_in_mm)
+    try:
+        scale_mm_to_vb = output_coordinate_space / max(
+            page.width_in_mm, page.height_in_mm
+        )
+    except ZeroDivisionError:
+        scale_mm_to_vb = 1.0
     margins = page.margins_in_mm
 
     # create scaling and rotation matrix:
     if abs(sx) < 1e-9:
         sx = 1.0
     if abs(sy) < 1e-9:
         sy = 1.0
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/matplotlib.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/matplotlib.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,17 +172,14 @@
 
     def draw_filled_paths(
         self,
         paths: Iterable[ezdxf.path.Path | ezdxf.path.Path2d],
         holes: Iterable[ezdxf.path.Path | ezdxf.path.Path2d],
         properties: BackendProperties,
     ):
-        # Hatch patterns are handled by the frontend since v0.18.1
-        if self.config.hatch_policy == HatchPolicy.SHOW_OUTLINE:
-            return
         linewidth = 0
         oriented_paths: list[ezdxf.path.Path | ezdxf.path.Path2d] = []
         for path in paths:
             try:
                 path = path.counter_clockwise()
             except ValueError:  # cannot detect path orientation
                 continue
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/mtext_complex.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/mtext_complex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/properties.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,18 +12,19 @@
     Iterable,
     NamedTuple,
 )
 import re
 import copy
 
 from ezdxf import options
+from ezdxf.colors import RGB
 from ezdxf.addons import acadctb
 from ezdxf.addons.drawing.config import Configuration
-from ezdxf.addons.drawing.type_hints import Color, RGB
-from ezdxf.colors import luminance, DXF_DEFAULT_COLORS, int2rgb
+from ezdxf.addons.drawing.type_hints import Color
+from ezdxf.colors import DXF_DEFAULT_COLORS, int2rgb
 from ezdxf.entities import (
     Attrib,
     Insert,
     Face3d,
     Linetype,
     Viewport,
     Layer,
@@ -67,16 +68,15 @@
 MODEL_SPACE_BG_COLOR = "#212830"
 PAPER_SPACE_BG_COLOR = "#ffffff"
 VIEWPORT_COLOR = "#aaaaaa"  # arbitrary choice
 OLE2FRAME_COLOR = "#89adba"  # arbitrary choice
 
 
 def is_dark_color(color: Color, dark: float = 0.2) -> bool:
-    luma = luminance(hex_to_rgb(color[:7]))
-    return luma <= dark
+    return RGB.from_hex(color).luminance <= dark
 
 
 class Filling:
     SOLID = 0
     PATTERN = 1
     GRADIENT = 2
 
@@ -154,39 +154,39 @@
             f"({self.color}, {self.linetype_name}, {self.lineweight}, "
             f'"{self.layer}")'
         )
 
     @property
     def rgb(self) -> RGB:
         """Returns color as RGB tuple."""
-        return hex_to_rgb(self.color[:7])  # ignore alpha if present
+        return RGB.from_hex(self.color)
 
     @property
     def luminance(self) -> float:
         """Returns perceived color luminance in range [0, 1] from dark to light."""
-        return luminance(self.rgb)
+        return self.rgb.luminance
 
 
 class BackendProperties(NamedTuple):
     """The backend receives a condensed version of the entity properties."""
     color: Color = "#000000"
     lineweight: float = 0.25  # in mm
     layer: str = "0"  # maybe useful to group entities (SVG, PDF)
     pen: int = 1  # equals the ACI (1-255), for pen based backends like plotters
     handle: str = ""  # top level entity handle
 
     @property
     def rgb(self) -> RGB:
         """Returns color as RGB tuple."""
-        return hex_to_rgb(self.color[:7])  # ignore alpha if present
+        return RGB.from_hex(self.color)
 
     @property
     def luminance(self) -> float:
         """Returns perceived color luminance in range [0, 1] from dark to light."""
-        return luminance(self.rgb)
+        return self.rgb.luminance
 
 
 class LayerProperties(Properties):
     """Modified attribute meaning:
 
     is_visible: Whether entities belonging to this layer should be drawn
     layer: Stores real layer name (mixed case)
@@ -925,15 +925,15 @@
 def hex_to_rgb(hex_string: Color) -> RGB:
     """Returns hex string color as (r, g, b) tuple."""
     hex_string = hex_string.lstrip("#")
     assert len(hex_string) == 6
     r = int(hex_string[0:2], 16)
     g = int(hex_string[2:4], 16)
     b = int(hex_string[4:6], 16)
-    return r, g, b
+    return RGB(r, g, b)
 
 
 def set_color_alpha(color: Color, alpha: int) -> Color:
     """Returns `color` including the new `alpha` channel in hex format:
     "#RRGGBBAA".
 
     Args:
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/pyqt.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/pyqt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/qtviewer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/qtviewer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/recorder.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/recorder.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,14 +15,22 @@
 from .backend import BackendInterface
 from .config import Configuration
 from .properties import BackendProperties
 from .type_hints import Color
 
 
 class RecordType(enum.Enum):
+    """Enum, determines the data record type.
+
+    Attributes:
+        POINTS:
+        SOLID_LINES:
+        PATH:
+        FILLED_PATHS:
+    """
     POINTS = enum.auto()
     SOLID_LINES = enum.auto()
     PATH = enum.auto()
     FILLED_PATHS = enum.auto()
 
 
 @dataclasses.dataclass
@@ -38,38 +46,28 @@
 
     def __init__(self) -> None:
         self.config = Configuration()
         self.background: Color = "#000000"
         self.records: list[DataRecord] = []
         self.properties: dict[int, BackendProperties] = dict()
 
-    def __copy__(self) -> Self:
-        recorder = self.__class__()
-        # config is a frozen dataclass:
-        recorder.config = self.config
-        recorder.background = self.background
-        # mutable - recordings are transformed inplace:
-        recorder.records = copy.deepcopy(self.records)
-        # hashes and BackendProperties are immutable, the properties dict may grow, but
-        # entries will never be removed:
-        recorder.properties = self.properties
-        return recorder
-
-    def copy_player(self) -> Player:
-        """Returns a :class:`Player` instance with a copy of the recordings, this player
-        needs more memory, but does not modify the original recordings.
-        """
-        return Player(self.__copy__(), shared_recordings=False)
+    def player(self) -> Player:
+        """Returns a :class:`Player` instance with the original recordings! Make a copy
+        of this player to protect the original recordings from being modified::
+
+            safe_player = recorder.player().copy()
 
-    def shared_player(self) -> Player:
-        """Returns a :class:`Player` instance with the original recordings! This player
-        is faster to create and needs less memory but is dangerous because it may modify
-        the original recordings.
         """
-        return Player(self, shared_recordings=True)
+        player = Player()
+        player.config = self.config
+        player.background = self.background
+        player.records = self.records
+        player.properties = self.properties
+        player.has_shared_recordings = True
+        return player
 
     def configure(self, config: Configuration) -> None:
         self.config = config
 
     def set_background(self, color: Color) -> None:
         self.background = color
 
@@ -141,69 +139,102 @@
     """Represents the override state for a data record.
 
     Attributes:
         properties: original or modified :class:`BackendProperties`
         is_visible: override visibility e.g. switch layers on/off
 
     """
+
     properties: BackendProperties
     is_visible: bool = True
 
 
 OverrideFunc: TypeAlias = Callable[[BackendProperties], Override]
 
 
 class Player:
     """Plays the recordings of the :class:`Recorder` backend on another backend."""
 
-    def __init__(self, recorder: Recorder, shared_recordings: bool) -> None:
-        self.config = recorder.config
-        self.background: Color = recorder.background
-        self.records: list[DataRecord] = recorder.records
-        self.properties: dict[int, BackendProperties] = recorder.properties
+    def __init__(self) -> None:
+        self.config = Configuration()
+        self.background: Color = "#000000"
+        self.records: list[DataRecord] = []
+        self.properties: dict[int, BackendProperties] = dict()
         self._bbox = BoundingBox2d()
-        self.has_shared_recordings: bool = shared_recordings
+        self.has_shared_recordings: bool = False
+
+    def __copy__(self) -> Self:
+        """Returns a copy of the player with non-shared recordings."""
+        player = self.__class__()
+        # config is a frozen dataclass:
+        player.config = self.config
+        player.background = self.background
+        # recordings are mutable - transformed inplace:
+        player.records = copy.deepcopy(self.records)
+        # the properties dict may grow, but entries will never be removed:
+        player.properties = self.properties
+        player.has_shared_recordings = False
+        return player
+
+    copy = __copy__
+
+    def recordings(self) -> Iterator[tuple[RecordType, BackendProperties, Any]]:
+        """Yields all recordings as `(RecordType, BackendProperties, Data)` tuples.
+
+        The content of the `Data` field is determined by the enum :class:`RecordType`:
+
+        - :attr:`RecordType.POINTS` returns a :class:`NumpyPoints2d` instance,
+          len() == 1 is a point, len() == 2 is a line, len() > 2 is a filled polygon
+        - :attr:`RecordType.SOLID_LINES` returns a :class:`NumpyPoints2d` instance
+          where each pair (n, n+1) represents the start- and end point of a line
+        - :attr:`RecordType.PATH`: returns a :class:`NumpyPath2d` instance that
+          represents a linear 2D path
+        - :attr:`RecordType.FILLED_PATHS` returns a tuple (exterior_paths, holes),
+          where exterior_paths and holes are tuples of :class:`NumpyPath2d`.
+
+        """
+        props = self.properties
+        for record in self.records:
+            properties = BackendProperties(
+                *props[record.property_hash][:4], record.handle
+            )
+            yield record.type, properties, record.data
 
     def replay(
         self, backend: BackendInterface, override: Optional[OverrideFunc] = None
     ) -> None:
         """Replay the recording on another backend that implements the
         :class:`BackendInterface`. The optional `override` function can be used to
         override the properties and state of data records, it gets the :class:`BackendProperties`
         as input and must return an :class:`Override` instance.
         """
 
         backend.configure(self.config)
         backend.set_background(self.background)
-        props = self.properties
-        for record in self.records:
-            properties = BackendProperties(
-                *props[record.property_hash][:4], record.handle
-            )
+        for record_type, properties, data in self.recordings():
             if override:
                 state = override(properties)
                 if not state.is_visible:
                     continue
                 properties = state.properties
-            t = record.type
-            if t == RecordType.POINTS:
-                vertices = record.data.vertices()
+            if record_type == RecordType.POINTS:
+                vertices = data.vertices()
                 if len(vertices) == 1:
                     backend.draw_point(vertices[0], properties)
                 elif len(vertices) == 2:
                     backend.draw_line(vertices[0], vertices[1], properties)
                 else:
                     backend.draw_filled_polygon(vertices, properties)
-            elif t == RecordType.SOLID_LINES:
-                backend.draw_solid_lines(take2(record.data.vertices()), properties)
-            elif t == RecordType.PATH:
-                backend.draw_path(record.data.to_path2d(), properties)
-            elif t == RecordType.FILLED_PATHS:
-                paths = [p.to_path2d() for p in record.data[0]]
-                holes = [p.to_path2d() for p in record.data[1]]
+            elif record_type == RecordType.SOLID_LINES:
+                backend.draw_solid_lines(take2(data.vertices()), properties)
+            elif record_type == RecordType.PATH:
+                backend.draw_path(data.to_path2d(), properties)
+            elif record_type == RecordType.FILLED_PATHS:
+                paths = [p.to_path2d() for p in data[0]]
+                holes = [p.to_path2d() for p in data[1]]
                 backend.draw_filled_paths(paths, holes, properties)
         backend.finalize()
 
     def transform(self, m: Matrix44) -> None:
         """Transforms the recordings inplace by a transformation matrix `m` of type
         :class:`~ezdxf.math.Matrix44`.
         """
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/svg.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/svg.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,18 +31,21 @@
         settings = copy.copy(settings)
         # The DXF coordinates are mapped to integer viewBox coordinates in the first
         # quadrant, producing compact SVG files. The larger the coordinate range, the
         # more precise and the lager the files.
         settings.output_coordinate_space = 1_000_000
 
         # This player changes the original recordings!
-        player = self.shared_player()
+        player = self.player()
 
         output_layout = layout.Layout(player.bbox(), flip_y=self._init_flip_y)
         page = output_layout.get_final_page(page, settings)
+        if page.width == 0 or page.height == 0:
+            return ET.Element("svg")  # empty page
+
         m = output_layout.get_placement_matrix(page, settings)
         player.transform(m)
         self._init_flip_y = False
         backend = self.make_backend(page, settings)
         player.replay(backend)
         return backend.get_xml_root_element()
 
@@ -51,16 +54,16 @@
         page: layout.Page,
         settings: layout.Settings = layout.Settings(),
         xml_declaration=True,
     ) -> str:
         """Returns the XML data as unicode string.
 
         Args:
-            page: page definition
-            settings: layout settings
+            page: page definition, see :class:`~ezdxf.addons.drawing.layout.Page`
+            settings: layout settings, see :class:`~ezdxf.addons.drawing.layout.Settings`
             xml_declaration: inserts the "<?xml version='1.0' encoding='utf-8'?>" string
                 in front of the <svg> element
 
         """
         xml = self.get_xml_root_element(page, settings)
         return ET.tostring(xml, encoding="unicode", xml_declaration=xml_declaration)
 
@@ -230,15 +233,15 @@
         return color[:7], alpha_to_opacity(color[7:9])
 
     def resolve_stroke_width(self, width: float) -> int:
         try:
             return self._stroke_width_cache[width]
         except KeyError:
             pass
-        stroke_width = self.fixed_stroke_width
+            stroke_width = self.fixed_stroke_width
         policy = self.lineweight_policy
         if policy == LineweightPolicy.ABSOLUTE:
             if self.lineweight_scaling:
                 width = max(self.min_lineweight, width) * self.lineweight_scaling
             else:
                 width = self.min_lineweight
             stroke_width = round(width * self.stroke_width_scale)
@@ -246,15 +249,14 @@
             stroke_width = map_lineweight_to_stroke_width(
                 width, self.min_stroke_width, self.max_stroke_width
             )
         self._stroke_width_cache[width] = stroke_width
         return stroke_width
 
     def set_background(self, color: Color) -> None:
-        # Do not alter the background color here!
         color_str = color[:7]
         opacity = alpha_to_opacity(color[7:9])
         self.background.set("fill", color_str)
         self.background.set("fill-opacity", str(opacity))
 
     def draw_point(self, pos: AnyVec, properties: BackendProperties) -> None:
         self.add_strokes(self.make_polyline_str([pos, pos]), properties)
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/text_renderer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/drawing/unified_text_renderer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/drawing/unified_text_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/classes_section.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/classes_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/const.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/crc.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/crc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/fileheader.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/fileheader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/header_section.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/header_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/dwg/loader.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/dwg/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/backend.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,16 +5,16 @@
 from typing_extensions import Self
 import abc
 import copy
 import enum
 import math
 from .deps import (
     Vec2,
-    Path,
-    luminance,
+    Path2d,
+    colors,
     Matrix44,
     BoundingBox2d,
 )
 from .properties import Properties, Pen
 from ezdxf.npshapes import NumpyPath2d, NumpyPoints2d
 
 # Page coordinates are always plot units:
@@ -23,23 +23,15 @@
 # 1016 plu = 1 inch
 # 3.39 plu = 1 dot @300 dpi
 # positive x-axis is horizontal from left to right
 # positive y-axis is vertical from bottom to top
 
 
 class Backend(abc.ABC):
-    """Abstract base class for implementing a low level output backends.
-
-    All input coordinates are page coordinates:
-
-        - 1 plot unit (plu) = 0.025mm
-        - 40 plu = 1 mm
-        - 1016 plu = 1 inch
-
-    """
+    """Abstract base class for implementing a low level output backends."""
 
     @abc.abstractmethod
     def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
         """Draws a polyline from a sequence `points`. The input coordinates are page
         coordinates in plot units. The `points` sequence can contain 0 or more
         points!
 
@@ -47,42 +39,53 @@
             properties: display :class:`Properties` for the polyline
             points: sequence of :class:`ezdxf.math.Vec2` instances
 
         """
         ...
 
     @abc.abstractmethod
-    def draw_filled_polygon(
-        self, properties: Properties, paths: Sequence[Path]
+    def draw_paths(
+        self, properties: Properties, paths: Sequence[Path2d], filled: bool
     ) -> None:
-        """Draws a filled polygon from the sequence of `paths`. The input coordinates
+        """Draws filled or outline paths from the sequence of `paths`. The input coordinates
         are page coordinates in plot units. The `paths` sequence can contain 0 or more
-        single :class:`~ezdxf.path.Path` instances.
+        single :class:`~ezdxf.path.Path` instances. Draws outline paths if
+        Properties.FillType is NONE and filled paths otherwise.
 
         Args:
             properties: display :class:`Properties` for the filled polygon
-            paths: sequence of single :class:`ezdxf.path.Path` instances
+            paths: sequence of single :class:`ezdxf.path.Path2d` instances
+            filled: draw filled paths if ``True`` otherwise outline paths
 
         """
         ...
 
 
 class RecordType(enum.Enum):
     POLYLINE = enum.auto()
-    FILLED_POLYGON = enum.auto()
+    FILLED_PATHS = enum.auto()
+    OUTLINE_PATHS = enum.auto()
 
 
 class DataRecord(NamedTuple):
     type: RecordType
     property_hash: int
     data: Any
 
 
 class Recorder(Backend):
-    """The :class:`Recorder` class records the output of the :class:`Plotter` class."""
+    """The :class:`Recorder` class records the output of the :class:`Plotter` class.
+
+    All input coordinates are page coordinates:
+
+    - 1 plot unit (plu) = 0.025mm
+    - 40 plu = 1 mm
+    - 1016 plu = 1 inch
+
+    """
 
     def __init__(self) -> None:
         self._records: list[DataRecord] = []
         self._properties: dict[int, Properties] = {}
         self._pens: Sequence[Pen] = []
 
     def player(self) -> Player:
@@ -93,33 +96,35 @@
 
         """
         return Player(self._records, self._properties)
 
     def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
         self.store(RecordType.POLYLINE, properties, NumpyPoints2d(points))
 
-    def draw_filled_polygon(
-        self, properties: Properties, paths: Sequence[Path]
+    def draw_paths(
+        self, properties: Properties, paths: Sequence[Path2d], filled: bool
     ) -> None:
         data = tuple(NumpyPath2d(p) for p in paths)
-        self.store(RecordType.FILLED_POLYGON, properties, data)
+        record_type = RecordType.FILLED_PATHS if filled else RecordType.OUTLINE_PATHS
+        self.store(record_type, properties, data)
 
     def store(self, record_type: RecordType, properties: Properties, args) -> None:
         prop_hash = properties.hash()
         if prop_hash not in self._properties:
             self._properties[prop_hash] = properties.copy()
         self._records.append(DataRecord(record_type, prop_hash, args))
         if len(self._pens) != len(properties.pen_table):
             self._pens = list(properties.pen_table.values())
 
 
 class Player:
     """This class replays the recordings of the :class:`Recorder` class on another
     backend. The class can modify the recorded output.
     """
+
     def __init__(self, records: list[DataRecord], properties: dict[int, Properties]):
         self._records: list[DataRecord] = records
         self._properties: dict[int, Properties] = properties
         self._bbox = BoundingBox2d()
 
     def __copy__(self) -> Self:
         """Returns a new :class:`Player` instance with a copy of recordings."""
@@ -127,17 +132,17 @@
         player = self.__class__(records, self._properties)
         player._bbox = self._bbox.copy()
         return player
 
     copy = __copy__
 
     def recordings(self) -> Iterator[tuple[RecordType, Properties, Any]]:
-        """Yields all recordings as [RecordType, Properties, Any] tuples.
+        """Yields all recordings as `(RecordType, Properties, Data)` tuples.
 
-        The last field is the data field and depends on :class:`RecordType`:
+        The content of the `Data` field is determined by the enum :class:`RecordType`:
 
         - :attr:`RecordType.POLYLINE` returns a :class:`NumpyPoints2d` instance
         - :attr:`RecordType.FILLED_POLYGON` returns a tuple of :class:`NumpyPath2d` instances
 
         """
         props = self._properties
         for record in self._records:
@@ -167,15 +172,17 @@
         props = self._properties
         for record in self._records:
             current_props = props.get(record.property_hash, current_props)
             if record.type == RecordType.POLYLINE:
                 backend.draw_polyline(current_props, record.data.vertices())
             else:
                 paths = [p.to_path2d() for p in record.data]
-                backend.draw_filled_polygon(current_props, paths)
+                backend.draw_paths(
+                    current_props, paths, filled=record.type == RecordType.FILLED_PATHS
+                )
 
     def transform(self, m: Matrix44) -> None:
         """Transforms the recordings by a transformation matrix `m` of type
         :class:`~ezdxf.math.Matrix44`.
         """
         for record in self._records:
             if record.type == RecordType.POLYLINE:
@@ -184,35 +191,35 @@
                 for path in record.data:
                     path.transform_inplace(m)
 
         if self._bbox.has_data:
             # fast, but maybe inaccurate update
             self._bbox = BoundingBox2d(m.fast_2d_transform(self._bbox.rect_vertices()))
 
-    def sort_filled_polygons(self) -> None:
-        """Sort filled polygons by descending luminance (from light to dark).
+    def sort_filled_paths(self) -> None:
+        """Sort filled paths by descending luminance (from light to dark).
 
-        This also changes the plot order in the way that all filled polygons are plotted
-        before the polylines.
+        This also changes the plot order in the way that all filled paths are plotted
+        before polylines and outline paths.
         """
-        polygons = []
-        polylines = []
+        fillings = []
+        outlines = []
         current = Properties()
         props = self._properties
         for record in self._records:
-            if record.type == RecordType.FILLED_POLYGON:
+            if record.type == RecordType.FILLED_PATHS:
                 current = props.get(record.property_hash, current)
-                key = luminance(current.resolve_fill_color())
-                polygons.append((key, record))
+                key = colors.luminance(current.resolve_fill_color())
+                fillings.append((key, record))
             else:
-                polylines.append(record)
+                outlines.append(record)
 
-        polygons.sort(key=lambda r: r[0], reverse=True)
-        records = [sort_rec[1] for sort_rec in polygons]
-        records.extend(polylines)
+        fillings.sort(key=lambda r: r[0], reverse=True)
+        records = [sort_rec[1] for sort_rec in fillings]
+        records.extend(outlines)
         self._records = records
 
 
 def placement_matrix(
     bbox: BoundingBox2d, sx: float = 1.0, sy: float = 1.0, rotation: float = 0.0
 ) -> Matrix44:
     """Returns a matrix to place the bbox in the first quadrant of the coordinate
@@ -221,10 +228,10 @@
     if abs(sx) < 1e-9:
         sx = 1.0
     if abs(sy) < 1e-9:
         sy = 1.0
     m = Matrix44.scale(sx, sy, 1.0)
     if rotation:
         m @= Matrix44.z_rotate(math.radians(rotation))
-    corners = m.transform_vertices(bbox.rect_vertices())
+    corners = m.fast_2d_transform(bbox.rect_vertices())
     tx, ty = BoundingBox2d(corners).extmin  # type: ignore
     return m @ Matrix44.translate(-tx, -ty, 0)
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/dxf_backend.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/acad_proxy_entity.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,140 +1,128 @@
-#  Copyright (c) 2023, Manfred Moitzi
+#  Copyright (c) 2021-2022, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import TYPE_CHECKING, Sequence, Optional, Iterable
-import enum
-
-from functools import lru_cache
-from ezdxf.gfxattribs import GfxAttribs
-from ezdxf.lldxf.const import VALID_DXF_LINEWEIGHTS, BYLAYER
-from ezdxf.entities import Hatch
-import ezdxf.path
-
-from .deps import Vec2, Path
-from .properties import Properties, RGB_NONE, RGB, RGB_BLACK, RGB_WHITE, Pen
-from .backend import Backend
+from typing import TYPE_CHECKING, Optional, Iterator
+from ezdxf.lldxf import const
+from ezdxf.lldxf.tags import Tags
+from .dxfentity import SubclassProcessor
+from .dxfgfx import DXFGraphic
+from . import factory
 
 if TYPE_CHECKING:
-    from ezdxf.eztypes import GenericLayoutType
-
-
-class ColorMode(enum.Enum):
-    # Use color index as primary color, ignores RGB color except for solid fill
-    ACI = enum.auto()
-
-    # Use always the RGB value
-    RGB = enum.auto()
-
+    from ezdxf.lldxf.tagwriter import AbstractTagWriter
+    from ezdxf.entities import DXFNamespace
 
-class DXFBackend(Backend):
-    """DXF backend.
 
-    The page content will be created in any given layout and 1 drawing unit is 1 plot
-    unit (1 plu = 0.025mm).
+# Group Codes of AcDbProxyEntity
+# https://help.autodesk.com/view/OARX/2018/ENU/?guid=GUID-89A690F9-E859-4D57-89EA-750F3FB76C6B
+# 100 AcDbProxyEntity
+# 90  Proxy entity class ID (always 498)
+# 91  Application entity's class ID. Class IDs are based on the order of
+#     the class in the CLASSES section. The first class is given the ID of
+#     500, the next is 501, and so on
+#
+# 92  Size of graphics data in bytes < R2010; R2010+ = 160
+# 310 Binary graphics data (multiple entries can appear) (optional)
+#
+# 96  Size of unknown data in bytes < R2010; R2010+ = 162
+# 311 Binary entity data (multiple entries can appear) (optional)
+#
+# 93  Size of entity data in bits <R2010; R2010+ = 161
+# 310 Binary entity data (multiple entries can appear) (optional)
+#
+# 330 or 340 or 350 or 360 - An object ID (multiple entries can appear) (optional)
+# 94  0 (indicates end of object ID section)
+# 95  Object drawing format when it becomes a proxy (a 32-bit unsigned integer):
+#     Low word is AcDbDwgVersion
+#     High word is MaintenanceReleaseVersion
+# 70  Original custom object data format:
+#     0 = DWG format
+#     1 = DXF format
+
+
+@factory.register_entity
+class ACADProxyEntity(DXFGraphic):
+    """READ ONLY ACAD_PROXY_ENTITY CLASS! DO NOT MODIFY!"""
 
-    All entities are assigned to a layer according to the pen number with the name schema
-    ``COLOR_<#>``. In order to be able to process the file better, it is also possible to
-    assign an :term:`ACI` color to the DXF entities according to the pen number by setting
-    the argument `color_mode` to :attr:`ColorMode.ACI`, but then the RGB color is lost
-    because the RGB color has always the higher priority over the :term:`ACI`.
+    DXFTYPE = "ACAD_PROXY_ENTITY"
+    MIN_DXF_VERSION_FOR_EXPORT = const.DXF2000
 
-    Args:
-        layout: any layout, modelspace, paperspace or block
-        color_mode: class:`ColorMode`
-        map_black_rgb_to_white_rgb: maps black fillings and lines to white.
-
-    """
-
-    def __init__(
-        self,
-        layout: GenericLayoutType,
-        color_mode=ColorMode.RGB,
-        map_black_rgb_to_white_rgb=False,
-    ) -> None:
+    def __init__(self) -> None:
         super().__init__()
-        self.layout = layout
+        self.acdb_proxy_entity: Optional[Tags] = None
 
-        doc = layout.doc
-        if doc is not None:
-            self.layers = doc.layers
-        else:
-            self.layers = None
-        self.color_mode = color_mode
+    def raw_copy(self):
+        raise const.DXFTypeError(f"Cloning of {self.dxftype()} not supported.")
 
-        # map black RGB to white RGB, does not affect ACI colors:
-        self.map_black_rgb_to_white_rgb = map_black_rgb_to_white_rgb
-
-    def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
-        count = len(points)
-        if count == 0:
-            return
-        attribs = self.make_dxf_attribs(properties)
-        if count > 2:
-            self.layout.add_lwpolyline(points, dxfattribs=attribs)
-        elif count == 2:
-            self.layout.add_line(points[0], points[1], dxfattribs=attribs)
+    def load_dxf_attribs(
+        self, processor: Optional[SubclassProcessor] = None
+    ) -> DXFNamespace:
+        dxf = super().load_dxf_attribs(processor)
+        if processor:
+            self.acdb_proxy_entity = processor.subclass_by_index(2)
+            self.load_proxy_graphic(processor.dxfversion)
+        return dxf
+
+    def load_proxy_graphic(self, dxfversion: Optional[str]) -> None:
+        if self.acdb_proxy_entity is not None:
+            if not dxfversion:
+                dxfversion = _detect_dxf_version(self.acdb_proxy_entity)
+            length_code = 92 if dxfversion < const.DXF2013 else 160
+            self.proxy_graphic = load_proxy_data(
+                self.acdb_proxy_entity, length_code, 310
+            )
+
+    def export_dxf(self, tagwriter: AbstractTagWriter) -> None:
+        # Proxy graphic is stored in AcDbProxyEntity and not as usual in
+        # AcDbEntity!
+        preserve_proxy_graphic = self.proxy_graphic
+        self.proxy_graphic = None
+        super().export_dxf(tagwriter)
+        self.proxy_graphic = preserve_proxy_graphic
+
+    def export_entity(self, tagwriter: AbstractTagWriter) -> None:
+        """Export entity specific data as DXF tags. (internal API)"""
+        # Base class and AcDbEntity export is done by parent class
+        super().export_entity(tagwriter)
+        if self.acdb_proxy_entity is not None:
+            tagwriter.write_tags(self.acdb_proxy_entity)
+        # XDATA export is done by the parent class
+
+    def __virtual_entities__(self) -> Iterator[DXFGraphic]:
+        """Implements the SupportsVirtualEntities protocol."""
+        from ezdxf.proxygraphic import ProxyGraphic
+
+        if self.proxy_graphic:
+            for e in ProxyGraphic(
+                self.proxy_graphic, self.doc
+            ).virtual_entities():
+                e.set_source_of_copy(self)
+                yield e
+        return []
+
+    def virtual_entities(self) -> Iterator[DXFGraphic]:
+        """Yields proxy graphic as "virtual" entities."""
+        return self.__virtual_entities__()
+
+
+def load_proxy_data(
+    tags: Tags, length_code: int, data_code: int = 310
+) -> Optional[bytes]:
+    try:
+        index = tags.tag_index(length_code)
+    except const.DXFValueError:
+        return None
+    binary_data = []
+    for code, value in tags[index + 1 :]:
+        if code == data_code:
+            binary_data.append(value)
         else:
-            self.layout.add_point(points[0], dxfattribs=attribs)
+            break  # at first tag with group code != data_code
+    return b"".join(binary_data)
+
 
-    def draw_filled_polygon(
-        self, properties: Properties, paths: Sequence[Path]
-    ) -> None:
-        attribs = self.make_dxf_attribs(properties)
-        # max sagitta distance of 10 plu = 0.25 mm
-        hatches = ezdxf.path.render_hatches(
-            self.layout, paths, edge_path=False, dxfattribs=attribs, distance=10
-        )
-        for hatch in hatches:
-            assert isinstance(hatch, Hatch)
-            rgb: Optional[RGB] = properties.resolve_fill_color()
-            if self.color_mode == ColorMode.ACI:
-                rgb = RGB_NONE
-            if self.map_black_rgb_to_white_rgb and rgb == RGB_BLACK:
-                rgb = RGB_WHITE
-            if rgb is RGB_NONE:
-                rgb = None
-            hatch.set_solid_fill(color=attribs.color, style=0, rgb=rgb)
-
-    def make_dxf_attribs(self, properties: Properties):
-        aci = properties.pen_index
-        if aci < 1 or aci > 255:
-            aci = 7
-
-        layer = f"COLOR_{aci}"
-        if self.layers and not self.layers.has_entry(layer):
-            self.layers.add(name=layer, color=aci)
-
-        attribs = GfxAttribs(
-            color=BYLAYER,
-            lineweight=make_lineweight(properties.pen_width),
-            layer=layer,
-        )
-        if self.color_mode == ColorMode.RGB:
-            color = properties.resolve_pen_color()
-            if self.map_black_rgb_to_white_rgb and color == RGB_BLACK:
-                color = RGB_WHITE
-            attribs.rgb = color
-        return attribs
-
-
-@lru_cache(maxsize=None)
-def make_lineweight(width: float) -> int:
-    width_int = int(width * 100)
-    for lw in VALID_DXF_LINEWEIGHTS:
-        if width_int <= lw:
-            return lw
-    return VALID_DXF_LINEWEIGHTS[-1]
-
-
-def make_ctb(pens: Iterable[Pen]):
-    from ezdxf.addons import acadctb
-
-    ctb = acadctb.new_ctb()
-    for pen in pens:
-        try:
-            style = ctb.new_style(pen.index)
-        except IndexError:
-            continue
-        style.set_lineweight(pen.width)
-        style.color = pen.color
-    return ctb
+def _detect_dxf_version(tags: Tags) -> str:
+    for tag in tags:
+        if 160 <= tag.code < 163:
+            return const.DXF2013
+    return const.DXF2000
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/interpreter.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/interpreter.py`

 * *Files 2% similar despite different names*

```diff
@@ -329,15 +329,15 @@
             return
 
         plotter = self.plotter
         # The last pen up/down state remains after leaving the PE command.
         pen_down = True
         # Ignores and preserves the current absolute/relative mode of the plotter.
         absolute = False
-        decimal_places = 0
+        frac_bin_bits = 0
         base = 64
         index = 0
         length = len(data)
         point_queue: list[Vec2] = []
 
         while index < length:
             char = data[index]
@@ -348,24 +348,24 @@
                     plotter.set_current_pen(int(values[0]))
                     if len(values) > 1:
                         point_queue.extend(to_points(values[1:]))
                 elif char == 60:  # "<" -  pen up and goto coordinates
                     pen_down = False
                 elif char == 62:  # ">" - fractional data
                     values, index = pe_decode(data, base=base, start=index)
-                    decimal_places = int(values[0])
+                    frac_bin_bits = int(values[0])
                     if len(values) > 1:
                         point_queue.extend(to_points(values[1:]))
                 elif char == 61:  # "=" - next coordinates are absolute
                     absolute = True
                 elif char == 55:  # "7" - 7-bit mode
                     base = 32
             else:
                 values, index = pe_decode(
-                    data, decimal_places=decimal_places, base=base, start=index
+                    data, frac_bits=frac_bin_bits, base=base, start=index
                 )
                 point_queue.extend(to_points(values))
 
             if point_queue:
                 plotter.pen_down()
                 if absolute:
                     # next point is absolute: make relative
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/page.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/page.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/plotter.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/plotter.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,20 +2,20 @@
 #  License: MIT License
 from __future__ import annotations
 from typing import Sequence, Iterator
 import math
 
 from .deps import (
     Vec2,
-    Path,
+    Path2d,
     NULLVEC2,
     ConstructionCircle,
     Bezier4P,
 )
-from .properties import RGB, Properties
+from .properties import RGB, Properties, FillType
 from .backend import Backend
 from .polygon_buffer import PolygonBuffer
 from .page import Page
 
 
 class Plotter:
     """
@@ -246,38 +246,32 @@
         # input coordinates are user coordinates
         current_page_location = self.page_location
         self.move_to_abs(end)  # user coordinates!
         if self.is_pen_down:
             # convert to page coordinates:
             ctrl1, ctrl2, end = self.page.page_points((ctrl1, ctrl2, end))
             # draw cubic bezier curve in absolute page coordinates:
-            curve = Bezier4P([current_page_location, ctrl1, ctrl2, end])
-            # distance of 10 plu is 0.25 mm
-            self.backend.draw_polyline(
-                self.properties, list(curve.flattening(distance=10))
-            )
+            p = Path2d(current_page_location)
+            p.curve4_to(end, ctrl1, ctrl2)
+            self.backend.draw_paths(self.properties, [p], filled=False)
 
     def plot_rel_cubic_bezier(self, ctrl1: Vec2, ctrl2: Vec2, end: Vec2):
         # input coordinates are user coordinates
         ctrl1, ctrl2, end = rel_to_abs_points_static(
             self.user_location, (ctrl1, ctrl2, end)
         )
         self.plot_abs_cubic_bezier(ctrl1, ctrl2, end)
 
-    def plot_filled_polygon_buffer(self, paths: Sequence[Path]):
+    def plot_filled_polygon_buffer(self, paths: Sequence[Path2d]):
         # input coordinates are page coordinates!
-        self.backend.draw_filled_polygon(self.properties, paths)
+        self.backend.draw_paths(self.properties, paths, filled=True)
 
-    def plot_outline_polygon_buffer(self, paths: Sequence[Path]):
+    def plot_outline_polygon_buffer(self, paths: Sequence[Path2d]):
         # input coordinates are page coordinates!
-        for path in paths:
-            path.close_sub_path()
-            self.backend.draw_polyline(
-                self.properties, Vec2.list(path.flattening(distance=10))
-            )
+        self.backend.draw_paths(self.properties, paths, filled=False)
 
 
 def rel_to_abs_points_dynamic(current: Vec2, points: Sequence[Vec2]) -> Iterator[Vec2]:
     """Returns the absolute location of increment points, each point is an increment
     of the previous point starting at the current pen location.
     """
     for point in points:
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/polygon_buffer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/polygon_buffer.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Sequence
 from .backend import Backend
-from .deps import Vec2, Path
+from .deps import Vec2, Path2d
 from .properties import Properties
 
 
 class PolygonBuffer(Backend):
     def __init__(self):
-        self.path = Path()
+        self.path = Path2d()
         self.start_new_sub_polygon = False
 
     def draw_polyline(self, properties: Properties, points: Sequence[Vec2]) -> None:
         if len(points) == 0:
             return
         index = 0
         if self.start_new_sub_polygon:
@@ -23,23 +23,31 @@
                 index += 1
                 if index == count:
                     return
             self.path.move_to(points[index])
         for p in points[index + 1 :]:
             self.path.line_to(p)
 
-    def draw_filled_polygon(
-        self, properties: Properties, paths: Sequence[Path]
+    def draw_paths(
+        self, properties: Properties, paths: Sequence[Path2d], filled: bool
     ) -> None:
-        raise NotImplementedError()
+        if filled:
+            raise NotImplementedError()
+        for p in paths:
+            if len(p) == 0:
+                continue
+            if self.start_new_sub_polygon:
+                self.start_new_sub_polygon = False
+                self.path.move_to(p.start)
+            self.path.append_path(p)
 
-    def get_paths(self) -> Sequence[Path]:
+    def get_paths(self) -> Sequence[Path2d]:
         return list(self.path.sub_paths())
 
     def close_path(self):
         if len(self.path):
             self.path.close_sub_path()
             self.start_new_sub_polygon = True
 
     def reset(self, location: Vec2) -> None:
-        self.path = Path(location)
+        self.path = Path2d(location)
         self.start_new_sub_polygon = False
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/properties.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/properties.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #  Copyright (c) 2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
-from typing import NamedTuple, Iterable
 import dataclasses
 import enum
 import copy
+from ezdxf.colors import RGB
 
 
 class FillType(enum.IntEnum):
     """Fill type enumeration."""
 
     NONE = 0
     SOLID = 1
@@ -20,26 +20,14 @@
 class FillMethod(enum.IntEnum):
     """Fill method enumeration."""
 
     EVEN_ODD = 0
     NON_ZERO_WINDING = 1
 
 
-class RGB(NamedTuple):
-    """Named tuple representing an RGB color value."""
-
-    r: int
-    g: int
-    b: int
-
-    def to_floats(self) -> tuple[float, float, float]:
-        """Returns the RGB color value as a tuple of floats in the range from 0 to 1."""
-        return self.r / 255, self.g / 255, self.b / 255
-
-
 RGB_NONE = RGB(-1, -1, -1)
 RGB_BLACK = RGB(0, 0, 0)
 RGB_WHITE = RGB(255, 255, 255)
 LIGHT_GREY = RGB(200, 200, 200)
 
 
 @dataclasses.dataclass
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/tokenizer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -157,18 +157,21 @@
     if name == "PE":
         args = (bytes([c for c in cmd[2:] if c > 32]),)
     else:
         args = tuple(s for s in cmd[2:].split(b","))  # type: ignore
     return Command(name, args)
 
 
-def pe_encode(value: float, decimal_places: int = 0, base: int = 64) -> bytes:
-    if decimal_places:
-        n = round(decimal_places * 3.33)
-        value *= 2 << n
+def fractional_bits(decimal_places: int) -> int:
+    return round(decimal_places * 3.33)
+
+
+def pe_encode(value: float, frac_bits: int = 0, base: int = 64) -> bytes:
+    if frac_bits:
+        value *= 1 << frac_bits
         x = round(value)
     else:
         x = round(value)
     if x >= 0:
         x *= 2
     else:
         x = abs(x) * 2 + 1
@@ -181,41 +184,41 @@
         chars.append(191 + x)
     else:
         chars.append(95 + x)
     return bytes(chars)
 
 
 def pe_decode(
-    s: bytes, decimal_places: int = 0, base=64, start: int = 0
+    s: bytes, frac_bits: int = 0, base=64, start: int = 0
 ) -> tuple[list[float], int]:
     def _decode():
         factors.reverse()
         x = 0
         for f in factors:
             x = x * base + f
         factors.clear()
         if x & 1:
             x = -(x - 1)
         x = x >> 1
         return x
 
+    n = 1 << frac_bits
     if base == 64:
         terminator = 191
     else:
         terminator = 95
     values: list[float] = []
     factors = []
     for index in range(start, len(s)):
         value = s[index]
         if value < 63:
             return values, index
         if value >= terminator:
             factors.append(value - terminator)
             x = _decode()
-            if decimal_places:
-                n = 2 << round(decimal_places * 3.33)
-                values.append(round(x / n, decimal_places))
+            if frac_bits:
+                values.append(x / n)
             else:
-                values.append(round(float(x), decimal_places))
+                values.append(float(x))
         else:
             factors.append(value - 63)
     return values, len(s)
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/addons/hpgl2/viewer.py` & `ezdxf-1.1.0b3/src/ezdxf/addons/hpgl2/viewer.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 # Copyright (c) 2023, Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-from typing import Any
+from typing import Any, TYPE_CHECKING
+
 import math
 import os
-import time
+import pathlib
 
-from ezdxf.math import BoundingBox2d, Matrix44
 from ezdxf.addons import xplayer
-from ezdxf.addons.xqt import QtWidgets, QtGui, QtCore
-from ezdxf.addons.drawing import svg, layout
+from ezdxf.addons.xqt import QtWidgets, QtGui, QtCore, QMessageBox
+from ezdxf.addons.drawing import svg, layout, pymupdf, dxf
 from ezdxf.addons.drawing.qtviewer import CADGraphicsView
 from ezdxf.addons.drawing.pyqt import PyQtPlaybackBackend
 
 from . import api
+from .deps import BoundingBox2d, Matrix44, colors
+
+if TYPE_CHECKING:
+    from ezdxf.document import Drawing
 
 VIEWER_NAME = "HPGL/2 Viewer"
 
 
 class HPGL2Widget(QtWidgets.QWidget):
     def __init__(self, view: CADGraphicsView) -> None:
         super().__init__()
@@ -39,36 +43,44 @@
 
     @property
     def player(self) -> api.Player:
         return self._player.copy()
 
     def plot(self, data: bytes) -> None:
         self._reset_backend()
-        self._player = api.record_plotter_output(
-            data, 0, 1.0, 1.0, api.MergeControl.AUTO
-        )
+        self._player = api.record_plotter_output(data, api.MergeControl.AUTO)
 
     def replay(
         self, bg_color="#ffffff", override=None, reset_view: bool = True
     ) -> None:
         self._reset_backend()
         self._view.begin_loading()
         new_scene = QtWidgets.QGraphicsScene()
         self._backend.set_scene(new_scene)
+        new_scene.addItem(self._bg_paper(bg_color))
+
         xplayer.hpgl2_to_drawing(
-            self._player, self._backend, bg_color=bg_color, override=override
+            self._player, self._backend, bg_color="", override=override
         )
         self._view.end_loading(new_scene)
         self._view.buffer_scene_rect()
         if reset_view:
             self._view.fit_to_scene()
 
+    def _bg_paper(self, color):
+        bbox = self._player.bbox()
+        insert = bbox.extmin
+        size = bbox.size
+        rect = QtWidgets.QGraphicsRectItem(insert.x, insert.y, size.x, size.y)
+        rect.setBrush(QtGui.QBrush(QtGui.QColor(color)))
+        return rect
+
 
 SPACING = 20
-DEFAULT_DPI = 72
+DEFAULT_DPI = 96
 COLOR_SCHEMA = [
     "Default",
     "Black on White",
     "White on Black",
     "Monochrome Light",
     "Monochrome Dark",
     "Blueprint High Contrast",
@@ -80,15 +92,16 @@
     def __init__(self) -> None:
         super().__init__()
         self._cad = HPGL2Widget(CADGraphicsView())
         self._view = self._cad.view
         self._player: api.Player = api.Player([], {})
         self._bbox: BoundingBox2d = BoundingBox2d()
         self._page_rotation = 0
-        self._color_schema = 0
+        self._color_scheme = 0
+        self._current_file = pathlib.Path()
 
         self.page_size_label = QtWidgets.QLabel()
         self.png_size_label = QtWidgets.QLabel()
         self.message_label = QtWidgets.QLabel()
         self.scaling_factor_line_edit = QtWidgets.QLineEdit("1")
         self.dpi_line_edit = QtWidgets.QLineEdit(str(DEFAULT_DPI))
 
@@ -104,14 +117,27 @@
         self.rotation_combo_box.addItems(["0", "90", "180", "270"])
         self.rotation_combo_box.currentIndexChanged.connect(self.update_rotation)
 
         self.color_combo_box = QtWidgets.QComboBox()
         self.color_combo_box.addItems(COLOR_SCHEMA)
         self.color_combo_box.currentIndexChanged.connect(self.update_colors)
 
+        self.aci_export_mode = QtWidgets.QCheckBox("ACI Export Mode")
+        self.aci_export_mode.setCheckState(QtCore.Qt.CheckState.Unchecked)
+
+        self.export_svg_button = QtWidgets.QPushButton("Export SVG")
+        self.export_svg_button.clicked.connect(self.export_svg)
+        self.export_png_button = QtWidgets.QPushButton("Export PNG")
+        self.export_png_button.clicked.connect(self.export_png)
+        self.export_pdf_button = QtWidgets.QPushButton("Export PDF")
+        self.export_pdf_button.clicked.connect(self.export_pdf)
+        self.export_dxf_button = QtWidgets.QPushButton("Export DXF")
+        self.export_dxf_button.clicked.connect(self.export_dxf)
+        self.disable_export_buttons(True)
+
         self.scaling_factor_line_edit.editingFinished.connect(self.update_sidebar)
         self.dpi_line_edit.editingFinished.connect(self.update_sidebar)
 
         layout = QtWidgets.QHBoxLayout()
         layout.setContentsMargins(0, 0, 0, 0)
 
         container = QtWidgets.QWidget()
@@ -174,76 +200,79 @@
 
         h_layout = QtWidgets.QHBoxLayout()
         h_layout.addWidget(QtWidgets.QLabel("DPI (PNG only):"))
         h_layout.addWidget(self.dpi_line_edit)
         v_layout.addLayout(h_layout)
         v_layout.addWidget(self.png_size_label)
 
-        export_png_button = QtWidgets.QPushButton("Export PNG")
-        export_png_button.clicked.connect(self.export_png)
-        export_png_button.setDisabled(True)
-        v_layout.addWidget(export_png_button)
-
-        export_svg_button = QtWidgets.QPushButton("Export SVG")
-        export_svg_button.clicked.connect(self.export_svg)
-        v_layout.addWidget(export_svg_button)
-
-        export_pdf_button = QtWidgets.QPushButton("Export PDF")
-        export_pdf_button.clicked.connect(self.export_pdf)
-        export_pdf_button.setDisabled(True)
-        v_layout.addWidget(export_pdf_button)
-
-        export_dxf_button = QtWidgets.QPushButton("Export DXF")
-        export_dxf_button.clicked.connect(self.export_dxf)
-        export_dxf_button.setDisabled(True)
-        v_layout.addWidget(export_dxf_button)
+        v_layout.addWidget(self.export_png_button)
+        v_layout.addWidget(self.export_svg_button)
+        v_layout.addWidget(self.export_pdf_button)
+
+        v_layout.addSpacing(SPACING)
+
+        v_layout.addWidget(self.aci_export_mode)
+        v_layout.addWidget(self.export_dxf_button)
 
         v_layout.addSpacing(SPACING)
 
         reset_button = QtWidgets.QPushButton("Reset")
         reset_button.clicked.connect(self.reset_values)
         v_layout.addWidget(reset_button)
 
         v_layout.addSpacing(SPACING)
 
         v_layout.addWidget(self.message_label)
         return sidebar
 
+    def disable_export_buttons(self, disabled: bool):
+        self.export_svg_button.setDisabled(disabled)
+        self.export_dxf_button.setDisabled(disabled)
+        if pymupdf.is_pymupdf_installed:
+            self.export_png_button.setDisabled(disabled)
+            self.export_pdf_button.setDisabled(disabled)
+        else:
+            print("PDF/PNG export requires the PyMuPdf package!")
+            self.export_png_button.setDisabled(True)
+            self.export_pdf_button.setDisabled(True)
+
     def load_plot_file(self, path: str | os.PathLike, force=False) -> None:
         try:
             with open(path, "rb") as fp:
                 data = fp.read()
             if force:
                 data = b"%1B" + data
             self.set_plot_data(data, path)
         except IOError as e:
             QtWidgets.QMessageBox.critical(self, "Loading Error", str(e))
 
     def select_plot_file(self) -> None:
         path, _ = QtWidgets.QFileDialog.getOpenFileName(
             self,
+            dir=str(self._current_file.parent),
             caption="Select HPGL/2 Plot File",
             filter="Plot Files (*.plt)",
         )
         if path:
             self.load_plot_file(path)
 
     def set_plot_data(self, data: bytes, filename: str | os.PathLike) -> None:
         try:
             self._cad.plot(data)
-        except api.Hpgl2Error:
-            # TODO: show MessageBox
-            msg = f"cannot load HPGL/2 file: {filename}"
-            print(msg)
+        except api.Hpgl2Error as e:
+            msg = f"Cannot plot HPGL/2 file '{filename}', {str(e)}"
+            QtWidgets.QMessageBox.critical(self, "Plot Error", msg)
             return
         self._player = self._cad.player
         self._bbox = self._player.bbox()
-        self.update_colors(self._color_schema)
+        self._current_file = pathlib.Path(filename)
+        self.update_colors(self._color_scheme)
         self.update_sidebar()
         self.setWindowTitle(f"{VIEWER_NAME} - " + str(filename))
+        self.disable_export_buttons(False)
 
     def resizeEvent(self, event: QtGui.QResizeEvent) -> None:
         self._view.fit_to_scene()
 
     def get_scale_factor(self) -> float:
         try:
             return float(self.scaling_factor_line_edit.text())
@@ -276,14 +305,17 @@
 
     def get_flip_x(self) -> bool:
         return self.flip_x_check_box.checkState() == QtCore.Qt.CheckState.Checked
 
     def get_flip_y(self) -> bool:
         return self.flip_y_check_box.checkState() == QtCore.Qt.CheckState.Checked
 
+    def get_aci_export_mode(self) -> bool:
+        return self.aci_export_mode.checkState() == QtCore.Qt.CheckState.Checked
+
     def update_sidebar(self):
         x, y = self.get_page_size()
         self.page_size_label.setText(f"Page Size: {x}x{y}mm")
         px, py = self.get_pixel_size()
         self.png_size_label.setText(f"PNG Size: {px}x{py}px")
         self.clear_message()
 
@@ -295,15 +327,15 @@
     def update_rotation(self, index: int):
         rotation = index * 90
         if rotation != self._page_rotation:
             self._page_rotation = rotation
             self.update_view()
 
     def update_colors(self, index: int):
-        self._color_schema = index
+        self._color_scheme = index
         self._cad.replay(*replay_properties(index))
         self.update_view()
 
     def view_transformation(self):
         if self._page_rotation == 0:
             m = Matrix44()
         else:
@@ -316,32 +348,32 @@
 
     def show_message(self, msg: str) -> None:
         self.message_label.setText(msg)
 
     def clear_message(self) -> None:
         self.message_label.setText("")
 
+    def get_export_name(self, suffix: str) -> str:
+        return str(self._current_file.with_suffix(suffix))
+
     def export_svg(self) -> None:
         path, _ = QtWidgets.QFileDialog.getSaveFileName(
             self,
+            dir=self.get_export_name(".svg"),
             caption="Save SVG File",
             filter="SVG Files (*.svg)",
         )
         if not path:
             return
         try:
-            t0 = time.perf_counter()
             with open(path, "wt") as fp:
                 fp.write(self.make_svg_string())
-            self.show_message(
-                f"SVG successfully in {time.perf_counter()-t0:.2f}s exported"
-            )
+            self.show_message("SVG successfully exported")
         except IOError as e:
-            # TODO: show MessageBox
-            print(str(e))
+            QMessageBox.critical(self, "Export Error", str(e))
 
     def get_export_matrix(self) -> Matrix44:
         scale = self.get_scale_factor()
         rotation = self._page_rotation
         sx = -scale if self.get_flip_x() else scale
         sy = -scale if self.get_flip_y() else scale
         if rotation in (90, 270):
@@ -353,31 +385,128 @@
 
     def make_svg_string(self) -> str:
         """Replays the HPGL/2 recordings on the SVGBackend of the drawing add-on."""
         player = self._player.copy()
         player.transform(self.get_export_matrix())
         size = player.bbox().size
         svg_backend = svg.SVGBackend()
-        bg_color, override = replay_properties(self._color_schema)
+        bg_color, override = replay_properties(self._color_scheme)
         xplayer.hpgl2_to_drawing(
             player, svg_backend, bg_color=bg_color, override=override
         )
         del player  # free memory as soon as possible
         # 40 plot units == 1mm
         page = layout.Page(width=size.x / 40, height=size.y / 40)
         return svg_backend.get_string(page)
 
     def export_pdf(self) -> None:
-        print("export HPGL/2 plot file as PDF")
+        path, _ = QtWidgets.QFileDialog.getSaveFileName(
+            self,
+            dir=self.get_export_name(".pdf"),
+            caption="Save PDF File",
+            filter="PDF Files (*.pdf)",
+        )
+        if not path:
+            return
+        try:
+            with open(path, "wb") as fp:
+                fp.write(self._pymupdf_export(fmt="pdf"))
+            self.show_message("PDF successfully exported")
+        except IOError as e:
+            QMessageBox.critical(self, "Export Error", str(e))
 
     def export_png(self) -> None:
-        print("export HPGL/2 plot file as PNG")
+        path, _ = QtWidgets.QFileDialog.getSaveFileName(
+            self,
+            dir=self.get_export_name(".png"),
+            caption="Save PNG File",
+            filter="PNG Files (*.png)",
+        )
+        if not path:
+            return
+        try:
+            with open(path, "wb") as fp:
+                fp.write(self._pymupdf_export(fmt="png"))
+            self.show_message("PNG successfully exported")
+        except IOError as e:
+            QMessageBox.critical(self, "Export Error", str(e))
+
+    def _pymupdf_export(self, fmt: str) -> bytes:
+        """Replays the HPGL/2 recordings on the PyMuPdfBackend of the drawing add-on."""
+        player = self._player.copy()
+        player.transform(self.get_export_matrix())
+        size = player.bbox().size
+        pdf_backend = pymupdf.PyMuPdfBackend()
+        bg_color, override = replay_properties(self._color_scheme)
+        xplayer.hpgl2_to_drawing(
+            player, pdf_backend, bg_color=bg_color, override=override
+        )
+        del player  # free memory as soon as possible
+        # 40 plot units == 1mm
+        page = layout.Page(width=size.x / 40, height=size.y / 40)
+        if fmt == "pdf":
+            return pdf_backend.get_pdf_bytes(page)
+        else:
+            return pdf_backend.get_pixmap_bytes(page, fmt=fmt, dpi=self.get_dpi())
 
     def export_dxf(self) -> None:
-        print("export HPGL/2 plot file as DXF")
+        path, _ = QtWidgets.QFileDialog.getSaveFileName(
+            self,
+            dir=self.get_export_name(".dxf"),
+            caption="Save DXF File",
+            filter="DXF Files (*.dxf)",
+        )
+        if not path:
+            return
+        doc = self._get_dxf_document()
+        try:
+            doc.saveas(path)
+            self.show_message("DXF successfully exported")
+        except IOError as e:
+            QMessageBox.critical(self, "Export Error", str(e))
+
+    def _get_dxf_document(self) -> Drawing:
+        import ezdxf
+        from ezdxf import zoom
+
+        color_mode = (
+            dxf.ColorMode.ACI if self.get_aci_export_mode() else dxf.ColorMode.RGB
+        )
+
+        doc = ezdxf.new()
+        msp = doc.modelspace()
+        player = self._player.copy()
+        bbox = player.bbox()
+
+        m = self.get_export_matrix()
+        corners = m.fast_2d_transform(bbox.rect_vertices())
+        # move content to origin:
+        tx, ty = BoundingBox2d(corners).extmin  # type: ignore
+        m @= Matrix44.translate(-tx, -ty, 0)
+        player.transform(m)
+        bbox = player.bbox()
+
+        dxf_backend = dxf.DXFBackend(msp, color_mode=color_mode)
+        bg_color, override = replay_properties(self._color_scheme)
+        if color_mode == dxf.ColorMode.RGB:
+            doc.layers.add("BACKGROUND")
+            bg = dxf.add_background(msp, bbox, colors.RGB.from_hex(bg_color))
+            bg.dxf.layer = "BACKGROUND"
+        # exports the HPGL/2 content in plot units (plu) as modelspace:
+        # 1 plu = 0.025mm or 40 plu == 1mm
+        xplayer.hpgl2_to_drawing(
+            player, dxf_backend, bg_color=bg_color, override=override
+        )
+        del player
+        if bbox.has_data:  # non-empty page
+            zoom.window(msp, bbox.extmin, bbox.extmax)
+            dxf.update_extents(doc, bbox)
+            # paperspace is set up in mm:
+            dxf.setup_paperspace(doc, bbox)
+        return doc
 
 
 def replay_properties(index: int) -> tuple[str, Any]:
     bg_color, override = "#ffffff", None  # default
     if index == 1:  # black on white
         bg_color, override = "#ffffff", xplayer.map_color("#000000")
     elif index == 2:  # white on black
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/acad_proxy_entity.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/point.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,128 +1,145 @@
-#  Copyright (c) 2021-2022, Manfred Moitzi
-#  License: MIT License
+# Copyright (c) 2019-2022 Manfred Moitzi
+# License: MIT License
 from __future__ import annotations
-from typing import TYPE_CHECKING, Optional, Iterator
-from ezdxf.lldxf import const
-from ezdxf.lldxf.tags import Tags
-from .dxfentity import SubclassProcessor
-from .dxfgfx import DXFGraphic
-from . import factory
+from typing import TYPE_CHECKING, Iterator, Optional
+from ezdxf.lldxf import validator
+from ezdxf.lldxf.attributes import (
+    DXFAttr,
+    DXFAttributes,
+    DefSubclass,
+    XType,
+    RETURN_DEFAULT,
+    group_code_mapping,
+    merge_group_code_mappings,
+)
+from ezdxf.lldxf.const import DXF12, SUBCLASS_MARKER
+from ezdxf.math import Vec3, Matrix44, NULLVEC, Z_AXIS, OCS
+from ezdxf.math.transformtools import (
+    transform_thickness_and_extrusion_without_ocs,
+)
+from .dxfentity import base_class, SubclassProcessor
+from .dxfgfx import DXFGraphic, acdb_entity, acdb_entity_group_codes
+from .factory import register_entity
 
 if TYPE_CHECKING:
-    from ezdxf.lldxf.tagwriter import AbstractTagWriter
     from ezdxf.entities import DXFNamespace
+    from ezdxf.lldxf.tagwriter import AbstractTagWriter
 
+__all__ = ["Point"]
 
-# Group Codes of AcDbProxyEntity
-# https://help.autodesk.com/view/OARX/2018/ENU/?guid=GUID-89A690F9-E859-4D57-89EA-750F3FB76C6B
-# 100 AcDbProxyEntity
-# 90  Proxy entity class ID (always 498)
-# 91  Application entity's class ID. Class IDs are based on the order of
-#     the class in the CLASSES section. The first class is given the ID of
-#     500, the next is 501, and so on
-#
-# 92  Size of graphics data in bytes < R2010; R2010+ = 160
-# 310 Binary graphics data (multiple entries can appear) (optional)
+# Point styling is a global setting, stored in the HEADER section as:
+# $PDMODE: https://knowledge.autodesk.com/support/autocad/learn-explore/caas/CloudHelp/cloudhelp/2019/ENU/AutoCAD-Core/files/GUID-82F9BB52-D026-4D6A-ABA6-BF29641F459B-htm.html
+# One of these values
+#   0 = center dot (.)
+#   1 = none ( )
+#   2 = cross (+)
+#   3 = x-cross (x)
+#   4 = tick (')
+# Combined with these bit values
+#  32 = circle
+#  64 = Square
 #
-# 96  Size of unknown data in bytes < R2010; R2010+ = 162
-# 311 Binary entity data (multiple entries can appear) (optional)
+# e.g. circle + square+center dot = 32 + 64 + 0 = 96
 #
-# 93  Size of entity data in bits <R2010; R2010+ = 161
-# 310 Binary entity data (multiple entries can appear) (optional)
-#
-# 330 or 340 or 350 or 360 - An object ID (multiple entries can appear) (optional)
-# 94  0 (indicates end of object ID section)
-# 95  Object drawing format when it becomes a proxy (a 32-bit unsigned integer):
-#     Low word is AcDbDwgVersion
-#     High word is MaintenanceReleaseVersion
-# 70  Original custom object data format:
-#     0 = DWG format
-#     1 = DXF format
-
-
-@factory.register_entity
-class ACADProxyEntity(DXFGraphic):
-    """READ ONLY ACAD_PROXY_ENTITY CLASS! DO NOT MODIFY!"""
-
-    DXFTYPE = "ACAD_PROXY_ENTITY"
-    MIN_DXF_VERSION_FOR_EXPORT = const.DXF2000
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.acdb_proxy_entity: Optional[Tags] = None
+# $PDSIZE: https://knowledge.autodesk.com/support/autocad/learn-explore/caas/CloudHelp/cloudhelp/2021/ENU/AutoCAD-Core/files/GUID-826CA91D-704B-400B-B784-7FCC9619AFB9-htm.html?st=$PDSIZE
+#  0 = 5% of draw area height
+# <0 = Specifies a percentage of the viewport size
+# >0 = Specifies an absolute size
+
+acdb_point = DefSubclass(
+    "AcDbPoint",
+    {
+        # Point location:
+        "location": DXFAttr(10, xtype=XType.point3d, default=NULLVEC),
+        # Thickness could be negative:
+        "thickness": DXFAttr(39, default=0, optional=True),
+        "extrusion": DXFAttr(
+            210,
+            xtype=XType.point3d,
+            default=Z_AXIS,
+            optional=True,
+            validator=validator.is_not_null_vector,
+            fixer=RETURN_DEFAULT,
+        ),
+        # angle of the x-axis for the UCS in effect when the point was drawn;
+        # used when PDMODE is nonzero:
+        "angle": DXFAttr(50, default=0, optional=True),
+    },
+)
+acdb_point_group_codes = group_code_mapping(acdb_point)
+merged_point_group_codes = merge_group_code_mappings(
+    acdb_entity_group_codes, acdb_point_group_codes  # type: ignore
+)
+
+
+@register_entity
+class Point(DXFGraphic):
+    """DXF POINT entity"""
 
-    def raw_copy(self):
-        raise const.DXFTypeError(f"Cloning of {self.dxftype()} not supported.")
+    DXFTYPE = "POINT"
+    DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_point)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
-        dxf = super().load_dxf_attribs(processor)
+        """Loading interface. (internal API)"""
+        # bypass DXFGraphic, loading proxy graphic is skipped!
+        dxf = super(DXFGraphic, self).load_dxf_attribs(processor)
         if processor:
-            self.acdb_proxy_entity = processor.subclass_by_index(2)
-            self.load_proxy_graphic(processor.dxfversion)
+            processor.simple_dxfattribs_loader(dxf, merged_point_group_codes)
         return dxf
 
-    def load_proxy_graphic(self, dxfversion: Optional[str]) -> None:
-        if self.acdb_proxy_entity is not None:
-            if not dxfversion:
-                dxfversion = _detect_dxf_version(self.acdb_proxy_entity)
-            length_code = 92 if dxfversion < const.DXF2013 else 160
-            self.proxy_graphic = load_proxy_data(
-                self.acdb_proxy_entity, length_code, 310
-            )
-
-    def export_dxf(self, tagwriter: AbstractTagWriter) -> None:
-        # Proxy graphic is stored in AcDbProxyEntity and not as usual in
-        # AcDbEntity!
-        preserve_proxy_graphic = self.proxy_graphic
-        self.proxy_graphic = None
-        super().export_dxf(tagwriter)
-        self.proxy_graphic = preserve_proxy_graphic
-
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags. (internal API)"""
-        # Base class and AcDbEntity export is done by parent class
         super().export_entity(tagwriter)
-        if self.acdb_proxy_entity is not None:
-            tagwriter.write_tags(self.acdb_proxy_entity)
-        # XDATA export is done by the parent class
-
-    def __virtual_entities__(self) -> Iterator[DXFGraphic]:
-        """Implements the SupportsVirtualEntities protocol."""
-        from ezdxf.proxygraphic import ProxyGraphic
-
-        if self.proxy_graphic:
-            for e in ProxyGraphic(
-                self.proxy_graphic, self.doc
-            ).virtual_entities():
-                e.set_source_of_copy(self)
-                yield e
-        return []
-
-    def virtual_entities(self) -> Iterator[DXFGraphic]:
-        """Yields proxy graphic as "virtual" entities."""
-        return self.__virtual_entities__()
-
-
-def load_proxy_data(
-    tags: Tags, length_code: int, data_code: int = 310
-) -> Optional[bytes]:
-    try:
-        index = tags.tag_index(length_code)
-    except const.DXFValueError:
-        return None
-    binary_data = []
-    for code, value in tags[index + 1 :]:
-        if code == data_code:
-            binary_data.append(value)
-        else:
-            break  # at first tag with group code != data_code
-    return b"".join(binary_data)
-
-
-def _detect_dxf_version(tags: Tags) -> str:
-    for tag in tags:
-        if 160 <= tag.code < 163:
-            return const.DXF2013
-    return const.DXF2000
+        if tagwriter.dxfversion > DXF12:
+            tagwriter.write_tag2(SUBCLASS_MARKER, acdb_point.name)
+        self.dxf.export_dxf_attribs(
+            tagwriter, ["location", "thickness", "extrusion", "angle"]
+        )
+
+    def transform(self, m: Matrix44) -> Point:
+        """Transform the POINT entity by transformation matrix `m` inplace."""
+        self.dxf.location = m.transform(self.dxf.location)
+        transform_thickness_and_extrusion_without_ocs(self, m)
+        # ignore dxf.angle!
+        self.post_transform(m)
+        return self
+
+    def translate(self, dx: float, dy: float, dz: float) -> Point:
+        """Optimized POINT translation about `dx` in x-axis, `dy` in y-axis and
+        `dz` in z-axis.
+        """
+        self.dxf.location = Vec3(dx, dy, dz) + self.dxf.location
+        # Avoid Matrix44 instantiation if not required:
+        if self.is_post_transform_required:
+            self.post_transform(Matrix44.translate(dx, dy, dz))
+        return self
+
+    def virtual_entities(
+        self, pdsize: float = 1, pdmode: int = 0
+    ) -> Iterator[DXFGraphic]:
+        """Yields the graphical representation of POINT as virtual DXF
+        primitives (LINE and CIRCLE).
+        The dimensionless point is rendered as zero-length line!
+
+        Check for this condition::
+
+            e.dxftype() == 'LINE' and e.dxf.start.isclose(e.dxf.end)
+
+        if the rendering engine can't handle zero-length lines.
+
+        Args:
+            pdsize: point size in drawing units
+            pdmode: point styling mode
+
+        """
+        from ezdxf.render import point
+        for e in point.virtual_entities(self, pdsize, pdmode):
+            e.set_source_of_copy(self)
+            yield e
+
+    def ocs(self) -> OCS:
+        # WCS entity which supports the "extrusion" attribute in a
+        # different way!
+        return OCS()
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/acad_table.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/acad_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/acis.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/appdata.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/appid.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/appid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/arc.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/attrib.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/block.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/blockrecord.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/blockrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/boundary_paths.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/circle.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dictionary.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dimension.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dimstyle.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dimstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dimstyleoverride.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dimstyleoverride.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dxfclass.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dxfentity.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dxfgfx.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dxfgroups.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dxfns.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dxfns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/dxfobj.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/ellipse.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/factory.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/geodata.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/geodata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/gradient.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/gradient.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,17 +44,17 @@
 
 
 class Gradient:
     def __init__(self, kind: int = 1, num: int = 2, type=GradientType.LINEAR):
         # 1 for gradient by default, 0 for Solid
         self.kind: int = kind
         self.number_of_colors: int = num
-        self.color1: RGB = (0, 0, 0)
+        self.color1: RGB = RGB(0, 0, 0)
         self.aci1: Optional[int] = None
-        self.color2: RGB = (255, 255, 255)
+        self.color2: RGB = RGB(255, 255, 255)
         self.aci2: Optional[int] = None
 
         # 1 = use a smooth transition between color1 and a specified tint
         self.one_color: int = 0
 
         # Use degree NOT radians for rotation, because there should be one
         # system for all angles:
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/hatch.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/hatch.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/helix.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/idbuffer.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/idbuffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/image.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/image.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/insert.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/layer.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/layout.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/leader.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/light.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/line.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/ltype.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/lwpolyline.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/lwpolyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/material.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/mesh.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/mleader.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/mline.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/mpolygon.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/mtext.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/mtext_columns.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/mtext_columns.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/objectcollection.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/objectcollection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/oleframe.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/oleframe.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/pattern.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/point.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/shape.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,145 +1,138 @@
 # Copyright (c) 2019-2022 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
-from typing import TYPE_CHECKING, Iterator, Optional
+from typing import TYPE_CHECKING, Optional
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
     RETURN_DEFAULT,
     group_code_mapping,
     merge_group_code_mappings,
 )
 from ezdxf.lldxf.const import DXF12, SUBCLASS_MARKER
-from ezdxf.math import Vec3, Matrix44, NULLVEC, Z_AXIS, OCS
-from ezdxf.math.transformtools import (
-    transform_thickness_and_extrusion_without_ocs,
-)
+from ezdxf.math import NULLVEC, Z_AXIS
+from ezdxf.math.transformtools import OCSTransform
 from .dxfentity import base_class, SubclassProcessor
-from .dxfgfx import DXFGraphic, acdb_entity, acdb_entity_group_codes
+from .dxfgfx import (
+    DXFGraphic,
+    acdb_entity,
+    elevation_to_z_axis,
+    acdb_entity_group_codes,
+)
 from .factory import register_entity
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
+    from ezdxf.math import Matrix44
+
 
-__all__ = ["Point"]
+__all__ = ["Shape"]
 
-# Point styling is a global setting, stored in the HEADER section as:
-# $PDMODE: https://knowledge.autodesk.com/support/autocad/learn-explore/caas/CloudHelp/cloudhelp/2019/ENU/AutoCAD-Core/files/GUID-82F9BB52-D026-4D6A-ABA6-BF29641F459B-htm.html
-# One of these values
-#   0 = center dot (.)
-#   1 = none ( )
-#   2 = cross (+)
-#   3 = x-cross (x)
-#   4 = tick (')
-# Combined with these bit values
-#  32 = circle
-#  64 = Square
-#
-# e.g. circle + square+center dot = 32 + 64 + 0 = 96
-#
-# $PDSIZE: https://knowledge.autodesk.com/support/autocad/learn-explore/caas/CloudHelp/cloudhelp/2021/ENU/AutoCAD-Core/files/GUID-826CA91D-704B-400B-B784-7FCC9619AFB9-htm.html?st=$PDSIZE
-#  0 = 5% of draw area height
-# <0 = Specifies a percentage of the viewport size
-# >0 = Specifies an absolute size
+# Description of the "name" attribute from the DWG documentation: 20.4.37 SHAPE (33)
+# In DXF the shape name is stored. When reading from DXF, the shape is found by
+# iterating over all the text styles and when the text style contains a shape file,
+# iterating over all the shapes until the one with the matching name is found.
 
-acdb_point = DefSubclass(
-    "AcDbPoint",
+acdb_shape = DefSubclass(
+    "AcDbShape",
     {
-        # Point location:
-        "location": DXFAttr(10, xtype=XType.point3d, default=NULLVEC),
+        # Elevation is a legacy feature from R11 and prior, do not use this
+        # attribute, store the entity elevation in the z-axis of the vertices.
+        # ezdxf does not export the elevation attribute!
+        "elevation": DXFAttr(38, default=0, optional=True),
         # Thickness could be negative:
         "thickness": DXFAttr(39, default=0, optional=True),
+        # Insertion point (in WCS)
+        "insert": DXFAttr(10, xtype=XType.point3d, default=NULLVEC),
+        # Shape size:
+        "size": DXFAttr(40, default=1),
+        # Shape name:
+        "name": DXFAttr(2, default=""),
+        # Rotation angle in degrees:
+        "rotation": DXFAttr(50, default=0, optional=True),
+        # Relative X scale factor
+        "xscale": DXFAttr(
+            41,
+            default=1,
+            optional=True,
+            validator=validator.is_not_zero,
+            fixer=RETURN_DEFAULT,
+        ),
+        # Oblique angle in degrees:
+        "oblique": DXFAttr(51, default=0, optional=True),
         "extrusion": DXFAttr(
             210,
             xtype=XType.point3d,
             default=Z_AXIS,
             optional=True,
             validator=validator.is_not_null_vector,
             fixer=RETURN_DEFAULT,
         ),
-        # angle of the x-axis for the UCS in effect when the point was drawn;
-        # used when PDMODE is nonzero:
-        "angle": DXFAttr(50, default=0, optional=True),
     },
 )
-acdb_point_group_codes = group_code_mapping(acdb_point)
-merged_point_group_codes = merge_group_code_mappings(
-    acdb_entity_group_codes, acdb_point_group_codes  # type: ignore
+acdb_shape_group_codes = group_code_mapping(acdb_shape)
+merged_shape_group_codes = merge_group_code_mappings(
+    acdb_entity_group_codes, acdb_shape_group_codes  # type: ignore
 )
 
 
 @register_entity
-class Point(DXFGraphic):
-    """DXF POINT entity"""
+class Shape(DXFGraphic):
+    """DXF SHAPE entity"""
 
-    DXFTYPE = "POINT"
-    DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_point)
+    DXFTYPE = "SHAPE"
+    DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_shape)
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         """Loading interface. (internal API)"""
         # bypass DXFGraphic, loading proxy graphic is skipped!
         dxf = super(DXFGraphic, self).load_dxf_attribs(processor)
         if processor:
-            processor.simple_dxfattribs_loader(dxf, merged_point_group_codes)
+            processor.simple_dxfattribs_loader(dxf, merged_shape_group_codes)
+            if processor.r12:
+                # Transform elevation attribute from R11 to z-axis values:
+                elevation_to_z_axis(dxf, ("center",))
         return dxf
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
-        """Export entity specific data as DXF tags. (internal API)"""
+        """Export entity specific data as DXF tags."""
         super().export_entity(tagwriter)
         if tagwriter.dxfversion > DXF12:
-            tagwriter.write_tag2(SUBCLASS_MARKER, acdb_point.name)
+            tagwriter.write_tag2(SUBCLASS_MARKER, acdb_shape.name)
         self.dxf.export_dxf_attribs(
-            tagwriter, ["location", "thickness", "extrusion", "angle"]
+            tagwriter,
+            [
+                "insert",
+                "size",
+                "name",
+                "thickness",
+                "rotation",
+                "xscale",
+                "oblique",
+                "extrusion",
+            ],
         )
 
-    def transform(self, m: Matrix44) -> Point:
-        """Transform the POINT entity by transformation matrix `m` inplace."""
-        self.dxf.location = m.transform(self.dxf.location)
-        transform_thickness_and_extrusion_without_ocs(self, m)
-        # ignore dxf.angle!
-        self.post_transform(m)
-        return self
+    def transform(self, m: Matrix44) -> Shape:
+        """Transform the SHAPE entity by transformation matrix `m` inplace."""
+        dxf = self.dxf
+        dxf.insert = m.transform(dxf.insert)  # DXF Reference: WCS?
+        ocs = OCSTransform(self.dxf.extrusion, m)
+
+        dxf.rotation = ocs.transform_deg_angle(dxf.rotation)
+        dxf.size = ocs.transform_length((0, dxf.size, 0))
+        dxf.x_scale = ocs.transform_length(
+            (dxf.x_scale, 0, 0), reflection=dxf.x_scale
+        )
+        if dxf.hasattr("thickness"):
+            dxf.thickness = ocs.transform_thickness(dxf.thickness)
 
-    def translate(self, dx: float, dy: float, dz: float) -> Point:
-        """Optimized POINT translation about `dx` in x-axis, `dy` in y-axis and
-        `dz` in z-axis.
-        """
-        self.dxf.location = Vec3(dx, dy, dz) + self.dxf.location
-        # Avoid Matrix44 instantiation if not required:
-        if self.is_post_transform_required:
-            self.post_transform(Matrix44.translate(dx, dy, dz))
+        dxf.extrusion = ocs.new_extrusion
+        self.post_transform(m)
         return self
-
-    def virtual_entities(
-        self, pdsize: float = 1, pdmode: int = 0
-    ) -> Iterator[DXFGraphic]:
-        """Yields the graphical representation of POINT as virtual DXF
-        primitives (LINE and CIRCLE).
-        The dimensionless point is rendered as zero-length line!
-
-        Check for this condition::
-
-            e.dxftype() == 'LINE' and e.dxf.start.isclose(e.dxf.end)
-
-        if the rendering engine can't handle zero-length lines.
-
-        Args:
-            pdsize: point size in drawing units
-            pdmode: point styling mode
-
-        """
-        from ezdxf.render import point
-        for e in point.virtual_entities(self, pdsize, pdmode):
-            e.set_source_of_copy(self)
-            yield e
-
-    def ocs(self) -> OCS:
-        # WCS entity which supports the "extrusion" attribute in a
-        # different way!
-        return OCS()
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/polygon.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/polygon.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
             xdata_bgcolor = self.get_xdata("HATCHBACKGROUNDCOLOR")
         except const.DXFValueError:
             return None
         color = xdata_bgcolor.get_first_value(1071, 0)
         try:
             return colors.int2rgb(int(color))  # type: ignore
         except ValueError:  # invalid data type
-            return 0, 0, 0
+            return RGB(0, 0, 0)
 
     @bgcolor.setter
     def bgcolor(self, rgb: RGB) -> None:
         color_value = (
             colors.rgb2int(rgb) | -0b111110000000000000000000000000
         )  # it's magic
 
@@ -204,16 +204,16 @@
 
     @bgcolor.deleter
     def bgcolor(self) -> None:
         self.discard_xdata("HATCHBACKGROUNDCOLOR")
 
     def set_gradient(
         self,
-        color1: RGB = (0, 0, 0),
-        color2: RGB = (255, 255, 255),
+        color1: RGB = RGB(0, 0, 0),
+        color2: RGB = RGB(255, 255, 255),
         rotation: float = 0.0,
         centered: float = 0.0,
         one_color: int = 0,
         tint: float = 0.0,
         name: str = "LINEAR",
     ) -> None:
         """Sets the gradient fill mode and removes all pattern fill related data, requires
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/polyline.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/shape.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/tolerance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,138 +1,104 @@
-# Copyright (c) 2019-2022 Manfred Moitzi
+# Copyright (c) 2019-2023 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
     RETURN_DEFAULT,
     group_code_mapping,
-    merge_group_code_mappings,
-)
-from ezdxf.lldxf.const import DXF12, SUBCLASS_MARKER
-from ezdxf.math import NULLVEC, Z_AXIS
-from ezdxf.math.transformtools import OCSTransform
-from .dxfentity import base_class, SubclassProcessor
-from .dxfgfx import (
-    DXFGraphic,
-    acdb_entity,
-    elevation_to_z_axis,
-    acdb_entity_group_codes,
 )
+from ezdxf.lldxf.const import SUBCLASS_MARKER, DXF2000
+from ezdxf.math import NULLVEC, Z_AXIS, X_AXIS
+from ezdxf.math.transformtools import transform_extrusion
+from .dxfentity import base_class, SubclassProcessor, DXFEntity
+from .dxfgfx import DXFGraphic, acdb_entity
 from .factory import register_entity
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
     from ezdxf.math import Matrix44
+    from ezdxf import xref
 
 
-__all__ = ["Shape"]
-
-# Description of the "name" attribute from the DWG documentation: 20.4.37 SHAPE (33)
-# In DXF the shape name is stored. When reading from DXF, the shape is found by
-# iterating over all the text styles and when the text style contains a shape file,
-# iterating over all the shapes until the one with the matching name is found.
+__all__ = ["Tolerance"]
 
-acdb_shape = DefSubclass(
-    "AcDbShape",
+acdb_tolerance = DefSubclass(
+    "AcDbFcf",
     {
-        # Elevation is a legacy feature from R11 and prior, do not use this
-        # attribute, store the entity elevation in the z-axis of the vertices.
-        # ezdxf does not export the elevation attribute!
-        "elevation": DXFAttr(38, default=0, optional=True),
-        # Thickness could be negative:
-        "thickness": DXFAttr(39, default=0, optional=True),
-        # Insertion point (in WCS)
-        "insert": DXFAttr(10, xtype=XType.point3d, default=NULLVEC),
-        # Shape size:
-        "size": DXFAttr(40, default=1),
-        # Shape name:
-        "name": DXFAttr(2, default=""),
-        # Rotation angle in degrees:
-        "rotation": DXFAttr(50, default=0, optional=True),
-        # Relative X scale factor
-        "xscale": DXFAttr(
-            41,
-            default=1,
-            optional=True,
-            validator=validator.is_not_zero,
-            fixer=RETURN_DEFAULT,
+        "dimstyle": DXFAttr(
+            3,
+            default="Standard",
+            validator=validator.is_valid_table_name,
         ),
-        # Oblique angle in degrees:
-        "oblique": DXFAttr(51, default=0, optional=True),
+        # Insertion point (in WCS):
+        "insert": DXFAttr(10, xtype=XType.point3d, default=NULLVEC),
+        # String representing the visual representation of the tolerance:
+        "content": DXFAttr(1, default=""),
         "extrusion": DXFAttr(
             210,
             xtype=XType.point3d,
             default=Z_AXIS,
             optional=True,
             validator=validator.is_not_null_vector,
             fixer=RETURN_DEFAULT,
         ),
+        # X-axis direction vector (in WCS):
+        "x_axis_vector": DXFAttr(
+            11,
+            xtype=XType.point3d,
+            default=X_AXIS,
+            validator=validator.is_not_null_vector,
+            fixer=RETURN_DEFAULT,
+        ),
     },
 )
-acdb_shape_group_codes = group_code_mapping(acdb_shape)
-merged_shape_group_codes = merge_group_code_mappings(
-    acdb_entity_group_codes, acdb_shape_group_codes  # type: ignore
-)
+acdb_tolerance_group_codes = group_code_mapping(acdb_tolerance)
 
 
 @register_entity
-class Shape(DXFGraphic):
-    """DXF SHAPE entity"""
+class Tolerance(DXFGraphic):
+    """DXF TOLERANCE entity"""
 
-    DXFTYPE = "SHAPE"
-    DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_shape)
+    DXFTYPE = "TOLERANCE"
+    DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_tolerance)
+    MIN_DXF_VERSION_FOR_EXPORT = DXF2000
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
-        """Loading interface. (internal API)"""
-        # bypass DXFGraphic, loading proxy graphic is skipped!
-        dxf = super(DXFGraphic, self).load_dxf_attribs(processor)
+        dxf = super().load_dxf_attribs(processor)
         if processor:
-            processor.simple_dxfattribs_loader(dxf, merged_shape_group_codes)
-            if processor.r12:
-                # Transform elevation attribute from R11 to z-axis values:
-                elevation_to_z_axis(dxf, ("center",))
+            processor.fast_load_dxfattribs(
+                dxf, acdb_tolerance_group_codes, subclass=2, recover=True
+            )
         return dxf
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         super().export_entity(tagwriter)
-        if tagwriter.dxfversion > DXF12:
-            tagwriter.write_tag2(SUBCLASS_MARKER, acdb_shape.name)
+        tagwriter.write_tag2(SUBCLASS_MARKER, acdb_tolerance.name)
         self.dxf.export_dxf_attribs(
             tagwriter,
-            [
-                "insert",
-                "size",
-                "name",
-                "thickness",
-                "rotation",
-                "xscale",
-                "oblique",
-                "extrusion",
-            ],
-        )
-
-    def transform(self, m: Matrix44) -> Shape:
-        """Transform the SHAPE entity by transformation matrix `m` inplace."""
-        dxf = self.dxf
-        dxf.insert = m.transform(dxf.insert)  # DXF Reference: WCS?
-        ocs = OCSTransform(self.dxf.extrusion, m)
-
-        dxf.rotation = ocs.transform_deg_angle(dxf.rotation)
-        dxf.size = ocs.transform_length((0, dxf.size, 0))
-        dxf.x_scale = ocs.transform_length(
-            (dxf.x_scale, 0, 0), reflection=dxf.x_scale
+            ["dimstyle", "insert", "content", "extrusion", "x_axis_vector"],
         )
-        if dxf.hasattr("thickness"):
-            dxf.thickness = ocs.transform_thickness(dxf.thickness)
 
-        dxf.extrusion = ocs.new_extrusion
+    def register_resources(self, registry: xref.Registry) -> None:
+        super().register_resources(registry)
+        registry.add_dim_style(self.dxf.dimstyle)
+
+    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
+        super().map_resources(clone, mapping)
+        clone.dxf.dimstyle = mapping.get_dim_style(self.dxf.dimstyle)
+
+    def transform(self, m: Matrix44) -> Tolerance:
+        """Transform the TOLERANCE entity by transformation matrix `m` inplace."""
+        self.dxf.insert = m.transform(self.dxf.insert)
+        self.dxf.x_axis_vector = m.transform_direction(self.dxf.x_axis_vector)
+        self.dxf.extrusion, _ = transform_extrusion(self.dxf.extrusion, m)
         self.post_transform(m)
         return self
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/solid.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/spline.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/subentity.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/subentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/sun.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/table.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/text.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/textstyle.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/textstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/tolerance.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/xline.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,104 +1,95 @@
-# Copyright (c) 2019-2023 Manfred Moitzi
+# Copyright (c) 2019-2022 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Optional
 from ezdxf.lldxf import validator
 from ezdxf.lldxf.attributes import (
     DXFAttr,
     DXFAttributes,
     DefSubclass,
     XType,
     RETURN_DEFAULT,
     group_code_mapping,
 )
 from ezdxf.lldxf.const import SUBCLASS_MARKER, DXF2000
-from ezdxf.math import NULLVEC, Z_AXIS, X_AXIS
-from ezdxf.math.transformtools import transform_extrusion
-from .dxfentity import base_class, SubclassProcessor, DXFEntity
+from ezdxf.math import Vec3, Matrix44, NULLVEC, Z_AXIS
+from .dxfentity import base_class, SubclassProcessor
 from .dxfgfx import DXFGraphic, acdb_entity
 from .factory import register_entity
 
 if TYPE_CHECKING:
     from ezdxf.entities import DXFNamespace
     from ezdxf.lldxf.tagwriter import AbstractTagWriter
-    from ezdxf.math import Matrix44
-    from ezdxf import xref
 
+__all__ = ["Ray", "XLine"]
 
-__all__ = ["Tolerance"]
-
-acdb_tolerance = DefSubclass(
-    "AcDbFcf",
+acdb_xline = DefSubclass(
+    "AcDbXline",
     {
-        "dimstyle": DXFAttr(
-            3,
-            default="Standard",
-            validator=validator.is_valid_table_name,
-        ),
-        # Insertion point (in WCS):
-        "insert": DXFAttr(10, xtype=XType.point3d, default=NULLVEC),
-        # String representing the visual representation of the tolerance:
-        "content": DXFAttr(1, default=""),
-        "extrusion": DXFAttr(
-            210,
-            xtype=XType.point3d,
-            default=Z_AXIS,
-            optional=True,
-            validator=validator.is_not_null_vector,
-            fixer=RETURN_DEFAULT,
-        ),
-        # X-axis direction vector (in WCS):
-        "x_axis_vector": DXFAttr(
+        "start": DXFAttr(10, xtype=XType.point3d, default=NULLVEC),
+        "unit_vector": DXFAttr(
             11,
             xtype=XType.point3d,
-            default=X_AXIS,
+            default=Z_AXIS,
             validator=validator.is_not_null_vector,
             fixer=RETURN_DEFAULT,
         ),
     },
 )
-acdb_tolerance_group_codes = group_code_mapping(acdb_tolerance)
+acdb_xline_group_codes = group_code_mapping(acdb_xline)
 
 
 @register_entity
-class Tolerance(DXFGraphic):
-    """DXF TOLERANCE entity"""
+class XLine(DXFGraphic):
+    """DXF XLINE entity"""
 
-    DXFTYPE = "TOLERANCE"
-    DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_tolerance)
+    DXFTYPE = "XLINE"
+    DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_xline)
     MIN_DXF_VERSION_FOR_EXPORT = DXF2000
+    XLINE_SUBCLASS = "AcDbXline"
 
     def load_dxf_attribs(
         self, processor: Optional[SubclassProcessor] = None
     ) -> DXFNamespace:
         dxf = super().load_dxf_attribs(processor)
         if processor:
             processor.fast_load_dxfattribs(
-                dxf, acdb_tolerance_group_codes, subclass=2, recover=True
+                dxf, acdb_xline_group_codes, subclass=2, recover=True
             )
         return dxf
 
     def export_entity(self, tagwriter: AbstractTagWriter) -> None:
         """Export entity specific data as DXF tags."""
         super().export_entity(tagwriter)
-        tagwriter.write_tag2(SUBCLASS_MARKER, acdb_tolerance.name)
-        self.dxf.export_dxf_attribs(
-            tagwriter,
-            ["dimstyle", "insert", "content", "extrusion", "x_axis_vector"],
-        )
-
-    def register_resources(self, registry: xref.Registry) -> None:
-        super().register_resources(registry)
-        registry.add_dim_style(self.dxf.dimstyle)
-
-    def map_resources(self, clone: DXFEntity, mapping: xref.ResourceMapper) -> None:
-        super().map_resources(clone, mapping)
-        clone.dxf.dimstyle = mapping.get_dim_style(self.dxf.dimstyle)
-
-    def transform(self, m: Matrix44) -> Tolerance:
-        """Transform the TOLERANCE entity by transformation matrix `m` inplace."""
-        self.dxf.insert = m.transform(self.dxf.insert)
-        self.dxf.x_axis_vector = m.transform_direction(self.dxf.x_axis_vector)
-        self.dxf.extrusion, _ = transform_extrusion(self.dxf.extrusion, m)
+        tagwriter.write_tag2(SUBCLASS_MARKER, self.XLINE_SUBCLASS)
+        self.dxf.export_dxf_attribs(tagwriter, ["start", "unit_vector"])
+
+    def transform(self, m: Matrix44) -> XLine:
+        """Transform the XLINE/RAY entity by transformation matrix `m` inplace."""
+        self.dxf.start = m.transform(self.dxf.start)
+        self.dxf.unit_vector = m.transform_direction(
+            self.dxf.unit_vector
+        ).normalize()
         self.post_transform(m)
         return self
+
+    def translate(self, dx: float, dy: float, dz: float) -> XLine:
+        """Optimized XLINE/RAY translation about `dx` in x-axis, `dy` in
+        y-axis and `dz` in z-axis.
+
+        """
+        self.dxf.start = Vec3(dx, dy, dz) + self.dxf.start
+        # Avoid Matrix44 instantiation if not required:
+        if self.is_post_transform_required:
+            self.post_transform(Matrix44.translate(dx, dy, dz))
+        return self
+
+
+@register_entity
+class Ray(XLine):
+    """DXF Ray entity"""
+
+    DXFTYPE = "RAY"
+    DXFATTRIBS = DXFAttributes(base_class, acdb_entity, acdb_xline)
+    MIN_DXF_VERSION_FOR_EXPORT = DXF2000
+    XLINE_SUBCLASS = "AcDbRay"
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/ucs.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/underlay.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/view.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/view.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/viewport.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/viewport.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,24 +58,25 @@
         # Height in paper space units:
         "height": DXFAttr(41, default=1),
         # Viewport status field: (according to the DXF Reference)
         # -1 = On, but is fully off-screen, or is one of the viewports that is not
         #      active because the $MAXACTVP count is currently being exceeded.
         #  0 = Off
         # <positive value> = On and active. The value indicates the order of
-        # stacking for the viewports, where 1 is the "active viewport", 2 is the
-        # next, and so on:
+        # stacking for the viewports, where 1 is the "active" viewport, 2 is the
+        # next, and so on. The "active" viewport determines how the paperspace layout
+        # is presented as a whole (location & zoom state)
         "status": DXFAttr(68, default=0),
         # Viewport id: (according to the DXF Reference)
         # Special VIEWPORT id == 1, this viewport defines the area of the layout
         # which is currently shown in the layout tab by the CAD application.
         # I guess this is meant by "active viewport" and therefore it is most likely
         # that this id is always 1.
         # This "active viewport" is mandatory for a valid DXF file.
-        # BricsCAD set id to -1 if the viewport is off and 'status' (group code 68)
+        # BricsCAD set this id to -1 if the viewport is off and 'status' (group code 68)
         # is not present.
         "id": DXFAttr(69, default=2),
         # DXF reference: View center point (in WCS):
         # Correction to the DXF reference:
         # This point represents the center point in model space (WCS) stored as
         # 2D point!
         "view_center_point": DXFAttr(12, xtype=XType.point2d, default=NULLVEC),
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/visualstyle.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/visualstyle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/vport.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/vport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/xdata.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/xdict.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/xdict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/entities/__init__.py` & `ezdxf-1.1.0b3/src/ezdxf/entities/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/fonts/fonts.py` & `ezdxf-1.1.0b3/src/ezdxf/fonts/fonts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #  Copyright (c) 2021-2023, Manfred Moitzi
 #  License: MIT License
 from __future__ import annotations
 from typing import Optional, TYPE_CHECKING, cast
 import abc
 import enum
 import logging
+import os
 import sys
 import pathlib
 
 from ezdxf import options
 from .font_face import FontFace
 from .font_manager import (
     FontManager,
@@ -309,14 +310,15 @@
     try:
         cache_file.write_text(s)
     except IOError as e:
         print(f"Error writing cache file: {str(e)}")
 
 
 def build_font_manager_cache(path: pathlib.Path) -> None:
+    font_manager.clear()
     font_manager.build()
     s = font_manager.dumps()
     if not path.parent.exists():
         path.parent.mkdir(parents=True)
     try:
         path.write_text(s)
     except IOError as e:
@@ -492,14 +494,21 @@
         and `width_factor`."""
         return self.glyph_cache.get_text_path(text, cap_height, width_factor)
 
     def space_width(self) -> float:
         """Returns the width of a "space" char."""
         return self._space_width
 
+# --------------------------------------------------------------------------------------
+# NOTES:
+# "romantic.ttf" uses the Private Use Area (PUA) codepoints (f000-e000) for its glyphs
+# and has no glyphs for the usual code points.
+# see example: "CADKitSamples\Proposed Townhouse.dxf"
+# I deleted this font from my system!
+
 
 class TrueTypeFont(_CachedFont):
     """Represents a TrueType font. Font measurement and glyph rendering is done by the
     `fontTools` package. The given cap height and width factor are the default values
     for measurements and glyph rendering. The extended methods can override these
     default values.
     """
@@ -520,14 +529,44 @@
             fallback_font_name = font_manager.fallback_font_name()
             logger.info(f"replacing unsupported font '{ttf}' by '{fallback_font_name}'")
             cache = TTFontRenderer(font_manager.get_ttf_font(fallback_font_name))
         self._glyph_caches[key] = cache
         return cache
 
 
+class _UnmanagedTrueTypeFont(_CachedFont):
+    font_render_type = FontRenderType.OUTLINE
+
+    def create_cache(self, ttf: str) -> Glyphs:
+        from .ttfonts import TTFontRenderer
+        from fontTools.ttLib import TTFont
+
+        key = ttf.lower()
+        try:
+            return self._glyph_caches[key]
+        except KeyError:
+            pass
+        cache = TTFontRenderer(TTFont(ttf, fontNumber=0))
+        self._glyph_caches[key] = cache
+        return cache
+
+
+def sideload_ttf(font_path: str | os.PathLike, cap_height) -> AbstractFont:
+    """This function bypasses the FontManager and loads the TrueType font straight from
+    the file system, requires the absolute font file path e.g. "C:/Windows/Fonts/Arial.ttf".
+
+    .. warning::
+
+        Expert feature, use with care: no fallback font and no error handling.
+
+    """
+
+    return _UnmanagedTrueTypeFont(str(font_path), cap_height)
+
+
 class ShapeFileFont(_CachedFont):
     """Represents a shapefile font (.shx, .shp). Font measurement and glyph rendering is
     done by the ezdxf.fonts.shapefile module. The given cap height and width factor are
     the default values for measurements and glyph rendering. The extended methods can
     override these default values.
 
     """
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/fonts/font_face.py` & `ezdxf-1.1.0b3/src/ezdxf/fonts/font_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/fonts/font_manager.py` & `ezdxf-1.1.0b3/src/ezdxf/fonts/font_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/fonts/font_measurements.py` & `ezdxf-1.1.0b3/src/ezdxf/fonts/font_measurements.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/fonts/glyphs.py` & `ezdxf-1.1.0b3/src/ezdxf/fonts/glyphs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/fonts/lff.py` & `ezdxf-1.1.0b3/src/ezdxf/fonts/lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/fonts/shapefile.py` & `ezdxf-1.1.0b3/src/ezdxf/fonts/shapefile.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/fonts/ttfonts.py` & `ezdxf-1.1.0b3/src/ezdxf/fonts/ttfonts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/layouts/base.py` & `ezdxf-1.1.0b3/src/ezdxf/layouts/base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/layouts/blocklayout.py` & `ezdxf-1.1.0b3/src/ezdxf/layouts/blocklayout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/layouts/layout.py` & `ezdxf-1.1.0b3/src/ezdxf/layouts/layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -410,16 +410,15 @@
         :meth:`~ezdxf.layouts.Layouts` class to rename paper space
         layouts.
 
         """
         self.dxf_layout.dxf.name = name
 
     def viewports(self) -> list[Viewport]:
-        """Get all VIEWPORT entities defined in this paperspace layout.
-        """
+        """Get all VIEWPORT entities defined in this paperspace layout."""
         return [e for e in self if e.is_alive and e.dxftype() == "VIEWPORT"]  # type: ignore
 
     def main_viewport(self) -> Optional[Viewport]:
         """Returns the main viewport of this paper space layout, or ``None``
         if no main viewport exist.
 
         """
@@ -430,24 +429,36 @@
 
     def add_viewport(
         self,
         center: UVec,
         size: tuple[float, float],
         view_center_point: UVec,
         view_height: float,
+        status: int = 2,
         dxfattribs=None,
     ) -> Viewport:
-        """Add a new :class:`~ezdxf.entities.Viewport` entity."""
+        """Add a new :class:`~ezdxf.entities.Viewport` entity.
+
+        Viewport :attr:`status`:
+
+            - -1 is on, but is fully off-screen, or is one of the viewports that is not
+              active because the $MAXACTVP count is currently being exceeded.
+            - 0 is off
+            - any value>0 is on and active. The value indicates the order of
+              stacking for the viewports, where 1 is the "active viewport", 2 is the
+              next, ...
+
+        """
         dxfattribs = dxfattribs or {}
         width, height = size
         attribs = {
             "center": center,  # center in paperspace
             "width": width,  # width in paperspace
             "height": height,  # height in paperspace
-            "status": 1,  # has by default the highest priority (stack order)
+            "status": status,
             "layer": "VIEWPORTS",
             # use separated layer to turn off for plotting
             "view_center_point": view_center_point,  # in modelspace
             "view_height": view_height,  # in modelspace
         }
         attribs.update(dxfattribs)
         viewport = cast("Viewport", self.new_entity("VIEWPORT", attribs))
@@ -542,14 +553,15 @@
         vp_height = size[1]
         # create 'main' viewport
         main_viewport = self.add_viewport(
             center=center,  # no influence to 'main' viewport?
             size=size,  # I don't get it, just use paper size!
             view_center_point=center,  # same as center
             view_height=vp_height,  # view height in paper space units
+            status=1,  # main viewport
         )
         if len(self.entity_space) > 1:
             # move main viewport to index 0 of entity space
             _vp = self.entity_space.pop()
             assert _vp is main_viewport
             self.entity_space.insert(0, main_viewport)
 
@@ -766,17 +778,17 @@
 
         # create 'main' viewport
         main_viewport = self.add_viewport(
             center=center,  # no influence to 'main' viewport?
             size=(vp_width, vp_height),  # I don't get it, just use paper size!
             view_center_point=center,  # same as center
             view_height=vp_height,  # view height in paper space units
+            status=1,  # main viewport
         )
         main_viewport.dxf.id = 1  # set as main viewport
-        main_viewport.dxf.status = 2  # AutoCAD default value
         main_viewport.dxf.render_mode = 1000  # AutoDesk default (view mode?)
 
     def get_paper_limits_r12(self) -> tuple[Vec2, Vec2]:
         """Returns paper limits in plot paper units."""
         limmin = self.doc.header.get("$PLIMMIN", (0, 0))
         limmax = self.doc.header.get("$PLIMMAX", (0, 0))
         return Vec2(limmin), Vec2(limmax)
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/layouts/layouts.py` & `ezdxf-1.1.0b3/src/ezdxf/layouts/layouts.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/attributes.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/const.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/const.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/encoding.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/extendedtags.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/extendedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/fileindex.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/fileindex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/hdrvars.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/hdrvars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/loader.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/packedtags.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/packedtags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/repair.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/repair.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/tagger.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/tagger.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/tags.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/tagwriter.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/tagwriter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/types.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/lldxf/validator.py` & `ezdxf-1.1.0b3/src/ezdxf/lldxf/validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/arc.py` & `ezdxf-1.1.0b3/src/ezdxf/math/arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/bbox.py` & `ezdxf-1.1.0b3/src/ezdxf/math/bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/bezier.py` & `ezdxf-1.1.0b3/src/ezdxf/math/bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/bezier_interpolation.py` & `ezdxf-1.1.0b3/src/ezdxf/math/bezier_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/box.py` & `ezdxf-1.1.0b3/src/ezdxf/math/box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/bspline.py` & `ezdxf-1.1.0b3/src/ezdxf/math/bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/bulge.py` & `ezdxf-1.1.0b3/src/ezdxf/math/bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/circle.py` & `ezdxf-1.1.0b3/src/ezdxf/math/circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/clipping.py` & `ezdxf-1.1.0b3/src/ezdxf/math/clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/clustering.py` & `ezdxf-1.1.0b3/src/ezdxf/math/clustering.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/construct2d.py` & `ezdxf-1.1.0b3/src/ezdxf/math/construct2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/construct3d.py` & `ezdxf-1.1.0b3/src/ezdxf/math/construct3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/cspline.py` & `ezdxf-1.1.0b3/src/ezdxf/math/cspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/curvetools.py` & `ezdxf-1.1.0b3/src/ezdxf/math/curvetools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/ellipse.py` & `ezdxf-1.1.0b3/src/ezdxf/math/ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/eulerspiral.py` & `ezdxf-1.1.0b3/src/ezdxf/math/eulerspiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/linalg.py` & `ezdxf-1.1.0b3/src/ezdxf/math/linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/line.py` & `ezdxf-1.1.0b3/src/ezdxf/math/line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/offset2d.py` & `ezdxf-1.1.0b3/src/ezdxf/math/offset2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/parametrize.py` & `ezdxf-1.1.0b3/src/ezdxf/math/parametrize.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/perlin.py` & `ezdxf-1.1.0b3/src/ezdxf/math/perlin.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/polyline.py` & `ezdxf-1.1.0b3/src/ezdxf/math/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/rtree.py` & `ezdxf-1.1.0b3/src/ezdxf/math/rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/shape.py` & `ezdxf-1.1.0b3/src/ezdxf/math/shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/surfaces.py` & `ezdxf-1.1.0b3/src/ezdxf/math/surfaces.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/transformtools.py` & `ezdxf-1.1.0b3/src/ezdxf/math/transformtools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/triangulation.py` & `ezdxf-1.1.0b3/src/ezdxf/math/triangulation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/ucs.py` & `ezdxf-1.1.0b3/src/ezdxf/math/ucs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# Copyright (c) 2018-2022 Manfred Moitzi
+# Copyright (c) 2018-2023 Manfred Moitzi
 # License: MIT License
 from __future__ import annotations
 from typing import TYPE_CHECKING, Sequence, Iterable, Optional
 from ezdxf.math import Vec3, UVec, X_AXIS, Y_AXIS, Z_AXIS, Matrix44
+from ezdxf.colors import RGB
 
 if TYPE_CHECKING:
     from ezdxf.layouts import BaseLayout
-    from ezdxf.colors import RGB
 
 __all__ = ["OCS", "UCS", "PassTroughUCS"]
 
 
 def render_axis(
     layout: BaseLayout,
     start: UVec,
     points: Sequence[UVec],
-    colors: RGB = (1, 3, 5),
+    colors: RGB = RGB(1, 3, 5),
 ) -> None:
     for point, color in zip(points, colors):
         layout.add_line(start, point, dxfattribs={"color": color})
 
 
 _1_OVER_64 = 1.0 / 64.0
 
@@ -91,15 +91,15 @@
         else:
             yield from points
 
     def render_axis(
         self,
         layout: BaseLayout,
         length: float = 1,
-        colors: RGB = (1, 3, 5),
+        colors: RGB = RGB(1, 3, 5),
     ) -> None:
         """Render axis as 3D lines into a `layout`."""
         render_axis(
             layout,
             start=(0, 0, 0),
             points=(
                 self.to_wcs(X_AXIS * length),
@@ -464,15 +464,15 @@
         x_axis = yz_vector.cross(z_axis)
         return UCS(origin=origin, ux=x_axis, uz=z_axis)
 
     def render_axis(
         self,
         layout: BaseLayout,
         length: float = 1,
-        colors: RGB = (1, 3, 5),
+        colors: RGB = RGB(1, 3, 5),
     ):
         """Render axis as 3D lines into a `layout`."""
         render_axis(
             layout,
             start=self.origin,
             points=(
                 self.to_wcs(X_AXIS * length),
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/_bezier3p.py` & `ezdxf-1.1.0b3/src/ezdxf/math/_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/_bezier4p.py` & `ezdxf-1.1.0b3/src/ezdxf/math/_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/_bspline.py` & `ezdxf-1.1.0b3/src/ezdxf/math/_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/_construct.py` & `ezdxf-1.1.0b3/src/ezdxf/math/_construct.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/_ctypes.py` & `ezdxf-1.1.0b3/src/ezdxf/math/_ctypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/_mapbox_earcut.py` & `ezdxf-1.1.0b3/src/ezdxf/math/_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/_matrix44.py` & `ezdxf-1.1.0b3/src/ezdxf/math/_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/_vector.py` & `ezdxf-1.1.0b3/src/ezdxf/math/_vector.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/math/__init__.py` & `ezdxf-1.1.0b3/src/ezdxf/math/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/path/commands.py` & `ezdxf-1.1.0b3/src/ezdxf/path/commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/path/converter.py` & `ezdxf-1.1.0b3/src/ezdxf/path/converter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/path/nesting.py` & `ezdxf-1.1.0b3/src/ezdxf/path/nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/path/path.py` & `ezdxf-1.1.0b3/src/ezdxf/path/path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/path/shapes.py` & `ezdxf-1.1.0b3/src/ezdxf/path/shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/path/tools.py` & `ezdxf-1.1.0b3/src/ezdxf/path/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
         paths: iterable of :class:`Path` or :class:`Path2d` objects
         m: transformation matrix of type :class:`~ezdxf.math.Matrix44`
 
     """
     return [p.transform(m) for p in paths]
 
 
-def transform_paths_to_ocs(paths: Iterable[Path|Path2d], ocs: OCS) -> list[Path]:
+def transform_paths_to_ocs(paths: Iterable[Path | Path2d], ocs: OCS) -> list[Path]:
     """Transform multiple :class:`Path` objects at once from WCS to OCS.
     Returns a list of the transformed :class:`Path` objects.
 
     Args:
         paths: iterable of :class:`Path` or :class:`Path2d` objects
         ocs: OCS transformation of type :class:`~ezdxf.math.OCS`
 
@@ -268,15 +268,15 @@
 
 
 # Path to entity converter and render utilities:
 
 
 def render_lwpolylines(
     layout: GenericLayoutType,
-    paths: Iterable[Path|Path2d],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
@@ -310,15 +310,15 @@
     for lwpolyline in lwpolylines:
         layout.add_entity(lwpolyline)
     return EntityQuery(lwpolylines)
 
 
 def render_polylines2d(
     layout: GenericLayoutType,
-    paths: Iterable[Path|Path2d],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = 0.01,
     segments: int = 4,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as 2D
@@ -352,15 +352,15 @@
     for polyline2d in polylines2d:
         layout.add_entity(polyline2d)
     return EntityQuery(polylines2d)
 
 
 def render_hatches(
     layout: GenericLayoutType,
-    paths: Iterable[Path|Path2d],
+    paths: Iterable[Path | Path2d],
     *,
     edge_path: bool = True,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     g1_tol: float = G1_TOL,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
@@ -401,15 +401,15 @@
     for hatch in hatches:
         layout.add_entity(hatch)
     return EntityQuery(hatches)
 
 
 def render_mpolygons(
     layout: GenericLayoutType,
-    paths: Iterable[Path|Path2d],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     extrusion: UVec = Z_AXIS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
@@ -445,15 +445,15 @@
     for polygon in polygons:
         layout.add_entity(polygon)
     return EntityQuery(polygons)
 
 
 def render_polylines3d(
     layout: GenericLayoutType,
-    paths: Iterable[Path|Path2d],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as 3D
     :class:`~ezdxf.entities.Polyline` entities.
@@ -481,15 +481,15 @@
     for polyline3d in polylines3d:
         layout.add_entity(polyline3d)
     return EntityQuery(polylines3d)
 
 
 def render_lines(
     layout: GenericLayoutType,
-    paths: Iterable[Path|Path2d],
+    paths: Iterable[Path | Path2d],
     *,
     distance: float = MAX_DISTANCE,
     segments: int = MIN_SEGMENTS,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as
     :class:`~ezdxf.entities.Line` entities.
@@ -516,15 +516,15 @@
     for line in lines:
         layout.add_entity(line)
     return EntityQuery(lines)
 
 
 def render_splines_and_polylines(
     layout: GenericLayoutType,
-    paths: Iterable[Path|Path2d],
+    paths: Iterable[Path | Path2d],
     *,
     g1_tol: float = G1_TOL,
     dxfattribs=None,
 ) -> EntityQuery:
     """Render the given `paths` into `layout` as :class:`~ezdxf.entities.Spline`
     and 3D :class:`~ezdxf.entities.Polyline` entities.
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.css` & `ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.html` & `ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.html`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.js` & `ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.js`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/pp/dxfpp.py` & `ezdxf-1.1.0b3/src/ezdxf/pp/dxfpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/pp/pprint.py` & `ezdxf-1.1.0b3/src/ezdxf/pp/pprint.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.css` & `ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.css`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/pp/rawpp.py` & `ezdxf-1.1.0b3/src/ezdxf/pp/rawpp.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/pp/reflinks.py` & `ezdxf-1.1.0b3/src/ezdxf/pp/reflinks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/abstract_mtext_renderer.py` & `ezdxf-1.1.0b3/src/ezdxf/render/abstract_mtext_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/arrows.py` & `ezdxf-1.1.0b3/src/ezdxf/render/arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/curves.py` & `ezdxf-1.1.0b3/src/ezdxf/render/curves.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/dimension.py` & `ezdxf-1.1.0b3/src/ezdxf/render/dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/dim_base.py` & `ezdxf-1.1.0b3/src/ezdxf/render/dim_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/dim_curved.py` & `ezdxf-1.1.0b3/src/ezdxf/render/dim_curved.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/dim_diameter.py` & `ezdxf-1.1.0b3/src/ezdxf/render/dim_diameter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/dim_linear.py` & `ezdxf-1.1.0b3/src/ezdxf/render/dim_linear.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/dim_ordinate.py` & `ezdxf-1.1.0b3/src/ezdxf/render/dim_ordinate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/dim_radius.py` & `ezdxf-1.1.0b3/src/ezdxf/render/dim_radius.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/forms.py` & `ezdxf-1.1.0b3/src/ezdxf/render/forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/hatching.py` & `ezdxf-1.1.0b3/src/ezdxf/render/hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/leader.py` & `ezdxf-1.1.0b3/src/ezdxf/render/leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/linetypes.py` & `ezdxf-1.1.0b3/src/ezdxf/render/linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/mesh.py` & `ezdxf-1.1.0b3/src/ezdxf/render/mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/mleader.py` & `ezdxf-1.1.0b3/src/ezdxf/render/mleader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/mline.py` & `ezdxf-1.1.0b3/src/ezdxf/render/mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/point.py` & `ezdxf-1.1.0b3/src/ezdxf/render/point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/polyline.py` & `ezdxf-1.1.0b3/src/ezdxf/render/polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/r12spline.py` & `ezdxf-1.1.0b3/src/ezdxf/render/r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/trace.py` & `ezdxf-1.1.0b3/src/ezdxf/render/trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/_linetypes.py` & `ezdxf-1.1.0b3/src/ezdxf/render/_linetypes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/render/__init__.py` & `ezdxf-1.1.0b3/src/ezdxf/render/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/16x16.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/16x16.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/24x24.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/24x24.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/256x256.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/256x256.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/32x32.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/32x32.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/48x48.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/48x48.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/64x64.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/64x64.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-copy-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-copy-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-find-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-find-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-bookmark-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-handle-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-handle-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-goto-line-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-goto-line-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-left-arrow-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-left-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-next-entity-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-next-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-prev-entity-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-prev-entity-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-right-arrow-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-right-arrow-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-show-in-tree-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-show-in-tree-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/resources/icon-store-bookmark-64px.png` & `ezdxf-1.1.0b3/src/ezdxf/resources/icon-store-bookmark-64px.png`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/acdsdata.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/acdsdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/blocks.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/blocks.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/classes.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/entities.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/header.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/header.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/headervars.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/headervars.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/objects.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/table.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/sections/tables.py` & `ezdxf-1.1.0b3/src/ezdxf/sections/tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/analyze.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/analyze.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/binarydata.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/binarydata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/codepage.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/codepage.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/complex_ltype.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/complex_ltype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/crypt.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/debug.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/debug.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/difftags.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/handle.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/indexing.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/juliandate.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/pattern.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/rawloader.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/rawloader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/standards.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/standards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/strip.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/strip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/test.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/test.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/text.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/text.py`

 * *Files 0% similar despite different names*

```diff
@@ -1531,15 +1531,15 @@
         self.consume_optional_terminator()
 
     def parse_rgb_color(self, ctx: MTextContext):
         rgb_expr = self.extract_int_expression()
         if rgb_expr:
             # in reversed order!
             b, g, r = int2rgb(int(rgb_expr) & 0xFFFFFF)
-            ctx.rgb = r, g, b
+            ctx.rgb = RGB(r, g, b)
         self.consume_optional_terminator()
 
     def extract_float_expression(self, relative=False) -> str:
         result = ""
         tail = self.scanner.tail()
         pattern = RE_FLOAT_X if relative else RE_FLOAT
         match = re.match(pattern, tail)
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/text_layout.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/text_size.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/zipmanager.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/zipmanager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/_iso_pattern.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/_iso_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf/tools/__init__.py` & `ezdxf-1.1.0b3/src/ezdxf/tools/__init__.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/src/ezdxf.egg-info/PKG-INFO` & `ezdxf-1.1.0b3/src/ezdxf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ezdxf
-Version: 1.1.0b2
+Version: 1.1.0b3
 Summary: A Python package to create/manipulate DXF drawings.
 Home-page: https://ezdxf.mozman.at
 Author: Manfred Moitzi
 Author-email: me@mozman.at
 License: MIT License
 Download-URL: https://pypi.org/project/ezdxf/
 Keywords: DXF,CAD
@@ -223,33 +223,37 @@
   `ezdxf.tools.fonts` module your code will break, sorry! Pin the `ezdxf` version to 
   v1.0.3 in your `requirements.txt` file to use the previous version!
 - NEW: `numpy` is a hard dependency, requires Python version >= 3.8
 - NEW: `fontTools` is a hard dependency
 - NEW: `ezdxf.path.Path2d()` class, `Path` class with `Vec2` vertices
 - NEW: `ezdxf.xref` new core module to manage XREFs and load resources from DXF files
 - NEW: `ezdxf.addons.hpgl2` add-on to convert HPGL/2 plot files to DXF, SVG, PDF, PNG
-- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF
-- NEW: native `SVG` backend for the `drawing` add-on
+- NEW: `ezdxf hpgl` command to view and/or convert HPGL/2 plot files to various formats: DXF, SVG, PDF, PNG
+- NEW: native `SVG`, `HPGL/2`  and `DXF` backends for the `drawing` add-on, these backends 
+  do not need additional libraries to work
+- NEW: `PyMuPdf` backend for the `drawing` add-on, support for PDF, PNG, PPM and PBM export
 - NEW: `ColorPolicy` and `BackgroundPolicy` configuration settings for the `drawing` 
   add-on to change/override foreground- and background color by the frontend 
+- NEW: `TextPolicy` configuration settings for the `drawing` add-on, render text as 
+  solid filling, outline path, replace text by (filled) rectangles or ignore text at all 
 - NEW: support for measuring and rendering of .shx, .shp and .lff fonts, the basic 
   stroke fonts included in CAD applications
 - NEW: added setter to `BlockLayout.base_point` property
 - CHANGED: moved font related modules into a new subpackage `ezdxf.fonts` 
   including a big refactoring
 - CHANGED: `FontFace` class - `weight` attribute is an int value (0-1000), `stretch` is 
   renamed to `width` and is also an int value (1-9) now
 - REMOVED: replaced `matplotlib` font support module by `fontTools`
 - REMOVED: configuration option `use_matplotlib` - is not needed anymore
 - REMOVED: configuration option `font_cache_directory` - is not needed anymore
 - CHANGED: text rendering for the `drawing` add-on and text measurement is done by the
   `fontTools` package
 - CHANGED: moved text rendering from backend classes to the `Frontend` class
 - CHANGED: moved clipping support from backend classes to the `Frontend` class
-- REMOVED: `PillowBackend` and the `pillow` command
+- REMOVED: `Pillow` backend and the `pillow` command
 - REMOVED: `geomdl` test dependency
 - BUGFIX: invalid bulge to Bezier curve conversion for bulge values >= 1
 - BUGFIX: [#855](https://github.com/mozman/ezdxf/issues/855)
   scale `MTEXT/MLEADER` inline commands "absolute text height" at transformation
 
 Version 1.0.3 - 2023-03-26
 --------------------------
```

## Comparing `ezdxf-1.1.0b2/src/ezdxf.egg-info/SOURCES.txt` & `ezdxf-1.1.0b3/src/ezdxf.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -197,20 +197,23 @@
 src/ezdxf/addons/browser/views.py
 src/ezdxf/addons/drawing/__init__.py
 src/ezdxf/addons/drawing/backend.py
 src/ezdxf/addons/drawing/clipper.py
 src/ezdxf/addons/drawing/config.py
 src/ezdxf/addons/drawing/debug_backend.py
 src/ezdxf/addons/drawing/debug_utils.py
+src/ezdxf/addons/drawing/dxf.py
 src/ezdxf/addons/drawing/frontend.py
 src/ezdxf/addons/drawing/gfxproxy.py
+src/ezdxf/addons/drawing/hpgl2.py
 src/ezdxf/addons/drawing/layout.py
 src/ezdxf/addons/drawing/matplotlib.py
 src/ezdxf/addons/drawing/mtext_complex.py
 src/ezdxf/addons/drawing/properties.py
+src/ezdxf/addons/drawing/pymupdf.py
 src/ezdxf/addons/drawing/pyqt.py
 src/ezdxf/addons/drawing/qtviewer.py
 src/ezdxf/addons/drawing/recorder.py
 src/ezdxf/addons/drawing/svg.py
 src/ezdxf/addons/drawing/text.py
 src/ezdxf/addons/drawing/text_renderer.py
 src/ezdxf/addons/drawing/type_hints.py
@@ -221,24 +224,20 @@
 src/ezdxf/addons/dwg/crc.py
 src/ezdxf/addons/dwg/fileheader.py
 src/ezdxf/addons/dwg/header_section.py
 src/ezdxf/addons/dwg/loader.py
 src/ezdxf/addons/hpgl2/__init__.py
 src/ezdxf/addons/hpgl2/api.py
 src/ezdxf/addons/hpgl2/backend.py
-src/ezdxf/addons/hpgl2/compiler.py
 src/ezdxf/addons/hpgl2/deps.py
-src/ezdxf/addons/hpgl2/dxf_backend.py
 src/ezdxf/addons/hpgl2/interpreter.py
 src/ezdxf/addons/hpgl2/page.py
-src/ezdxf/addons/hpgl2/pdf_backend.py
 src/ezdxf/addons/hpgl2/plotter.py
 src/ezdxf/addons/hpgl2/polygon_buffer.py
 src/ezdxf/addons/hpgl2/properties.py
-src/ezdxf/addons/hpgl2/svg_backend.py
 src/ezdxf/addons/hpgl2/tokenizer.py
 src/ezdxf/addons/hpgl2/viewer.py
 src/ezdxf/entities/__init__.py
 src/ezdxf/entities/acad_proxy_entity.py
 src/ezdxf/entities/acad_table.py
 src/ezdxf/entities/acis.py
 src/ezdxf/entities/appdata.py
@@ -768,28 +767,30 @@
 tests/test_08_addons/test_804_importer.py
 tests/test_08_addons/test_805_pycsg.py
 tests/test_08_addons/test_806_acadctb.py
 tests/test_08_addons/test_807_dwg_loader_basics.py
 tests/test_08_addons/test_810_drawing_properties.py
 tests/test_08_addons/test_811a_drawing_frontend.py
 tests/test_08_addons/test_811b_drawing_recorder.py
+tests/test_08_addons/test_811c_viewport_processing.py
 tests/test_08_addons/test_812_drawing_graphic_proxy.py
 tests/test_08_addons/test_813_geo_interface.py
 tests/test_08_addons/test_814_text2path.py
 tests/test_08_addons/test_815_dxf_browser.py
 tests/test_08_addons/test_816_bin_packing.py
 tests/test_08_addons/test_817_genetic_algorithm.py
 tests/test_08_addons/test_818_meshex.py
 tests/test_08_addons/test_819_menger_sponge.py
 tests/test_08_addons/test_820_openscad.py
 tests/test_08_addons/test_821_hpgl2.py
 tests/test_08_addons/test_821_hpgl2_polygon_encoded.py
 tests/test_08_addons/test_822_clipper.py
 tests/test_08_addons/test_823_drawing_layout.py
 tests/test_08_addons/test_824_svg_drawing_backend.py
+tests/test_08_addons/test_825_hpgl2_drawing_backend.py
 tests/test_09_cython_acceleration/test_901_acc_vec2.py
 tests/test_09_cython_acceleration/test_902_acc_vec3.py
 tests/test_09_cython_acceleration/test_903_acc_matrix44.py
 tests/test_09_cython_acceleration/test_904_acc_bezier4p.py
 tests/test_09_cython_acceleration/test_905_acc_bezier3p.py
 tests/test_09_cython_acceleration/test_906_acc_bspline.py
 tests/test_10_issues/test_issue_414_bbox_calculation.py
```

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_001_dxf_types.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_002_dxf_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_003_dxf_binary_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_004_dxf_value.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_005_packed_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_010_binary_data.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_010_binary_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_012_crypt.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_012_crypt.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_013_juliandate.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_013_juliandate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_014_multi_tags_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_015_entity_structure_validator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_016_encoding.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_016_encoding.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_018_handle.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_018_handle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_019_complex_line_type.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_020_validators_and_fixer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_021_fix_line_coordinates.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_023_fix_invalid_located_group_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_024_render_tag.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_024_render_tag.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_040_tags.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_040_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_041_group_tags.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_041_group_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_042_tags_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_043_filter_invalid_point_codes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_050_extended_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_051_load_dxf_structure.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_052_tag_writer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_053_embedded_object_tags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_054_dxfattr.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_055_recover_loader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_056_decode_dxf_unicode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py` & `ezdxf-1.1.0b3/tests/test_00_dxf_low_level_structs/test_057_group_code_mapping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_101_dxfnamespace.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_101_dxfnamespace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_102_appdata.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_102_appdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_103_reactors.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_103_reactors.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_104_extension_dict.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_104_extension_dict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_105_xdata.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_105_xdata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_110_dxfentity.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_110_dxfentity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_111_unknown_dxf_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112a_dxfgfx.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112a_dxfgfx.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_112b_dxfobj.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_112b_dxfobj.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_113_dxfclass.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_113_dxfclass.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_114_factory.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_114_factory.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_115_new_empty_drawing.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_115_new_empty_drawing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_116_dictionary.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_116_dictionary.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_117_layer_table_entry.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_117_layer_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_119_ucs_table_entry.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_119_ucs_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_120_style_table_entry.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_120_style_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_121_ltype_table_entry.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_121_ltype_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_123_view_table_entry.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_123_view_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_124_dimstyle_table_entry.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_125_image_def.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_125_image_def.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_126_image_def_reactor.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_126_image_def_reactor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_127_raster_variables.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_127_raster_variables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_128_pdf_definition.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_128_pdf_definition.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_129_xrecord.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_129_xrecord.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_130_id_buffer.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_130_id_buffer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_131_field_list.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_131_field_list.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_132_layer_filter.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_132_layer_filter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_133_sun.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_133_sun.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_134_material.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_134_material.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_135_geo_data.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_135_geo_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_136_vba_project.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_136_vba_project.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_137_sortentstable.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_137_sortentstable.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_138_setup_visual_styles.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_138_setup_visual_styles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_139_user_record.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_139_user_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_140_block_record.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_140_block_record.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_01_dxf_entities/test_141_layer_vp_override.py` & `ezdxf-1.1.0b3/tests/test_01_dxf_entities/test_141_layer_vp_override.py`

 * *Files 1% similar despite different names*

```diff
@@ -144,24 +144,26 @@
     def vp1(self, doc):
         layout: Paperspace = doc.layout("Layout1")  # type: ignore
         return layout.add_viewport(
             center=(2.5, 2.5),
             size=(5, 5),
             view_center_point=(7.5, 7.5),
             view_height=10,
+            status=2,
         )
 
     @pytest.fixture(scope="class")
     def vp2(self, doc):
         layout: Paperspace = doc.layout("Layout1")  # type: ignore
         return layout.add_viewport(
             center=(2.5, 2.5),
             size=(5, 5),
             view_center_point=(7.5, 7.5),
             view_height=10,
+            status=3,
         )
 
     @staticmethod
     def set_all_ovr(ovr: LayerOverrides, vp_handle, color, alpha, ltype, lw):
         ovr.set_color(vp_handle, color)
         ovr.set_transparency(vp_handle, alpha)
         ovr.set_linetype(vp_handle, ltype)
```

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/conftest.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_200_line.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_200_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_201_point.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_201_point.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_202_circle.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_202_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_203_arc.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_203_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_204_shape.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_204_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_205_solid.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_205_solid.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_206_text.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_206_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_207_attdef.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_207_attdef.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_208_attrib.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_208_attrib.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_209_vertex.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_209_vertex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_1.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_2.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_explode.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_210_polyline_vertex_attributes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_211_viewport.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_211_viewport.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_212_insert.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_212_insert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_213_minsert.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_213_minsert.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_214_block.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_214_block.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_215_dimension.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_215_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_216_dimlines_R12.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_216_dimlines_R12.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_217_dimlines_R2000.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_218_poly_line_mesh_face.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_219_dxf_r2000_generics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_1.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_220_lwpolyline_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_221_ellipse.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_221_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_222_xline.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_222_xline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_223_ray.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_223_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_224_group.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_224_group.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_225_mtext.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_225_mtext.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_226_spline_with_linear_segments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_227_mesh_packed_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_228_mesh.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_228_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229a_hatch_dxf_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229b_hatch_extended.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229b_hatch_extended.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_229c_hatch_transformations.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230a_image_as_virtual_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_230b_image_in_layout_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_231_underlay_2.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_231_underlay_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_acis_2.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_acis_2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_232_surface.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_232_surface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_233_helix.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_233_helix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_234_light.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_234_light.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_235_leader.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_235_leader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_236_multileader.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_236_multileader.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_237_mline.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_237_mline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_238_tolerance.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_238_tolerance.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_239_proxy_graphic.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_239_proxy_graphic.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_240_arc_dimension.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_240_arc_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_241_hyperlink.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_241_hyperlink.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_242_random_transform.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_242_random_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_243_replace_entity.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_243_replace_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_244_large_radial_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_245_wipeout.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_245_wipeout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_246_spline_audit.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_246_spline_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_247_mtext_columns_R2018.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mpolygon.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mpolygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_248_mtext_linked_columns_R2000_to_R2013.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_249_boundary_paths.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_249_boundary_paths.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_250_virtual_boundary_path_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_251_upright.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_251_upright.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_252_acad_proxy_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_253_ole2frame.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_253_ole2frame.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_02_dxf_graphics/test_254_get_font_name.py` & `ezdxf-1.1.0b3/tests/test_02_dxf_graphics/test_254_get_font_name.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_300_layout.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_300_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_301_add_gfx_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_302_block_references.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_302_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_303_auto_block_references.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_303_auto_block_references.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_304_new_entity_space.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_304_new_entity_space.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_305_copy_and_move_entity_to_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_306_copy_linked_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_307_groupby.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_307_groupby.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_308_query.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_308_query.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_309_query_parser.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_309_query_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_311_add_foreign_entity.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_312_virtual_layout.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_312_virtual_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_03_dxf_layouts/test_313_redraw_order.py` & `ezdxf-1.1.0b3/tests/test_03_dxf_layouts/test_313_redraw_order.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_401_headersection.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_401_headersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_402_classessection.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_402_classessection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_403_entity_database.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_403_entity_database.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404a_tables.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404a_tables.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_404b_object_collections.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_405_classes.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_405_classes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_406_blocks_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_407_entity_section.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_407_entity_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_408_objects_section.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_408_objects_section.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_409_create_objects.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_409_create_objects.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_410_table.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_410_table.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_411_acds_data.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_411_acds_data.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_412_rename_layer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_413_dxfgroups.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_414_block_reference_content.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_415_layout_management.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_415_layout_management.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416a_disassemble.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_416b_recursive_decompose.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_417_bbox.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_417_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_418_copy_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_420_load_dxf_file.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_421_new_drawings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_422_drawing_object.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_423_read_proe_r2004.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_424_audit.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_424_audit.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_425_limits_and_extents.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_426_ezdxf_metadata.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_427_appsettings.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_427_appsettings.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py` & `ezdxf-1.1.0b3/tests/test_04_dxf_high_level_structs/test_428_r12_name_translator.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/conftest.py` & `ezdxf-1.1.0b3/tests/test_05_tools/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_500_units.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_500_units.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_501_truecolor.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_501_truecolor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_502_raw_color.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_502_raw_color.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_503_indexing.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_503_indexing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_504_suppress_zeros.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_504_suppress_zeros.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_507_dxf_pretty_printer.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_507_dxf_pretty_printer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_508_read_zip.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_508_read_zip.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_509_comments.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_509_comments.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_510_byte_stream.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_510_byte_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_511_bit_stream.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_511_bit_stream.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_512_pattern.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_512_pattern.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_513_reorder_entities.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_513_reorder_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_514_text.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_514_text.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_515a_fonts_truetype.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_515a_fonts_truetype.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_515b_fonts_shapefiles.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_515b_fonts_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_515c_fonts_lff.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_515c_fonts_lff.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_516_zoom.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_516_zoom.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_517_text_layout.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_517_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_519_mtext_editor.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_519_mtext_editor.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_520_mtext_context.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_520_mtext_context.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_521_mtext_parser.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_521_mtext_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_522_text_scanner.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_522_text_scanner.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_523_text_size.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_523_text_size.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_524_block_reference_manager.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_524_block_reference_manager.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_525_transparency.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_525_transparency.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_526_explode.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_526_explode.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_527_gfxattribs.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_527_gfxattribs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_528_difftags.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_528_difftags.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_529_acis_sat.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_529_acis_sat.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_530_acis_sab.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_530_acis_sab.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_531_acis_entities.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_531_acis_entities.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_532_acis_mesh.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_532_acis_mesh.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_533_shapefiles.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_533_shapefiles.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_534_dwg_info.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_534_dwg_info.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_535_xref_basic.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_535_xref_basic.py`

 * *Files 0% similar despite different names*

```diff
@@ -1208,15 +1208,19 @@
     def psp(self) -> Paperspace:
         doc = ezdxf.new(setup=True)
         psp = doc.page_setup("MyLayout", fmt="ISO A3")
         ucs = doc.tables.ucs.add("MyUCS")
         visualstyle = doc.rootdict["ACAD_VISUALSTYLE"]["2dWireframe"]
         circle = psp.add_circle((100, 100), radius=50)
         vp = psp.add_viewport(
-            center=(100, 100), size=(100, 100), view_center_point=(0, 0), view_height=10
+            center=(100, 100),
+            size=(100, 100),
+            view_center_point=(0, 0),
+            view_height=10,
+            status=2,
         )
         vp.dxf.clipping_boundary_handle = circle.dxf.handle
         vp.dxf.ucs_handle = ucs.dxf.handle
         vp.dxf.visual_style_handle = visualstyle.dxf.handle
         sun = factory.create_db_entry("SUN", {"owner": vp.dxf.handle}, doc)
         doc.objects.add_object(sun)
         vp.dxf.sun_handle = sun.dxf.handle
```

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_536_xref_conflict.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_536_xref_conflict.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_537_transform.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_537_transform.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_538_scale_mtext_inline_commands.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_538_scale_mtext_inline_commands.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_539_npshapes.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_539_npshapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_05_tools/test_540_lff_parser.py` & `ezdxf-1.1.0b3/tests/test_05_tools/test_540_lff_parser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/conftest.py` & `ezdxf-1.1.0b3/tests/test_06_math/conftest.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_600_base.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_600_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_601_bulge.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_601_bulge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_602_vec3.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_602_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_603_vec2.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_603_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_604_banded_matrix.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_604_banded_matrix.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_604_linalg.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_604_linalg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_605_matrix44.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_605_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_606_convexhull.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_606_convexhull.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_607_perlin_noise.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_607_perlin_noise.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_608_intersection_line_line_2d.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_608_intersection_line_line_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_609_point_on_line.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_609_point_on_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_610_ocs.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_610_ocs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_611_ucs.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_611_ucs.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_612_ucs_pass_trough.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_612_ucs_pass_trough.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_613_point_in_poygon.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_613_point_in_poygon.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_614_construct_3d.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_614_construct_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_615_rytz_axis.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_615_rytz_axis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_616_plane.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_616_plane.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_617_clockwise_orientation.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_617_clockwise_orientation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_618_clipping.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_618_clipping.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_619_greiner_hormann.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_619_greiner_hormann.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_620_knot.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_620_knot.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_621_bspline.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_621_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_622_bsplineu.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_622_bsplineu.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_623_rbspline.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_623_rbspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_624_global_bspline_interpolation.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_624_global_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_626_local_bspline_interpolation.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_626_local_bspline_interpolation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_627_bspline_basis.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_627_bspline_basis.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_629_bezier.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_629_bezier.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_630a_bezier4p_base.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_630a_bezier4p_base.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_630b_bezier4p_functions.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_630b_bezier4p_functions.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_631_euler_spiral.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_631_euler_spiral.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_632_bezier3p.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_632_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_640_bbox.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_640_bbox.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_641_construction_ray.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_641_construction_ray.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_642_construction_line.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_642_construction_line.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_643_construction_box.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_643_construction_box.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_644_construction_circle.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_644_construction_circle.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_645_construction_arc.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_645_construction_arc.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_646_offset_vertices_2d.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_646_offset_vertices_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_647_transform_tools.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_647_transform_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_648_construction_ellipse.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_648_construction_ellipse.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_650_elliptic_arc_span.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_650_elliptic_arc_span.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_651_construction_polyline.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_651_construction_polyline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_652_approx_param_t.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_652_approx_param_t.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_653_polyline_intersection.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_653_polyline_intersection.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_654_rtree.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_654_rtree.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_655_dbscan.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_655_dbscan.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_656_k_means.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_656_k_means.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_657_mapbox_earcut.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_657_mapbox_earcut.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_658_bevel_tools.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_658_bevel_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_659_intersection_line_polygon_3d.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_659_intersection_line_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_660_intersection_ray_polygon_3d.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_660_intersection_ray_polygon_3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_661_is_face_normal_pointing_outwards.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_06_math/test_662_is_convex_polygon_2d.py` & `ezdxf-1.1.0b3/tests/test_06_math/test_662_is_convex_polygon_2d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_701_arrows.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_701_arrows.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_702_render_forms.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_702_render_forms.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_703_mesh_builder.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_703_mesh_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_704_render_linear_dimension.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_704_render_linear_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_705_shape.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_705_shape.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_707_trace.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_707_trace.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_708a_path.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_708a_path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_708b_path_tools.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_708b_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_708c_matplotlib_path_tools.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_708c_matplotlib_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_708d_qpainter_path_tools.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_708d_qpainter_path_tools.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_708e_path_shapes.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_708e_path_shapes.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_708f_path_nesting.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_708f_path_nesting.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_709_linetype_renderer.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_709_linetype_renderer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_711_points.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_711_points.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_712_render_curved_dimension.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_712_render_curved_dimension.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_713_mleader_builder.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_713_mleader_builder.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_714_mleader_render_engine.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_714_mleader_render_engine.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_715_hatching.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_715_hatching.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_07_render/test_715_issue_747_explode_3d_dim.py` & `ezdxf-1.1.0b3/tests/test_07_render/test_715_issue_747_explode_3d_dim.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_800_mtext_surrogate.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_800_mtext_surrogate.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_801_r12spline.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_801_r12spline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_802_table_painter.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_802_table_painter.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_803_entities_to_code.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_803_entities_to_code.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_804_importer.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_804_importer.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_805_pycsg.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_805_pycsg.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_806_acadctb.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_806_acadctb.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_807_dwg_loader_basics.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_807_dwg_loader_basics.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_810_drawing_properties.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_810_drawing_properties.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_811a_drawing_frontend.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_811a_drawing_frontend.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2020-2022, Manfred Moitzi
+# Copyright (c) 2020-2023, Manfred Moitzi
 # License: MIT License
 
 import pytest
 import ezdxf
 from ezdxf.addons.drawing import Frontend, RenderContext
 from ezdxf.addons.drawing.properties import BackendProperties
```

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_811b_drawing_recorder.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_811b_drawing_recorder.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 @pytest.fixture
 def frontend(doc, ctx):
     return Frontend(ctx, Recorder())
 
 
 def replay(frontend, backend):
-    player = frontend.out.copy_player()
+    player = frontend.out.player().copy()
     player.replay(backend)
     return backend.collector
 
 
 def test_replay_layout(msp, frontend):
     msp.add_point((0, 0))
     msp.add_point((0, 0))
@@ -95,15 +95,15 @@
         [(0, 0), (1, 0), (2, 0)], dxfattribs={"color": 1, "lineweight": 70}
     )
     # recording:
     backend_recorder = Recorder()
     Frontend(ctx, backend_recorder).draw_entities(msp)
 
     # replay:
-    player = backend_recorder.copy_player()
+    player = backend_recorder.player().copy()
     replay_backend = PathBackend()
     player.replay(replay_backend, override)
 
     properties = replay_backend.collector[1][2]
     assert properties.color == "#00ff00"
     assert properties.lineweight == pytest.approx(0.5)
     assert properties.layer == "1"
@@ -132,12 +132,12 @@
 
 def test_bounding_box(msp, frontend):
     recorder = frontend.out
     assert isinstance(recorder, Recorder)
 
     msp.add_lwpolyline([(0, 0), (200, 0), (200, 100), (0, 100)])
     frontend.draw_layout(msp)
-    player = recorder.copy_player()
+    player = recorder.player().copy()
     player.replay(PathBackend())
     bbox = player.bbox()
     assert bbox.extmin.isclose((0, 0))
     assert bbox.extmax.isclose((200, 100))
```

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_812_drawing_graphic_proxy.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_812_drawing_graphic_proxy.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_813_geo_interface.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_813_geo_interface.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_814_text2path.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_814_text2path.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_815_dxf_browser.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_815_dxf_browser.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_816_bin_packing.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_816_bin_packing.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_817_genetic_algorithm.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_817_genetic_algorithm.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_818_meshex.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_818_meshex.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_819_menger_sponge.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_819_menger_sponge.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_820_openscad.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_820_openscad.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_821_hpgl2.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_821_hpgl2.py`

 * *Files 5% similar despite different names*

```diff
@@ -74,898 +74,906 @@
 00000490: 2020 2064 6566 2064 7261 775f 706f 6c79     def draw_poly
 000004a0: 6c69 6e65 2873 656c 662c 2070 726f 7065  line(self, prope
 000004b0: 7274 6965 732c 2070 6f69 6e74 7329 202d  rties, points) -
 000004c0: 3e20 4e6f 6e65 3a0d 0a20 2020 2020 2020  > None:..       
 000004d0: 2073 656c 662e 7265 7375 6c74 2e61 7070   self.result.app
 000004e0: 656e 6428 5b22 506f 6c79 6c69 6e65 222c  end(["Polyline",
 000004f0: 2070 6f69 6e74 735d 290d 0a0d 0a20 2020   points])....   
-00000500: 2064 6566 2064 7261 775f 6669 6c6c 6564   def draw_filled
-00000510: 5f70 6f6c 7967 6f6e 2873 656c 662c 2070  _polygon(self, p
-00000520: 726f 7065 7274 6965 732c 2070 6174 6873  roperties, paths
-00000530: 2920 2d3e 204e 6f6e 653a 0d0a 2020 2020  ) -> None:..    
-00000540: 2020 2020 7365 6c66 2e72 6573 756c 742e      self.result.
-00000550: 6170 7065 6e64 285b 2246 696c 6c65 6450  append(["FilledP
-00000560: 6f6c 7967 6f6e 222c 2070 6174 6873 5d29  olygon", paths])
-00000570: 0d0a 0d0a 0d0a 6465 6620 706c 6f74 2873  ......def plot(s
-00000580: 3a20 6279 7465 7329 3a0d 0a20 2020 2063  : bytes):..    c
-00000590: 6f6d 6d61 6e64 7320 3d20 6170 692e 6870  ommands = api.hp
-000005a0: 676c 325f 636f 6d6d 616e 6473 2868 7067  gl2_commands(hpg
-000005b0: 6c32 2873 2929 0d0a 2020 2020 6261 636b  l2(s))..    back
-000005c0: 656e 6420 3d20 4d79 4261 636b 656e 6428  end = MyBackend(
-000005d0: 290d 0a20 2020 2061 7069 2e50 6c6f 7474  )..    api.Plott
-000005e0: 6572 2862 6163 6b65 6e64 290d 0a20 2020  er(backend)..   
-000005f0: 2070 6c6f 7474 6572 203d 2061 7069 2e50   plotter = api.P
-00000600: 6c6f 7474 6572 2862 6163 6b65 6e64 290d  lotter(backend).
-00000610: 0a20 2020 2069 6e74 6572 7072 6574 6572  .    interpreter
-00000620: 203d 2061 7069 2e49 6e74 6572 7072 6574   = api.Interpret
-00000630: 6572 2870 6c6f 7474 6572 290d 0a20 2020  er(plotter)..   
-00000640: 2069 6e74 6572 7072 6574 6572 2e72 756e   interpreter.run
-00000650: 2863 6f6d 6d61 6e64 7329 0d0a 2020 2020  (commands)..    
-00000660: 7265 7475 726e 2069 6e74 6572 7072 6574  return interpret
-00000670: 6572 0d0a 0d0a 0d0a 6465 6620 6765 745f  er......def get_
-00000680: 7265 7375 6c74 2870 6c6f 7474 6572 293a  result(plotter):
-00000690: 0d0a 2020 2020 7265 7475 726e 2070 6c6f  ..    return plo
-000006a0: 7474 6572 2e62 6163 6b65 6e64 2e72 6573  tter.backend.res
-000006b0: 756c 740d 0a0d 0a0d 0a63 6c61 7373 2054  ult......class T
-000006c0: 6573 7452 656e 6465 7245 6e67 696e 653a  estRenderEngine:
-000006d0: 0d0a 2020 2020 4070 7974 6573 742e 6d61  ..    @pytest.ma
-000006e0: 726b 2e70 6172 616d 6574 7269 7a65 2822  rk.parametrize("
-000006f0: 636d 6422 2c20 5b62 2250 443b 5041 3230  cmd", [b"PD;PA20
-00000700: 3030 2c38 3030 303b 222c 2062 2250 553b  00,8000;", b"PU;
-00000710: 5041 3230 3030 2c38 3030 303b 225d 290d  PA2000,8000;"]).
-00000720: 0a20 2020 2064 6566 2074 6573 745f 7065  .    def test_pe
-00000730: 6e5f 6162 736f 6c75 7465 2873 656c 662c  n_absolute(self,
-00000740: 2063 6d64 293a 0d0a 2020 2020 2020 2020   cmd):..        
-00000750: 6970 203d 2070 6c6f 7428 636d 6429 0d0a  ip = plot(cmd)..
-00000760: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-00000770: 702e 706c 6f74 7465 722e 7573 6572 5f6c  p.plotter.user_l
-00000780: 6f63 6174 696f 6e20 3d3d 2056 6563 3228  ocation == Vec2(
-00000790: 3230 3030 2c20 3830 3030 290d 0a0d 0a20  2000, 8000).... 
-000007a0: 2020 2064 6566 2074 6573 745f 7365 6c65     def test_sele
-000007b0: 6374 5f70 656e 2873 656c 6629 3a0d 0a20  ct_pen(self):.. 
-000007c0: 2020 2020 2020 2069 7020 3d20 706c 6f74         ip = plot
-000007d0: 2862 2253 5037 3b22 290d 0a20 2020 2020  (b"SP7;")..     
-000007e0: 2020 2061 7373 6572 7420 6970 2e70 6c6f     assert ip.plo
-000007f0: 7474 6572 2e70 726f 7065 7274 6965 732e  tter.properties.
-00000800: 7065 6e5f 696e 6465 7820 3d3d 2037 0d0a  pen_index == 7..
-00000810: 0d0a 2020 2020 2020 2020 6970 203d 2070  ..        ip = p
-00000820: 6c6f 7428 6222 5043 332c 3230 2c33 302c  lot(b"PC3,20,30,
-00000830: 3430 3b50 5730 2e31 382c 333b 5350 333b  40;PW0.18,3;SP3;
-00000840: 2229 0d0a 2020 2020 2020 2020 7072 6f70  ")..        prop
-00000850: 6572 7469 6573 203d 2069 702e 706c 6f74  erties = ip.plot
-00000860: 7465 722e 7072 6f70 6572 7469 6573 0d0a  ter.properties..
-00000870: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
-00000880: 726f 7065 7274 6965 732e 7065 6e5f 696e  roperties.pen_in
-00000890: 6465 7820 3d3d 2033 0d0a 2020 2020 2020  dex == 3..      
-000008a0: 2020 6173 7365 7274 2070 726f 7065 7274    assert propert
-000008b0: 6965 732e 7065 6e5f 7769 6474 6820 3d3d  ies.pen_width ==
-000008c0: 2030 2e31 380d 0a20 2020 2020 2020 2061   0.18..        a
-000008d0: 7373 6572 7420 7072 6f70 6572 7469 6573  ssert properties
-000008e0: 2e70 656e 5f63 6f6c 6f72 203d 3d20 5247  .pen_color == RG
-000008f0: 4228 3230 2c20 3330 2c20 3430 290d 0a0d  B(20, 30, 40)...
-00000900: 0a20 2020 2064 6566 2074 6573 745f 7365  .    def test_se
-00000910: 745f 7065 6e5f 7769 6474 6828 7365 6c66  t_pen_width(self
-00000920: 293a 0d0a 2020 2020 2020 2020 6970 203d  ):..        ip =
-00000930: 2070 6c6f 7428 6222 5057 302e 3138 2c32   plot(b"PW0.18,2
-00000940: 3b22 290d 0a20 2020 2020 2020 2070 726f  ;")..        pro
-00000950: 7065 7274 6965 7320 3d20 6970 2e70 6c6f  perties = ip.plo
-00000960: 7474 6572 2e70 726f 7065 7274 6965 730d  tter.properties.
-00000970: 0a0d 0a20 2020 2020 2020 2061 7373 6572  ...        asser
-00000980: 7420 7072 6f70 6572 7469 6573 2e70 656e  t properties.pen
-00000990: 5f77 6964 7468 203d 3d20 7072 6f70 6572  _width == proper
-000009a0: 7469 6573 2e44 4546 4155 4c54 5f50 454e  ties.DEFAULT_PEN
-000009b0: 2e77 6964 7468 0d0a 2020 2020 2020 2020  .width..        
-000009c0: 7065 6e20 3d20 7072 6f70 6572 7469 6573  pen = properties
-000009d0: 2e67 6574 5f70 656e 2832 290d 0a20 2020  .get_pen(2)..   
-000009e0: 2020 2020 2061 7373 6572 7420 7065 6e2e       assert pen.
-000009f0: 7769 6474 6820 3d3d 2030 2e31 380d 0a0d  width == 0.18...
-00000a00: 0a20 2020 2064 6566 2074 6573 745f 7365  .    def test_se
-00000a10: 745f 6375 7272 656e 745f 7065 6e5f 7769  t_current_pen_wi
-00000a20: 6474 6828 7365 6c66 293a 0d0a 2020 2020  dth(self):..    
-00000a30: 2020 2020 6970 203d 2070 6c6f 7428 6222      ip = plot(b"
-00000a40: 5057 302e 3138 3b22 290d 0a20 2020 2020  PW0.18;")..     
-00000a50: 2020 2061 7373 6572 7420 6970 2e70 6c6f     assert ip.plo
-00000a60: 7474 6572 2e70 726f 7065 7274 6965 732e  tter.properties.
-00000a70: 7065 6e5f 7769 6474 6820 3d3d 2030 2e31  pen_width == 0.1
-00000a80: 380d 0a0d 0a20 2020 2064 6566 2074 6573  8....    def tes
-00000a90: 745f 7365 745f 7065 6e5f 636f 6c6f 7228  t_set_pen_color(
-00000aa0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00000ab0: 6970 203d 2070 6c6f 7428 6222 5043 322c  ip = plot(b"PC2,
-00000ac0: 3230 2c33 302c 3430 3b22 290d 0a20 2020  20,30,40;")..   
-00000ad0: 2020 2020 2070 656e 203d 2069 702e 706c       pen = ip.pl
-00000ae0: 6f74 7465 722e 7072 6f70 6572 7469 6573  otter.properties
-00000af0: 2e67 6574 5f70 656e 2832 290d 0a20 2020  .get_pen(2)..   
-00000b00: 2020 2020 2061 7373 6572 7420 7065 6e2e       assert pen.
-00000b10: 636f 6c6f 7220 3d3d 2052 4742 2832 302c  color == RGB(20,
-00000b20: 2033 302c 2034 3029 0d0a 2020 2020 2020   30, 40)..      
-00000b30: 2020 6173 7365 7274 2028 0d0a 2020 2020    assert (..    
-00000b40: 2020 2020 2020 2020 6970 2e70 6c6f 7474          ip.plott
-00000b50: 6572 2e70 726f 7065 7274 6965 732e 7065  er.properties.pe
-00000b60: 6e5f 636f 6c6f 7220 3d3d 2069 702e 706c  n_color == ip.pl
-00000b70: 6f74 7465 722e 7072 6f70 6572 7469 6573  otter.properties
-00000b80: 2e44 4546 4155 4c54 5f50 454e 2e63 6f6c  .DEFAULT_PEN.col
-00000b90: 6f72 0d0a 2020 2020 2020 2020 290d 0a0d  or..        )...
-00000ba0: 0a20 2020 2064 6566 2074 6573 745f 7365  .    def test_se
-00000bb0: 745f 6669 6c6c 5f74 7970 655f 6861 7463  t_fill_type_hatc
-00000bc0: 6869 6e67 2873 656c 6629 3a0d 0a20 2020  hing(self):..   
-00000bd0: 2020 2020 2069 7020 3d20 706c 6f74 2862       ip = plot(b
-00000be0: 2246 5433 2c38 302c 3435 3b22 290d 0a20  "FT3,80,45;").. 
-00000bf0: 2020 2020 2020 2070 726f 7073 203d 2069         props = i
-00000c00: 702e 706c 6f74 7465 722e 7072 6f70 6572  p.plotter.proper
-00000c10: 7469 6573 0d0a 2020 2020 2020 2020 6173  ties..        as
-00000c20: 7365 7274 2070 726f 7073 2e66 696c 6c5f  sert props.fill_
-00000c30: 7479 7065 203d 3d20 4669 6c6c 5479 7065  type == FillType
-00000c40: 2e48 4154 4348 494e 470d 0a20 2020 2020  .HATCHING..     
-00000c50: 2020 2061 7373 6572 7420 7072 6f70 732e     assert props.
-00000c60: 6669 6c6c 5f68 6174 6368 5f6c 696e 655f  fill_hatch_line_
-00000c70: 7370 6163 696e 6720 3d3d 2038 300d 0a20  spacing == 80.. 
-00000c80: 2020 2020 2020 2061 7373 6572 7420 7072         assert pr
-00000c90: 6f70 732e 6669 6c6c 5f68 6174 6368 5f6c  ops.fill_hatch_l
-00000ca0: 696e 655f 616e 676c 6520 3d3d 2034 350d  ine_angle == 45.
-00000cb0: 0a0d 0a20 2020 2064 6566 2074 6573 745f  ...    def test_
-00000cc0: 7365 745f 6669 6c6c 5f74 7970 655f 7368  set_fill_type_sh
-00000cd0: 6164 696e 6728 7365 6c66 293a 0d0a 2020  ading(self):..  
-00000ce0: 2020 2020 2020 6970 203d 2070 6c6f 7428        ip = plot(
-00000cf0: 6222 4654 3130 2c33 373b 2229 0d0a 2020  b"FT10,37;")..  
-00000d00: 2020 2020 2020 7072 6f70 7320 3d20 6970        props = ip
-00000d10: 2e70 6c6f 7474 6572 2e70 726f 7065 7274  .plotter.propert
-00000d20: 6965 730d 0a20 2020 2020 2020 2061 7373  ies..        ass
-00000d30: 6572 7420 7072 6f70 732e 6669 6c6c 5f74  ert props.fill_t
-00000d40: 7970 6520 3d3d 2046 696c 6c54 7970 652e  ype == FillType.
-00000d50: 5348 4144 494e 470d 0a20 2020 2020 2020  SHADING..       
-00000d60: 2061 7373 6572 7420 7072 6f70 732e 6669   assert props.fi
-00000d70: 6c6c 5f73 6861 6469 6e67 5f64 656e 7369  ll_shading_densi
-00000d80: 7479 203d 3d20 3337 0d0a 0d0a 2020 2020  ty == 37....    
-00000d90: 6465 6620 7465 7374 5f70 656e 5f72 656c  def test_pen_rel
-00000da0: 6174 6976 6528 7365 6c66 293a 0d0a 2020  ative(self):..  
-00000db0: 2020 2020 2020 6970 203d 2070 6c6f 7428        ip = plot(
-00000dc0: 6222 5041 3130 3030 2c31 3030 303b 5052  b"PA1000,1000;PR
-00000dd0: 3530 302c 2d35 3030 3b22 290d 0a20 2020  500,-500;")..   
-00000de0: 2020 2020 2061 7373 6572 7420 6970 2e70       assert ip.p
-00000df0: 6c6f 7474 6572 2e75 7365 725f 6c6f 6361  lotter.user_loca
-00000e00: 7469 6f6e 203d 3d20 5665 6332 2831 3530  tion == Vec2(150
-00000e10: 302c 2035 3030 290d 0a0d 0a20 2020 2064  0, 500)....    d
-00000e20: 6566 2074 6573 745f 706f 6c79 6c69 6e65  ef test_polyline
-00000e30: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00000e40: 2069 7020 3d20 706c 6f74 2862 2250 4432   ip = plot(b"PD2
-00000e50: 3030 302c 3830 3030 2c34 3030 302c 3230  000,8000,4000,20
-00000e60: 3030 2c35 3030 302c 3530 3030 3b22 290d  00,5000,5000;").
-00000e70: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-00000e80: 203d 2067 6574 5f72 6573 756c 7428 6970   = get_result(ip
-00000e90: 2e70 6c6f 7474 6572 295b 305d 0d0a 2020  .plotter)[0]..  
-00000ea0: 2020 2020 2020 6173 7365 7274 2063 6f6d        assert com
-00000eb0: 6d61 6e64 5b30 5d20 3d3d 2022 506f 6c79  mand[0] == "Poly
-00000ec0: 6c69 6e65 220d 0a20 2020 2020 2020 2070  line"..        p
-00000ed0: 6f69 6e74 7320 3d20 636f 6d6d 616e 645b  oints = command[
-00000ee0: 315d 0d0a 2020 2020 2020 2020 6173 7365  1]..        asse
-00000ef0: 7274 206c 656e 2870 6f69 6e74 7329 203d  rt len(points) =
-00000f00: 3d20 340d 0a20 2020 2020 2020 2061 7373  = 4..        ass
-00000f10: 6572 7420 706f 696e 7473 5b30 5d20 3d3d  ert points[0] ==
-00000f20: 2056 6563 3228 302c 2030 290d 0a20 2020   Vec2(0, 0)..   
-00000f30: 2020 2020 2061 7373 6572 7420 706f 696e       assert poin
-00000f40: 7473 5b33 5d20 3d3d 2056 6563 3228 3530  ts[3] == Vec2(50
-00000f50: 3030 2c20 3530 3030 290d 0a20 2020 2020  00, 5000)..     
-00000f60: 2020 2061 7373 6572 7420 6970 2e70 6c6f     assert ip.plo
-00000f70: 7474 6572 2e75 7365 725f 6c6f 6361 7469  tter.user_locati
-00000f80: 6f6e 203d 3d20 5665 6332 2835 3030 302c  on == Vec2(5000,
-00000f90: 2035 3030 3029 0d0a 0d0a 2020 2020 6465   5000)....    de
-00000fa0: 6620 7465 7374 5f63 7562 6963 5f62 657a  f test_cubic_bez
-00000fb0: 6965 725f 6375 7276 655f 7065 6e5f 646f  ier_curve_pen_do
-00000fc0: 776e 2873 656c 6629 3a0d 0a20 2020 2020  wn(self):..     
-00000fd0: 2020 2069 7020 3d20 706c 6f74 2862 2250     ip = plot(b"P
-00000fe0: 443b 425a 3230 3030 2c38 3030 302c 3430  D;BZ2000,8000,40
-00000ff0: 3030 2c32 3030 302c 3530 3030 2c35 3030  00,2000,5000,500
-00001000: 303b 2229 0d0a 2020 2020 2020 2020 636f  0;")..        co
-00001010: 6d6d 616e 6420 3d20 6765 745f 7265 7375  mmand = get_resu
-00001020: 6c74 2869 702e 706c 6f74 7465 7229 5b30  lt(ip.plotter)[0
-00001030: 5d0d 0a20 2020 2020 2020 2070 6f69 6e74  ]..        point
-00001040: 7320 3d20 636f 6d6d 616e 645b 315d 0d0a  s = command[1]..
-00001050: 2020 2020 2020 2020 6173 7365 7274 2063          assert c
-00001060: 6f6d 6d61 6e64 5b30 5d20 3d3d 2022 506f  ommand[0] == "Po
-00001070: 6c79 6c69 6e65 220d 0a20 2020 2020 2020  lyline"..       
-00001080: 2061 7373 6572 7420 706f 696e 7473 5b30   assert points[0
-00001090: 5d20 3d3d 2056 6563 3228 302c 2030 290d  ] == Vec2(0, 0).
-000010a0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000010b0: 706f 696e 7473 5b2d 315d 203d 3d20 5665  points[-1] == Ve
-000010c0: 6332 2835 3030 302c 2035 3030 3029 0d0a  c2(5000, 5000)..
-000010d0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-000010e0: 702e 706c 6f74 7465 722e 7573 6572 5f6c  p.plotter.user_l
-000010f0: 6f63 6174 696f 6e20 3d3d 2056 6563 3228  ocation == Vec2(
-00001100: 3530 3030 2c20 3530 3030 290d 0a0d 0a20  5000, 5000).... 
-00001110: 2020 2064 6566 2074 6573 745f 6375 6269     def test_cubi
-00001120: 635f 6265 7a69 6572 5f63 7572 7665 5f70  c_bezier_curve_p
-00001130: 656e 5f75 7028 7365 6c66 293a 0d0a 2020  en_up(self):..  
-00001140: 2020 2020 2020 6970 203d 2070 6c6f 7428        ip = plot(
-00001150: 6222 5055 3b42 5a32 3030 302c 3830 3030  b"PU;BZ2000,8000
-00001160: 2c34 3030 302c 3230 3030 2c35 3030 302c  ,4000,2000,5000,
-00001170: 3530 3030 3b22 290d 0a20 2020 2020 2020  5000;")..       
-00001180: 2061 7373 6572 7420 6c65 6e28 6765 745f   assert len(get_
-00001190: 7265 7375 6c74 2869 702e 706c 6f74 7465  result(ip.plotte
-000011a0: 7229 2920 3d3d 2030 0d0a 2020 2020 2020  r)) == 0..      
-000011b0: 2020 6173 7365 7274 2069 702e 706c 6f74    assert ip.plot
-000011c0: 7465 722e 7573 6572 5f6c 6f63 6174 696f  ter.user_locatio
-000011d0: 6e20 3d3d 2056 6563 3228 3530 3030 2c20  n == Vec2(5000, 
-000011e0: 3530 3030 290d 0a0d 0a20 2020 2064 6566  5000)....    def
-000011f0: 2074 6573 745f 6369 7263 6c65 2873 656c   test_circle(sel
-00001200: 6629 3a0d 0a20 2020 2020 2020 2069 7020  f):..        ip 
-00001210: 3d20 706c 6f74 2862 2250 553b 5041 3230  = plot(b"PU;PA20
-00001220: 3030 2c38 3030 303b 5044 3b43 4935 3030  00,8000;PD;CI500
-00001230: 3b22 290d 0a20 2020 2020 2020 2063 6f6d  ;")..        com
-00001240: 6d61 6e64 203d 2067 6574 5f72 6573 756c  mand = get_resul
-00001250: 7428 6970 2e70 6c6f 7474 6572 295b 305d  t(ip.plotter)[0]
-00001260: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00001270: 2063 6f6d 6d61 6e64 5b30 5d20 3d3d 2022   command[0] == "
-00001280: 506f 6c79 6c69 6e65 220d 0a20 2020 2020  Polyline"..     
-00001290: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
-000012a0: 6d6d 616e 645b 315d 2920 3d3d 2037 3320  mmand[1]) == 73 
-000012b0: 2023 2064 6566 6175 6c74 2063 686f 7264   # default chord
-000012c0: 5f61 6e67 6c65 2069 7320 3520 6465 670d  _angle is 5 deg.
-000012d0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000012e0: 6970 2e70 6c6f 7474 6572 2e75 7365 725f  ip.plotter.user_
-000012f0: 6c6f 6361 7469 6f6e 203d 3d20 5665 6332  location == Vec2
-00001300: 2832 3030 302c 2038 3030 3029 0d0a 0d0a  (2000, 8000)....
-00001310: 2020 2020 6465 6620 7465 7374 5f61 6273      def test_abs
-00001320: 5f61 7263 2873 656c 6629 3a0d 0a20 2020  _arc(self):..   
-00001330: 2020 2020 2069 7020 3d20 706c 6f74 2862       ip = plot(b
-00001340: 2250 5531 3030 2c31 3030 3b50 443b 4141  "PU100,100;PD;AA
-00001350: 3230 302c 3130 302c 2d31 3830 3b22 290d  200,100,-180;").
-00001360: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-00001370: 203d 2067 6574 5f72 6573 756c 7428 6970   = get_result(ip
-00001380: 2e70 6c6f 7474 6572 295b 305d 0d0a 2020  .plotter)[0]..  
-00001390: 2020 2020 2020 6173 7365 7274 2063 6f6d        assert com
-000013a0: 6d61 6e64 5b30 5d20 3d3d 2022 506f 6c79  mand[0] == "Poly
-000013b0: 6c69 6e65 220d 0a20 2020 2020 2020 2061  line"..        a
-000013c0: 7373 6572 7420 6c65 6e28 636f 6d6d 616e  ssert len(comman
-000013d0: 645b 315d 2920 3d3d 2033 3720 2023 2064  d[1]) == 37  # d
-000013e0: 6566 6175 6c74 2063 686f 7264 5f61 6e67  efault chord_ang
-000013f0: 6c65 2069 7320 3520 6465 670d 0a20 2020  le is 5 deg..   
-00001400: 2020 2020 2061 7373 6572 7420 6970 2e70       assert ip.p
-00001410: 6c6f 7474 6572 2e75 7365 725f 6c6f 6361  lotter.user_loca
-00001420: 7469 6f6e 2e69 7363 6c6f 7365 2828 3330  tion.isclose((30
-00001430: 302c 2031 3030 2929 0d0a 0d0a 2020 2020  0, 100))....    
-00001440: 6465 6620 7465 7374 5f72 656c 5f61 7263  def test_rel_arc
-00001450: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00001460: 2069 7020 3d20 706c 6f74 2862 2250 5531   ip = plot(b"PU1
-00001470: 3030 2c31 3030 3b50 443b 4152 3130 302c  00,100;PD;AR100,
-00001480: 302c 2d31 3830 3b22 290d 0a20 2020 2020  0,-180;")..     
-00001490: 2020 2063 6f6d 6d61 6e64 203d 2067 6574     command = get
-000014a0: 5f72 6573 756c 7428 6970 2e70 6c6f 7474  _result(ip.plott
-000014b0: 6572 295b 305d 0d0a 2020 2020 2020 2020  er)[0]..        
-000014c0: 6173 7365 7274 2063 6f6d 6d61 6e64 5b30  assert command[0
-000014d0: 5d20 3d3d 2022 506f 6c79 6c69 6e65 220d  ] == "Polyline".
-000014e0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000014f0: 6c65 6e28 636f 6d6d 616e 645b 315d 2920  len(command[1]) 
-00001500: 3d3d 2033 3720 2023 2064 6566 6175 6c74  == 37  # default
-00001510: 2063 686f 7264 5f61 6e67 6c65 2069 7320   chord_angle is 
-00001520: 3520 6465 670d 0a20 2020 2020 2020 2061  5 deg..        a
-00001530: 7373 6572 7420 6970 2e70 6c6f 7474 6572  ssert ip.plotter
-00001540: 2e75 7365 725f 6c6f 6361 7469 6f6e 2e69  .user_location.i
-00001550: 7363 6c6f 7365 2828 3330 302c 2031 3030  sclose((300, 100
-00001560: 2929 0d0a 0d0a 2020 2020 6465 6620 7465  ))....    def te
-00001570: 7374 5f61 6273 5f61 7263 5f74 6872 6565  st_abs_arc_three
-00001580: 5f70 6f69 6e74 735f 636c 6f63 6b77 6973  _points_clockwis
-00001590: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
-000015a0: 2020 6970 203d 2070 6c6f 7428 6222 5055    ip = plot(b"PU
-000015b0: 3130 302c 3130 303b 5044 3b41 5432 3030  100,100;PD;AT200
-000015c0: 2c32 3030 2c33 3030 2c31 3030 3b22 290d  ,200,300,100;").
-000015d0: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
-000015e0: 203d 2067 6574 5f72 6573 756c 7428 6970   = get_result(ip
-000015f0: 2e70 6c6f 7474 6572 295b 305d 0d0a 2020  .plotter)[0]..  
-00001600: 2020 2020 2020 6173 7365 7274 2063 6f6d        assert com
-00001610: 6d61 6e64 5b30 5d20 3d3d 2022 506f 6c79  mand[0] == "Poly
-00001620: 6c69 6e65 220d 0a20 2020 2020 2020 2070  line"..        p
-00001630: 6f69 6e74 7320 3d20 636f 6d6d 616e 645b  oints = command[
-00001640: 315d 0d0a 2020 2020 2020 2020 6173 7365  1]..        asse
-00001650: 7274 206c 656e 2870 6f69 6e74 7329 203d  rt len(points) =
-00001660: 3d20 3337 2020 2320 6465 6661 756c 7420  = 37  # default 
-00001670: 6368 6f72 645f 616e 676c 6520 6973 2035  chord_angle is 5
-00001680: 2064 6567 0d0a 2020 2020 2020 2020 6173   deg..        as
-00001690: 7365 7274 2070 6f69 6e74 735b 3138 5d2e  sert points[18].
-000016a0: 6973 636c 6f73 6528 2832 3030 2c20 3230  isclose((200, 20
-000016b0: 3029 290d 0a20 2020 2020 2020 2061 7373  0))..        ass
-000016c0: 6572 7420 6970 2e70 6c6f 7474 6572 2e75  ert ip.plotter.u
-000016d0: 7365 725f 6c6f 6361 7469 6f6e 2e69 7363  ser_location.isc
-000016e0: 6c6f 7365 2828 3330 302c 2031 3030 2929  lose((300, 100))
-000016f0: 0d0a 0d0a 2020 2020 6465 6620 7465 7374  ....    def test
-00001700: 5f61 6273 5f61 7263 5f74 6872 6565 5f70  _abs_arc_three_p
-00001710: 6f69 6e74 735f 636f 756e 7465 725f 636c  oints_counter_cl
-00001720: 6f63 6b77 6973 6528 7365 6c66 293a 0d0a  ockwise(self):..
-00001730: 2020 2020 2020 2020 6970 203d 2070 6c6f          ip = plo
-00001740: 7428 6222 5055 3130 302c 3130 303b 5044  t(b"PU100,100;PD
-00001750: 3b41 5432 3030 2c30 2c33 3030 2c31 3030  ;AT200,0,300,100
-00001760: 3b22 290d 0a20 2020 2020 2020 2063 6f6d  ;")..        com
-00001770: 6d61 6e64 203d 2067 6574 5f72 6573 756c  mand = get_resul
-00001780: 7428 6970 2e70 6c6f 7474 6572 295b 305d  t(ip.plotter)[0]
-00001790: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-000017a0: 2063 6f6d 6d61 6e64 5b30 5d20 3d3d 2022   command[0] == "
-000017b0: 506f 6c79 6c69 6e65 220d 0a20 2020 2020  Polyline"..     
-000017c0: 2020 2070 6f69 6e74 7320 3d20 636f 6d6d     points = comm
-000017d0: 616e 645b 315d 0d0a 2020 2020 2020 2020  and[1]..        
-000017e0: 6173 7365 7274 206c 656e 2870 6f69 6e74  assert len(point
-000017f0: 7329 203d 3d20 3337 2020 2320 6465 6661  s) == 37  # defa
-00001800: 756c 7420 6368 6f72 645f 616e 676c 6520  ult chord_angle 
-00001810: 6973 2035 2064 6567 0d0a 2020 2020 2020  is 5 deg..      
-00001820: 2020 6173 7365 7274 2070 6f69 6e74 735b    assert points[
-00001830: 3138 5d2e 6973 636c 6f73 6528 2832 3030  18].isclose((200
-00001840: 2c20 3029 290d 0a20 2020 2020 2020 2061  , 0))..        a
-00001850: 7373 6572 7420 6970 2e70 6c6f 7474 6572  ssert ip.plotter
-00001860: 2e75 7365 725f 6c6f 6361 7469 6f6e 2e69  .user_location.i
-00001870: 7363 6c6f 7365 2828 3330 302c 2031 3030  sclose((300, 100
-00001880: 2929 0d0a 0d0a 2020 2020 6465 6620 7465  ))....    def te
-00001890: 7374 5f72 656c 5f61 7263 5f74 6872 6565  st_rel_arc_three
-000018a0: 5f70 6f69 6e74 735f 636c 6f63 6b77 6973  _points_clockwis
-000018b0: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
-000018c0: 2020 6970 203d 2070 6c6f 7428 6222 5055    ip = plot(b"PU
-000018d0: 3130 302c 3130 303b 5044 3b52 5431 3030  100,100;PD;RT100
-000018e0: 2c31 3030 2c32 3030 2c30 3b22 290d 0a20  ,100,200,0;").. 
-000018f0: 2020 2020 2020 2063 6f6d 6d61 6e64 203d         command =
-00001900: 2067 6574 5f72 6573 756c 7428 6970 2e70   get_result(ip.p
-00001910: 6c6f 7474 6572 295b 305d 0d0a 2020 2020  lotter)[0]..    
-00001920: 2020 2020 6173 7365 7274 2063 6f6d 6d61      assert comma
-00001930: 6e64 5b30 5d20 3d3d 2022 506f 6c79 6c69  nd[0] == "Polyli
-00001940: 6e65 220d 0a20 2020 2020 2020 2070 6f69  ne"..        poi
-00001950: 6e74 7320 3d20 636f 6d6d 616e 645b 315d  nts = command[1]
-00001960: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00001970: 206c 656e 2870 6f69 6e74 7329 203d 3d20   len(points) == 
-00001980: 3337 2020 2320 6465 6661 756c 7420 6368  37  # default ch
-00001990: 6f72 645f 616e 676c 6520 6973 2035 2064  ord_angle is 5 d
-000019a0: 6567 0d0a 2020 2020 2020 2020 6173 7365  eg..        asse
-000019b0: 7274 2070 6f69 6e74 735b 3138 5d2e 6973  rt points[18].is
-000019c0: 636c 6f73 6528 2832 3030 2c20 3230 3029  close((200, 200)
-000019d0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-000019e0: 7420 6970 2e70 6c6f 7474 6572 2e75 7365  t ip.plotter.use
-000019f0: 725f 6c6f 6361 7469 6f6e 2e69 7363 6c6f  r_location.isclo
-00001a00: 7365 2828 3330 302c 2031 3030 2929 0d0a  se((300, 100))..
-00001a10: 0d0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
-00001a20: 6f6c 796c 696e 655f 656e 636f 6465 6428  olyline_encoded(
-00001a30: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
-00001a40: 6970 203d 2070 6c6f 7428 6222 5045 373d  ip = plot(b"PE7=
-00001a50: 555e 7847 4968 3b22 290d 0a20 2020 2020  U^xGIh;")..     
-00001a60: 2020 2063 6f6d 6d61 6e64 203d 2067 6574     command = get
-00001a70: 5f72 6573 756c 7428 6970 2e70 6c6f 7474  _result(ip.plott
-00001a80: 6572 295b 305d 0d0a 2020 2020 2020 2020  er)[0]..        
-00001a90: 6173 7365 7274 2063 6f6d 6d61 6e64 5b30  assert command[0
-00001aa0: 5d20 3d3d 2022 506f 6c79 6c69 6e65 220d  ] == "Polyline".
-00001ab0: 0a0d 0a0d 0a63 6c61 7373 2054 6573 7454  .....class TestT
-00001ac0: 6f6b 656e 697a 6572 3a0d 0a20 2020 2064  okenizer:..    d
-00001ad0: 6566 2070 6172 7365 2873 656c 662c 2073  ef parse(self, s
-00001ae0: 3a20 6279 7465 7329 3a0d 0a20 2020 2020  : bytes):..     
-00001af0: 2020 2072 6574 7572 6e20 6170 692e 6870     return api.hp
-00001b00: 676c 325f 636f 6d6d 616e 6473 2873 290d  gl2_commands(s).
-00001b10: 0a0d 0a20 2020 2040 7079 7465 7374 2e6d  ...    @pytest.m
-00001b20: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
-00001b30: 0d0a 2020 2020 2020 2020 2273 222c 0d0a  ..        "s",..
-00001b40: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
-00001b50: 2020 2020 2020 2062 221b 252d 3142 4250         b".%-1BBP
-00001b60: 3b22 2c0d 0a20 2020 2020 2020 2020 2020  ;",..           
-00001b70: 2062 221b 2530 4242 503b 222c 0d0a 2020   b".%0BBP;",..  
-00001b80: 2020 2020 2020 2020 2020 6222 1b25 3142            b".%1B
-00001b90: 4250 3b22 2c0d 0a20 2020 2020 2020 2020  BP;",..         
-00001ba0: 2020 2062 221b 2532 4242 503b 222c 0d0a     b".%2BBP;",..
-00001bb0: 2020 2020 2020 2020 2020 2020 6222 1b25              b".%
-00001bc0: 3342 4250 3b22 2c0d 0a20 2020 2020 2020  3BBP;",..       
-00001bd0: 205d 2c0d 0a20 2020 2029 0d0a 2020 2020   ],..    )..    
-00001be0: 6465 6620 7465 7374 5f65 7363 6170 6528  def test_escape(
-00001bf0: 7365 6c66 2c20 7329 3a0d 0a20 2020 2020  self, s):..     
-00001c00: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
-00001c10: 2e70 6172 7365 2873 290d 0a20 2020 2020  .parse(s)..     
-00001c20: 2020 2061 7373 6572 7420 7265 7375 6c74     assert result
-00001c30: 5b30 5d2e 6e61 6d65 203d 3d20 2242 5022  [0].name == "BP"
-00001c40: 0d0a 0d0a 2020 2020 4070 7974 6573 742e  ....    @pytest.
-00001c50: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
-00001c60: 280d 0a20 2020 2020 2020 2022 7322 2c0d  (..        "s",.
-00001c70: 0a20 2020 2020 2020 205b 0d0a 2020 2020  .        [..    
-00001c80: 2020 2020 2020 2020 6222 494e 3b50 553b          b"IN;PU;
-00001c90: 5044 3b22 2c0d 0a20 2020 2020 2020 2020  PD;",..         
-00001ca0: 2020 2062 2249 4e3b 5055 3b50 4422 2c0d     b"IN;PU;PD",.
-00001cb0: 0a20 2020 2020 2020 2020 2020 2062 2249  .            b"I
-00001cc0: 4e50 5550 4422 2c0d 0a20 2020 2020 2020  NPUPD",..       
-00001cd0: 2020 2020 2062 2249 4e20 5055 2050 4422       b"IN PU PD"
-00001ce0: 2c0d 0a20 2020 2020 2020 2020 2020 2062  ,..            b
-00001cf0: 2220 494e 5055 2050 4422 2c0d 0a20 2020  " INPU PD",..   
-00001d00: 2020 2020 205d 2c0d 0a20 2020 2029 0d0a       ],..    )..
-00001d10: 2020 2020 6465 6620 7465 7374 5f73 686f      def test_sho
-00001d20: 7274 5f63 6f6d 6d61 6e64 7328 7365 6c66  rt_commands(self
-00001d30: 2c20 7329 3a0d 0a20 2020 2020 2020 2072  , s):..        r
-00001d40: 6573 756c 7420 3d20 7365 6c66 2e70 6172  esult = self.par
-00001d50: 7365 2868 7067 6c32 2873 2929 0d0a 2020  se(hpgl2(s))..  
-00001d60: 2020 2020 2020 6173 7365 7274 206c 656e        assert len
-00001d70: 2872 6573 756c 7429 203d 3d20 330d 0a20  (result) == 3.. 
-00001d80: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
-00001d90: 7375 6c74 5b30 5d2e 6e61 6d65 203d 3d20  sult[0].name == 
-00001da0: 2249 4e22 0d0a 2020 2020 2020 2020 6173  "IN"..        as
-00001db0: 7365 7274 2072 6573 756c 745b 315d 2e6e  sert result[1].n
-00001dc0: 616d 6520 3d3d 2022 5055 220d 0a20 2020  ame == "PU"..   
-00001dd0: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
-00001de0: 6c74 5b32 5d2e 6e61 6d65 203d 3d20 2250  lt[2].name == "P
-00001df0: 4422 0d0a 0d0a 2020 2020 4070 7974 6573  D"....    @pytes
-00001e00: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
-00001e10: 7a65 280d 0a20 2020 2020 2020 2022 732c  ze(..        "s,
-00001e20: 6922 2c0d 0a20 2020 2020 2020 205b 0d0a  i",..        [..
-00001e30: 2020 2020 2020 2020 2020 2020 2862 2250              (b"P
-00001e40: 4554 4553 5422 2c20 3029 2c0d 0a20 2020  ETEST", 0),..   
-00001e50: 2020 2020 2020 2020 2028 6222 5055 5045           (b"PUPE
-00001e60: 5445 5354 3b50 4422 2c20 3129 2c0d 0a20  TEST;PD", 1),.. 
-00001e70: 2020 2020 2020 2020 2020 2028 6222 5055             (b"PU
-00001e80: 5055 5045 5445 5354 3b50 4422 2c20 3229  PUPETEST;PD", 2)
-00001e90: 2c0d 0a20 2020 2020 2020 205d 2c0d 0a20  ,..        ],.. 
-00001ea0: 2020 2029 0d0a 2020 2020 6465 6620 7465     )..    def te
-00001eb0: 7374 5f70 655f 636f 6d6d 616e 6428 7365  st_pe_command(se
-00001ec0: 6c66 2c20 732c 2069 293a 0d0a 2020 2020  lf, s, i):..    
-00001ed0: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
-00001ee0: 662e 7061 7273 6528 6870 676c 3228 7329  f.parse(hpgl2(s)
-00001ef0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00001f00: 7420 7265 7375 6c74 5b69 5d2e 6e61 6d65  t result[i].name
-00001f10: 203d 3d20 2250 4522 0d0a 2020 2020 2020   == "PE"..      
-00001f20: 2020 6173 7365 7274 2072 6573 756c 745b    assert result[
-00001f30: 695d 2e61 7267 735b 305d 203d 3d20 6222  i].args[0] == b"
-00001f40: 5445 5354 220d 0a0d 0a20 2020 2064 6566  TEST"....    def
-00001f50: 2074 6573 745f 3030 3128 7365 6c66 293a   test_001(self):
-00001f60: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00001f70: 203d 2073 656c 662e 7061 7273 6528 6870   = self.parse(hp
-00001f80: 676c 3228 6222 5041 3b50 4132 3030 302c  gl2(b"PA;PA2000,
-00001f90: 3830 3030 2229 290d 0a20 2020 2020 2020  8000"))..       
-00001fa0: 2061 7373 6572 7420 7265 7375 6c74 5b30   assert result[0
-00001fb0: 5d2e 6e61 6d65 203d 3d20 2250 4122 0d0a  ].name == "PA"..
-00001fc0: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-00001fd0: 6573 756c 745b 315d 2e6e 616d 6520 3d3d  esult[1].name ==
-00001fe0: 2022 5041 220d 0a0d 0a20 2020 2064 6566   "PA"....    def
-00001ff0: 2074 6573 745f 3030 3228 7365 6c66 293a   test_002(self):
-00002000: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
-00002010: 203d 2073 656c 662e 7061 7273 6528 6870   = self.parse(hp
-00002020: 676c 3228 6222 5055 5350 3050 4722 2929  gl2(b"PUSP0PG"))
-00002030: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00002040: 2072 6573 756c 745b 305d 2e6e 616d 6520   result[0].name 
-00002050: 3d3d 2022 5055 220d 0a20 2020 2020 2020  == "PU"..       
-00002060: 2061 7373 6572 7420 7265 7375 6c74 5b31   assert result[1
-00002070: 5d2e 6e61 6d65 203d 3d20 2253 5022 0d0a  ].name == "SP"..
-00002080: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
-00002090: 6573 756c 745b 315d 2e61 7267 735b 305d  esult[1].args[0]
-000020a0: 203d 3d20 6222 3022 0d0a 2020 2020 2020   == b"0"..      
-000020b0: 2020 6173 7365 7274 2072 6573 756c 745b    assert result[
-000020c0: 325d 2e6e 616d 6520 3d3d 2022 5047 220d  2].name == "PG".
-000020d0: 0a0d 0a20 2020 2064 6566 2074 6573 745f  ...    def test_
-000020e0: 6669 6c74 6572 5f6e 6f6e 5f70 7269 6e74  filter_non_print
-000020f0: 6162 6c65 5f63 6861 7273 5f66 726f 6d5f  able_chars_from_
-00002100: 7065 5f63 6f6d 6d61 6e64 2873 656c 6629  pe_command(self)
-00002110: 3a0d 0a20 2020 2020 2020 2072 6573 756c  :..        resul
-00002120: 7420 3d20 7365 6c66 2e70 6172 7365 2868  t = self.parse(h
-00002130: 7067 6c32 2862 2250 4578 7878 7878 5c72  pgl2(b"PExxxxx\r
-00002140: 5c6e 7878 7878 783b 2229 290d 0a20 2020  \nxxxxx;"))..   
-00002150: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
-00002160: 6c74 5b30 5d2e 6172 6773 5b30 5d20 3d3d  lt[0].args[0] ==
-00002170: 2062 2278 7878 7878 7878 7878 7822 0d0a   b"xxxxxxxxxx"..
-00002180: 0d0a 2020 2020 6465 6620 7465 7374 5f6e  ..    def test_n
-00002190: 6f5f 6870 676c 325f 6461 7461 2873 656c  o_hpgl2_data(sel
-000021a0: 6629 3a0d 0a20 2020 2020 2020 2023 2045  f):..        # E
-000021b0: 6361 7065 2073 6571 7565 6e63 6520 746f  cape sequence to
-000021c0: 2065 6e74 6572 2048 5047 4c32 206d 6f64   enter HPGL2 mod
-000021d0: 6520 6973 206d 6973 7369 6e67 3a20 2022  e is missing:  "
-000021e0: 1b25 3142 220d 0a20 2020 2020 2020 2061  .%1B"..        a
-000021f0: 7373 6572 7420 6c65 6e28 7365 6c66 2e70  ssert len(self.p
-00002200: 6172 7365 2862 2241 4e59 5445 5854 3b49  arse(b"ANYTEXT;I
-00002210: 4e3b 4250 3b22 2929 203d 3d20 300d 0a0d  N;BP;")) == 0...
-00002220: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
-00002230: 6b2e 7061 7261 6d65 7472 697a 6528 2262  k.parametrize("b
-00002240: 222c 205b 0d0a 2020 2020 2020 2020 6222  ", [..        b"
-00002250: 4c42 204d 5920 6c61 6265 6c20 0350 4133  LB MY label .PA3
-00002260: 3831 2c30 5349 302e 3132 352c 302e 3235  81,0SI0.125,0.25
-00002270: 4449 302c 313b 222c 0d0a 2020 2020 2020  DI0,1;",..      
-00002280: 2020 6222 4c42 4d59 206c 6162 656c 2003    b"LBMY label .
-00002290: 5041 3338 312c 3053 4930 2e31 3235 2c30  PA381,0SI0.125,0
-000022a0: 2e32 3544 4930 2c31 3b22 0d0a 2020 2020  .25DI0,1;"..    
-000022b0: 5d29 0d0a 2020 2020 6465 6620 7465 7374  ])..    def test
-000022c0: 5f6c 6162 656c 5f77 6974 685f 7465 726d  _label_with_term
-000022d0: 696e 6174 6f72 2873 656c 662c 2062 293a  inator(self, b):
-000022e0: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
-000022f0: 6473 203d 2073 656c 662e 7061 7273 6528  ds = self.parse(
-00002300: 6870 676c 3228 6229 290d 0a20 2020 2020  hpgl2(b))..     
-00002310: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
-00002320: 6d6d 616e 6473 2920 3d3d 2034 0d0a 0d0a  mmands) == 4....
-00002330: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00002340: 2e70 6172 616d 6574 7269 7a65 280d 0a20  .parametrize(.. 
-00002350: 2020 2020 2020 2022 6222 2c0d 0a20 2020         "b",..   
-00002360: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
-00002370: 2020 2020 6222 4454 5c30 344c 4220 5475      b"DT\04LB Tu
-00002380: 6520 4465 6320 3138 2031 363a 3230 3a30  e Dec 18 16:20:0
-00002390: 3520 3230 3031 205c 3034 5041 3338 312c  5 2001 \04PA381,
-000023a0: 3053 4930 2e31 3235 2c30 2e32 3544 4930  0SI0.125,0.25DI0
-000023b0: 2c31 3b22 2c0d 0a20 2020 2020 2020 2020  ,1;",..         
-000023c0: 2020 2062 2244 545c 3034 2c30 4c42 2054     b"DT\04,0LB T
-000023d0: 7565 2044 6563 2031 3820 3136 3a32 303a  ue Dec 18 16:20:
-000023e0: 3035 2032 3030 3120 5c30 3450 4133 3831  05 2001 \04PA381
-000023f0: 2c30 5349 302e 3132 352c 302e 3235 4449  ,0SI0.125,0.25DI
-00002400: 302c 313b 222c 0d0a 2020 2020 2020 2020  0,1;",..        
-00002410: 2020 2020 6222 4454 5c30 342c 313b 4c42      b"DT\04,1;LB
-00002420: 2054 7565 2044 6563 2031 3820 3136 3a32   Tue Dec 18 16:2
-00002430: 303a 3035 2032 3030 3120 5c30 3450 4133  0:05 2001 \04PA3
-00002440: 3831 2c30 5349 302e 3132 352c 302e 3235  81,0SI0.125,0.25
-00002450: 4449 302c 313b 222c 0d0a 2020 2020 2020  DI0,1;",..      
-00002460: 2020 5d2c 0d0a 2020 2020 290d 0a20 2020    ],..    )..   
-00002470: 2064 6566 2074 6573 745f 6c61 6265 6c5f   def test_label_
-00002480: 7769 7468 5f63 7573 746f 6d5f 7465 726d  with_custom_term
-00002490: 696e 6174 6f72 2873 656c 662c 2062 293a  inator(self, b):
-000024a0: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
-000024b0: 6473 203d 2073 656c 662e 7061 7273 6528  ds = self.parse(
-000024c0: 6870 676c 3228 6229 290d 0a20 2020 2020  hpgl2(b))..     
-000024d0: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
-000024e0: 6d6d 616e 6473 2920 3d3d 2034 0d0a 0d0a  mmands) == 4....
-000024f0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
-00002500: 2e70 6172 616d 6574 7269 7a65 280d 0a20  .parametrize(.. 
-00002510: 2020 2020 2020 2022 6222 2c0d 0a20 2020         "b",..   
-00002520: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
-00002530: 2020 2020 6222 4454 5c30 344c 4220 4d59      b"DT\04LB MY
-00002540: 206c 6162 656c 5c30 3444 544c 4220 4d79   label\04DTLB My
-00002550: 206f 7468 6572 206c 6162 656c 2003 222c   other label .",
-00002560: 0d0a 2020 2020 2020 2020 2020 2020 6222  ..            b"
-00002570: 4454 5c30 344c 4220 4d59 206c 6162 656c  DT\04LB MY label
-00002580: 5c30 3444 543b 4c42 204d 7920 6f74 6865  \04DT;LB My othe
-00002590: 7220 6c61 6265 6c20 0322 2c0d 0a20 2020  r label .",..   
-000025a0: 2020 2020 205d 2c0d 0a20 2020 2029 0d0a       ],..    )..
-000025b0: 2020 2020 6465 6620 7465 7374 5f72 6573      def test_res
-000025c0: 6574 5f63 7573 746f 6d5f 7465 726d 696e  et_custom_termin
-000025d0: 6174 6f72 2873 656c 662c 2062 293a 0d0a  ator(self, b):..
-000025e0: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
-000025f0: 203d 2073 656c 662e 7061 7273 6528 6870   = self.parse(hp
-00002600: 676c 3228 6229 290d 0a20 2020 2020 2020  gl2(b))..       
-00002610: 2061 7373 6572 7420 6c65 6e28 636f 6d6d   assert len(comm
-00002620: 616e 6473 2920 3d3d 2032 0d0a 0d0a 0d0a  ands) == 2......
-00002630: 636c 6173 7320 5465 7374 5061 6765 436f  class TestPageCo
-00002640: 6f72 6469 6e61 7465 733a 0d0a 2020 2020  ordinates:..    
-00002650: 4070 7974 6573 742e 6669 7874 7572 6528  @pytest.fixture(
-00002660: 7363 6f70 653d 2263 6c61 7373 2229 0d0a  scope="class")..
-00002670: 2020 2020 6465 6620 7061 6765 2873 656c      def page(sel
-00002680: 6629 3a0d 0a20 2020 2020 2020 2070 6167  f):..        pag
-00002690: 655f 203d 2050 6167 6528 3130 3030 2c20  e_ = Page(1000, 
-000026a0: 3130 3030 290d 0a20 2020 2020 2020 2070  1000)..        p
-000026b0: 6167 655f 2e73 6574 5f75 6373 2856 6563  age_.set_ucs(Vec
-000026c0: 3228 3530 302c 2035 3030 292c 2073 783d  2(500, 500), sx=
-000026d0: 322c 2073 793d 3329 0d0a 2020 2020 2020  2, sy=3)..      
-000026e0: 2020 7265 7475 726e 2070 6167 655f 0d0a    return page_..
-000026f0: 0d0a 2020 2020 6465 6620 7465 7374 5f75  ..    def test_u
-00002700: 7365 725f 746f 5f70 6167 655f 636f 6f72  ser_to_page_coor
-00002710: 6469 6e61 7465 7328 7365 6c66 2c20 7061  dinates(self, pa
-00002720: 6765 293a 0d0a 2020 2020 2020 2020 6173  ge):..        as
-00002730: 7365 7274 2070 6167 652e 7061 6765 5f70  sert page.page_p
-00002740: 6f69 6e74 2830 2c20 3029 2e69 7363 6c6f  oint(0, 0).isclo
-00002750: 7365 2828 3530 302c 2035 3030 2929 0d0a  se((500, 500))..
-00002760: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
-00002770: 6167 652e 7061 6765 5f70 6f69 6e74 2831  age.page_point(1
-00002780: 302c 2031 3029 2e69 7363 6c6f 7365 2828  0, 10).isclose((
-00002790: 3532 302c 2035 3330 2929 0d0a 0d0a 2020  520, 530))....  
-000027a0: 2020 6465 6620 7465 7374 5f75 7365 725f    def test_user_
-000027b0: 7665 6374 6f72 5f74 6f5f 7061 6765 5f76  vector_to_page_v
-000027c0: 6563 746f 7228 7365 6c66 2c20 7061 6765  ector(self, page
-000027d0: 293a 0d0a 2020 2020 2020 2020 6173 7365  ):..        asse
-000027e0: 7274 2070 6167 652e 7061 6765 5f76 6563  rt page.page_vec
-000027f0: 746f 7228 302c 2030 292e 6973 636c 6f73  tor(0, 0).isclos
-00002800: 6528 2830 2c20 3029 290d 0a20 2020 2020  e((0, 0))..     
-00002810: 2020 2061 7373 6572 7420 7061 6765 2e70     assert page.p
-00002820: 6167 655f 7665 6374 6f72 2831 302c 2031  age_vector(10, 1
-00002830: 3029 2e69 7363 6c6f 7365 2828 3230 2c20  0).isclose((20, 
-00002840: 3330 2929 0d0a 0d0a 0d0a 636c 6173 7320  30))......class 
-00002850: 5465 7374 5061 6765 416e 6973 6f74 726f  TestPageAnisotro
-00002860: 7069 6353 6361 6c69 6e67 3a0d 0a20 2020  picScaling:..   
-00002870: 2064 6566 2074 6573 745f 6973 6f74 726f   def test_isotro
-00002880: 7069 635f 7363 616c 696e 6728 7365 6c66  pic_scaling(self
-00002890: 293a 0d0a 2020 2020 2020 2020 7061 6765  ):..        page
-000028a0: 203d 2050 6167 6528 3130 3030 2c20 3130   = Page(1000, 10
-000028b0: 3030 290d 0a20 2020 2020 2020 2070 6167  00)..        pag
-000028c0: 652e 7365 745f 7363 616c 696e 675f 706f  e.set_scaling_po
-000028d0: 696e 7473 2856 6563 3228 3130 302c 2031  ints(Vec2(100, 1
-000028e0: 3030 292c 2056 6563 3228 3230 302c 2032  00), Vec2(200, 2
-000028f0: 3030 2929 0d0a 2020 2020 2020 2020 7061  00))..        pa
-00002900: 6765 2e73 6574 5f61 6e69 736f 7472 6f70  ge.set_anisotrop
-00002910: 6963 5f73 6361 6c69 6e67 282d 3130 2c20  ic_scaling(-10, 
-00002920: 3130 2c20 2d31 302c 2031 3029 0d0a 2020  10, -10, 10)..  
-00002930: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
-00002940: 652e 7573 6572 5f73 6361 6c69 6e67 2069  e.user_scaling i
-00002950: 7320 5472 7565 0d0a 2020 2020 2020 2020  s True..        
-00002960: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
-00002970: 5f70 6f69 6e74 2830 2c20 3029 2e69 7363  _point(0, 0).isc
-00002980: 6c6f 7365 2828 3135 302c 2031 3530 2929  lose((150, 150))
-00002990: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-000029a0: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
-000029b0: 282d 3130 2c20 2d31 3029 2e69 7363 6c6f  (-10, -10).isclo
-000029c0: 7365 2828 3130 302c 2031 3030 2929 0d0a  se((100, 100))..
-000029d0: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
-000029e0: 6167 652e 7061 6765 5f70 6f69 6e74 2831  age.page_point(1
-000029f0: 302c 2031 3029 2e69 7363 6c6f 7365 2828  0, 10).isclose((
-00002a00: 3230 302c 2032 3030 2929 0d0a 0d0a 2020  200, 200))....  
-00002a10: 2020 6465 6620 7465 7374 5f61 6e69 736f    def test_aniso
-00002a20: 7472 6f70 6963 5f73 6361 6c69 6e67 2873  tropic_scaling(s
-00002a30: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
-00002a40: 6167 6520 3d20 5061 6765 2831 3030 302c  age = Page(1000,
-00002a50: 2031 3030 3029 0d0a 2020 2020 2020 2020   1000)..        
-00002a60: 7061 6765 2e73 6574 5f73 6361 6c69 6e67  page.set_scaling
-00002a70: 5f70 6f69 6e74 7328 5665 6332 2831 3030  _points(Vec2(100
-00002a80: 2c20 3130 3029 2c20 5665 6332 2832 3030  , 100), Vec2(200
-00002a90: 2c20 3230 3029 290d 0a20 2020 2020 2020  , 200))..       
-00002aa0: 2070 6167 652e 7365 745f 616e 6973 6f74   page.set_anisot
-00002ab0: 726f 7069 635f 7363 616c 696e 6728 2d31  ropic_scaling(-1
-00002ac0: 302c 2031 302c 202d 3230 2c20 3230 290d  0, 10, -20, 20).
-00002ad0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00002ae0: 7061 6765 2e75 7365 725f 7363 616c 696e  page.user_scalin
-00002af0: 6720 6973 2054 7275 650d 0a20 2020 2020  g is True..     
-00002b00: 2020 2061 7373 6572 7420 7061 6765 2e70     assert page.p
-00002b10: 6167 655f 706f 696e 7428 302c 2030 292e  age_point(0, 0).
-00002b20: 6973 636c 6f73 6528 2831 3530 2c20 3135  isclose((150, 15
-00002b30: 3029 290d 0a20 2020 2020 2020 2061 7373  0))..        ass
-00002b40: 6572 7420 7061 6765 2e70 6167 655f 706f  ert page.page_po
-00002b50: 696e 7428 2d31 302c 202d 3230 292e 6973  int(-10, -20).is
-00002b60: 636c 6f73 6528 2831 3030 2c20 3130 3029  close((100, 100)
-00002b70: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00002b80: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
-00002b90: 7428 3130 2c20 3230 292e 6973 636c 6f73  t(10, 20).isclos
-00002ba0: 6528 2832 3030 2c20 3230 3029 290d 0a0d  e((200, 200))...
-00002bb0: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
-00002bc0: 7665 7273 655f 616e 6973 6f74 726f 7069  verse_anisotropi
-00002bd0: 635f 7363 616c 696e 6728 7365 6c66 293a  c_scaling(self):
-00002be0: 0d0a 2020 2020 2020 2020 7061 6765 203d  ..        page =
-00002bf0: 2050 6167 6528 3130 3030 2c20 3130 3030   Page(1000, 1000
-00002c00: 290d 0a20 2020 2020 2020 2070 6167 652e  )..        page.
-00002c10: 7365 745f 7363 616c 696e 675f 706f 696e  set_scaling_poin
-00002c20: 7473 2856 6563 3228 3130 302c 2031 3030  ts(Vec2(100, 100
-00002c30: 292c 2056 6563 3228 3230 302c 2032 3030  ), Vec2(200, 200
-00002c40: 2929 0d0a 2020 2020 2020 2020 2320 7265  ))..        # re
-00002c50: 7665 7273 6520 7820 616e 6420 7920 6178  verse x and y ax
-00002c60: 6973 3a0d 0a20 2020 2020 2020 2070 6167  is:..        pag
-00002c70: 652e 7365 745f 616e 6973 6f74 726f 7069  e.set_anisotropi
-00002c80: 635f 7363 616c 696e 6728 3130 2c20 2d31  c_scaling(10, -1
-00002c90: 302c 2032 302c 202d 3230 290d 0a20 2020  0, 20, -20)..   
-00002ca0: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
-00002cb0: 2e75 7365 725f 7363 616c 696e 6720 6973  .user_scaling is
-00002cc0: 2054 7275 650d 0a20 2020 2020 2020 2061   True..        a
-00002cd0: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
-00002ce0: 706f 696e 7428 302c 2030 292e 6973 636c  point(0, 0).iscl
-00002cf0: 6f73 6528 2831 3530 2c20 3135 3029 290d  ose((150, 150)).
-00002d00: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-00002d10: 7061 6765 2e70 6167 655f 706f 696e 7428  page.page_point(
-00002d20: 3130 2c20 3230 292e 6973 636c 6f73 6528  10, 20).isclose(
-00002d30: 2831 3030 2c20 3130 3029 290d 0a20 2020  (100, 100))..   
-00002d40: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
-00002d50: 2e70 6167 655f 706f 696e 7428 2d31 302c  .page_point(-10,
-00002d60: 202d 3230 292e 6973 636c 6f73 6528 2832   -20).isclose((2
-00002d70: 3030 2c20 3230 3029 290d 0a0d 0a0d 0a63  00, 200))......c
-00002d80: 6c61 7373 2054 6573 7450 6167 6549 736f  lass TestPageIso
-00002d90: 7472 6f70 6963 5363 616c 696e 673a 0d0a  tropicScaling:..
-00002da0: 2020 2020 6465 6620 7465 7374 5f69 736f      def test_iso
-00002db0: 7472 6f70 6963 5f62 6f74 746f 6d5f 7769  tropic_bottom_wi
-00002dc0: 6e64 6f77 5f35 3028 7365 6c66 293a 0d0a  ndow_50(self):..
-00002dd0: 2020 2020 2020 2020 7061 6765 203d 2050          page = P
-00002de0: 6167 6528 3130 3030 2c20 3130 3030 290d  age(1000, 1000).
-00002df0: 0a20 2020 2020 2020 2070 6167 652e 7365  .        page.se
-00002e00: 745f 7363 616c 696e 675f 706f 696e 7473  t_scaling_points
-00002e10: 2856 6563 3228 3130 302c 2031 3030 292c  (Vec2(100, 100),
-00002e20: 2056 6563 3228 3230 302c 2032 3030 2929   Vec2(200, 200))
-00002e30: 0d0a 2020 2020 2020 2020 7061 6765 2e73  ..        page.s
-00002e40: 6574 5f69 736f 7472 6f70 6963 5f73 6361  et_isotropic_sca
-00002e50: 6c69 6e67 2830 2c20 3230 2c20 302c 2031  ling(0, 20, 0, 1
-00002e60: 3029 0d0a 2020 2020 2020 2020 6173 7365  0)..        asse
-00002e70: 7274 2070 6167 652e 7573 6572 5f73 6361  rt page.user_sca
-00002e80: 6c69 6e67 2069 7320 5472 7565 0d0a 2020  ling is True..  
-00002e90: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
-00002ea0: 652e 7061 6765 5f70 6f69 6e74 2830 2c20  e.page_point(0, 
-00002eb0: 3029 2e69 7363 6c6f 7365 2828 3130 302c  0).isclose((100,
-00002ec0: 2031 3235 2929 0d0a 2020 2020 2020 2020   125))..        
-00002ed0: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
-00002ee0: 5f70 6f69 6e74 2831 302c 2035 292e 6973  _point(10, 5).is
-00002ef0: 636c 6f73 6528 2831 3530 2c20 3135 3029  close((150, 150)
-00002f00: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00002f10: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
-00002f20: 7428 3230 2c20 3130 292e 6973 636c 6f73  t(20, 10).isclos
-00002f30: 6528 2832 3030 2c20 3137 3529 290d 0a0d  e((200, 175))...
-00002f40: 0a20 2020 2064 6566 2074 6573 745f 6973  .    def test_is
-00002f50: 6f74 726f 7069 635f 626f 7474 6f6d 5f77  otropic_bottom_w
-00002f60: 696e 646f 775f 3028 7365 6c66 293a 0d0a  indow_0(self):..
-00002f70: 2020 2020 2020 2020 7061 6765 203d 2050          page = P
-00002f80: 6167 6528 3130 3030 2c20 3130 3030 290d  age(1000, 1000).
-00002f90: 0a20 2020 2020 2020 2070 6167 652e 7365  .        page.se
-00002fa0: 745f 7363 616c 696e 675f 706f 696e 7473  t_scaling_points
-00002fb0: 2856 6563 3228 3130 302c 2031 3030 292c  (Vec2(100, 100),
-00002fc0: 2056 6563 3228 3230 302c 2032 3030 2929   Vec2(200, 200))
-00002fd0: 0d0a 2020 2020 2020 2020 7061 6765 2e73  ..        page.s
-00002fe0: 6574 5f69 736f 7472 6f70 6963 5f73 6361  et_isotropic_sca
-00002ff0: 6c69 6e67 2830 2c20 3230 2c20 302c 2031  ling(0, 20, 0, 1
-00003000: 302c 2030 2c20 3029 0d0a 2020 2020 2020  0, 0, 0)..      
-00003010: 2020 6173 7365 7274 2070 6167 652e 7061    assert page.pa
-00003020: 6765 5f70 6f69 6e74 2830 2c20 3029 2e69  ge_point(0, 0).i
-00003030: 7363 6c6f 7365 2828 3130 302c 2031 3030  sclose((100, 100
-00003040: 2929 0d0a 2020 2020 2020 2020 6173 7365  ))..        asse
-00003050: 7274 2070 6167 652e 7061 6765 5f70 6f69  rt page.page_poi
-00003060: 6e74 2831 302c 2035 292e 6973 636c 6f73  nt(10, 5).isclos
-00003070: 6528 2831 3530 2c20 3132 3529 290d 0a20  e((150, 125)).. 
-00003080: 2020 2020 2020 2061 7373 6572 7420 7061         assert pa
-00003090: 6765 2e70 6167 655f 706f 696e 7428 3230  ge.page_point(20
-000030a0: 2c20 3130 292e 6973 636c 6f73 6528 2832  , 10).isclose((2
-000030b0: 3030 2c20 3135 3029 290d 0a0d 0a20 2020  00, 150))....   
-000030c0: 2064 6566 2074 6573 745f 6973 6f74 726f   def test_isotro
-000030d0: 7069 635f 626f 7474 6f6d 5f77 696e 646f  pic_bottom_windo
-000030e0: 775f 3130 3028 7365 6c66 293a 0d0a 2020  w_100(self):..  
-000030f0: 2020 2020 2020 7061 6765 203d 2050 6167        page = Pag
-00003100: 6528 3130 3030 2c20 3130 3030 290d 0a20  e(1000, 1000).. 
-00003110: 2020 2020 2020 2070 6167 652e 7365 745f         page.set_
-00003120: 7363 616c 696e 675f 706f 696e 7473 2856  scaling_points(V
-00003130: 6563 3228 3130 302c 2031 3030 292c 2056  ec2(100, 100), V
-00003140: 6563 3228 3230 302c 2032 3030 2929 0d0a  ec2(200, 200))..
-00003150: 2020 2020 2020 2020 7061 6765 2e73 6574          page.set
-00003160: 5f69 736f 7472 6f70 6963 5f73 6361 6c69  _isotropic_scali
-00003170: 6e67 2830 2c20 3230 2c20 302c 2031 302c  ng(0, 20, 0, 10,
-00003180: 2031 2c20 3129 0d0a 2020 2020 2020 2020   1, 1)..        
-00003190: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
-000031a0: 5f70 6f69 6e74 2830 2c20 3029 2e69 7363  _point(0, 0).isc
-000031b0: 6c6f 7365 2828 3130 302c 2031 3530 2929  lose((100, 150))
-000031c0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-000031d0: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
-000031e0: 2831 302c 2035 292e 6973 636c 6f73 6528  (10, 5).isclose(
-000031f0: 2831 3530 2c20 3137 3529 290d 0a20 2020  (150, 175))..   
-00003200: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
-00003210: 2e70 6167 655f 706f 696e 7428 3230 2c20  .page_point(20, 
-00003220: 3130 292e 6973 636c 6f73 6528 2832 3030  10).isclose((200
-00003230: 2c20 3230 3029 290d 0a0d 0a20 2020 2064  , 200))....    d
-00003240: 6566 2074 6573 745f 6973 6f74 726f 7069  ef test_isotropi
-00003250: 635f 6c65 6674 5f77 696e 646f 775f 3530  c_left_window_50
-00003260: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00003270: 2070 6167 6520 3d20 5061 6765 2831 3030   page = Page(100
-00003280: 302c 2031 3030 3029 0d0a 2020 2020 2020  0, 1000)..      
-00003290: 2020 7061 6765 2e73 6574 5f73 6361 6c69    page.set_scali
-000032a0: 6e67 5f70 6f69 6e74 7328 5665 6332 2831  ng_points(Vec2(1
-000032b0: 3030 2c20 3130 3029 2c20 5665 6332 2832  00, 100), Vec2(2
-000032c0: 3030 2c20 3230 3029 290d 0a20 2020 2020  00, 200))..     
-000032d0: 2020 2070 6167 652e 7365 745f 6973 6f74     page.set_isot
-000032e0: 726f 7069 635f 7363 616c 696e 6728 302c  ropic_scaling(0,
-000032f0: 2031 302c 2030 2c20 3230 290d 0a20 2020   10, 0, 20)..   
-00003300: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
-00003310: 2e70 6167 655f 706f 696e 7428 302c 2030  .page_point(0, 0
-00003320: 292e 6973 636c 6f73 6528 2831 3235 2c20  ).isclose((125, 
-00003330: 3130 3029 290d 0a20 2020 2020 2020 2061  100))..        a
-00003340: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
-00003350: 706f 696e 7428 352c 2031 3029 2e69 7363  point(5, 10).isc
-00003360: 6c6f 7365 2828 3135 302c 2031 3530 2929  lose((150, 150))
-00003370: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
-00003380: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
-00003390: 2831 302c 2032 3029 2e69 7363 6c6f 7365  (10, 20).isclose
-000033a0: 2828 3137 352c 2032 3030 2929 0d0a 0d0a  ((175, 200))....
-000033b0: 2020 2020 6465 6620 7465 7374 5f69 736f      def test_iso
-000033c0: 7472 6f70 6963 5f6c 6566 745f 7769 6e64  tropic_left_wind
-000033d0: 6f77 5f30 2873 656c 6629 3a0d 0a20 2020  ow_0(self):..   
-000033e0: 2020 2020 2070 6167 6520 3d20 5061 6765       page = Page
-000033f0: 2831 3030 302c 2031 3030 3029 0d0a 2020  (1000, 1000)..  
-00003400: 2020 2020 2020 7061 6765 2e73 6574 5f73        page.set_s
-00003410: 6361 6c69 6e67 5f70 6f69 6e74 7328 5665  caling_points(Ve
-00003420: 6332 2831 3030 2c20 3130 3029 2c20 5665  c2(100, 100), Ve
-00003430: 6332 2832 3030 2c20 3230 3029 290d 0a20  c2(200, 200)).. 
-00003440: 2020 2020 2020 2070 6167 652e 7365 745f         page.set_
-00003450: 6973 6f74 726f 7069 635f 7363 616c 696e  isotropic_scalin
-00003460: 6728 302c 2031 302c 2030 2c20 3230 2c20  g(0, 10, 0, 20, 
-00003470: 302c 2030 290d 0a20 2020 2020 2020 2061  0, 0)..        a
-00003480: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
-00003490: 706f 696e 7428 302c 2030 292e 6973 636c  point(0, 0).iscl
-000034a0: 6f73 6528 2831 3030 2c20 3130 3029 290d  ose((100, 100)).
-000034b0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
-000034c0: 7061 6765 2e70 6167 655f 706f 696e 7428  page.page_point(
-000034d0: 352c 2031 3029 2e69 7363 6c6f 7365 2828  5, 10).isclose((
-000034e0: 3132 352c 2031 3530 2929 0d0a 2020 2020  125, 150))..    
-000034f0: 2020 2020 6173 7365 7274 2070 6167 652e      assert page.
-00003500: 7061 6765 5f70 6f69 6e74 2831 302c 2032  page_point(10, 2
-00003510: 3029 2e69 7363 6c6f 7365 2828 3135 302c  0).isclose((150,
-00003520: 2032 3030 2929 0d0a 0d0a 2020 2020 6465   200))....    de
-00003530: 6620 7465 7374 5f69 736f 7472 6f70 6963  f test_isotropic
-00003540: 5f6c 6566 745f 7769 6e64 6f77 5f31 3030  _left_window_100
-00003550: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
-00003560: 2070 6167 6520 3d20 5061 6765 2831 3030   page = Page(100
-00003570: 302c 2031 3030 3029 0d0a 2020 2020 2020  0, 1000)..      
-00003580: 2020 7061 6765 2e73 6574 5f73 6361 6c69    page.set_scali
-00003590: 6e67 5f70 6f69 6e74 7328 5665 6332 2831  ng_points(Vec2(1
-000035a0: 3030 2c20 3130 3029 2c20 5665 6332 2832  00, 100), Vec2(2
-000035b0: 3030 2c20 3230 3029 290d 0a20 2020 2020  00, 200))..     
-000035c0: 2020 2070 6167 652e 7365 745f 6973 6f74     page.set_isot
-000035d0: 726f 7069 635f 7363 616c 696e 6728 302c  ropic_scaling(0,
-000035e0: 2031 302c 2030 2c20 3230 2c20 312c 2031   10, 0, 20, 1, 1
-000035f0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00003600: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
-00003610: 7428 302c 2030 292e 6973 636c 6f73 6528  t(0, 0).isclose(
-00003620: 2831 3530 2c20 3130 3029 290d 0a20 2020  (150, 100))..   
-00003630: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
-00003640: 2e70 6167 655f 706f 696e 7428 352c 2031  .page_point(5, 1
-00003650: 3029 2e69 7363 6c6f 7365 2828 3137 352c  0).isclose((175,
-00003660: 2031 3530 2929 0d0a 2020 2020 2020 2020   150))..        
-00003670: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
-00003680: 5f70 6f69 6e74 2831 302c 2032 3029 2e69  _point(10, 20).i
-00003690: 7363 6c6f 7365 2828 3230 302c 2032 3030  sclose((200, 200
-000036a0: 2929 0d0a 0d0a 0d0a 6465 6620 7465 7374  ))......def test
-000036b0: 5f61 7263 5f61 6e67 6c65 7328 293a 0d0a  _arc_angles():..
-000036c0: 2020 2020 6672 6f6d 2065 7a64 7866 2e61      from ezdxf.a
-000036d0: 6464 6f6e 732e 6870 676c 322e 706c 6f74  ddons.hpgl2.plot
-000036e0: 7465 7220 696d 706f 7274 2061 7263 5f61  ter import arc_a
-000036f0: 6e67 6c65 730d 0a0d 0a20 2020 2061 6e67  ngles....    ang
-00003700: 6c65 7320 3d20 6c69 7374 2861 7263 5f61  les = list(arc_a
-00003710: 6e67 6c65 7328 302c 2033 3630 2c20 3529  ngles(0, 360, 5)
-00003720: 290d 0a20 2020 2061 7373 6572 7420 6c65  )..    assert le
-00003730: 6e28 616e 676c 6573 2920 3d3d 2037 330d  n(angles) == 73.
-00003740: 0a20 2020 2061 7373 6572 7420 616e 676c  .    assert angl
-00003750: 6573 5b2d 315d 203d 3d20 7079 7465 7374  es[-1] == pytest
-00003760: 2e61 7070 726f 7828 3336 3029 0d0a 0d0a  .approx(360)....
-00003770: 2020 2020 616e 676c 6573 203d 206c 6973      angles = lis
-00003780: 7428 6172 635f 616e 676c 6573 2830 2c20  t(arc_angles(0, 
-00003790: 2d33 3630 2c20 3529 290d 0a20 2020 2061  -360, 5))..    a
-000037a0: 7373 6572 7420 6c65 6e28 616e 676c 6573  ssert len(angles
-000037b0: 2920 3d3d 2037 330d 0a20 2020 2061 7373  ) == 73..    ass
-000037c0: 6572 7420 616e 676c 6573 5b2d 315d 203d  ert angles[-1] =
-000037d0: 3d20 7079 7465 7374 2e61 7070 726f 7828  = pytest.approx(
-000037e0: 2d33 3630 290d 0a0d 0a0d 0a64 6566 2074  -360)......def t
-000037f0: 6573 745f 7377 6565 7069 6e67 5f61 6e67  est_sweeping_ang
-00003800: 6c65 2829 3a0d 0a20 2020 2066 726f 6d20  le():..    from 
-00003810: 657a 6478 662e 6164 646f 6e73 2e68 7067  ezdxf.addons.hpg
-00003820: 6c32 2e70 6c6f 7474 6572 2069 6d70 6f72  l2.plotter impor
-00003830: 7420 7377 6565 7069 6e67 5f61 6e67 6c65  t sweeping_angle
-00003840: 0d0a 0d0a 2020 2020 6173 7365 7274 2073  ....    assert s
-00003850: 7765 6570 696e 675f 616e 676c 6528 302c  weeping_angle(0,
-00003860: 2034 352c 2039 3029 203d 3d20 3930 0d0a   45, 90) == 90..
-00003870: 2020 2020 6173 7365 7274 2073 7765 6570      assert sweep
-00003880: 696e 675f 616e 676c 6528 3930 2c20 3435  ing_angle(90, 45
-00003890: 2c20 3029 203d 3d20 2d39 300d 0a20 2020  , 0) == -90..   
-000038a0: 2061 7373 6572 7420 7377 6565 7069 6e67   assert sweeping
-000038b0: 5f61 6e67 6c65 2833 3330 2c20 302c 2033  _angle(330, 0, 3
-000038c0: 3029 203d 3d20 3630 0d0a 2020 2020 6173  0) == 60..    as
-000038d0: 7365 7274 2073 7765 6570 696e 675f 616e  sert sweeping_an
-000038e0: 676c 6528 3333 302c 2031 3830 2c20 3330  gle(330, 180, 30
-000038f0: 2920 3d3d 202d 3330 300d 0a20 2020 2061  ) == -300..    a
-00003900: 7373 6572 7420 7377 6565 7069 6e67 5f61  ssert sweeping_a
-00003910: 6e67 6c65 2833 302c 2030 2c20 3333 3029  ngle(30, 0, 330)
-00003920: 203d 3d20 2d36 300d 0a20 2020 2061 7373   == -60..    ass
-00003930: 6572 7420 7377 6565 7069 6e67 5f61 6e67  ert sweeping_ang
-00003940: 6c65 2833 302c 2031 3830 2c20 3333 3029  le(30, 180, 330)
-00003950: 203d 3d20 3330 300d 0a0d 0a0d 0a63 6c61   == 300......cla
-00003960: 7373 2054 6573 7450 6c61 6365 6d65 6e74  ss TestPlacement
-00003970: 4d61 7472 6978 3a0d 0a20 2020 2064 6566  Matrix:..    def
-00003980: 2074 6573 745f 7368 6966 745f 746f 5f6f   test_shift_to_o
-00003990: 7269 6769 6e5f 5131 2873 656c 6629 3a0d  rigin_Q1(self):.
-000039a0: 0a20 2020 2020 2020 2062 626f 7820 3d20  .        bbox = 
-000039b0: 426f 756e 6469 6e67 426f 7832 6428 5b28  BoundingBox2d([(
-000039c0: 3130 2c20 3130 292c 2028 3230 2c20 3230  10, 10), (20, 20
-000039d0: 295d 290d 0a20 2020 2020 2020 206d 203d  )])..        m =
-000039e0: 2070 6c61 6365 6d65 6e74 5f6d 6174 7269   placement_matri
-000039f0: 7828 6262 6f78 290d 0a20 2020 2020 2020  x(bbox)..       
-00003a00: 2061 7373 6572 7420 6d2e 7472 616e 7366   assert m.transf
-00003a10: 6f72 6d28 2831 302c 2031 3029 292e 6973  orm((10, 10)).is
-00003a20: 636c 6f73 6528 2830 2c20 3029 290d 0a20  close((0, 0)).. 
-00003a30: 2020 2020 2020 2061 7373 6572 7420 6d2e         assert m.
-00003a40: 7472 616e 7366 6f72 6d28 2832 302c 2032  transform((20, 2
-00003a50: 3029 292e 6973 636c 6f73 6528 2831 302c  0)).isclose((10,
-00003a60: 2031 3029 290d 0a0d 0a20 2020 2064 6566   10))....    def
-00003a70: 2074 6573 745f 7368 6966 745f 746f 5f6f   test_shift_to_o
-00003a80: 7269 6769 6e5f 5133 2873 656c 6629 3a0d  rigin_Q3(self):.
-00003a90: 0a20 2020 2020 2020 2062 626f 7820 3d20  .        bbox = 
-00003aa0: 426f 756e 6469 6e67 426f 7832 6428 5b28  BoundingBox2d([(
-00003ab0: 2d31 302c 202d 3130 292c 2028 2d32 302c  -10, -10), (-20,
-00003ac0: 202d 3230 295d 290d 0a20 2020 2020 2020   -20)])..       
-00003ad0: 206d 203d 2070 6c61 6365 6d65 6e74 5f6d   m = placement_m
-00003ae0: 6174 7269 7828 6262 6f78 290d 0a20 2020  atrix(bbox)..   
-00003af0: 2020 2020 2061 7373 6572 7420 6d2e 7472       assert m.tr
-00003b00: 616e 7366 6f72 6d28 282d 3130 2c20 2d31  ansform((-10, -1
-00003b10: 3029 292e 6973 636c 6f73 6528 2831 302c  0)).isclose((10,
-00003b20: 2031 3029 290d 0a20 2020 2020 2020 2061   10))..        a
-00003b30: 7373 6572 7420 6d2e 7472 616e 7366 6f72  ssert m.transfor
-00003b40: 6d28 282d 3230 2c20 2d32 3029 292e 6973  m((-20, -20)).is
-00003b50: 636c 6f73 6528 2830 2c20 3029 290d 0a0d  close((0, 0))...
-00003b60: 0a20 2020 2064 6566 2074 6573 745f 726f  .    def test_ro
-00003b70: 7461 7465 2873 656c 6629 3a0d 0a20 2020  tate(self):..   
-00003b80: 2020 2020 2023 2073 697a 6520 3d20 3130       # size = 10
-00003b90: 2078 2033 300d 0a20 2020 2020 2020 2062   x 30..        b
-00003ba0: 626f 7820 3d20 426f 756e 6469 6e67 426f  box = BoundingBo
-00003bb0: 7832 6428 5b28 3130 2c20 3130 292c 2028  x2d([(10, 10), (
-00003bc0: 3230 2c20 3430 295d 290d 0a20 2020 2020  20, 40)])..     
-00003bd0: 2020 206d 203d 2070 6c61 6365 6d65 6e74     m = placement
-00003be0: 5f6d 6174 7269 7828 6262 6f78 2c20 726f  _matrix(bbox, ro
-00003bf0: 7461 7469 6f6e 3d39 3029 0d0a 2020 2020  tation=90)..    
-00003c00: 2020 2020 6173 7365 7274 206d 2e74 7261      assert m.tra
-00003c10: 6e73 666f 726d 2828 3130 2c20 3130 2929  nsform((10, 10))
-00003c20: 2e69 7363 6c6f 7365 2828 3330 2c20 3029  .isclose((30, 0)
-00003c30: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
-00003c40: 7420 6d2e 7472 616e 7366 6f72 6d28 2832  t m.transform((2
-00003c50: 302c 2034 3029 292e 6973 636c 6f73 6528  0, 40)).isclose(
-00003c60: 2830 2c20 3130 2929 0d0a 0d0a 0d0a 6966  (0, 10))......if
-00003c70: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
-00003c80: 6d61 696e 5f5f 223a 0d0a 2020 2020 7079  main__":..    py
-00003c90: 7465 7374 2e6d 6169 6e28 5b5f 5f66 696c  test.main([__fil
-00003ca0: 655f 5f5d 290d 0a                        e__])..
+00000500: 2064 6566 2064 7261 775f 7061 7468 7328   def draw_paths(
+00000510: 7365 6c66 2c20 7072 6f70 6572 7469 6573  self, properties
+00000520: 2c20 7061 7468 732c 2066 696c 6c65 643a  , paths, filled:
+00000530: 2062 6f6f 6c29 202d 3e20 4e6f 6e65 3a0d   bool) -> None:.
+00000540: 0a20 2020 2020 2020 2069 6620 6669 6c6c  .        if fill
+00000550: 6564 3a0d 0a20 2020 2020 2020 2020 2020  ed:..           
+00000560: 2073 656c 662e 7265 7375 6c74 2e61 7070   self.result.app
+00000570: 656e 6428 5b22 4669 6c6c 6564 5061 7468  end(["FilledPath
+00000580: 222c 2070 6174 6873 5d29 0d0a 2020 2020  ", paths])..    
+00000590: 2020 2020 656c 7365 3a0d 0a20 2020 2020      else:..     
+000005a0: 2020 2020 2020 2073 656c 662e 7265 7375         self.resu
+000005b0: 6c74 2e61 7070 656e 6428 5b22 4f75 746c  lt.append(["Outl
+000005c0: 696e 6550 6174 6822 2c20 7061 7468 735d  inePath", paths]
+000005d0: 290d 0a0d 0a0d 0a64 6566 2070 6c6f 7428  )......def plot(
+000005e0: 733a 2062 7974 6573 293a 0d0a 2020 2020  s: bytes):..    
+000005f0: 636f 6d6d 616e 6473 203d 2061 7069 2e68  commands = api.h
+00000600: 7067 6c32 5f63 6f6d 6d61 6e64 7328 6870  pgl2_commands(hp
+00000610: 676c 3228 7329 290d 0a20 2020 2062 6163  gl2(s))..    bac
+00000620: 6b65 6e64 203d 204d 7942 6163 6b65 6e64  kend = MyBackend
+00000630: 2829 0d0a 2020 2020 6170 692e 506c 6f74  ()..    api.Plot
+00000640: 7465 7228 6261 636b 656e 6429 0d0a 2020  ter(backend)..  
+00000650: 2020 706c 6f74 7465 7220 3d20 6170 692e    plotter = api.
+00000660: 506c 6f74 7465 7228 6261 636b 656e 6429  Plotter(backend)
+00000670: 0d0a 2020 2020 696e 7465 7270 7265 7465  ..    interprete
+00000680: 7220 3d20 6170 692e 496e 7465 7270 7265  r = api.Interpre
+00000690: 7465 7228 706c 6f74 7465 7229 0d0a 2020  ter(plotter)..  
+000006a0: 2020 696e 7465 7270 7265 7465 722e 7275    interpreter.ru
+000006b0: 6e28 636f 6d6d 616e 6473 290d 0a20 2020  n(commands)..   
+000006c0: 2072 6574 7572 6e20 696e 7465 7270 7265   return interpre
+000006d0: 7465 720d 0a0d 0a0d 0a64 6566 2067 6574  ter......def get
+000006e0: 5f72 6573 756c 7428 706c 6f74 7465 7229  _result(plotter)
+000006f0: 3a0d 0a20 2020 2072 6574 7572 6e20 706c  :..    return pl
+00000700: 6f74 7465 722e 6261 636b 656e 642e 7265  otter.backend.re
+00000710: 7375 6c74 0d0a 0d0a 0d0a 636c 6173 7320  sult......class 
+00000720: 5465 7374 5265 6e64 6572 456e 6769 6e65  TestRenderEngine
+00000730: 3a0d 0a20 2020 2040 7079 7465 7374 2e6d  :..    @pytest.m
+00000740: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+00000750: 2263 6d64 222c 205b 6222 5044 3b50 4132  "cmd", [b"PD;PA2
+00000760: 3030 302c 3830 3030 3b22 2c20 6222 5055  000,8000;", b"PU
+00000770: 3b50 4132 3030 302c 3830 3030 3b22 5d29  ;PA2000,8000;"])
+00000780: 0d0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
+00000790: 656e 5f61 6273 6f6c 7574 6528 7365 6c66  en_absolute(self
+000007a0: 2c20 636d 6429 3a0d 0a20 2020 2020 2020  , cmd):..       
+000007b0: 2069 7020 3d20 706c 6f74 2863 6d64 290d   ip = plot(cmd).
+000007c0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000007d0: 6970 2e70 6c6f 7474 6572 2e75 7365 725f  ip.plotter.user_
+000007e0: 6c6f 6361 7469 6f6e 203d 3d20 5665 6332  location == Vec2
+000007f0: 2832 3030 302c 2038 3030 3029 0d0a 0d0a  (2000, 8000)....
+00000800: 2020 2020 6465 6620 7465 7374 5f73 656c      def test_sel
+00000810: 6563 745f 7065 6e28 7365 6c66 293a 0d0a  ect_pen(self):..
+00000820: 2020 2020 2020 2020 6970 203d 2070 6c6f          ip = plo
+00000830: 7428 6222 5350 373b 2229 0d0a 2020 2020  t(b"SP7;")..    
+00000840: 2020 2020 6173 7365 7274 2069 702e 706c      assert ip.pl
+00000850: 6f74 7465 722e 7072 6f70 6572 7469 6573  otter.properties
+00000860: 2e70 656e 5f69 6e64 6578 203d 3d20 370d  .pen_index == 7.
+00000870: 0a0d 0a20 2020 2020 2020 2069 7020 3d20  ...        ip = 
+00000880: 706c 6f74 2862 2250 4333 2c32 302c 3330  plot(b"PC3,20,30
+00000890: 2c34 303b 5057 302e 3138 2c33 3b53 5033  ,40;PW0.18,3;SP3
+000008a0: 3b22 290d 0a20 2020 2020 2020 2070 726f  ;")..        pro
+000008b0: 7065 7274 6965 7320 3d20 6970 2e70 6c6f  perties = ip.plo
+000008c0: 7474 6572 2e70 726f 7065 7274 6965 730d  tter.properties.
+000008d0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000008e0: 7072 6f70 6572 7469 6573 2e70 656e 5f69  properties.pen_i
+000008f0: 6e64 6578 203d 3d20 330d 0a20 2020 2020  ndex == 3..     
+00000900: 2020 2061 7373 6572 7420 7072 6f70 6572     assert proper
+00000910: 7469 6573 2e70 656e 5f77 6964 7468 203d  ties.pen_width =
+00000920: 3d20 302e 3138 0d0a 2020 2020 2020 2020  = 0.18..        
+00000930: 6173 7365 7274 2070 726f 7065 7274 6965  assert propertie
+00000940: 732e 7065 6e5f 636f 6c6f 7220 3d3d 2052  s.pen_color == R
+00000950: 4742 2832 302c 2033 302c 2034 3029 0d0a  GB(20, 30, 40)..
+00000960: 0d0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
+00000970: 6574 5f70 656e 5f77 6964 7468 2873 656c  et_pen_width(sel
+00000980: 6629 3a0d 0a20 2020 2020 2020 2069 7020  f):..        ip 
+00000990: 3d20 706c 6f74 2862 2250 5730 2e31 382c  = plot(b"PW0.18,
+000009a0: 323b 2229 0d0a 2020 2020 2020 2020 7072  2;")..        pr
+000009b0: 6f70 6572 7469 6573 203d 2069 702e 706c  operties = ip.pl
+000009c0: 6f74 7465 722e 7072 6f70 6572 7469 6573  otter.properties
+000009d0: 0d0a 0d0a 2020 2020 2020 2020 6173 7365  ....        asse
+000009e0: 7274 2070 726f 7065 7274 6965 732e 7065  rt properties.pe
+000009f0: 6e5f 7769 6474 6820 3d3d 2070 726f 7065  n_width == prope
+00000a00: 7274 6965 732e 4445 4641 554c 545f 5045  rties.DEFAULT_PE
+00000a10: 4e2e 7769 6474 680d 0a20 2020 2020 2020  N.width..       
+00000a20: 2070 656e 203d 2070 726f 7065 7274 6965   pen = propertie
+00000a30: 732e 6765 745f 7065 6e28 3229 0d0a 2020  s.get_pen(2)..  
+00000a40: 2020 2020 2020 6173 7365 7274 2070 656e        assert pen
+00000a50: 2e77 6964 7468 203d 3d20 302e 3138 0d0a  .width == 0.18..
+00000a60: 0d0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
+00000a70: 6574 5f63 7572 7265 6e74 5f70 656e 5f77  et_current_pen_w
+00000a80: 6964 7468 2873 656c 6629 3a0d 0a20 2020  idth(self):..   
+00000a90: 2020 2020 2069 7020 3d20 706c 6f74 2862       ip = plot(b
+00000aa0: 2250 5730 2e31 383b 2229 0d0a 2020 2020  "PW0.18;")..    
+00000ab0: 2020 2020 6173 7365 7274 2069 702e 706c      assert ip.pl
+00000ac0: 6f74 7465 722e 7072 6f70 6572 7469 6573  otter.properties
+00000ad0: 2e70 656e 5f77 6964 7468 203d 3d20 302e  .pen_width == 0.
+00000ae0: 3138 0d0a 0d0a 2020 2020 6465 6620 7465  18....    def te
+00000af0: 7374 5f73 6574 5f70 656e 5f63 6f6c 6f72  st_set_pen_color
+00000b00: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+00000b10: 2069 7020 3d20 706c 6f74 2862 2250 4332   ip = plot(b"PC2
+00000b20: 2c32 302c 3330 2c34 303b 2229 0d0a 2020  ,20,30,40;")..  
+00000b30: 2020 2020 2020 7065 6e20 3d20 6970 2e70        pen = ip.p
+00000b40: 6c6f 7474 6572 2e70 726f 7065 7274 6965  lotter.propertie
+00000b50: 732e 6765 745f 7065 6e28 3229 0d0a 2020  s.get_pen(2)..  
+00000b60: 2020 2020 2020 6173 7365 7274 2070 656e        assert pen
+00000b70: 2e63 6f6c 6f72 203d 3d20 5247 4228 3230  .color == RGB(20
+00000b80: 2c20 3330 2c20 3430 290d 0a20 2020 2020  , 30, 40)..     
+00000b90: 2020 2061 7373 6572 7420 280d 0a20 2020     assert (..   
+00000ba0: 2020 2020 2020 2020 2069 702e 706c 6f74           ip.plot
+00000bb0: 7465 722e 7072 6f70 6572 7469 6573 2e70  ter.properties.p
+00000bc0: 656e 5f63 6f6c 6f72 203d 3d20 6970 2e70  en_color == ip.p
+00000bd0: 6c6f 7474 6572 2e70 726f 7065 7274 6965  lotter.propertie
+00000be0: 732e 4445 4641 554c 545f 5045 4e2e 636f  s.DEFAULT_PEN.co
+00000bf0: 6c6f 720d 0a20 2020 2020 2020 2029 0d0a  lor..        )..
+00000c00: 0d0a 2020 2020 6465 6620 7465 7374 5f73  ..    def test_s
+00000c10: 6574 5f66 696c 6c5f 7479 7065 5f68 6174  et_fill_type_hat
+00000c20: 6368 696e 6728 7365 6c66 293a 0d0a 2020  ching(self):..  
+00000c30: 2020 2020 2020 6970 203d 2070 6c6f 7428        ip = plot(
+00000c40: 6222 4654 332c 3830 2c34 353b 2229 0d0a  b"FT3,80,45;")..
+00000c50: 2020 2020 2020 2020 7072 6f70 7320 3d20          props = 
+00000c60: 6970 2e70 6c6f 7474 6572 2e70 726f 7065  ip.plotter.prope
+00000c70: 7274 6965 730d 0a20 2020 2020 2020 2061  rties..        a
+00000c80: 7373 6572 7420 7072 6f70 732e 6669 6c6c  ssert props.fill
+00000c90: 5f74 7970 6520 3d3d 2046 696c 6c54 7970  _type == FillTyp
+00000ca0: 652e 4841 5443 4849 4e47 0d0a 2020 2020  e.HATCHING..    
+00000cb0: 2020 2020 6173 7365 7274 2070 726f 7073      assert props
+00000cc0: 2e66 696c 6c5f 6861 7463 685f 6c69 6e65  .fill_hatch_line
+00000cd0: 5f73 7061 6369 6e67 203d 3d20 3830 0d0a  _spacing == 80..
+00000ce0: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
+00000cf0: 726f 7073 2e66 696c 6c5f 6861 7463 685f  rops.fill_hatch_
+00000d00: 6c69 6e65 5f61 6e67 6c65 203d 3d20 3435  line_angle == 45
+00000d10: 0d0a 0d0a 2020 2020 6465 6620 7465 7374  ....    def test
+00000d20: 5f73 6574 5f66 696c 6c5f 7479 7065 5f73  _set_fill_type_s
+00000d30: 6861 6469 6e67 2873 656c 6629 3a0d 0a20  hading(self):.. 
+00000d40: 2020 2020 2020 2069 7020 3d20 706c 6f74         ip = plot
+00000d50: 2862 2246 5431 302c 3337 3b22 290d 0a20  (b"FT10,37;").. 
+00000d60: 2020 2020 2020 2070 726f 7073 203d 2069         props = i
+00000d70: 702e 706c 6f74 7465 722e 7072 6f70 6572  p.plotter.proper
+00000d80: 7469 6573 0d0a 2020 2020 2020 2020 6173  ties..        as
+00000d90: 7365 7274 2070 726f 7073 2e66 696c 6c5f  sert props.fill_
+00000da0: 7479 7065 203d 3d20 4669 6c6c 5479 7065  type == FillType
+00000db0: 2e53 4841 4449 4e47 0d0a 2020 2020 2020  .SHADING..      
+00000dc0: 2020 6173 7365 7274 2070 726f 7073 2e66    assert props.f
+00000dd0: 696c 6c5f 7368 6164 696e 675f 6465 6e73  ill_shading_dens
+00000de0: 6974 7920 3d3d 2033 370d 0a0d 0a20 2020  ity == 37....   
+00000df0: 2064 6566 2074 6573 745f 7065 6e5f 7265   def test_pen_re
+00000e00: 6c61 7469 7665 2873 656c 6629 3a0d 0a20  lative(self):.. 
+00000e10: 2020 2020 2020 2069 7020 3d20 706c 6f74         ip = plot
+00000e20: 2862 2250 4131 3030 302c 3130 3030 3b50  (b"PA1000,1000;P
+00000e30: 5235 3030 2c2d 3530 303b 2229 0d0a 2020  R500,-500;")..  
+00000e40: 2020 2020 2020 6173 7365 7274 2069 702e        assert ip.
+00000e50: 706c 6f74 7465 722e 7573 6572 5f6c 6f63  plotter.user_loc
+00000e60: 6174 696f 6e20 3d3d 2056 6563 3228 3135  ation == Vec2(15
+00000e70: 3030 2c20 3530 3029 0d0a 0d0a 2020 2020  00, 500)....    
+00000e80: 6465 6620 7465 7374 5f70 6f6c 796c 696e  def test_polylin
+00000e90: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
+00000ea0: 2020 6970 203d 2070 6c6f 7428 6222 5044    ip = plot(b"PD
+00000eb0: 3230 3030 2c38 3030 302c 3430 3030 2c32  2000,8000,4000,2
+00000ec0: 3030 302c 3530 3030 2c35 3030 303b 2229  000,5000,5000;")
+00000ed0: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+00000ee0: 6420 3d20 6765 745f 7265 7375 6c74 2869  d = get_result(i
+00000ef0: 702e 706c 6f74 7465 7229 5b30 5d0d 0a20  p.plotter)[0].. 
+00000f00: 2020 2020 2020 2061 7373 6572 7420 636f         assert co
+00000f10: 6d6d 616e 645b 305d 203d 3d20 2250 6f6c  mmand[0] == "Pol
+00000f20: 796c 696e 6522 0d0a 2020 2020 2020 2020  yline"..        
+00000f30: 706f 696e 7473 203d 2063 6f6d 6d61 6e64  points = command
+00000f40: 5b31 5d0d 0a20 2020 2020 2020 2061 7373  [1]..        ass
+00000f50: 6572 7420 6c65 6e28 706f 696e 7473 2920  ert len(points) 
+00000f60: 3d3d 2034 0d0a 2020 2020 2020 2020 6173  == 4..        as
+00000f70: 7365 7274 2070 6f69 6e74 735b 305d 203d  sert points[0] =
+00000f80: 3d20 5665 6332 2830 2c20 3029 0d0a 2020  = Vec2(0, 0)..  
+00000f90: 2020 2020 2020 6173 7365 7274 2070 6f69        assert poi
+00000fa0: 6e74 735b 335d 203d 3d20 5665 6332 2835  nts[3] == Vec2(5
+00000fb0: 3030 302c 2035 3030 3029 0d0a 2020 2020  000, 5000)..    
+00000fc0: 2020 2020 6173 7365 7274 2069 702e 706c      assert ip.pl
+00000fd0: 6f74 7465 722e 7573 6572 5f6c 6f63 6174  otter.user_locat
+00000fe0: 696f 6e20 3d3d 2056 6563 3228 3530 3030  ion == Vec2(5000
+00000ff0: 2c20 3530 3030 290d 0a0d 0a20 2020 2064  , 5000)....    d
+00001000: 6566 2074 6573 745f 6375 6269 635f 6265  ef test_cubic_be
+00001010: 7a69 6572 5f63 7572 7665 5f70 656e 5f64  zier_curve_pen_d
+00001020: 6f77 6e28 7365 6c66 293a 0d0a 2020 2020  own(self):..    
+00001030: 2020 2020 6970 203d 2070 6c6f 7428 6222      ip = plot(b"
+00001040: 5044 3b42 5a32 3030 302c 3830 3030 2c34  PD;BZ2000,8000,4
+00001050: 3030 302c 3230 3030 2c35 3030 302c 3530  000,2000,5000,50
+00001060: 3030 3b22 290d 0a20 2020 2020 2020 2063  00;")..        c
+00001070: 6f6d 6d61 6e64 203d 2067 6574 5f72 6573  ommand = get_res
+00001080: 756c 7428 6970 2e70 6c6f 7474 6572 295b  ult(ip.plotter)[
+00001090: 305d 0d0a 2020 2020 2020 2020 6173 7365  0]..        asse
+000010a0: 7274 2063 6f6d 6d61 6e64 5b30 5d20 3d3d  rt command[0] ==
+000010b0: 2022 4f75 746c 696e 6550 6174 6822 0d0a   "OutlinePath"..
+000010c0: 0d0a 2020 2020 2020 2020 7061 7468 7320  ..        paths 
+000010d0: 3d20 636f 6d6d 616e 645b 315d 0d0a 2020  = command[1]..  
+000010e0: 2020 2020 2020 7061 7468 3020 3d20 7061        path0 = pa
+000010f0: 7468 735b 305d 0d0a 2020 2020 2020 2020  ths[0]..        
+00001100: 6173 7365 7274 2070 6174 6830 2e73 7461  assert path0.sta
+00001110: 7274 203d 3d20 5665 6332 2830 2c20 3029  rt == Vec2(0, 0)
+00001120: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00001130: 2070 6174 6830 2e65 6e64 203d 3d20 5665   path0.end == Ve
+00001140: 6332 2835 3030 302c 2035 3030 3029 0d0a  c2(5000, 5000)..
+00001150: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+00001160: 702e 706c 6f74 7465 722e 7573 6572 5f6c  p.plotter.user_l
+00001170: 6f63 6174 696f 6e20 3d3d 2056 6563 3228  ocation == Vec2(
+00001180: 3530 3030 2c20 3530 3030 290d 0a0d 0a20  5000, 5000).... 
+00001190: 2020 2064 6566 2074 6573 745f 6375 6269     def test_cubi
+000011a0: 635f 6265 7a69 6572 5f63 7572 7665 5f70  c_bezier_curve_p
+000011b0: 656e 5f75 7028 7365 6c66 293a 0d0a 2020  en_up(self):..  
+000011c0: 2020 2020 2020 6970 203d 2070 6c6f 7428        ip = plot(
+000011d0: 6222 5055 3b42 5a32 3030 302c 3830 3030  b"PU;BZ2000,8000
+000011e0: 2c34 3030 302c 3230 3030 2c35 3030 302c  ,4000,2000,5000,
+000011f0: 3530 3030 3b22 290d 0a20 2020 2020 2020  5000;")..       
+00001200: 2061 7373 6572 7420 6c65 6e28 6765 745f   assert len(get_
+00001210: 7265 7375 6c74 2869 702e 706c 6f74 7465  result(ip.plotte
+00001220: 7229 2920 3d3d 2030 0d0a 2020 2020 2020  r)) == 0..      
+00001230: 2020 6173 7365 7274 2069 702e 706c 6f74    assert ip.plot
+00001240: 7465 722e 7573 6572 5f6c 6f63 6174 696f  ter.user_locatio
+00001250: 6e20 3d3d 2056 6563 3228 3530 3030 2c20  n == Vec2(5000, 
+00001260: 3530 3030 290d 0a0d 0a20 2020 2064 6566  5000)....    def
+00001270: 2074 6573 745f 6369 7263 6c65 2873 656c   test_circle(sel
+00001280: 6629 3a0d 0a20 2020 2020 2020 2069 7020  f):..        ip 
+00001290: 3d20 706c 6f74 2862 2250 553b 5041 3230  = plot(b"PU;PA20
+000012a0: 3030 2c38 3030 303b 5044 3b43 4935 3030  00,8000;PD;CI500
+000012b0: 3b22 290d 0a20 2020 2020 2020 2063 6f6d  ;")..        com
+000012c0: 6d61 6e64 203d 2067 6574 5f72 6573 756c  mand = get_resul
+000012d0: 7428 6970 2e70 6c6f 7474 6572 295b 305d  t(ip.plotter)[0]
+000012e0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+000012f0: 2063 6f6d 6d61 6e64 5b30 5d20 3d3d 2022   command[0] == "
+00001300: 506f 6c79 6c69 6e65 220d 0a20 2020 2020  Polyline"..     
+00001310: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
+00001320: 6d6d 616e 645b 315d 2920 3d3d 2037 3320  mmand[1]) == 73 
+00001330: 2023 2064 6566 6175 6c74 2063 686f 7264   # default chord
+00001340: 5f61 6e67 6c65 2069 7320 3520 6465 670d  _angle is 5 deg.
+00001350: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00001360: 6970 2e70 6c6f 7474 6572 2e75 7365 725f  ip.plotter.user_
+00001370: 6c6f 6361 7469 6f6e 203d 3d20 5665 6332  location == Vec2
+00001380: 2832 3030 302c 2038 3030 3029 0d0a 0d0a  (2000, 8000)....
+00001390: 2020 2020 6465 6620 7465 7374 5f61 6273      def test_abs
+000013a0: 5f61 7263 2873 656c 6629 3a0d 0a20 2020  _arc(self):..   
+000013b0: 2020 2020 2069 7020 3d20 706c 6f74 2862       ip = plot(b
+000013c0: 2250 5531 3030 2c31 3030 3b50 443b 4141  "PU100,100;PD;AA
+000013d0: 3230 302c 3130 302c 2d31 3830 3b22 290d  200,100,-180;").
+000013e0: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+000013f0: 203d 2067 6574 5f72 6573 756c 7428 6970   = get_result(ip
+00001400: 2e70 6c6f 7474 6572 295b 305d 0d0a 2020  .plotter)[0]..  
+00001410: 2020 2020 2020 6173 7365 7274 2063 6f6d        assert com
+00001420: 6d61 6e64 5b30 5d20 3d3d 2022 506f 6c79  mand[0] == "Poly
+00001430: 6c69 6e65 220d 0a20 2020 2020 2020 2061  line"..        a
+00001440: 7373 6572 7420 6c65 6e28 636f 6d6d 616e  ssert len(comman
+00001450: 645b 315d 2920 3d3d 2033 3720 2023 2064  d[1]) == 37  # d
+00001460: 6566 6175 6c74 2063 686f 7264 5f61 6e67  efault chord_ang
+00001470: 6c65 2069 7320 3520 6465 670d 0a20 2020  le is 5 deg..   
+00001480: 2020 2020 2061 7373 6572 7420 6970 2e70       assert ip.p
+00001490: 6c6f 7474 6572 2e75 7365 725f 6c6f 6361  lotter.user_loca
+000014a0: 7469 6f6e 2e69 7363 6c6f 7365 2828 3330  tion.isclose((30
+000014b0: 302c 2031 3030 2929 0d0a 0d0a 2020 2020  0, 100))....    
+000014c0: 6465 6620 7465 7374 5f72 656c 5f61 7263  def test_rel_arc
+000014d0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000014e0: 2069 7020 3d20 706c 6f74 2862 2250 5531   ip = plot(b"PU1
+000014f0: 3030 2c31 3030 3b50 443b 4152 3130 302c  00,100;PD;AR100,
+00001500: 302c 2d31 3830 3b22 290d 0a20 2020 2020  0,-180;")..     
+00001510: 2020 2063 6f6d 6d61 6e64 203d 2067 6574     command = get
+00001520: 5f72 6573 756c 7428 6970 2e70 6c6f 7474  _result(ip.plott
+00001530: 6572 295b 305d 0d0a 2020 2020 2020 2020  er)[0]..        
+00001540: 6173 7365 7274 2063 6f6d 6d61 6e64 5b30  assert command[0
+00001550: 5d20 3d3d 2022 506f 6c79 6c69 6e65 220d  ] == "Polyline".
+00001560: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00001570: 6c65 6e28 636f 6d6d 616e 645b 315d 2920  len(command[1]) 
+00001580: 3d3d 2033 3720 2023 2064 6566 6175 6c74  == 37  # default
+00001590: 2063 686f 7264 5f61 6e67 6c65 2069 7320   chord_angle is 
+000015a0: 3520 6465 670d 0a20 2020 2020 2020 2061  5 deg..        a
+000015b0: 7373 6572 7420 6970 2e70 6c6f 7474 6572  ssert ip.plotter
+000015c0: 2e75 7365 725f 6c6f 6361 7469 6f6e 2e69  .user_location.i
+000015d0: 7363 6c6f 7365 2828 3330 302c 2031 3030  sclose((300, 100
+000015e0: 2929 0d0a 0d0a 2020 2020 6465 6620 7465  ))....    def te
+000015f0: 7374 5f61 6273 5f61 7263 5f74 6872 6565  st_abs_arc_three
+00001600: 5f70 6f69 6e74 735f 636c 6f63 6b77 6973  _points_clockwis
+00001610: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
+00001620: 2020 6970 203d 2070 6c6f 7428 6222 5055    ip = plot(b"PU
+00001630: 3130 302c 3130 303b 5044 3b41 5432 3030  100,100;PD;AT200
+00001640: 2c32 3030 2c33 3030 2c31 3030 3b22 290d  ,200,300,100;").
+00001650: 0a20 2020 2020 2020 2063 6f6d 6d61 6e64  .        command
+00001660: 203d 2067 6574 5f72 6573 756c 7428 6970   = get_result(ip
+00001670: 2e70 6c6f 7474 6572 295b 305d 0d0a 2020  .plotter)[0]..  
+00001680: 2020 2020 2020 6173 7365 7274 2063 6f6d        assert com
+00001690: 6d61 6e64 5b30 5d20 3d3d 2022 506f 6c79  mand[0] == "Poly
+000016a0: 6c69 6e65 220d 0a20 2020 2020 2020 2070  line"..        p
+000016b0: 6f69 6e74 7320 3d20 636f 6d6d 616e 645b  oints = command[
+000016c0: 315d 0d0a 2020 2020 2020 2020 6173 7365  1]..        asse
+000016d0: 7274 206c 656e 2870 6f69 6e74 7329 203d  rt len(points) =
+000016e0: 3d20 3337 2020 2320 6465 6661 756c 7420  = 37  # default 
+000016f0: 6368 6f72 645f 616e 676c 6520 6973 2035  chord_angle is 5
+00001700: 2064 6567 0d0a 2020 2020 2020 2020 6173   deg..        as
+00001710: 7365 7274 2070 6f69 6e74 735b 3138 5d2e  sert points[18].
+00001720: 6973 636c 6f73 6528 2832 3030 2c20 3230  isclose((200, 20
+00001730: 3029 290d 0a20 2020 2020 2020 2061 7373  0))..        ass
+00001740: 6572 7420 6970 2e70 6c6f 7474 6572 2e75  ert ip.plotter.u
+00001750: 7365 725f 6c6f 6361 7469 6f6e 2e69 7363  ser_location.isc
+00001760: 6c6f 7365 2828 3330 302c 2031 3030 2929  lose((300, 100))
+00001770: 0d0a 0d0a 2020 2020 6465 6620 7465 7374  ....    def test
+00001780: 5f61 6273 5f61 7263 5f74 6872 6565 5f70  _abs_arc_three_p
+00001790: 6f69 6e74 735f 636f 756e 7465 725f 636c  oints_counter_cl
+000017a0: 6f63 6b77 6973 6528 7365 6c66 293a 0d0a  ockwise(self):..
+000017b0: 2020 2020 2020 2020 6970 203d 2070 6c6f          ip = plo
+000017c0: 7428 6222 5055 3130 302c 3130 303b 5044  t(b"PU100,100;PD
+000017d0: 3b41 5432 3030 2c30 2c33 3030 2c31 3030  ;AT200,0,300,100
+000017e0: 3b22 290d 0a20 2020 2020 2020 2063 6f6d  ;")..        com
+000017f0: 6d61 6e64 203d 2067 6574 5f72 6573 756c  mand = get_resul
+00001800: 7428 6970 2e70 6c6f 7474 6572 295b 305d  t(ip.plotter)[0]
+00001810: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00001820: 2063 6f6d 6d61 6e64 5b30 5d20 3d3d 2022   command[0] == "
+00001830: 506f 6c79 6c69 6e65 220d 0a20 2020 2020  Polyline"..     
+00001840: 2020 2070 6f69 6e74 7320 3d20 636f 6d6d     points = comm
+00001850: 616e 645b 315d 0d0a 2020 2020 2020 2020  and[1]..        
+00001860: 6173 7365 7274 206c 656e 2870 6f69 6e74  assert len(point
+00001870: 7329 203d 3d20 3337 2020 2320 6465 6661  s) == 37  # defa
+00001880: 756c 7420 6368 6f72 645f 616e 676c 6520  ult chord_angle 
+00001890: 6973 2035 2064 6567 0d0a 2020 2020 2020  is 5 deg..      
+000018a0: 2020 6173 7365 7274 2070 6f69 6e74 735b    assert points[
+000018b0: 3138 5d2e 6973 636c 6f73 6528 2832 3030  18].isclose((200
+000018c0: 2c20 3029 290d 0a20 2020 2020 2020 2061  , 0))..        a
+000018d0: 7373 6572 7420 6970 2e70 6c6f 7474 6572  ssert ip.plotter
+000018e0: 2e75 7365 725f 6c6f 6361 7469 6f6e 2e69  .user_location.i
+000018f0: 7363 6c6f 7365 2828 3330 302c 2031 3030  sclose((300, 100
+00001900: 2929 0d0a 0d0a 2020 2020 6465 6620 7465  ))....    def te
+00001910: 7374 5f72 656c 5f61 7263 5f74 6872 6565  st_rel_arc_three
+00001920: 5f70 6f69 6e74 735f 636c 6f63 6b77 6973  _points_clockwis
+00001930: 6528 7365 6c66 293a 0d0a 2020 2020 2020  e(self):..      
+00001940: 2020 6970 203d 2070 6c6f 7428 6222 5055    ip = plot(b"PU
+00001950: 3130 302c 3130 303b 5044 3b52 5431 3030  100,100;PD;RT100
+00001960: 2c31 3030 2c32 3030 2c30 3b22 290d 0a20  ,100,200,0;").. 
+00001970: 2020 2020 2020 2063 6f6d 6d61 6e64 203d         command =
+00001980: 2067 6574 5f72 6573 756c 7428 6970 2e70   get_result(ip.p
+00001990: 6c6f 7474 6572 295b 305d 0d0a 2020 2020  lotter)[0]..    
+000019a0: 2020 2020 6173 7365 7274 2063 6f6d 6d61      assert comma
+000019b0: 6e64 5b30 5d20 3d3d 2022 506f 6c79 6c69  nd[0] == "Polyli
+000019c0: 6e65 220d 0a20 2020 2020 2020 2070 6f69  ne"..        poi
+000019d0: 6e74 7320 3d20 636f 6d6d 616e 645b 315d  nts = command[1]
+000019e0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+000019f0: 206c 656e 2870 6f69 6e74 7329 203d 3d20   len(points) == 
+00001a00: 3337 2020 2320 6465 6661 756c 7420 6368  37  # default ch
+00001a10: 6f72 645f 616e 676c 6520 6973 2035 2064  ord_angle is 5 d
+00001a20: 6567 0d0a 2020 2020 2020 2020 6173 7365  eg..        asse
+00001a30: 7274 2070 6f69 6e74 735b 3138 5d2e 6973  rt points[18].is
+00001a40: 636c 6f73 6528 2832 3030 2c20 3230 3029  close((200, 200)
+00001a50: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00001a60: 7420 6970 2e70 6c6f 7474 6572 2e75 7365  t ip.plotter.use
+00001a70: 725f 6c6f 6361 7469 6f6e 2e69 7363 6c6f  r_location.isclo
+00001a80: 7365 2828 3330 302c 2031 3030 2929 0d0a  se((300, 100))..
+00001a90: 0d0a 2020 2020 6465 6620 7465 7374 5f70  ..    def test_p
+00001aa0: 6f6c 796c 696e 655f 656e 636f 6465 6428  olyline_encoded(
+00001ab0: 7365 6c66 293a 0d0a 2020 2020 2020 2020  self):..        
+00001ac0: 6970 203d 2070 6c6f 7428 6222 5045 373d  ip = plot(b"PE7=
+00001ad0: 555e 7847 4968 3b22 290d 0a20 2020 2020  U^xGIh;")..     
+00001ae0: 2020 2063 6f6d 6d61 6e64 203d 2067 6574     command = get
+00001af0: 5f72 6573 756c 7428 6970 2e70 6c6f 7474  _result(ip.plott
+00001b00: 6572 295b 305d 0d0a 2020 2020 2020 2020  er)[0]..        
+00001b10: 6173 7365 7274 2063 6f6d 6d61 6e64 5b30  assert command[0
+00001b20: 5d20 3d3d 2022 506f 6c79 6c69 6e65 220d  ] == "Polyline".
+00001b30: 0a0d 0a0d 0a63 6c61 7373 2054 6573 7454  .....class TestT
+00001b40: 6f6b 656e 697a 6572 3a0d 0a20 2020 2064  okenizer:..    d
+00001b50: 6566 2070 6172 7365 2873 656c 662c 2073  ef parse(self, s
+00001b60: 3a20 6279 7465 7329 3a0d 0a20 2020 2020  : bytes):..     
+00001b70: 2020 2072 6574 7572 6e20 6170 692e 6870     return api.hp
+00001b80: 676c 325f 636f 6d6d 616e 6473 2873 290d  gl2_commands(s).
+00001b90: 0a0d 0a20 2020 2040 7079 7465 7374 2e6d  ...    @pytest.m
+00001ba0: 6172 6b2e 7061 7261 6d65 7472 697a 6528  ark.parametrize(
+00001bb0: 0d0a 2020 2020 2020 2020 2273 222c 0d0a  ..        "s",..
+00001bc0: 2020 2020 2020 2020 5b0d 0a20 2020 2020          [..     
+00001bd0: 2020 2020 2020 2062 221b 252d 3142 4250         b".%-1BBP
+00001be0: 3b22 2c0d 0a20 2020 2020 2020 2020 2020  ;",..           
+00001bf0: 2062 221b 2530 4242 503b 222c 0d0a 2020   b".%0BBP;",..  
+00001c00: 2020 2020 2020 2020 2020 6222 1b25 3142            b".%1B
+00001c10: 4250 3b22 2c0d 0a20 2020 2020 2020 2020  BP;",..         
+00001c20: 2020 2062 221b 2532 4242 503b 222c 0d0a     b".%2BBP;",..
+00001c30: 2020 2020 2020 2020 2020 2020 6222 1b25              b".%
+00001c40: 3342 4250 3b22 2c0d 0a20 2020 2020 2020  3BBP;",..       
+00001c50: 205d 2c0d 0a20 2020 2029 0d0a 2020 2020   ],..    )..    
+00001c60: 6465 6620 7465 7374 5f65 7363 6170 6528  def test_escape(
+00001c70: 7365 6c66 2c20 7329 3a0d 0a20 2020 2020  self, s):..     
+00001c80: 2020 2072 6573 756c 7420 3d20 7365 6c66     result = self
+00001c90: 2e70 6172 7365 2873 290d 0a20 2020 2020  .parse(s)..     
+00001ca0: 2020 2061 7373 6572 7420 7265 7375 6c74     assert result
+00001cb0: 5b30 5d2e 6e61 6d65 203d 3d20 2242 5022  [0].name == "BP"
+00001cc0: 0d0a 0d0a 2020 2020 4070 7974 6573 742e  ....    @pytest.
+00001cd0: 6d61 726b 2e70 6172 616d 6574 7269 7a65  mark.parametrize
+00001ce0: 280d 0a20 2020 2020 2020 2022 7322 2c0d  (..        "s",.
+00001cf0: 0a20 2020 2020 2020 205b 0d0a 2020 2020  .        [..    
+00001d00: 2020 2020 2020 2020 6222 494e 3b50 553b          b"IN;PU;
+00001d10: 5044 3b22 2c0d 0a20 2020 2020 2020 2020  PD;",..         
+00001d20: 2020 2062 2249 4e3b 5055 3b50 4422 2c0d     b"IN;PU;PD",.
+00001d30: 0a20 2020 2020 2020 2020 2020 2062 2249  .            b"I
+00001d40: 4e50 5550 4422 2c0d 0a20 2020 2020 2020  NPUPD",..       
+00001d50: 2020 2020 2062 2249 4e20 5055 2050 4422       b"IN PU PD"
+00001d60: 2c0d 0a20 2020 2020 2020 2020 2020 2062  ,..            b
+00001d70: 2220 494e 5055 2050 4422 2c0d 0a20 2020  " INPU PD",..   
+00001d80: 2020 2020 205d 2c0d 0a20 2020 2029 0d0a       ],..    )..
+00001d90: 2020 2020 6465 6620 7465 7374 5f73 686f      def test_sho
+00001da0: 7274 5f63 6f6d 6d61 6e64 7328 7365 6c66  rt_commands(self
+00001db0: 2c20 7329 3a0d 0a20 2020 2020 2020 2072  , s):..        r
+00001dc0: 6573 756c 7420 3d20 7365 6c66 2e70 6172  esult = self.par
+00001dd0: 7365 2868 7067 6c32 2873 2929 0d0a 2020  se(hpgl2(s))..  
+00001de0: 2020 2020 2020 6173 7365 7274 206c 656e        assert len
+00001df0: 2872 6573 756c 7429 203d 3d20 330d 0a20  (result) == 3.. 
+00001e00: 2020 2020 2020 2061 7373 6572 7420 7265         assert re
+00001e10: 7375 6c74 5b30 5d2e 6e61 6d65 203d 3d20  sult[0].name == 
+00001e20: 2249 4e22 0d0a 2020 2020 2020 2020 6173  "IN"..        as
+00001e30: 7365 7274 2072 6573 756c 745b 315d 2e6e  sert result[1].n
+00001e40: 616d 6520 3d3d 2022 5055 220d 0a20 2020  ame == "PU"..   
+00001e50: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
+00001e60: 6c74 5b32 5d2e 6e61 6d65 203d 3d20 2250  lt[2].name == "P
+00001e70: 4422 0d0a 0d0a 2020 2020 4070 7974 6573  D"....    @pytes
+00001e80: 742e 6d61 726b 2e70 6172 616d 6574 7269  t.mark.parametri
+00001e90: 7a65 280d 0a20 2020 2020 2020 2022 732c  ze(..        "s,
+00001ea0: 6922 2c0d 0a20 2020 2020 2020 205b 0d0a  i",..        [..
+00001eb0: 2020 2020 2020 2020 2020 2020 2862 2250              (b"P
+00001ec0: 4554 4553 5422 2c20 3029 2c0d 0a20 2020  ETEST", 0),..   
+00001ed0: 2020 2020 2020 2020 2028 6222 5055 5045           (b"PUPE
+00001ee0: 5445 5354 3b50 4422 2c20 3129 2c0d 0a20  TEST;PD", 1),.. 
+00001ef0: 2020 2020 2020 2020 2020 2028 6222 5055             (b"PU
+00001f00: 5055 5045 5445 5354 3b50 4422 2c20 3229  PUPETEST;PD", 2)
+00001f10: 2c0d 0a20 2020 2020 2020 205d 2c0d 0a20  ,..        ],.. 
+00001f20: 2020 2029 0d0a 2020 2020 6465 6620 7465     )..    def te
+00001f30: 7374 5f70 655f 636f 6d6d 616e 6428 7365  st_pe_command(se
+00001f40: 6c66 2c20 732c 2069 293a 0d0a 2020 2020  lf, s, i):..    
+00001f50: 2020 2020 7265 7375 6c74 203d 2073 656c      result = sel
+00001f60: 662e 7061 7273 6528 6870 676c 3228 7329  f.parse(hpgl2(s)
+00001f70: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00001f80: 7420 7265 7375 6c74 5b69 5d2e 6e61 6d65  t result[i].name
+00001f90: 203d 3d20 2250 4522 0d0a 2020 2020 2020   == "PE"..      
+00001fa0: 2020 6173 7365 7274 2072 6573 756c 745b    assert result[
+00001fb0: 695d 2e61 7267 735b 305d 203d 3d20 6222  i].args[0] == b"
+00001fc0: 5445 5354 220d 0a0d 0a20 2020 2064 6566  TEST"....    def
+00001fd0: 2074 6573 745f 3030 3128 7365 6c66 293a   test_001(self):
+00001fe0: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00001ff0: 203d 2073 656c 662e 7061 7273 6528 6870   = self.parse(hp
+00002000: 676c 3228 6222 5041 3b50 4132 3030 302c  gl2(b"PA;PA2000,
+00002010: 3830 3030 2229 290d 0a20 2020 2020 2020  8000"))..       
+00002020: 2061 7373 6572 7420 7265 7375 6c74 5b30   assert result[0
+00002030: 5d2e 6e61 6d65 203d 3d20 2250 4122 0d0a  ].name == "PA"..
+00002040: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
+00002050: 6573 756c 745b 315d 2e6e 616d 6520 3d3d  esult[1].name ==
+00002060: 2022 5041 220d 0a0d 0a20 2020 2064 6566   "PA"....    def
+00002070: 2074 6573 745f 3030 3228 7365 6c66 293a   test_002(self):
+00002080: 0d0a 2020 2020 2020 2020 7265 7375 6c74  ..        result
+00002090: 203d 2073 656c 662e 7061 7273 6528 6870   = self.parse(hp
+000020a0: 676c 3228 6222 5055 5350 3050 4722 2929  gl2(b"PUSP0PG"))
+000020b0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+000020c0: 2072 6573 756c 745b 305d 2e6e 616d 6520   result[0].name 
+000020d0: 3d3d 2022 5055 220d 0a20 2020 2020 2020  == "PU"..       
+000020e0: 2061 7373 6572 7420 7265 7375 6c74 5b31   assert result[1
+000020f0: 5d2e 6e61 6d65 203d 3d20 2253 5022 0d0a  ].name == "SP"..
+00002100: 2020 2020 2020 2020 6173 7365 7274 2072          assert r
+00002110: 6573 756c 745b 315d 2e61 7267 735b 305d  esult[1].args[0]
+00002120: 203d 3d20 6222 3022 0d0a 2020 2020 2020   == b"0"..      
+00002130: 2020 6173 7365 7274 2072 6573 756c 745b    assert result[
+00002140: 325d 2e6e 616d 6520 3d3d 2022 5047 220d  2].name == "PG".
+00002150: 0a0d 0a20 2020 2064 6566 2074 6573 745f  ...    def test_
+00002160: 6669 6c74 6572 5f6e 6f6e 5f70 7269 6e74  filter_non_print
+00002170: 6162 6c65 5f63 6861 7273 5f66 726f 6d5f  able_chars_from_
+00002180: 7065 5f63 6f6d 6d61 6e64 2873 656c 6629  pe_command(self)
+00002190: 3a0d 0a20 2020 2020 2020 2072 6573 756c  :..        resul
+000021a0: 7420 3d20 7365 6c66 2e70 6172 7365 2868  t = self.parse(h
+000021b0: 7067 6c32 2862 2250 4578 7878 7878 5c72  pgl2(b"PExxxxx\r
+000021c0: 5c6e 7878 7878 783b 2229 290d 0a20 2020  \nxxxxx;"))..   
+000021d0: 2020 2020 2061 7373 6572 7420 7265 7375       assert resu
+000021e0: 6c74 5b30 5d2e 6172 6773 5b30 5d20 3d3d  lt[0].args[0] ==
+000021f0: 2062 2278 7878 7878 7878 7878 7822 0d0a   b"xxxxxxxxxx"..
+00002200: 0d0a 2020 2020 6465 6620 7465 7374 5f6e  ..    def test_n
+00002210: 6f5f 6870 676c 325f 6461 7461 2873 656c  o_hpgl2_data(sel
+00002220: 6629 3a0d 0a20 2020 2020 2020 2023 2045  f):..        # E
+00002230: 6361 7065 2073 6571 7565 6e63 6520 746f  cape sequence to
+00002240: 2065 6e74 6572 2048 5047 4c32 206d 6f64   enter HPGL2 mod
+00002250: 6520 6973 206d 6973 7369 6e67 3a20 2022  e is missing:  "
+00002260: 1b25 3142 220d 0a20 2020 2020 2020 2061  .%1B"..        a
+00002270: 7373 6572 7420 6c65 6e28 7365 6c66 2e70  ssert len(self.p
+00002280: 6172 7365 2862 2241 4e59 5445 5854 3b49  arse(b"ANYTEXT;I
+00002290: 4e3b 4250 3b22 2929 203d 3d20 300d 0a0d  N;BP;")) == 0...
+000022a0: 0a20 2020 2040 7079 7465 7374 2e6d 6172  .    @pytest.mar
+000022b0: 6b2e 7061 7261 6d65 7472 697a 6528 2262  k.parametrize("b
+000022c0: 222c 205b 0d0a 2020 2020 2020 2020 6222  ", [..        b"
+000022d0: 4c42 204d 5920 6c61 6265 6c20 0350 4133  LB MY label .PA3
+000022e0: 3831 2c30 5349 302e 3132 352c 302e 3235  81,0SI0.125,0.25
+000022f0: 4449 302c 313b 222c 0d0a 2020 2020 2020  DI0,1;",..      
+00002300: 2020 6222 4c42 4d59 206c 6162 656c 2003    b"LBMY label .
+00002310: 5041 3338 312c 3053 4930 2e31 3235 2c30  PA381,0SI0.125,0
+00002320: 2e32 3544 4930 2c31 3b22 0d0a 2020 2020  .25DI0,1;"..    
+00002330: 5d29 0d0a 2020 2020 6465 6620 7465 7374  ])..    def test
+00002340: 5f6c 6162 656c 5f77 6974 685f 7465 726d  _label_with_term
+00002350: 696e 6174 6f72 2873 656c 662c 2062 293a  inator(self, b):
+00002360: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+00002370: 6473 203d 2073 656c 662e 7061 7273 6528  ds = self.parse(
+00002380: 6870 676c 3228 6229 290d 0a20 2020 2020  hpgl2(b))..     
+00002390: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
+000023a0: 6d6d 616e 6473 2920 3d3d 2034 0d0a 0d0a  mmands) == 4....
+000023b0: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+000023c0: 2e70 6172 616d 6574 7269 7a65 280d 0a20  .parametrize(.. 
+000023d0: 2020 2020 2020 2022 6222 2c0d 0a20 2020         "b",..   
+000023e0: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
+000023f0: 2020 2020 6222 4454 5c30 344c 4220 5475      b"DT\04LB Tu
+00002400: 6520 4465 6320 3138 2031 363a 3230 3a30  e Dec 18 16:20:0
+00002410: 3520 3230 3031 205c 3034 5041 3338 312c  5 2001 \04PA381,
+00002420: 3053 4930 2e31 3235 2c30 2e32 3544 4930  0SI0.125,0.25DI0
+00002430: 2c31 3b22 2c0d 0a20 2020 2020 2020 2020  ,1;",..         
+00002440: 2020 2062 2244 545c 3034 2c30 4c42 2054     b"DT\04,0LB T
+00002450: 7565 2044 6563 2031 3820 3136 3a32 303a  ue Dec 18 16:20:
+00002460: 3035 2032 3030 3120 5c30 3450 4133 3831  05 2001 \04PA381
+00002470: 2c30 5349 302e 3132 352c 302e 3235 4449  ,0SI0.125,0.25DI
+00002480: 302c 313b 222c 0d0a 2020 2020 2020 2020  0,1;",..        
+00002490: 2020 2020 6222 4454 5c30 342c 313b 4c42      b"DT\04,1;LB
+000024a0: 2054 7565 2044 6563 2031 3820 3136 3a32   Tue Dec 18 16:2
+000024b0: 303a 3035 2032 3030 3120 5c30 3450 4133  0:05 2001 \04PA3
+000024c0: 3831 2c30 5349 302e 3132 352c 302e 3235  81,0SI0.125,0.25
+000024d0: 4449 302c 313b 222c 0d0a 2020 2020 2020  DI0,1;",..      
+000024e0: 2020 5d2c 0d0a 2020 2020 290d 0a20 2020    ],..    )..   
+000024f0: 2064 6566 2074 6573 745f 6c61 6265 6c5f   def test_label_
+00002500: 7769 7468 5f63 7573 746f 6d5f 7465 726d  with_custom_term
+00002510: 696e 6174 6f72 2873 656c 662c 2062 293a  inator(self, b):
+00002520: 0d0a 2020 2020 2020 2020 636f 6d6d 616e  ..        comman
+00002530: 6473 203d 2073 656c 662e 7061 7273 6528  ds = self.parse(
+00002540: 6870 676c 3228 6229 290d 0a20 2020 2020  hpgl2(b))..     
+00002550: 2020 2061 7373 6572 7420 6c65 6e28 636f     assert len(co
+00002560: 6d6d 616e 6473 2920 3d3d 2034 0d0a 0d0a  mmands) == 4....
+00002570: 2020 2020 4070 7974 6573 742e 6d61 726b      @pytest.mark
+00002580: 2e70 6172 616d 6574 7269 7a65 280d 0a20  .parametrize(.. 
+00002590: 2020 2020 2020 2022 6222 2c0d 0a20 2020         "b",..   
+000025a0: 2020 2020 205b 0d0a 2020 2020 2020 2020       [..        
+000025b0: 2020 2020 6222 4454 5c30 344c 4220 4d59      b"DT\04LB MY
+000025c0: 206c 6162 656c 5c30 3444 544c 4220 4d79   label\04DTLB My
+000025d0: 206f 7468 6572 206c 6162 656c 2003 222c   other label .",
+000025e0: 0d0a 2020 2020 2020 2020 2020 2020 6222  ..            b"
+000025f0: 4454 5c30 344c 4220 4d59 206c 6162 656c  DT\04LB MY label
+00002600: 5c30 3444 543b 4c42 204d 7920 6f74 6865  \04DT;LB My othe
+00002610: 7220 6c61 6265 6c20 0322 2c0d 0a20 2020  r label .",..   
+00002620: 2020 2020 205d 2c0d 0a20 2020 2029 0d0a       ],..    )..
+00002630: 2020 2020 6465 6620 7465 7374 5f72 6573      def test_res
+00002640: 6574 5f63 7573 746f 6d5f 7465 726d 696e  et_custom_termin
+00002650: 6174 6f72 2873 656c 662c 2062 293a 0d0a  ator(self, b):..
+00002660: 2020 2020 2020 2020 636f 6d6d 616e 6473          commands
+00002670: 203d 2073 656c 662e 7061 7273 6528 6870   = self.parse(hp
+00002680: 676c 3228 6229 290d 0a20 2020 2020 2020  gl2(b))..       
+00002690: 2061 7373 6572 7420 6c65 6e28 636f 6d6d   assert len(comm
+000026a0: 616e 6473 2920 3d3d 2032 0d0a 0d0a 0d0a  ands) == 2......
+000026b0: 636c 6173 7320 5465 7374 5061 6765 436f  class TestPageCo
+000026c0: 6f72 6469 6e61 7465 733a 0d0a 2020 2020  ordinates:..    
+000026d0: 4070 7974 6573 742e 6669 7874 7572 6528  @pytest.fixture(
+000026e0: 7363 6f70 653d 2263 6c61 7373 2229 0d0a  scope="class")..
+000026f0: 2020 2020 6465 6620 7061 6765 2873 656c      def page(sel
+00002700: 6629 3a0d 0a20 2020 2020 2020 2070 6167  f):..        pag
+00002710: 655f 203d 2050 6167 6528 3130 3030 2c20  e_ = Page(1000, 
+00002720: 3130 3030 290d 0a20 2020 2020 2020 2070  1000)..        p
+00002730: 6167 655f 2e73 6574 5f75 6373 2856 6563  age_.set_ucs(Vec
+00002740: 3228 3530 302c 2035 3030 292c 2073 783d  2(500, 500), sx=
+00002750: 322c 2073 793d 3329 0d0a 2020 2020 2020  2, sy=3)..      
+00002760: 2020 7265 7475 726e 2070 6167 655f 0d0a    return page_..
+00002770: 0d0a 2020 2020 6465 6620 7465 7374 5f75  ..    def test_u
+00002780: 7365 725f 746f 5f70 6167 655f 636f 6f72  ser_to_page_coor
+00002790: 6469 6e61 7465 7328 7365 6c66 2c20 7061  dinates(self, pa
+000027a0: 6765 293a 0d0a 2020 2020 2020 2020 6173  ge):..        as
+000027b0: 7365 7274 2070 6167 652e 7061 6765 5f70  sert page.page_p
+000027c0: 6f69 6e74 2830 2c20 3029 2e69 7363 6c6f  oint(0, 0).isclo
+000027d0: 7365 2828 3530 302c 2035 3030 2929 0d0a  se((500, 500))..
+000027e0: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
+000027f0: 6167 652e 7061 6765 5f70 6f69 6e74 2831  age.page_point(1
+00002800: 302c 2031 3029 2e69 7363 6c6f 7365 2828  0, 10).isclose((
+00002810: 3532 302c 2035 3330 2929 0d0a 0d0a 2020  520, 530))....  
+00002820: 2020 6465 6620 7465 7374 5f75 7365 725f    def test_user_
+00002830: 7665 6374 6f72 5f74 6f5f 7061 6765 5f76  vector_to_page_v
+00002840: 6563 746f 7228 7365 6c66 2c20 7061 6765  ector(self, page
+00002850: 293a 0d0a 2020 2020 2020 2020 6173 7365  ):..        asse
+00002860: 7274 2070 6167 652e 7061 6765 5f76 6563  rt page.page_vec
+00002870: 746f 7228 302c 2030 292e 6973 636c 6f73  tor(0, 0).isclos
+00002880: 6528 2830 2c20 3029 290d 0a20 2020 2020  e((0, 0))..     
+00002890: 2020 2061 7373 6572 7420 7061 6765 2e70     assert page.p
+000028a0: 6167 655f 7665 6374 6f72 2831 302c 2031  age_vector(10, 1
+000028b0: 3029 2e69 7363 6c6f 7365 2828 3230 2c20  0).isclose((20, 
+000028c0: 3330 2929 0d0a 0d0a 0d0a 636c 6173 7320  30))......class 
+000028d0: 5465 7374 5061 6765 416e 6973 6f74 726f  TestPageAnisotro
+000028e0: 7069 6353 6361 6c69 6e67 3a0d 0a20 2020  picScaling:..   
+000028f0: 2064 6566 2074 6573 745f 6973 6f74 726f   def test_isotro
+00002900: 7069 635f 7363 616c 696e 6728 7365 6c66  pic_scaling(self
+00002910: 293a 0d0a 2020 2020 2020 2020 7061 6765  ):..        page
+00002920: 203d 2050 6167 6528 3130 3030 2c20 3130   = Page(1000, 10
+00002930: 3030 290d 0a20 2020 2020 2020 2070 6167  00)..        pag
+00002940: 652e 7365 745f 7363 616c 696e 675f 706f  e.set_scaling_po
+00002950: 696e 7473 2856 6563 3228 3130 302c 2031  ints(Vec2(100, 1
+00002960: 3030 292c 2056 6563 3228 3230 302c 2032  00), Vec2(200, 2
+00002970: 3030 2929 0d0a 2020 2020 2020 2020 7061  00))..        pa
+00002980: 6765 2e73 6574 5f61 6e69 736f 7472 6f70  ge.set_anisotrop
+00002990: 6963 5f73 6361 6c69 6e67 282d 3130 2c20  ic_scaling(-10, 
+000029a0: 3130 2c20 2d31 302c 2031 3029 0d0a 2020  10, -10, 10)..  
+000029b0: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
+000029c0: 652e 7573 6572 5f73 6361 6c69 6e67 2069  e.user_scaling i
+000029d0: 7320 5472 7565 0d0a 2020 2020 2020 2020  s True..        
+000029e0: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
+000029f0: 5f70 6f69 6e74 2830 2c20 3029 2e69 7363  _point(0, 0).isc
+00002a00: 6c6f 7365 2828 3135 302c 2031 3530 2929  lose((150, 150))
+00002a10: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00002a20: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
+00002a30: 282d 3130 2c20 2d31 3029 2e69 7363 6c6f  (-10, -10).isclo
+00002a40: 7365 2828 3130 302c 2031 3030 2929 0d0a  se((100, 100))..
+00002a50: 2020 2020 2020 2020 6173 7365 7274 2070          assert p
+00002a60: 6167 652e 7061 6765 5f70 6f69 6e74 2831  age.page_point(1
+00002a70: 302c 2031 3029 2e69 7363 6c6f 7365 2828  0, 10).isclose((
+00002a80: 3230 302c 2032 3030 2929 0d0a 0d0a 2020  200, 200))....  
+00002a90: 2020 6465 6620 7465 7374 5f61 6e69 736f    def test_aniso
+00002aa0: 7472 6f70 6963 5f73 6361 6c69 6e67 2873  tropic_scaling(s
+00002ab0: 656c 6629 3a0d 0a20 2020 2020 2020 2070  elf):..        p
+00002ac0: 6167 6520 3d20 5061 6765 2831 3030 302c  age = Page(1000,
+00002ad0: 2031 3030 3029 0d0a 2020 2020 2020 2020   1000)..        
+00002ae0: 7061 6765 2e73 6574 5f73 6361 6c69 6e67  page.set_scaling
+00002af0: 5f70 6f69 6e74 7328 5665 6332 2831 3030  _points(Vec2(100
+00002b00: 2c20 3130 3029 2c20 5665 6332 2832 3030  , 100), Vec2(200
+00002b10: 2c20 3230 3029 290d 0a20 2020 2020 2020  , 200))..       
+00002b20: 2070 6167 652e 7365 745f 616e 6973 6f74   page.set_anisot
+00002b30: 726f 7069 635f 7363 616c 696e 6728 2d31  ropic_scaling(-1
+00002b40: 302c 2031 302c 202d 3230 2c20 3230 290d  0, 10, -20, 20).
+00002b50: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002b60: 7061 6765 2e75 7365 725f 7363 616c 696e  page.user_scalin
+00002b70: 6720 6973 2054 7275 650d 0a20 2020 2020  g is True..     
+00002b80: 2020 2061 7373 6572 7420 7061 6765 2e70     assert page.p
+00002b90: 6167 655f 706f 696e 7428 302c 2030 292e  age_point(0, 0).
+00002ba0: 6973 636c 6f73 6528 2831 3530 2c20 3135  isclose((150, 15
+00002bb0: 3029 290d 0a20 2020 2020 2020 2061 7373  0))..        ass
+00002bc0: 6572 7420 7061 6765 2e70 6167 655f 706f  ert page.page_po
+00002bd0: 696e 7428 2d31 302c 202d 3230 292e 6973  int(-10, -20).is
+00002be0: 636c 6f73 6528 2831 3030 2c20 3130 3029  close((100, 100)
+00002bf0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00002c00: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
+00002c10: 7428 3130 2c20 3230 292e 6973 636c 6f73  t(10, 20).isclos
+00002c20: 6528 2832 3030 2c20 3230 3029 290d 0a0d  e((200, 200))...
+00002c30: 0a20 2020 2064 6566 2074 6573 745f 7265  .    def test_re
+00002c40: 7665 7273 655f 616e 6973 6f74 726f 7069  verse_anisotropi
+00002c50: 635f 7363 616c 696e 6728 7365 6c66 293a  c_scaling(self):
+00002c60: 0d0a 2020 2020 2020 2020 7061 6765 203d  ..        page =
+00002c70: 2050 6167 6528 3130 3030 2c20 3130 3030   Page(1000, 1000
+00002c80: 290d 0a20 2020 2020 2020 2070 6167 652e  )..        page.
+00002c90: 7365 745f 7363 616c 696e 675f 706f 696e  set_scaling_poin
+00002ca0: 7473 2856 6563 3228 3130 302c 2031 3030  ts(Vec2(100, 100
+00002cb0: 292c 2056 6563 3228 3230 302c 2032 3030  ), Vec2(200, 200
+00002cc0: 2929 0d0a 2020 2020 2020 2020 2320 7265  ))..        # re
+00002cd0: 7665 7273 6520 7820 616e 6420 7920 6178  verse x and y ax
+00002ce0: 6973 3a0d 0a20 2020 2020 2020 2070 6167  is:..        pag
+00002cf0: 652e 7365 745f 616e 6973 6f74 726f 7069  e.set_anisotropi
+00002d00: 635f 7363 616c 696e 6728 3130 2c20 2d31  c_scaling(10, -1
+00002d10: 302c 2032 302c 202d 3230 290d 0a20 2020  0, 20, -20)..   
+00002d20: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00002d30: 2e75 7365 725f 7363 616c 696e 6720 6973  .user_scaling is
+00002d40: 2054 7275 650d 0a20 2020 2020 2020 2061   True..        a
+00002d50: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
+00002d60: 706f 696e 7428 302c 2030 292e 6973 636c  point(0, 0).iscl
+00002d70: 6f73 6528 2831 3530 2c20 3135 3029 290d  ose((150, 150)).
+00002d80: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00002d90: 7061 6765 2e70 6167 655f 706f 696e 7428  page.page_point(
+00002da0: 3130 2c20 3230 292e 6973 636c 6f73 6528  10, 20).isclose(
+00002db0: 2831 3030 2c20 3130 3029 290d 0a20 2020  (100, 100))..   
+00002dc0: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00002dd0: 2e70 6167 655f 706f 696e 7428 2d31 302c  .page_point(-10,
+00002de0: 202d 3230 292e 6973 636c 6f73 6528 2832   -20).isclose((2
+00002df0: 3030 2c20 3230 3029 290d 0a0d 0a0d 0a63  00, 200))......c
+00002e00: 6c61 7373 2054 6573 7450 6167 6549 736f  lass TestPageIso
+00002e10: 7472 6f70 6963 5363 616c 696e 673a 0d0a  tropicScaling:..
+00002e20: 2020 2020 6465 6620 7465 7374 5f69 736f      def test_iso
+00002e30: 7472 6f70 6963 5f62 6f74 746f 6d5f 7769  tropic_bottom_wi
+00002e40: 6e64 6f77 5f35 3028 7365 6c66 293a 0d0a  ndow_50(self):..
+00002e50: 2020 2020 2020 2020 7061 6765 203d 2050          page = P
+00002e60: 6167 6528 3130 3030 2c20 3130 3030 290d  age(1000, 1000).
+00002e70: 0a20 2020 2020 2020 2070 6167 652e 7365  .        page.se
+00002e80: 745f 7363 616c 696e 675f 706f 696e 7473  t_scaling_points
+00002e90: 2856 6563 3228 3130 302c 2031 3030 292c  (Vec2(100, 100),
+00002ea0: 2056 6563 3228 3230 302c 2032 3030 2929   Vec2(200, 200))
+00002eb0: 0d0a 2020 2020 2020 2020 7061 6765 2e73  ..        page.s
+00002ec0: 6574 5f69 736f 7472 6f70 6963 5f73 6361  et_isotropic_sca
+00002ed0: 6c69 6e67 2830 2c20 3230 2c20 302c 2031  ling(0, 20, 0, 1
+00002ee0: 3029 0d0a 2020 2020 2020 2020 6173 7365  0)..        asse
+00002ef0: 7274 2070 6167 652e 7573 6572 5f73 6361  rt page.user_sca
+00002f00: 6c69 6e67 2069 7320 5472 7565 0d0a 2020  ling is True..  
+00002f10: 2020 2020 2020 6173 7365 7274 2070 6167        assert pag
+00002f20: 652e 7061 6765 5f70 6f69 6e74 2830 2c20  e.page_point(0, 
+00002f30: 3029 2e69 7363 6c6f 7365 2828 3130 302c  0).isclose((100,
+00002f40: 2031 3235 2929 0d0a 2020 2020 2020 2020   125))..        
+00002f50: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
+00002f60: 5f70 6f69 6e74 2831 302c 2035 292e 6973  _point(10, 5).is
+00002f70: 636c 6f73 6528 2831 3530 2c20 3135 3029  close((150, 150)
+00002f80: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00002f90: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
+00002fa0: 7428 3230 2c20 3130 292e 6973 636c 6f73  t(20, 10).isclos
+00002fb0: 6528 2832 3030 2c20 3137 3529 290d 0a0d  e((200, 175))...
+00002fc0: 0a20 2020 2064 6566 2074 6573 745f 6973  .    def test_is
+00002fd0: 6f74 726f 7069 635f 626f 7474 6f6d 5f77  otropic_bottom_w
+00002fe0: 696e 646f 775f 3028 7365 6c66 293a 0d0a  indow_0(self):..
+00002ff0: 2020 2020 2020 2020 7061 6765 203d 2050          page = P
+00003000: 6167 6528 3130 3030 2c20 3130 3030 290d  age(1000, 1000).
+00003010: 0a20 2020 2020 2020 2070 6167 652e 7365  .        page.se
+00003020: 745f 7363 616c 696e 675f 706f 696e 7473  t_scaling_points
+00003030: 2856 6563 3228 3130 302c 2031 3030 292c  (Vec2(100, 100),
+00003040: 2056 6563 3228 3230 302c 2032 3030 2929   Vec2(200, 200))
+00003050: 0d0a 2020 2020 2020 2020 7061 6765 2e73  ..        page.s
+00003060: 6574 5f69 736f 7472 6f70 6963 5f73 6361  et_isotropic_sca
+00003070: 6c69 6e67 2830 2c20 3230 2c20 302c 2031  ling(0, 20, 0, 1
+00003080: 302c 2030 2c20 3029 0d0a 2020 2020 2020  0, 0, 0)..      
+00003090: 2020 6173 7365 7274 2070 6167 652e 7061    assert page.pa
+000030a0: 6765 5f70 6f69 6e74 2830 2c20 3029 2e69  ge_point(0, 0).i
+000030b0: 7363 6c6f 7365 2828 3130 302c 2031 3030  sclose((100, 100
+000030c0: 2929 0d0a 2020 2020 2020 2020 6173 7365  ))..        asse
+000030d0: 7274 2070 6167 652e 7061 6765 5f70 6f69  rt page.page_poi
+000030e0: 6e74 2831 302c 2035 292e 6973 636c 6f73  nt(10, 5).isclos
+000030f0: 6528 2831 3530 2c20 3132 3529 290d 0a20  e((150, 125)).. 
+00003100: 2020 2020 2020 2061 7373 6572 7420 7061         assert pa
+00003110: 6765 2e70 6167 655f 706f 696e 7428 3230  ge.page_point(20
+00003120: 2c20 3130 292e 6973 636c 6f73 6528 2832  , 10).isclose((2
+00003130: 3030 2c20 3135 3029 290d 0a0d 0a20 2020  00, 150))....   
+00003140: 2064 6566 2074 6573 745f 6973 6f74 726f   def test_isotro
+00003150: 7069 635f 626f 7474 6f6d 5f77 696e 646f  pic_bottom_windo
+00003160: 775f 3130 3028 7365 6c66 293a 0d0a 2020  w_100(self):..  
+00003170: 2020 2020 2020 7061 6765 203d 2050 6167        page = Pag
+00003180: 6528 3130 3030 2c20 3130 3030 290d 0a20  e(1000, 1000).. 
+00003190: 2020 2020 2020 2070 6167 652e 7365 745f         page.set_
+000031a0: 7363 616c 696e 675f 706f 696e 7473 2856  scaling_points(V
+000031b0: 6563 3228 3130 302c 2031 3030 292c 2056  ec2(100, 100), V
+000031c0: 6563 3228 3230 302c 2032 3030 2929 0d0a  ec2(200, 200))..
+000031d0: 2020 2020 2020 2020 7061 6765 2e73 6574          page.set
+000031e0: 5f69 736f 7472 6f70 6963 5f73 6361 6c69  _isotropic_scali
+000031f0: 6e67 2830 2c20 3230 2c20 302c 2031 302c  ng(0, 20, 0, 10,
+00003200: 2031 2c20 3129 0d0a 2020 2020 2020 2020   1, 1)..        
+00003210: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
+00003220: 5f70 6f69 6e74 2830 2c20 3029 2e69 7363  _point(0, 0).isc
+00003230: 6c6f 7365 2828 3130 302c 2031 3530 2929  lose((100, 150))
+00003240: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00003250: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
+00003260: 2831 302c 2035 292e 6973 636c 6f73 6528  (10, 5).isclose(
+00003270: 2831 3530 2c20 3137 3529 290d 0a20 2020  (150, 175))..   
+00003280: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00003290: 2e70 6167 655f 706f 696e 7428 3230 2c20  .page_point(20, 
+000032a0: 3130 292e 6973 636c 6f73 6528 2832 3030  10).isclose((200
+000032b0: 2c20 3230 3029 290d 0a0d 0a20 2020 2064  , 200))....    d
+000032c0: 6566 2074 6573 745f 6973 6f74 726f 7069  ef test_isotropi
+000032d0: 635f 6c65 6674 5f77 696e 646f 775f 3530  c_left_window_50
+000032e0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000032f0: 2070 6167 6520 3d20 5061 6765 2831 3030   page = Page(100
+00003300: 302c 2031 3030 3029 0d0a 2020 2020 2020  0, 1000)..      
+00003310: 2020 7061 6765 2e73 6574 5f73 6361 6c69    page.set_scali
+00003320: 6e67 5f70 6f69 6e74 7328 5665 6332 2831  ng_points(Vec2(1
+00003330: 3030 2c20 3130 3029 2c20 5665 6332 2832  00, 100), Vec2(2
+00003340: 3030 2c20 3230 3029 290d 0a20 2020 2020  00, 200))..     
+00003350: 2020 2070 6167 652e 7365 745f 6973 6f74     page.set_isot
+00003360: 726f 7069 635f 7363 616c 696e 6728 302c  ropic_scaling(0,
+00003370: 2031 302c 2030 2c20 3230 290d 0a20 2020   10, 0, 20)..   
+00003380: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+00003390: 2e70 6167 655f 706f 696e 7428 302c 2030  .page_point(0, 0
+000033a0: 292e 6973 636c 6f73 6528 2831 3235 2c20  ).isclose((125, 
+000033b0: 3130 3029 290d 0a20 2020 2020 2020 2061  100))..        a
+000033c0: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
+000033d0: 706f 696e 7428 352c 2031 3029 2e69 7363  point(5, 10).isc
+000033e0: 6c6f 7365 2828 3135 302c 2031 3530 2929  lose((150, 150))
+000033f0: 0d0a 2020 2020 2020 2020 6173 7365 7274  ..        assert
+00003400: 2070 6167 652e 7061 6765 5f70 6f69 6e74   page.page_point
+00003410: 2831 302c 2032 3029 2e69 7363 6c6f 7365  (10, 20).isclose
+00003420: 2828 3137 352c 2032 3030 2929 0d0a 0d0a  ((175, 200))....
+00003430: 2020 2020 6465 6620 7465 7374 5f69 736f      def test_iso
+00003440: 7472 6f70 6963 5f6c 6566 745f 7769 6e64  tropic_left_wind
+00003450: 6f77 5f30 2873 656c 6629 3a0d 0a20 2020  ow_0(self):..   
+00003460: 2020 2020 2070 6167 6520 3d20 5061 6765       page = Page
+00003470: 2831 3030 302c 2031 3030 3029 0d0a 2020  (1000, 1000)..  
+00003480: 2020 2020 2020 7061 6765 2e73 6574 5f73        page.set_s
+00003490: 6361 6c69 6e67 5f70 6f69 6e74 7328 5665  caling_points(Ve
+000034a0: 6332 2831 3030 2c20 3130 3029 2c20 5665  c2(100, 100), Ve
+000034b0: 6332 2832 3030 2c20 3230 3029 290d 0a20  c2(200, 200)).. 
+000034c0: 2020 2020 2020 2070 6167 652e 7365 745f         page.set_
+000034d0: 6973 6f74 726f 7069 635f 7363 616c 696e  isotropic_scalin
+000034e0: 6728 302c 2031 302c 2030 2c20 3230 2c20  g(0, 10, 0, 20, 
+000034f0: 302c 2030 290d 0a20 2020 2020 2020 2061  0, 0)..        a
+00003500: 7373 6572 7420 7061 6765 2e70 6167 655f  ssert page.page_
+00003510: 706f 696e 7428 302c 2030 292e 6973 636c  point(0, 0).iscl
+00003520: 6f73 6528 2831 3030 2c20 3130 3029 290d  ose((100, 100)).
+00003530: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+00003540: 7061 6765 2e70 6167 655f 706f 696e 7428  page.page_point(
+00003550: 352c 2031 3029 2e69 7363 6c6f 7365 2828  5, 10).isclose((
+00003560: 3132 352c 2031 3530 2929 0d0a 2020 2020  125, 150))..    
+00003570: 2020 2020 6173 7365 7274 2070 6167 652e      assert page.
+00003580: 7061 6765 5f70 6f69 6e74 2831 302c 2032  page_point(10, 2
+00003590: 3029 2e69 7363 6c6f 7365 2828 3135 302c  0).isclose((150,
+000035a0: 2032 3030 2929 0d0a 0d0a 2020 2020 6465   200))....    de
+000035b0: 6620 7465 7374 5f69 736f 7472 6f70 6963  f test_isotropic
+000035c0: 5f6c 6566 745f 7769 6e64 6f77 5f31 3030  _left_window_100
+000035d0: 2873 656c 6629 3a0d 0a20 2020 2020 2020  (self):..       
+000035e0: 2070 6167 6520 3d20 5061 6765 2831 3030   page = Page(100
+000035f0: 302c 2031 3030 3029 0d0a 2020 2020 2020  0, 1000)..      
+00003600: 2020 7061 6765 2e73 6574 5f73 6361 6c69    page.set_scali
+00003610: 6e67 5f70 6f69 6e74 7328 5665 6332 2831  ng_points(Vec2(1
+00003620: 3030 2c20 3130 3029 2c20 5665 6332 2832  00, 100), Vec2(2
+00003630: 3030 2c20 3230 3029 290d 0a20 2020 2020  00, 200))..     
+00003640: 2020 2070 6167 652e 7365 745f 6973 6f74     page.set_isot
+00003650: 726f 7069 635f 7363 616c 696e 6728 302c  ropic_scaling(0,
+00003660: 2031 302c 2030 2c20 3230 2c20 312c 2031   10, 0, 20, 1, 1
+00003670: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00003680: 7420 7061 6765 2e70 6167 655f 706f 696e  t page.page_poin
+00003690: 7428 302c 2030 292e 6973 636c 6f73 6528  t(0, 0).isclose(
+000036a0: 2831 3530 2c20 3130 3029 290d 0a20 2020  (150, 100))..   
+000036b0: 2020 2020 2061 7373 6572 7420 7061 6765       assert page
+000036c0: 2e70 6167 655f 706f 696e 7428 352c 2031  .page_point(5, 1
+000036d0: 3029 2e69 7363 6c6f 7365 2828 3137 352c  0).isclose((175,
+000036e0: 2031 3530 2929 0d0a 2020 2020 2020 2020   150))..        
+000036f0: 6173 7365 7274 2070 6167 652e 7061 6765  assert page.page
+00003700: 5f70 6f69 6e74 2831 302c 2032 3029 2e69  _point(10, 20).i
+00003710: 7363 6c6f 7365 2828 3230 302c 2032 3030  sclose((200, 200
+00003720: 2929 0d0a 0d0a 0d0a 6465 6620 7465 7374  ))......def test
+00003730: 5f61 7263 5f61 6e67 6c65 7328 293a 0d0a  _arc_angles():..
+00003740: 2020 2020 6672 6f6d 2065 7a64 7866 2e61      from ezdxf.a
+00003750: 6464 6f6e 732e 6870 676c 322e 706c 6f74  ddons.hpgl2.plot
+00003760: 7465 7220 696d 706f 7274 2061 7263 5f61  ter import arc_a
+00003770: 6e67 6c65 730d 0a0d 0a20 2020 2061 6e67  ngles....    ang
+00003780: 6c65 7320 3d20 6c69 7374 2861 7263 5f61  les = list(arc_a
+00003790: 6e67 6c65 7328 302c 2033 3630 2c20 3529  ngles(0, 360, 5)
+000037a0: 290d 0a20 2020 2061 7373 6572 7420 6c65  )..    assert le
+000037b0: 6e28 616e 676c 6573 2920 3d3d 2037 330d  n(angles) == 73.
+000037c0: 0a20 2020 2061 7373 6572 7420 616e 676c  .    assert angl
+000037d0: 6573 5b2d 315d 203d 3d20 7079 7465 7374  es[-1] == pytest
+000037e0: 2e61 7070 726f 7828 3336 3029 0d0a 0d0a  .approx(360)....
+000037f0: 2020 2020 616e 676c 6573 203d 206c 6973      angles = lis
+00003800: 7428 6172 635f 616e 676c 6573 2830 2c20  t(arc_angles(0, 
+00003810: 2d33 3630 2c20 3529 290d 0a20 2020 2061  -360, 5))..    a
+00003820: 7373 6572 7420 6c65 6e28 616e 676c 6573  ssert len(angles
+00003830: 2920 3d3d 2037 330d 0a20 2020 2061 7373  ) == 73..    ass
+00003840: 6572 7420 616e 676c 6573 5b2d 315d 203d  ert angles[-1] =
+00003850: 3d20 7079 7465 7374 2e61 7070 726f 7828  = pytest.approx(
+00003860: 2d33 3630 290d 0a0d 0a0d 0a64 6566 2074  -360)......def t
+00003870: 6573 745f 7377 6565 7069 6e67 5f61 6e67  est_sweeping_ang
+00003880: 6c65 2829 3a0d 0a20 2020 2066 726f 6d20  le():..    from 
+00003890: 657a 6478 662e 6164 646f 6e73 2e68 7067  ezdxf.addons.hpg
+000038a0: 6c32 2e70 6c6f 7474 6572 2069 6d70 6f72  l2.plotter impor
+000038b0: 7420 7377 6565 7069 6e67 5f61 6e67 6c65  t sweeping_angle
+000038c0: 0d0a 0d0a 2020 2020 6173 7365 7274 2073  ....    assert s
+000038d0: 7765 6570 696e 675f 616e 676c 6528 302c  weeping_angle(0,
+000038e0: 2034 352c 2039 3029 203d 3d20 3930 0d0a   45, 90) == 90..
+000038f0: 2020 2020 6173 7365 7274 2073 7765 6570      assert sweep
+00003900: 696e 675f 616e 676c 6528 3930 2c20 3435  ing_angle(90, 45
+00003910: 2c20 3029 203d 3d20 2d39 300d 0a20 2020  , 0) == -90..   
+00003920: 2061 7373 6572 7420 7377 6565 7069 6e67   assert sweeping
+00003930: 5f61 6e67 6c65 2833 3330 2c20 302c 2033  _angle(330, 0, 3
+00003940: 3029 203d 3d20 3630 0d0a 2020 2020 6173  0) == 60..    as
+00003950: 7365 7274 2073 7765 6570 696e 675f 616e  sert sweeping_an
+00003960: 676c 6528 3333 302c 2031 3830 2c20 3330  gle(330, 180, 30
+00003970: 2920 3d3d 202d 3330 300d 0a20 2020 2061  ) == -300..    a
+00003980: 7373 6572 7420 7377 6565 7069 6e67 5f61  ssert sweeping_a
+00003990: 6e67 6c65 2833 302c 2030 2c20 3333 3029  ngle(30, 0, 330)
+000039a0: 203d 3d20 2d36 300d 0a20 2020 2061 7373   == -60..    ass
+000039b0: 6572 7420 7377 6565 7069 6e67 5f61 6e67  ert sweeping_ang
+000039c0: 6c65 2833 302c 2031 3830 2c20 3333 3029  le(30, 180, 330)
+000039d0: 203d 3d20 3330 300d 0a0d 0a0d 0a63 6c61   == 300......cla
+000039e0: 7373 2054 6573 7450 6c61 6365 6d65 6e74  ss TestPlacement
+000039f0: 4d61 7472 6978 3a0d 0a20 2020 2064 6566  Matrix:..    def
+00003a00: 2074 6573 745f 7368 6966 745f 746f 5f6f   test_shift_to_o
+00003a10: 7269 6769 6e5f 5131 2873 656c 6629 3a0d  rigin_Q1(self):.
+00003a20: 0a20 2020 2020 2020 2062 626f 7820 3d20  .        bbox = 
+00003a30: 426f 756e 6469 6e67 426f 7832 6428 5b28  BoundingBox2d([(
+00003a40: 3130 2c20 3130 292c 2028 3230 2c20 3230  10, 10), (20, 20
+00003a50: 295d 290d 0a20 2020 2020 2020 206d 203d  )])..        m =
+00003a60: 2070 6c61 6365 6d65 6e74 5f6d 6174 7269   placement_matri
+00003a70: 7828 6262 6f78 290d 0a20 2020 2020 2020  x(bbox)..       
+00003a80: 2061 7373 6572 7420 6d2e 7472 616e 7366   assert m.transf
+00003a90: 6f72 6d28 2831 302c 2031 3029 292e 6973  orm((10, 10)).is
+00003aa0: 636c 6f73 6528 2830 2c20 3029 290d 0a20  close((0, 0)).. 
+00003ab0: 2020 2020 2020 2061 7373 6572 7420 6d2e         assert m.
+00003ac0: 7472 616e 7366 6f72 6d28 2832 302c 2032  transform((20, 2
+00003ad0: 3029 292e 6973 636c 6f73 6528 2831 302c  0)).isclose((10,
+00003ae0: 2031 3029 290d 0a0d 0a20 2020 2064 6566   10))....    def
+00003af0: 2074 6573 745f 7368 6966 745f 746f 5f6f   test_shift_to_o
+00003b00: 7269 6769 6e5f 5133 2873 656c 6629 3a0d  rigin_Q3(self):.
+00003b10: 0a20 2020 2020 2020 2062 626f 7820 3d20  .        bbox = 
+00003b20: 426f 756e 6469 6e67 426f 7832 6428 5b28  BoundingBox2d([(
+00003b30: 2d31 302c 202d 3130 292c 2028 2d32 302c  -10, -10), (-20,
+00003b40: 202d 3230 295d 290d 0a20 2020 2020 2020   -20)])..       
+00003b50: 206d 203d 2070 6c61 6365 6d65 6e74 5f6d   m = placement_m
+00003b60: 6174 7269 7828 6262 6f78 290d 0a20 2020  atrix(bbox)..   
+00003b70: 2020 2020 2061 7373 6572 7420 6d2e 7472       assert m.tr
+00003b80: 616e 7366 6f72 6d28 282d 3130 2c20 2d31  ansform((-10, -1
+00003b90: 3029 292e 6973 636c 6f73 6528 2831 302c  0)).isclose((10,
+00003ba0: 2031 3029 290d 0a20 2020 2020 2020 2061   10))..        a
+00003bb0: 7373 6572 7420 6d2e 7472 616e 7366 6f72  ssert m.transfor
+00003bc0: 6d28 282d 3230 2c20 2d32 3029 292e 6973  m((-20, -20)).is
+00003bd0: 636c 6f73 6528 2830 2c20 3029 290d 0a0d  close((0, 0))...
+00003be0: 0a20 2020 2064 6566 2074 6573 745f 726f  .    def test_ro
+00003bf0: 7461 7465 2873 656c 6629 3a0d 0a20 2020  tate(self):..   
+00003c00: 2020 2020 2023 2073 697a 6520 3d20 3130       # size = 10
+00003c10: 2078 2033 300d 0a20 2020 2020 2020 2062   x 30..        b
+00003c20: 626f 7820 3d20 426f 756e 6469 6e67 426f  box = BoundingBo
+00003c30: 7832 6428 5b28 3130 2c20 3130 292c 2028  x2d([(10, 10), (
+00003c40: 3230 2c20 3430 295d 290d 0a20 2020 2020  20, 40)])..     
+00003c50: 2020 206d 203d 2070 6c61 6365 6d65 6e74     m = placement
+00003c60: 5f6d 6174 7269 7828 6262 6f78 2c20 726f  _matrix(bbox, ro
+00003c70: 7461 7469 6f6e 3d39 3029 0d0a 2020 2020  tation=90)..    
+00003c80: 2020 2020 6173 7365 7274 206d 2e74 7261      assert m.tra
+00003c90: 6e73 666f 726d 2828 3130 2c20 3130 2929  nsform((10, 10))
+00003ca0: 2e69 7363 6c6f 7365 2828 3330 2c20 3029  .isclose((30, 0)
+00003cb0: 290d 0a20 2020 2020 2020 2061 7373 6572  )..        asser
+00003cc0: 7420 6d2e 7472 616e 7366 6f72 6d28 2832  t m.transform((2
+00003cd0: 302c 2034 3029 292e 6973 636c 6f73 6528  0, 40)).isclose(
+00003ce0: 2830 2c20 3130 2929 0d0a 0d0a 0d0a 6966  (0, 10))......if
+00003cf0: 205f 5f6e 616d 655f 5f20 3d3d 2022 5f5f   __name__ == "__
+00003d00: 6d61 696e 5f5f 223a 0d0a 2020 2020 7079  main__":..    py
+00003d10: 7465 7374 2e6d 6169 6e28 5b5f 5f66 696c  test.main([__fil
+00003d20: 655f 5f5d 290d 0a                        e__])..
```

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_822_clipper.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_822_clipper.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_823_drawing_layout.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_823_drawing_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_08_addons/test_824_svg_drawing_backend.py` & `ezdxf-1.1.0b3/tests/test_08_addons/test_824_svg_drawing_backend.py`

 * *Files 6% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 
 NS = {
     "http://www.w3.org/2000/svg": "",
 }
 
 
 class TestSVGBackend:
-    @pytest.fixture()
+    @pytest.fixture
     def backend(self):
         backend_ = svg.SVGBackend()
         properties = BackendProperties(color="#ff0000", lineweight=0.25)
         points = Vec2.list([(0, 0), (100, 0), (100, 100), (0, 100)])
         backend_.draw_filled_polygon(points, properties)
         return backend_
 
@@ -81,9 +81,16 @@
         xml = ET.fromstring(result)
         assert xml.tag.endswith("svg") is True
         assert xml.attrib["width"] == "400mm"
         assert xml.attrib["height"] == "300mm"
         assert xml.attrib["viewBox"] == "0 0 1000000 750000"
 
 
+def test_empty_page():
+    backend_ = svg.SVGBackend()
+    backend_.draw_point(Vec2(0, 0), BackendProperties())
+    result = backend_.get_string(layout.Page(0, 0), xml_declaration=False)
+    assert result == "<svg />"
+
+
 if __name__ == "__main__":
     pytest.main([__file__])
```

## Comparing `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_901_acc_vec2.py` & `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_901_acc_vec2.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_902_acc_vec3.py` & `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_902_acc_vec3.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_903_acc_matrix44.py` & `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_903_acc_matrix44.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py` & `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_904_acc_bezier4p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py` & `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_905_acc_bezier3p.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_09_cython_acceleration/test_906_acc_bspline.py` & `ezdxf-1.1.0b3/tests/test_09_cython_acceleration/test_906_acc_bspline.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_414_bbox_calculation.py` & `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_414_bbox_calculation.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py` & `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_557_reload_dimension_text_style.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_574_flattening_error.py` & `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_574_flattening_error.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py` & `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_589_incorrect_virtual_face3d.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_749_text_layout.py` & `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_749_text_layout.py`

 * *Files identical despite different names*

## Comparing `ezdxf-1.1.0b2/tests/test_10_issues/test_issue_873_circle_inverted_normal.py` & `ezdxf-1.1.0b3/tests/test_10_issues/test_issue_873_circle_inverted_normal.py`

 * *Files identical despite different names*

