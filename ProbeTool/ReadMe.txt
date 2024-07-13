This code stub is provided for three reasons:
1:  This is M6 remap code for QtDragon which is production-usable, 
    because changes the customization code founds on LinuxCNC at the 
    time this repository was uploaded (7/12/2024):
    a) it performs all the steps necessary for manual tool change 
    using a tool-setter probe to determine the final tool offset for
    those using rigs that don't have repeatable tool-holders.
    b) it restores use of G38.2 in place of G38.3 which was changed
    by Pull Request 2562.
2:  This is the core of pull Request # 2706 at 
    https://github.com/LinuxCNC/linuxcnc/pull/2706 which was not
    yet merged as of uploading this repository, so I am providing it
    here in case anyone finds and wants to use this code before it 
    is merged, or in case it is never merged. 
3:  In case this code is changed later on the offical LinuxCNC 
    github, it may be that someone may want this version.

To install this, do the following:

A.  Use the instructions for installing QtDragon that are current 
    for your version. 
B.  Take note of the location of the M6 remap code in your installation.
    On my installation, this was:
    ~linuxcnc/configs/ConfigName01/nc_subroutines
C.  Replace the qt_auto_tool_probe.ngc at that location with this 
    version.
D.  Follow the workflow instructions within the code for setting up your 
    starting parameters: Block Height (aka tool setter height), & 
    Workpiece height.

Enjoy and be safe. 

All the best,

Vector Hasting
