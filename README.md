# ChonOS Embedded Multi-agent System Manager

|![](https://github.com/chon-group/dpkg-chonos-embeddedmas/assets/32855001/6a5c4bd4-c76b-40b0-b5ea-a652f8d3ac03)|
|:--:|
|ChonOS-EmbeddedMAS provides a command line multi-agent system manager it allows the hosting of BDI-based MAS in the reasoning layer of a cyber-physical system.|

## How to Install?
In a terminal run the commands below:

```console
echo "deb [trusted=yes] http://packages.chon.group/ chonos main" | sudo tee /etc/apt/sources.list.d/chonos.list
sudo apt update
sudo apt install chonos-embeddedmas
```


## How to use?

List of options and arguments:
+ --import    \- imports a MAS2J Project.

+ --start     \- starts the Embedded MAS.

+ --stop      \- stops the Embedded MAS.

+ -f [file]   \- defines the MAS2J project file.

+ -m [value]  \- defines how much heap memory (in MB) will be allocated to the Embedded MAS. By default, it will be allocated between 256 MB until 1024 MB. This option makes it possible to adjust the performance of the Embedded MAS.

### Examples:
- Importing the .ZIP file from the MAS2J Project.
    ```console
    root@machine:~# chonosEmbeddedMAS --import -f /home/user/MAS2Jproject.zip
    ```

- Executes the MAS2J Project previously imported. 
    ```console
    root@machine:~# chonosEmbeddedMAS --start
    ```

- Executes the MAS2J Project previously imported and allocates 512 MB for heap memory.  
    ```console
    root@machine:~# chonosEmbeddedMAS --start -m 512
    ```


## COPYRIGHT
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />The [_Cognitive Hardware on Networks Operating
System (chonOS)_](http://os.chon.group/) and is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>. The licensor cannot revoke these freedoms as long as you follow the license terms:

* __Attribution__ — You must give __appropriate credit__ like below:

Lazarin, N., Pantoja, C., Viterbo, J. (2026). An Operating-System Infrastructure for Embedded BDI-Based Multi-agent Systems. In: Gervasi, O., et al. Computational Science and Its Applications – ICCSA 2026. ICCSA 2026. Lecture Notes in Computer Science, vol 16769. Springer, Cham. [https://doi.org/10.1007/978-3-032-30494-0_37](https://www.researchgate.net/publication/405508586_An_Operating-System_Infrastructure_for_Embedded_BDI-based_Multi-Agent_Systems)

