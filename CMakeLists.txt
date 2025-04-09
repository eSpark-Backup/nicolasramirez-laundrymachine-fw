SET(SOURCES screens/ui_HomeScreen.c
    ui.c
    components/ui_comp_hook.c
    ui_helpers.c
    images/ui_img_washicon_png.c
    images/ui_img_smallwashicon_png.c
    images/ui_img_smallturbineicon_png.c
    images/ui_img_turbineicon_png.c
    images/ui_img_eevalogo_png.c
    images/ui_img_settingsicon_png.c
    images/ui_img_infoicon_png.c)

add_library(ui ${SOURCES})
