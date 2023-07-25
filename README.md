# Google Drive problem FIXED (Windows)
#### I had a problem with my Google Drive, it took me so long to figure out the solution but in the end it is quite simple. 
#### In this repository I will explain you how you can fix GDrive.

#### Go to C:\Windows\System32\drivers\etc in your file explorer. Now open "hosts" file as an administrator in your text editor.
#### If your file looks like this:
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

Then you have a problem.
