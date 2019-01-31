# URLDUMP

This is a utility that scans a directory for .url (Windows) and .webloc (MacOS) shortcut files and produce a Markdown-formatted listing. I have a folder full of these that I'd like to scan and organize.

The utility is written as a NodeJS utility that installs to your command path via NPM.

## Installing

If you don't have Node, install it. Then clone this repo. Issue the following commands. 
```
> cd urldump
> npm install
> npm link
```
The `npm link` command installs urldump as a global command. (Mac) If you need to delete it and `npm unlink` fails, go to `usr/local/bin/` and delete the `urldump@` symlink there.

## Using

This is a pretty basic command.
```
> urldump             # scans current directory for webloc and url
> urldump <dir>       # scans for subpath in current directory
> urldump /full/path  # scan the specified full path
```
Formatted text is output to the console, so to capture it to a file do something like this:
```
> urldump > index.md
```
The formatting is as a bulleted list:

`* 2013/11/03 [Name of Shortcut File](http://url-to-destination)`

That's all it does! It's pretty straightforward.



* 2018/12/13 [ Intel IoT Platform Reference Architecture](https://www.intel.de/content/www/de/de/internet-of-things/white-papers/iot-platform-reference-architecture-paper.html)
* 2018/12/13 [A Reference Architecture for the Internet of Things W02](https://wso2.com/whitepapers/a-reference-architecture-for-the-internet-of-things/)
* 2018/12/13 [AWS Application Architecture Center](https://aws.amazon.com/architecture/)
* 2018/12/13 [Azure IoT Fundamentals Microsoft Docs](https://docs.microsoft.com/en-us/azure/iot-fundamentals/)
* 2018/12/13 [Azure IoT Reference Architecture](http://aka.ms/iotrefarchitecture)
* 2018/12/13 [EbolonIoTReferenceArchitectures IoT Reference Architectures](https://github.com/Ebolon/IoT-Reference-Architectures)
* 2018/12/13 [Microsoft Azure Documentation Microsoft Docs](https://docs.microsoft.com/en-us/azure/index)
* 2018/12/13 [Search iot architecture](https://azure.microsoft.com/en-us/search/?q=iot%20architecture)
