# команда list

cmake_minimum_required(VERSION 3.28)

set (myList a b c)
list(LENGTH myList len)
message("length = ${len}")

list (GET myList 2 1 letters)
message("letters = ${letters}")