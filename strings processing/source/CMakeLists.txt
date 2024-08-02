cmake_minimum_required(VERSION 3.28)

# Find
set(longStr abcdef)
set(shortStr ef)

string(FIND ${longStr} ${shortStr} findResult)
message("Find Result = ${findResult}")

string(REPLACE  ${shortStr} vodka replaceResult ${longStr})
message("Replace result =  ${replaceResult}")
