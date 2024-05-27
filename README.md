# BATLab
EVSELab - HUST  
Le Minh Quan  
**BATLab** is an abbreviation for **Battery Automated Testing Laboratory**.  
![BATLab](images/BATLab)

# Overview
BATLab is a software developed to automate experimental procedures and test the characteristics and parameters of batteries. This software is developed within the .NET Framework under the .NET Platform, utilizing the C# language and packages from NuGet.

This repository serves as a prototype for the BATLab software, which is built upon existing serial monitor software solutions (e.g. [Serial Oscilloscope](https://github.com/xioTechnologies/Serial-Oscilloscope)) and battery testers software (e.g. [ZKETech EB Tester Software](http://www.zketech.com/nd.jsp?id=14)) available in the community (utilizing software reverse engineering techniques).

## Key Features
- **Serial Monitor:** BATLab has the capability to run independently as a serial monitor (inheriting functionalities from [Serial Oscilloscope](https://github.com/xioTechnologies/Serial-Oscilloscope)), enabling real-time monitoring and analysis of embedded device performance without the need for additional software. This dual-window system enhances threading capabilities, ensuring efficient handling of data transmission and reception, thereby optimizing performance during testing and analysis.
- **Data Logging:** BATLab logs test data into CSV files with timestamps, allowing for easy analysis and comparison of voltage and current trends over time.
- **Graphical Analysis:** The software includes a feature to plot voltage-current characteristic graphs over time during battery testing, providing visual insights into battery performance.
- **Automated Battery Testing**: BATLab features automated battery testing functionality, enabling hands-free operation and saving on labor, time, and costs. This feature is especially useful for continuous testing scenarios lasting up to 10 hours, where the software can autonomously conduct experiments, freeing up resources for other tasks.

## Requirements
- **Visual Studio Code and SWD4CS:** Due to limitations in hardware and memory, this repository utilizes Visual Studio Code as the Editor combined with [SWD4CS](https://danpapa-hry.hateblo.jp/entry/2022/02/23/210416) for building the graphical user interface (GUI) instead of using Visual Studio IDE. Specific instructions can be found [here](https://danpapa-hry.hateblo.jp/entry/2022/02/23/210416).
- **BBBidir and BMS 1.0:** - BATLab in this repository is used in conjunction with [BBBidir](https://github.com/renivimere/BBBidir) to achieve the most efficient automation of experimental procedures. In newer versions, the emergence of [BMS 1.0](https://github.com/renivimere/BMS_1.0) is notable. Please refer to the above repositories to gain a deeper understanding of the operational mechanism of this automated battery testing system.


### Note

- Due to security considerations, subsequent developmental versions of BATLab are not publicly available in this repository. This repository solely contains a prototype for the software. However, the source code provided here is relatively simple and well-structured, facilitating easy reuse.
- Feel free to download and utilize the source code provided in this repository. If desired and resources permit, you can also use Visual Studio IDE to compile this source code. However, you may encounter errors due to missing packages.
- Remember that this repository is merely an idea and not a complete industrial tool; the most important things lie in the functions, classes, and handlers.
