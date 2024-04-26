qt_add_executable(
    hello_world_qt_cmake
    main.cpp
    scenemodifier.cpp
)

target_link_libraries(hello_world_qt_cmake PRIVATE 
    Qt6::Core
    Qt6::Gui
    Qt6::Widgets
    Qt6::3DCore
    Qt6::3DExtras
    Qt6::3DRender
    Qt6::3DInput
)
set_target_properties(hello_world_qt_cmake PROPERTIES
    WIN32_EXECUTABLE ON
    MACOSX_BUNDLE ON
)