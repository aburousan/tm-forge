

INKSCAPE= /Applications/Inkscape.app/Contents/MacOS/inkscape --batch-process


icons24= \
	post-modern/24x24/main/tm_cloud.png	\
	post-modern/24x24/main/tm_cloud_download.png	\
	post-modern/24x24/main/tm_cloud_upload.png	\
	post-modern/24x24/main/tm_cloud_home.png	\
	post-modern/24x24/main/tm_cloud_mail.png	\
	post-modern/24x24/main/tm_cloud_mail_new.png	\
	post-modern/24x24/main/tm_cloud_file.png	\
	post-modern/24x24/main/tm_cloud_dir.png	\
	post-modern/24x24/main/tm_back.png	\
	post-modern/24x24/main/tm_build.png	\
	post-modern/24x24/main/tm_cancel.png	\
	post-modern/24x24/main/tm_copy.png	\
	post-modern/24x24/main/tm_cut.png	\
	post-modern/24x24/main/tm_find.png	\
	post-modern/24x24/main/tm_forward.png	\
	post-modern/24x24/main/tm_language.png	\
	post-modern/24x24/main/tm_larrow.png	\
	post-modern/24x24/main/tm_larrow_bar.png	\
	post-modern/24x24/main/tm_larrow_double.png	\
	post-modern/24x24/main/tm_load.png	\
	post-modern/24x24/main/tm_new.png	\
	post-modern/24x24/main/tm_open.png	\
	post-modern/24x24/main/tm_paste.png	\
	post-modern/24x24/main/tm_preferences.png	\
	post-modern/24x24/main/tm_print.png	\
	post-modern/24x24/main/tm_rarrow.png	\
	post-modern/24x24/main/tm_rarrow_bar.png	\
	post-modern/24x24/main/tm_rarrow_double.png	\
	post-modern/24x24/main/tm_redo.png	\
	post-modern/24x24/main/tm_reload.png	\
	post-modern/24x24/main/tm_replace.png	\
	post-modern/24x24/main/tm_save.png	\
	post-modern/24x24/main/tm_spell.png	\
	post-modern/24x24/main/tm_undo.png	
	
icons20= \
	post-modern/20x20/mode/tm_animate.png	\
	post-modern/20x20/mode/tm_color.png	\
	post-modern/20x20/mode/tm_image.png	\
	post-modern/20x20/mode/tm_link.png	\
	post-modern/20x20/mode/tm_macro.png	\
	post-modern/20x20/mode/tm_overlays.png	\
	post-modern/20x20/mode/tm_shell.png	\
	post-modern/20x20/mode/tm_switch.png	\
	post-modern/20x20/mode/tm_table.png	

icons16= \
	post-modern/16x16/focus/tm_search_first.png	\
	post-modern/16x16/focus/tm_search_last.png	\
	post-modern/16x16/focus/tm_search_next.png	\
	post-modern/16x16/focus/tm_search_previous.png	\
	post-modern/16x16/focus/tm_go.png	\
	post-modern/16x16/focus/tm_stop.png	\
	post-modern/16x16/focus/tm_exit_left.png	\
	post-modern/16x16/focus/tm_exit_right.png	\
	post-modern/16x16/focus/tm_add.png	\
	post-modern/16x16/focus/tm_theme.png	\
	post-modern/16x16/focus/tm_similar_first.png	\
	post-modern/16x16/focus/tm_similar_last.png	\
	post-modern/16x16/focus/tm_similar_next.png	\
	post-modern/16x16/focus/tm_similar_previous.png	\
	post-modern/16x16/focus/tm_lock_closed.png	\
	post-modern/16x16/focus/tm_lock_open.png	\
	post-modern/16x16/focus/tm_like.png	\
	post-modern/16x16/focus/tm_insert_down.png	\
	post-modern/16x16/focus/tm_insert_left.png	\
	post-modern/16x16/focus/tm_insert_right.png	\
	post-modern/16x16/focus/tm_insert_up.png	\
	post-modern/16x16/focus/tm_focus_delete.png	\
	post-modern/16x16/focus/tm_focus_help.png	\
	post-modern/16x16/focus/tm_focus_prefs.png	\
	post-modern/16x16/focus/tm_focus_style.png	\
	post-modern/16x16/focus/tm_focus_search.png	\
	post-modern/16x16/focus/tm_filter.png	\
	post-modern/16x16/focus/tm_delete_down.png	\
	post-modern/16x16/focus/tm_delete_left.png	\
	post-modern/16x16/focus/tm_delete_right.png	\
	post-modern/16x16/focus/tm_delete_up.png	


icons24x2= $(icons24:.png=_x2.png)
icons24x4= $(icons24:.png=_x4.png)

icons20x2= $(icons20:.png=_x2.png)
icons20x4= $(icons20:.png=_x4.png)

icons16x2= $(icons16:.png=_x2.png)
icons16x4= $(icons16:.png=_x4.png)

all_icons= $(icons24) $(icons24x2) $(icons24x4) $(icons20) $(icons20x2) $(icons20x4) $(icons16) $(icons16x2) $(icons16x4)

all: $(all_icons)

install: all
	find . -name '*.png' -exec cp {} ~/.TeXmacs/misc/pixmaps/. \;

PHONY: all install

$(icons24): %.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 24 -o $@ $<

$(icons24x2): %_x2.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 48 -o $@ $<

$(icons24x4): %_x4.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 96 -o $@ $<

$(icons20): %.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 20 -o $@ $<

$(icons20x2): %_x2.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 40 -o $@ $<

$(icons20x4): %_x4.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 80 -o $@ $<

$(icons16): %.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 16 -o $@ $<

$(icons16x2): %_x2.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 32 -o $@ $<

$(icons16x4): %_x4.png : src/%.svg
	$(INKSCAPE) --export-type="png" -w 64 -o $@ $<

