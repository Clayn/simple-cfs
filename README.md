# simple-cfs
This project a simple "usage layer" to an CFS Implementation. 

The idea is that while you are already implementation independable using the CFS API you still have to worry on how to get the filesystem. So this project will make file access even easier by using simple objects that will use the filesystem defined at one location. In other words create the filesystem once and work with files and directories as they do all the cfs operations needed. 

This allows you to swtich the filesystem easier than before. Now you have to change the 'mounted' filesystem at one point and all your previous created files and directories will suddenly use that one. However you have to be sure what you are doing since this may cause some troubles thinking you just wrote to an file and suddenly that file doesn't exists.
