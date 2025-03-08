# std
A standard cross language library.

Built in collaboration with the Low Level Team (LLT). Together the low level team has built sections and different parts of a complete standard library.

This standard library sits as a thin wrapper above operating system functionality.

A full list of features include:
  Memory      (Memory allocation, memory mapping, shared memory, memory protection (pages?))
  IO Stream   (Memory, Buffer, File, TCP Socket, UDP Socket, UNIX Domain Socket, Device, Window, Pipes, Message Queues, ...)
  IO Info     (filesystem, socket address, ...)
  Time        (Date, Time, Timers)
  Process     (Process, Thread, Signals, Scheduling, Synchronization)
  System      (OS Details, Architecture Details, Resource Limits, User/Group Information, Permissions, ...)

### Memory
interaction with OS managed memory, memory that can't or would be inconvenient on the stack can exist on the 'heap'.

### IO Stream
An IO stream in this scenario refers to any functinoality with meaningless input and output as its main purpose.
The IO stream contains functionality for writing into the stream, reading from the stream and controlling the stream.

Streams are mostly similar for example memory, buffers, files, sockets of all types, pipes and message queues all have simialr functionality.
This functionality mainly differs for special streams like device streams (i.e. keyboard input) or terminal and window.
These streams can still be read and writt

### IO Info (IOI)
IO Info is mainly duo to a lack of creative thinking. In this case everything here mainly refers to stream creation.
The specifics of each stream relies in its creation like the file system for file streams and address resolution for socket streams.
Most of this and IO stream is provided by SimpleIO by LowLevelIO.

### Time
Time is the most overlooked fetures of operating systems needed in scheduling, cron jobs and repeatable events.

### Process
Threads, program, scheduling and synchronization without these there is no real optimization.
This section is hopefully self explanatory

### System
Everything else done by the system, less well known but equally vital, maybe (i have seen some operating systems with some wacky system calls)

