# ROSAL
ROSAL - Real Time Operating System Abstraction Layer



## Project Description
ROSAL is a **R**eal Time **O**perating **S**ystem **A**bstraction **L**ayer created specifically for projects using C++ as the target programming language. The main purpose of this abstraction layer is to make your code independent of the underlying RTOS, giving you the option to switch it at any point in time and also enabling testing your code in desktop environments.



## Motivation for this project
The main motivation for the creation of this project was the absence of a good Real Time Operating System Abstraction Layer to be used in C++ projects.
If you want to start a new IoT/Embedded project, you have a very important initial decision to make related to the RTOS that you will use for your project. Most of the RTOS are created in C language, so using some of them is not that easy in C++, requiring you to create some sort of wrapper on top of the existing C API. Testing code in a desktop environment is also something that some RTOS platforms are lacking because they were created specifically for a target set of hardware in mid. Finally if you want to switch from one RTOS to another one in the middle of the project for any reason, you will have a lot of work to convert your code to the new selected RTOS. 



## NASA OSAL is almost perfect, but not for all of us
If you never heard of Nasa [OSAL](https://github.com/nasa/osal), [cFE](https://github.com/nasa/cFE) and [cFS](https://github.com/nasa/cFS), I strongly recommend you to take a look at these projects. They created a very high quality code and it follows the same idea of abstracting the underlying operating system and building on top of this abstraction, allowing developers to have the flexibility to use the best option according to their needs and enabling switch from one OS to another. The only two main downsides why I believe this is almost perfect but not for me is related to the fact that the system is created in C and will require some C++ wrapper if you want to use only C++ in your project. The second complain is related to the fact that they support only two RTOSes out of the box [RTEMS](https://www.rtems.org/) and [VxWorks]( https://www.windriver.com/products/vxworks). You can expand it to use other RTOS but is up to you to integrate and test it.



## List of some RTOS and projects that become inspirational for ROSAL:
* Zephyr: https://www.zephyrproject.org/
* FreeRTOS: https://www.freertos.org/
* ThreadX: https://azure.microsoft.com/en-us/services/rtos/
* µC/OS: https://www.micrium.com/rtos/
* µOS++: http://micro-os-plus.github.io/
* Mbed OS: https://os.mbed.com/
* NuttX https://nuttx.apache.org/
* RTEMS: https://www.rtems.org/
* Chibios: https://www.chibios.org/dokuwiki/doku.php
* Distortos: https://distortos.org/
* scmRTOS: https://github.com/scmrtos/scmrtos
* VxWorks: https://www.windriver.com/products/vxworks
* NASA OSAL: https://github.com/nasa/osal
* NASA cFS: https://github.com/nasa/cFS
* Nasa cFE: https://github.com/nasa/cFE


## Similarities and Differences
If you review the list of these RTOSes you will quickly realize that they share a lot of common characteristics, but at the same time they are different, because they were created in different times, with different purposes and scope. As part of this project we will try to create an abstraction layer that will share the common attributes of most of them but keep in mind that it will still be required for you to use services provided by the underlying RTOS with functionality not abstracted by ROSAL.



## Version History
* Still in planning phase


## Known issues
* Not known issues so far


## License
ROSAL was created by Pablo Abraham and is provided under the terms of the
[Apache 2.0 License](https://opensource.org/licenses/Apache-2.0).
