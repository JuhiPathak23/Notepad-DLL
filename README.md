# Notepad DLL
This project introduces a Dynamic Link Library (DLL) designed to enhance the functionality of the Notepad application on Windows. The DLL integrates custom menu items and demonstrates basic text manipulation capabilities, showcasing the power of DLLs in extending software functionality.

## Introduction
A DLL is a library that contains code and data that can be used by more than one program at the same time. For example, in Windows operating systems, the Comdlg32 DLL performs common dialog box related functions. Each program can use the functionality that is contained in this DLL to implement an Open dialog box. It helps promote code reuse and efficient memory usage. By using a DLL, a program can be modularized into separate components. For example, an accounting program may be sold by module. Each module can be loaded into the main program at run time if that module is installed. Because the modules are separate, the load time of the program is faster. And a module is only loaded when that functionality is requested.

This DLL project represents a significant milestone in my journey of learning software development on Windows. It provided an opportunity to delve into the intricacies of DLLs, their role in software extension, and their integration with existing applications like Notepad.

## Key Features
1. Custom Menu Integration: Adds a custom menu item to Notepad for executing specialized actions.
2. Text Manipulation: Demonstrates basic text manipulation within Notepad, illustrating the potential for extending application capabilities through DLLs.
   
## Learning Experience
As a novice in DLL development, this project served as a practical learning experience:
1. Discovery: I discovered the concept of DLLs and their role in software modularity and extension.
2. Implementation: Through trial and error, I learned to implement basic DLL functionalities, starting with integrating custom menu items and manipulating text within Notepad.
3. Challenges: Overcoming challenges such as understanding DLL entry points (DllMain), managing memory, and ensuring compatibility with different versions of Windows contributed significantly to my learning curve.
4. Cool stuff: I got to discover how I can easily list any project IDs on the system and used a DLL injector for the same.
   ## ![Screenshot 2024-07-02 014957](https://github.com/JuhiPathak23/Notepad-DLL/assets/73741643/259fc59b-79ef-4b04-879e-b6579d145d9b)
   ## ![image](https://github.com/JuhiPathak23/Notepad-DLL/assets/73741643/7667bb6f-ee26-4129-8318-13c0ae9ce3a5)

## How It Helped Me Make My First DLL
Creating this Notepad DLL was instrumental in:
1. Hands-On Learning: Providing hands-on experience in coding, debugging, and refining software components.
2. Problem-Solving: Encountering and resolving issues related to DLL integration, such as correct function signatures and handling of Windows messages.
3. Building Confidence: Boosting my confidence in software development by successfully creating and integrating a functional DLL into a widely-used Windows application.

## Usage
### Building the DLL
To build the DLL, you can use a C compiler such as gcc on Windows or Visual Studio:

    bash
    gcc -shared -o MainDLL.dll MainDLL.c -Wl,--out-implib,libMainDLL.a
### Injecting the DLL
Use a DLL injector tool like Process Hacker to inject notepaddll.dll into a running instance of Notepad.

### Legal and Ethical Considerations
Respect the terms of service and usage guidelines of any software application you interact with using DLLs.
Use DLLs responsibly and for legitimate purposes only, adhering to ethical development practices.

## Feedback
Feedback and contributions to improve this project are welcome! Feel free to fork this repository, make enhancements, and submit pull requests.
