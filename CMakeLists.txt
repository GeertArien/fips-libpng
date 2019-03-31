#
# project: fips-libpng
#
cmake_minimum_required(VERSION 2.8)

# include the fips main cmake file
get_filename_component(FIPS_ROOT_DIR "../fips" ABSOLUTE)
include("${FIPS_ROOT_DIR}/cmake/fips.cmake")

fips_setup(PROJECT fips-libpng)
fips_include_directories(png)
fips_add_subdirectory(png)
fips_finish()


