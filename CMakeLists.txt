add_executable(bop
        bop.c
        )

# pull in common dependencies
target_link_libraries(bop pico_stdlib)

# create map/bin/hex file etc.
pico_add_extra_outputs(bop)

# add url via pico_set_program_url
example_auto_set_url(bop)
