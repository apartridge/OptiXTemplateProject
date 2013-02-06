OptiXTemplateProject
====================

An OptiX template project for Visual Studio 2010. Based on the SDK example PathTracer by NVIDIA, but it should
be clean and stripped from CMake files and SDK references. It does contain some parts of the SDK Sample 
Framework which were necessary
for it to run. This works as an isolated project and working example of OptiX which may be more suited to
develop from than the SDK...

Contains DLL's necessary for it to run (tested on X64 Win7). Copy them into the x64/Debug folder (which is both output directory, 
intermediate directory and working directory). The .cu files are compiled into PTX by NVCC and placed in that folder,
where it is read by the runtime for loading of OptiX programs. If you have trouble, double check the include/library directories
in project configuration to suit your system.
