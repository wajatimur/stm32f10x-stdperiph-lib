# STM32F10x Standard Peripherals Library
## Version 3.5

The STM32F10x Standard Peripherals library covers 3 abstraction levels, and includes:

- A complete register address mapping with all bits, bit fields and registers declared in C.  This avoids a cumbersome task and more important, it brings the benefits of a bug free reference mapping file, speeding up the early project phase. 

- A collection of routines and data structures which covers all peripheral functions (drivers with common API). It can directly be used as a reference framework, since it also includes macros for supporting core-related intrinsic features and common constants and data types definition. 

- A set of examples covering all available peripherals with template projects for the most common development toolchains. With the appropriate hardware evaluation board, this allows to get started with a brand new micro within few hours.

Each driver consists of a set of functions covering all peripheral functionalities. The development of each driver is driven by a common API (application programming interface) which standardizes the driver structure, the functions and the parameter names.
The driver source code is developed in ‘Strict ANSI-C’ (relaxed ANSI-C for projects and example files). It is fully documented and is MISRA-C 2004 compliant. Writing the whole library in ‘Strict ANSI-C’ makes it independent from the software toolchain. Only the start-up files depend on the toolchain.

The Standard Peripherals Library implements run-time failure detection by checking the input values for all library functions. Such dynamic checking contributes towards enhancing the robustness of the software. Run-time detection is suitable for user application development and debugging. It adds an overhead which can be removed from the final application code to minimize code size and execution speed. For more details refer to Section Run-time checking.

Since the Standard Peripherals Library is generic and covers all peripheral functionalities, the size and/or execution speed of the application code may not be optimized. For many applications, the library may be used as is. However, for applications having tough constraints in terms of code size and/or execution speed, the library drivers should be used as a reference on how to configure the peripheral and tailor them to specific application requirements. 

Note: The performance of application code, in terms of size and/or speed, depends also from the C compiler optimization settings. To help make the application code smaller, faster or balanced between size and speed you should consider fine-tuning the optimizations according to your application needs. For more information please refer to your C compiler documentation.

The enclosed firmware and all the related documentation are not covered by a License Agreement, if you need such License you can contact your local STMicroelectronics office.

THE PRESENT FIRMWARE WHICH IS FOR GUIDANCE ONLY AIMS AT PROVIDING CUSTOMERS WITH CODING INFORMATION REGARDING THEIR PRODUCTS IN ORDER FOR THEM TO SAVE TIME. AS A RESULT, STMICROELECTRONICS SHALL NOT BE HELD LIABLE FOR ANY DIRECT, INDIRECT OR CONSEQUENTIAL DAMAGES WITH RESPECT TO ANY CLAIMS ARISING FROM THE CONTENT OF SUCH FIRMWARE AND/OR THE USE MADE BY CUSTOMERS OF THE CODING INFORMATION CONTAINED HEREIN IN CONNECTION WITH THEIR PRODUCTS.
