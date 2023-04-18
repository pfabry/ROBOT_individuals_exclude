# ROBOT_individuals_exclude

Test for --individuals exclude parameter for ROBOT extract. 

The following command lines were used:
```
 robot extract --input obi.owl --method TOP --term-file entity.txt --output obiV1.owl
 robot extract --input obi.owl --method TOP --term-file entity.txt --individuals exclude --output obiV2.owl
```
entity.txt = "BFO:0000001"

2 versions of ROBOT tested: local (1.9.0) and via ODK (1.9.3)

In addition, the --force true option does not seems to work? When using it with an empty term-file I get an error message: 
```
robot extract --input obi.owl --method TOP --term-file empty.txt --force true --output obiV3.owl
MISSING TERMS ERROR term(s) are required with --term or --term-file
For details see: http://robot.obolibrary.org/errors#missing-terms-error
Use the -vvv option to show the stack trace.
Use the --help option to see usage information.
```
