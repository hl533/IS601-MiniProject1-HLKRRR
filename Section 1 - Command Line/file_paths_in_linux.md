# file paths in linux

A path is a unique location to a file or a folder in a file system of an OS.A path to a file is a combination of / and alpha-numeric characters.

 

**Absolute Path-name**

 

An absolute path is defined as the specifying the location of a file or directory from the root directory(/). 

**To write an absolute path-name:**

 

-   Start at the root directory ( / ) and work down.

-   Write a slash ( / ) after every directory name (last one is optional)

 

**For Example :**

 

$cat abc.sql

 

will work  **only**  if the fie  **“abc.sql”**  exists in your current directory. However, if this file is not present in your working directory and is present somewhere else say in /home/kt , then this command will work only if you will use it like shown below:

 

cat /home/kt/abc.sql

 

In the above example, if the first character of a pathname is /, the file’s location must be determined with respect to root. When you have more than one / in a pathname, for each such /, you have to descend one level in the file system like in the above kt is one level below home, and thus two levels below root.

 

> An  **absolute path**  is defined as specifying the location of a file or directory from the root directory(/). In other words,we can say that an absolute path is a complete path from start of actual file system from / directory.

 

**Relative path**

 

Relative path is defined as the path related to the present working directly(pwd). It starts at your current directory and  **never starts with a /** .

 

To be more specific let’s take a look on the below figure in which if we are looking for photos then absolute path for it will be provided as  _/home/jono/photos_ **but assuming that we are already present in jono directory then the relative path for the same can be written as simple** _photos_. 

![](https://media.geeksforgeeks.org/wp-content/uploads/absolutePathNames.jpg)

 

**Using . and .. in Relative Path-names**

 

UNIX offers a shortcut in the  **relative pathname**– that uses either the current or parent directory as reference and specifies the path relative to it. A relative path-name uses one of these cryptic symbols:

 

**.(a single dot)** - this represents the current directory.

**..(two dots)** - this represents the parent directory.

 

Now, what this actually means is that if we are currently in directory /home/kt/abc and now you can use  **..**  as an argument to  **cd**  to move to the parent directory /home/kt as :

 

 

  

 

$pwd

/home/kt/abc

$cd ..               ***moves one level up***

$pwd

/home/kt

 

**NOTE:**Now / when used with .. has a different meaning ;instead of moving down a level,it moves one level up:

 

 

$pwd

/home/kt/abc        ***moves two level up***

$cd ../..

$pwd

/home

 

**Example of Absolute and Relative Path**

 

Suppose you are currently located in home/kt and you want to change your directory to home/kt/abc. Let’s see both the absolute and relative path concepts to do this:

 

1.  **Changing directory with relative path concept :**

   

    $pwd

    /home/kt

    $cd abc                  

    $pwd

    /home/kt/abc        

    

2.  **Changing directory with absolute path concept:**

   

    $pwd

    /home/kt

    $cd /home/kt/abc

    $pwd

    /home/kt/abc

    [https://www.geeksforgeeks.org/absolute-relative-pathnames-unix/](https://www.geeksforgeeks.org/absolute-relative-pathnames-unix/)
