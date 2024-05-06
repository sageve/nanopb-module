if (CONFIG_NANOPB_TEST)
    zephyr_library()

    zephyr_library_sources(src/test.c)
    zephyr_include_directories(include)
endif()