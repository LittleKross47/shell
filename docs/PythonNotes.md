# Python notes

## CSCI - P436 | _Brandon Young_

### optparse __DEPRECIATED__

[optparse documentation](https://docs.python.org/3/library/optparse.html)

```Python
from optparse import OptionParser

parser = OptionParser()
parser.add_option("-f", "--file", dest="filename",
                  help="write report to FILE", metavar="FILE")
parser.add_option("-q", "--quiet",
                  action="store_false", dest="verbose", default=True,
                  help="don't print status messages to stdout")

(options, args) = parser.parse_args()
```

### argparse __CURRENT__

[argparse docs](https://docs.python.org/3/howto/argparse.html#id1)

```python3
import argparse
parser = argparse.ArgumentParser()
parser.parse_args()
```

### commented out code

```python
# def test():
#     args = sys.argv

#     Input processing
#     test = fileinput.input()
#     Flags
#     if args.__len__() == 1 and test:
#         sys.stdout.write("Help documentation...\n")
#     else:
#         Each case represents a flag at any specific element in the args array
#         for i in range(1,args.__len__()):
#             if args.__len__() == 1:
#                 printStdIn()
#             if args[i] == "-v" or args[i] == "-V" or args[i] == "--get-version":
#                 sys.stdout.write("Version 1.0.0\n")
#             if args[i] == "-h" or args[i] == "-H" or args[i] == "-?" or args[i] == "--Help" or args[i] == "--get-help":
#                sys.stdout.write("Help documentation...")
#             if args[i] == "-f" or args[i] == "-F" or args[i] == "--input-file" or args[i] == "--Input-File":
#                 inputfile = open(args[i + 1])
#                 break
#             else:
#                 inputfile = open(args[i])
```

### P_05 Notes

[How to print help when no params are passed](https://stackoverflow.com/questions/4042452/display-help-message-with-python-argparse-when-script-is-called-without-any-argu)  
[How to detect if a file exists](https://stackoverflow.com/questions/82831/how-do-i-check-whether-a-file-exists-without-exceptions)

#### Lists

[List info](https://www.w3schools.com/python/python_lists.asp)  
[2D lists](https://www.geeksforgeeks.org/python-using-2d-arrays-lists-the-right-way/)