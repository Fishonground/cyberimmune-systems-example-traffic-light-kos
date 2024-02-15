project (ControlSystem)

# Tools for using NK parser.
include (platform/nk)

# Set compile flags.
project_header_default ("STANDARD_GNU_11:YES" "STRICT_WARNINGS:NO")

add_executable (Diagnostic "src/diagnostic.c")
add_dependencies (Diagnostic traffic_light_idl_files traffic_light_diagnostic_edl_files)