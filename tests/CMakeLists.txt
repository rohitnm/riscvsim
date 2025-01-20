add_executable(test_riscv
    # Add the test source files here
)

# Link with the main simulator
target_link_libraries(test_riscv PRIVATE riscv_simulator)
