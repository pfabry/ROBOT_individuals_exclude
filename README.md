# ROBOT_individuals_exclude

Test for --individuals exclude parameter for ROBOT extract. 

The following command lines were used:

 - robot extract --input obi.owl --method TOP --term-file entity.txt --output obiV1.owl
 - robot extract --input obi.owl --method TOP --term-file entity.txt --individuals exclude --output obiV2.owl

entity.txt = "BFO:0000001"

2 versions of ROBOT tested: local (1.9.0) and via ODK (1.9.3)
