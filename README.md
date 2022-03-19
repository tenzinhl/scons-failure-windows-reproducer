# SCons Failure Reproduction Repository

What a mouthful haha. Anyways, just a simple repo to reproduce an error I'm encountering
where SCons won't build simple stuff by default unless the "USERPROFILE" variable is added
to the environment.

## Project Structure

Each folder represents a single contained example. Sample output included with each.
Output was produced by running `$ scons` in the folder.

`working-example` is a folder containing a working example

## My setup

- Windows 10
- Python 3.8.3
- SCons 4.3.0
- winlibs MinGW-w64 (UCRT)
