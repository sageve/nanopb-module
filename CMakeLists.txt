if (CONFIG_NANOPB_TEST)
    zephyr_library()

    list(APPEND CMAKE_MODULE_PATH ${ZEPHYR_BASE}/modules/nanopb)
    include(nanopb)

    zephyr_library_sources(src/test.c)
    zephyr_include_directories(include)
endif()