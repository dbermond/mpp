# vim: syntax=cmake
# ----------------------------------------------------------------------------
# add libvpu implement
# ----------------------------------------------------------------------------
add_library(utils STATIC
    mpi_enc_utils.c
    utils.c
    iniparser.c
    dictionary.c
    )

target_link_libraries(utils mpp_base)
