cmake_minimum_required(VERSION 3.28)
project(variables)

include(CMakePrintHelpers)

# Set variable
set(myVar a b c)

# Get variable value
# ${myVar}

# Print variable value
cmake_print_variables(myVar)
message(${myVar})

# Simple multi-line content with bracket syntax
set(multiLine [[
First line
Second line
]])
cmake_print_variables(multiLine)

# unset variable
unset(multiLine)
cmake_print_variables(multiLine)