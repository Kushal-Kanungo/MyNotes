# System Calls

Date: October 5, 2022 1:38 PM
Status: Done

- **System Calls** :
    
    Provide mechanisms to Apps in user space interact with kernel and then hardware . Because Apps do not have permission to hardware directly. System Calls are the only way.
    
    - **Example: Mkdir**
        
        Mkdir indirectly call kernel and ask the file management
        
        Mkdir is just a wrapper of actual **System call**
        
        Mkdir interacts with kernel through **System Calls**
        
    - **Example : Creating a Process**
        
        User executes a process.(US)
        
        Gets system call(US)
        
        Exec. system call to create process(kernel)
        
        Return to US
        

Transition of US and Kernel is done by **Software Interrupts**

> Actual implementation is written in C or we can say System Calls are written in C language.
> 

System Call Interface is present in kernel which have written what to do when a particular system call is arrived.

![Untitled](System%20Calls%200b4f3c91f108468c9cf809f098aa5d76/Untitled.png)

# Types Of System Calls

- **Process Control**
    1. end, abort
    2. load, execute
    3. create, terminate process
    4. wait for time
    5. allocate and free memory
    6. wait event, signal event
- **File Management**
    1. create and delete file
    2. open and close
    3. read, write, reposition
    4. get file attributes and set file attribute
- **Device Management**
    1. request device, release device
    2. read, write
    3. get and set attributes
    4. logically attach and detach device
- **Communication Management**
    1. create and delete communication connection
    2. send and receive message
    3. transfer status info
    4. attach and detach remote device
- **Information Management**
    1. set and get system time
    2. get and set system data
    3. get and set process, file, attributes