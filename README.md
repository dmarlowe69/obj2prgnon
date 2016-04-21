OBJ2PRGNON allows an interface file to be converted into a program file without
loading it into memory. The orginal program OBJ2PRG had a limitation that the the interface file
could contain gaps in memory from record to record. The memory requested by the interface file had to be 
contiguous.

This revisised version supports gaps by filling them will a padding byte ($AA). 

This program will make sure that in non contiguos is up in memeory and not back. If it
finds a record with an eralier address, it will trucate the PRG file report the error and exit.
The resulting PRG file will contain a memory image defined up to the break.
