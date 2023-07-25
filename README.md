# Google Drive problem FIXED (Windows)
#### I had a problem with my Google Drive, it took me so long to figure out the solution but in the end it is quite simple. 
#### In this repository I will explain you how you can fix GDrive.

#### Go to C:\Windows\System32\drivers\etc in your file explorer. Now open "hosts" file as an administrator in your text editor.
#### If you have a problem in this file, then it will look like this:
```
  # Copyright (c) 1993-2009 Microsoft Corp.
  #
  # This is a sample HOSTS file used by Microsoft TCP/IP for Windows.
  #
  # This file contains the mappings of IP addresses to host names. Each
  # entry should be kept on an individual line. The IP address should
  # be placed in the first column followed by the corresponding host name.
  # The IP address and the host name should be separated by at least one
  # space.
  #
  # Additionally, comments (such as these) may be inserted on individual
  # lines or following the machine name denoted by a '#' symbol.
  #
  # For example:
  #
  #      102.54.94.97     rhino.acme.com          # source server
  #       38.25.63.10     x.acme.com              # x client host
  
  # localhost name resolution is handled within DNS itself.
  #  127.0.0.1       localhost
  #  ::1             localhost

  // My commentary
  // some 0.0.0.0's depends on your software installed,
  // For instance, if you have Adobe Premiere Pro installed, you will probably have this line:
  0.0.0.0 genuine.adobe.com
  ...
  ...

  // My commentary
  // and then this "clients google" lines
  // All the problem is in this lines
  // I had all this lines from 0 to 9, but you can have only one or two

  127.0.0.1 clients.google.com
  127.0.0.1 clients0.google.com
  127.0.0.1 clients1.google.com
  127.0.0.1 clients3.google.com
  127.0.0.1 clients4.google.com
  127.0.0.1 clients5.google.com
  127.0.0.1 clients6.google.com
  127.0.0.1 clients7.google.com
  127.0.0.1 clients8.google.com
  127.0.0.1 clients9.google.com
```

### So, I deleted all the client.google lines and it helped.
### You will also have a problem with Google Chrome Extensions if you have this lines in "hosts" file.
##### (Extensions will not download)
### If you have this problem but you "hosts" file is empty (except big commentary), then I don't know how to fix this.


