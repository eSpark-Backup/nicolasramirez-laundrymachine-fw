idf_component_register(
                        SRCS "ui.c" "waveshare_rgb_lcd_port.c" "main.c" "lvgl_port.c"

                        "screens/ui_Home.c"
                        "screens/ui_WashDryLoad.c"
                        "screens/ui_WashDryWash.c"
                        "screens/ui_WashDryDry.c"
                        "screens/ui_JustWashConfirmation.c"
                        "screens/ui_WDConfirmation.c"
                        "screens/ui_successFinal.c"
                        "screens/ui_CycleProgress.c"

                        "ui_helpers.c"

                        "images/ui_img_HomeScreen.c"
                        "images/ui_img_WD_LoadSizeV1.c"
                        "images/ui_img_LoadSize_WashModeV2.c"
                        "images/ui_img_LoadSize_DryMode.c"
                        "images/ui_img_WD_ConfirmationScreenStensil.c"
                        "images/ui_img_WD_Final.c"
                        "images/ui_img_WD_CycleProgressStensil.c"
                        "images/ui_img_SmallLoadFrame.c"
                        "images/ui_img_CleanWashFrame.c"
                        "images/ui_img_DelicatesDryFrame.c"
                        "images/ui_img_DelicatesWashFrame.c"
                        "images/ui_img_EcoDryFrame.c"
                        "images/ui_img_FastestDryFrame.c"
                        "images/ui_img_FullLoadFrame.c"
                        "images/ui_img_IntenseWashFrame.c"
                        "images/ui_img_QuitestDryFrame.c"
                        "images/ui_img_JD_DelicatesFrame.c"
                        "images/ui_img_JD_EcoFrame.c"
                        "images/ui_img_JD_FastestFrame.c"
                        "images/ui_img_JD_FullLoadFrame.c"
                        "images/ui_img_JD_QuitestFrame.c"
                        "images/ui_img_JD_SmallLoadFrame.c"
                        "images/ui_img_JW_CnfrmCleanImg.c"
                        "images/ui_img_JW_CnfrmDelicatesImg.c"
                        "images/ui_img_JW_CnfrmIntenseImg.c"
                        "images/ui_img_JW_CnfrmSpinImg.c"
                        
                        INCLUDE_DIRS ".")

idf_component_get_property(lvgl_lib lvgl__lvgl COMPONENT_LIB)
target_compile_options(${lvgl_lib} PRIVATE -Wno-format)
