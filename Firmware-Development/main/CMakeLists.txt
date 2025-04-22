idf_component_register(
                        SRCS "ui.c" "waveshare_rgb_lcd_port.c" "main.c" "lvgl_port.c"
                        "screens/ui_HomeScreen.c"
                        "screens/ui_TimerStartScreen.c"
                        "screens/ui_LastSuccessScreen.c"
                        "screens/ui_DryScreen.c"
                        "screens/ui_infoScreen.c"
                        "screens/ui_WashDryScreen.c"
                        "screens/ui_WashDryDetailScreen.c"
                        "screens/ui_WashScreen.c"
                       
                        # "components/ui_comp_hook.c"
                        "ui_helpers.c"
                        "images/ui_img_washicon_png.c"
                        "images/ui_img_smallwashicon_png.c"
                        "images/ui_img_smallturbineicon_png.c"
                        "images/ui_img_turbineicon_png.c"
                        "images/ui_img_eevalogo_png.c"
                        "images/ui_img_settingsicon_png.c"
                        "images/ui_img_infoicon_png.c"
                        "images/ui_img_ion_image_png.c"
                        "images/ui_img_alarmclock_png.c"
                        "images/ui_img_last_screen_png.c"
                        "images/ui_img_qrcode_png.c"
                        "images/ui_img_backicon_png.c"
                        "images/ui_img_frame_12_png.c"
                        "images/ui_img_frame_13_png.c"
                        "images/ui_img_frame_14_png.c"
                        "images/ui_img_clockicon_png.c"
                        INCLUDE_DIRS ".")

idf_component_get_property(lvgl_lib lvgl__lvgl COMPONENT_LIB)
target_compile_options(${lvgl_lib} PRIVATE -Wno-format)
