# chonosEmbeddedMAS - ChonOS Embedded Multi-agent System Manager

## DESCRIPTION
A manager of the Jason Embedded Multi-agent Systems.

List of options and arguments:
+ --import    \- imports a MAS2J Project.

+ --start     \- starts the Embedded MAS.

+ --stop      \- stops the Embedded MAS.

+ -f [file]   \- defines the MAS2J project file.

+ -l term     \- shows the Log in the terminal.

+ -m [value]  \- defines how much heap memory (in MB) will be allocated to the Embedded MAS. By default, it will be allocated between 256 MB until 1024 MB. This option makes it possible to adjust the performance of the Embedded MAS.

## EXAMPLE
Importing the .ZIP file from the MAS2J Project.
```console
root@machine:~# chonosEmbeddedMAS --import -f /home/user/MAS2Jproject.zip
```

Executes the MAS2J Project previously imported. 
```console
root@machine:~# chonosEmbeddedMAS --start
```

Executes the MAS2J Project previously imported and allocates 512 MB for heap memory.  
```console
root@machine:~# chonosEmbeddedMAS --start -m 512
```

## COPYRIGHT
https://github.com/chon-group/jasonEmbedded
