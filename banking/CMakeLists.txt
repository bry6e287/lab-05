
project(banking_lib)

if (NOT TARGET libbanking)
    add_library(libbanking STATIC
        /Account.cpp
        /Transaction.cpp
    )

    install(TARGETS libbanking
        ARCHIVE DESTINATION lib
        LIBRARY DESTINATION lib
    )
endif(NOT TARGET libbanking)

include_directories()
