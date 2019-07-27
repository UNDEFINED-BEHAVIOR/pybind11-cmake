project(PyBind11CmakeExample)

pybind11_add_module(${PROJECT_NAME})

target_sources(
    ${PROJECT_NAME}
    PUBLIC
    src/main.cpp
)

target_include_directories(
    ${PROJECT_NAME}
    PUBLIC
    include
)

install(TARGETS ${PROJECT_NAME} DESTINATION ${CMAKE_SOURCE_DIR}/scripts)