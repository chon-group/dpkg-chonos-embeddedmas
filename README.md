# ChonOS Embedded Multi-agent System Manager

|![]()|
|:--:|
|ChonOS-EmbeddedMAS provides a command line multi-agent system manager.|

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
<a rel="license" href="http://creativecommons.org/licenses/by/4.0/"><img alt="Creative Commons License" style="border-width:0" src="https://i.creativecommons.org/l/by/4.0/88x31.png" /></a><br />The Chonos-Log is part of the [_Cognitive Hardware on Networks Operating
System (chonOS)_](http://os.chon.group/) and is licensed under a <a rel="license" href="http://creativecommons.org/licenses/by/4.0/">Creative Commons Attribution 4.0 International License</a>. The licensor cannot revoke these freedoms as long as you follow the license terms:

* __Attribution__ — You must give __appropriate credit__ like below:

LAZARIN, Nilson Mori; PANTOJA, Carlos Eduardo; VITERBO, José. Towards a Toolkit for Teaching AI Supported by Robotic-agents: Proposal and First Impressions. In: WORKSHOP SOBRE EDUCAÇÃO EM COMPUTAÇÃO (WEI), 31. , 2023, João Pessoa/PB. Anais [...]. Porto Alegre: Sociedade Brasileira de Computação, 2023 . p. 20-29. ISSN 2595-6175. DOI: https://doi.org/10.5753/wei.2023.229753.


<details>
<summary> Bibtex citation format</summary>

```
@inproceedings{chonOS,
 author = {Nilson Lazarin and Carlos Pantoja and José Viterbo},
 title = { Towards a Toolkit for Teaching AI Supported by Robotic-agents: Proposal and First Impressions},
 booktitle = {Anais do XXXI Workshop sobre Educação em Computação},
 location = {João Pessoa/PB},
 year = {2023},
 issn = {2595-6175},
 pages = {20--29},
 publisher = {SBC},
 address = {Porto Alegre, RS, Brasil},
 doi = {10.5753/wei.2023.229753},
 url = {https://sol.sbc.org.br/index.php/wei/article/view/24887}
}

```
</details>
