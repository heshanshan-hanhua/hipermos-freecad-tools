#########################
#Date               Name        Description of Change
#2021/07/01         ZJF         Add BaseHH
#2021/08/17         LL          Add GuiFC
#2021/11/12         ZJF         Add RunTimeDebug
#2021/12/19          LL         Add HiperMOS dir
#2021/13/31         WS          delete HiperMOS dir
#########################
add_subdirectory(Build)
add_subdirectory(3rdParty)
add_subdirectory(Base)
add_subdirectory(App)
add_subdirectory(Main)
add_subdirectory(Mod)
add_subdirectory(Ext)
add_subdirectory(Doc)
add_subdirectory(BaseHH)
add_subdirectory(RunTimeDebug)

if(BUILD_GUI)
    add_subdirectory(Gui)
    add_subdirectory(GuiFC)
    if(UNIX AND NOT APPLE)
        add_subdirectory(XDGData)
    endif()
endif(BUILD_GUI)
if(BUILD_TEMPLATE)
    add_subdirectory(Tools/_TEMPLATE_)
endif(BUILD_TEMPLATE)


if(FREECAD_CREATE_MAC_APP)
    add_subdirectory(MacAppBundle)
endif(FREECAD_CREATE_MAC_APP)