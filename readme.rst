Scorpion Vision 10.2.1.579 Release Notes
========================================
This is a release version of Scorpion Vision Version X - 10.2.

- 10.2.1.579: 

    - New Sony ZCL 2.12 RC1 Camera Driver
    - Installer download - does both 32 bit and 64 bit files
    - **New TF3** - production quality but still work in progress :)

            - optional template tracelines
            - centerpoints as CrossHair symbol
            - added thread statistics

- 10.2.1.578: Maintenance Release

    - Licensing Update - tool count now counts all tools

        - Lite - 150 tools
        - Basic - 500 tools
    
    - Fixed BaseTool/Toolbox protections - “Required minimum license”

        - Scorpion Maintenance licence did not work properly

    - **New TF3** - production quality but still work in progress :)

        - Updated helpfile to many new functions
        - Prefilter documented - handles empty filterstring
        - Templates
            - template toolbar replaces left/right control panels
            - fixed active template filter dialog for linked filter
            - added “delete all templates”

        - Training    
            - added add all templates
            - added auto template name 
            - fixed training zoom, roi and partial roi
            - added ‘NoSearch’ visualization circles for unprocessed ROI’s
        - Larger masking tools 

    - DataInput
        - Lists defaults to “Immediate”
        - Extended python interface
            - access to parameters
            - easy access to controls
            - Indicatorpanel
            - StatePanel
        - Updated demo: STP-2012-0040-DataInput 1.0.0.14
        - Improved/extended some GUI operations
        - added DataInput properties dialog - replaces multiple single operations

    - IndicatorPanel
        - Properties dialog replaces multiple single operations
    - Saves global application settings on “Save”
        - previously save on normal application close
    - Image logging
        - shows free disk until limit and total sizes
        - low disk as Info1 in system log - reported first time only
    - ColorSegmentor
        - ignores empty postfilter
    - Curves
        - fixed 2GB limitation of VirtualMemory

- 10.2.1.575: Maintenance Release

    - Important - Image Logger file deletion bug fix
    - LaserProfiler3D --> Beta
    - PolygonMatch1,2 and 3 
        - new Translation only mode - important
    - Watchout - New TF3- Constraints Enable 
        - must be toggled to get correct operation
    - **TF3 - getting better all the time :) in progress**
        - fixed dynamic rotation and scale links4
        - always valid MaxScore - added threshold result
        - new MultiMatch - important new feature
        - removed bug - solutions outside ROI
        - improved GUI for score setup 
        - be aware of minor compatibility issues
    - Important Arrlib fix for 568
    - **Dialogs is sized to screen size - great feature**
    - **Improved toolbox navigation** 
        - close all dialogs
        - parent dialogs are automatically closed

- 10.2.1.568: Major update

    - Scorpion Arrlib is 10-20 % faster - a general and important improvement
        - choosing the right interpolation mode can provide an additional 5-15 %
    - Interpolation mode is managed from the toolbox
        - NN - Nearest neighbor is chosen for speed
        - Bilinear is the default
        - Cubic provides an accurate option for special cases
        - Smart Wide does a smart job on wide tracelines
    - Important - TemplateFinder3 is a complete new tool - 
        - prefilter for improved matching
        - multiroi for multiple inspection from one tf3
        - better explanation of resampling modes
                - important when working in 3D 
        - better default values
        - regex for dynamic templates
        - saving templates to files for faster context switching
        - very important - max polygon match pr polygon 
            - ---> can define no match polygons/edges to better segment detection
            - can be vital addition to tf3 for demanding applications 
        - bug fixes and improvements
    - Dense Stereo Vision is supported using
        - STC-0084 StereoRectify3D 1.0.0.2
        - STC-0083 DisparityMap3D 0.9.1.9
    - STP-0072-DisparityMap 1.0.0.2
    - ColorSegmentor is now a much better tool 
        - with postfilter, named filters and dynamic filteractivation
        - check STP-0075-ColorSegmentor
    - Latest OpenCV 2.4.8 is supported - update Numpy 1.8.0 and SciPy 0.13.2 versions
    - A huge update to Scorpion Tool Components - download all to the Scorpion template   directory and get the fine and useful extensions
    - Updated GUI and Icons
    - ImageLogger can set disk limit to 1 GByte down from 5 GByte
    - Updated - 64bit ZCL driver Sony XCG cameras
    - Soon to be available a SVM - Support Vector Machine classification STC
        - state of the art machine learning in a clever STC package

    - Updated Demo profiles
        - **SDP-0087 Advanced Training - 3D Pizza Measurement - version 1.0.0.7**
            - real-time 3d point cloud generation with new LaserProfiler3D
        - SDP-2012-0019-3DPipePicking
            - Demonstration of 3D Pipe Picking from a bin using Scorpion 3D Stinger Stereo Vision
        - STP-0073-Scorpion-Toolbox-Performance 1.0.0.3
            - valuable test program to benchmark scorpion computers
        - SDP-2012-0019-3DPipePicking 1.0.0.21
            - Demonstration of 3D Pipe Picking using Scorpion 3D Stinger Stereo Vision
        - SDP-2012-0018-3DPipeBinPicking
            - Demonstration of 3D Pipe Picking from a bin using Scorpion 3D Stinger Stereo Vision
        - SDP-2012-0041-Locate-3D-Empty 1.0.0.14
            - Practical solution to detect empty box using two multiline lasers
        - STP-0072-DisparityMap 1.0.0.2
            - Empty box using beta DisparityMap3D STC - super dense stereo vision example

    - STC-Updates
        - STC-0001-MinimumPolygonToPolygonDistance_2.1.0.22
        - STC-0011-ImageFilter_3.3.0.33
        - STC-0022-LocateEdgePoint3D_1.2.0.39
        - STC-0025-PolygonExtrema_1.0.0.10
        - STC-0034-PolygonFilter2D_1.1.0.40
        - STC-0036-SortLocate3D_1.1.0.21
        - STC-0038-FitLine3D_1.2.0.22
        - STC-0043-PointInPolygon2D_1.0.0.4
        - STC-0055-FindPaths2D_1.0.0.20
        - STC-0064-LocatePaths3D_1.0.0.24
        - New
            - STC-0008-Visualize3D_1.2.0.12
            - STC-0078-GridMapper_0.9.0.8
            - STC-0084 StereoRectify3D_1.0.0.1
            - STC-0082 MultiExpoMerger_0.9.0.2
            - STC-0066-PolygonMaskImage_1.0.0.5
        
- 10.2.1.567
    - Arrlib Beta has a faster traceline setting - this is experimental 
        - provides 10-20% general speedup
        - less accuracy - must be verified

- 10.2.1.566
    - SingleLineFinder - removed 3D pointcloud options
        - use LaserProfiler3D

- 10.2.1.564
    - Image Logging - JPG compression
    - IO - fixed persistence of active
    - ColorMatcher - works like a color intensity meter
        - added decimation
        - added result options
        - dynamic roi linking
    - PolygonMatch2 accepts template parameter linking
    - ExternalData - Duplicate data items
    - PolygonMatch3
        - accepts template parameter linking
        - added browse positions
        - added geometric model support
        - updated child reference options
            - mean / area center of gravity
            - all polygon center of gravity
            - offset and rotation
            - explicit point and rotation
        - New tool - Advanced 3D
            - LaserProfiler3D in beta
        - CircleFinder2D - enhance multisearch
        - Mainform - fix "Operator Camera Recovery" persistence
        - Tool threading support - ImageMixer, ImageConverter and Locate3D

- 10.2.1.562
    - Blob4 - new bounding box modes
        - MinArea and align Bounding Rect
    - Template Parameter linking
        - supported by  dynamic parameters and polygon editor
    - **New template parameter linking** in tools
        - P%1i.Value_x
            - %ni - n is n’th integer number in current tool name
            - n = [1..> - index from start
            - <..-1] - index from end
    - Toolbox menu - added Duplicate
    - Fixes
        - logging statistics
        - error deleting un-monitored io signals
        - prevent create duplicate events
        - CircleGauger exception outside image
        - LineFromPoints handle zero length line
    - CircleFinder2D
        - added multi-search
        - ready for serious action
    - Locate3D
        - improve dictionary parsing
        - added StrictPointMapping
        - Fixed single point stereointersection from 8.3.0.470
            - only using multiple points 

- 10.2.1.559
    - Major speed improvement on camera aquisition to allow up to 350 frame / second
        - added ‘Smart image routing’
        - optimized continous mode
        - automatic routing of images from same camera
            - no need for Grab;image=no commands
        - buffers all incoming images in high speed
        - new statistics in camera setup dialog
        - added camera autostop in continous mode
        - used with continous=n, where n>1 for autostop
            - n > 1 then n is the number is images to capture before autostop
        - Central Camera.AutoStop - called when images=n
    - Major FastMode GUI Improvement
        - Statistics
        - Actions/Commands
        - Historylist
    - SingleLineFinder
        - ScanCount - no of scans in current pointcloud
        - LineCount - no of ‘good’ scans in current pointcloud
        - fixed memoryleak
        - fixed missing ‘empty’ lines in pointcloud if PointCount=0
        - minor speed optimization

- 10.2.0.558    
    - Updated GUI and added weigths TF3
    - Major Fix in PolygonMatch3
    - PM2 UPDATE

- 10.2.0.556
    - ObjectPosition3D support templates, result reference and threading
    - PlaneFit3D - major performance improvment with proper constraints and better ransac
    - DataInput - missing refrash in 10.2.0.555

The main features updates of 10.2 are:

- New - History Mode in Curves
    - can graphs values persistent over days and weeks
    - very valuable to verify the performance and stability of a vision system
- Important - Variant change works in real-time
    - significant performance improvement on ExternalDictionary context shift
- New update Sony ZCL driver for XCG GigE cameras
    - We advice to run the driver in Original Mode
    - The driver support running multiple apps on a single computer
    - We suspect the driver to be an important update from Sony :)
- Numerous fixes and improvements
- TemplateFinder3 added Size and Angle constraints
    - improves the robustness
    - significant improvements when reading text and numbers
- Scorpion Help File
    - new images
    - first draft for STC documentation
- Update Getting Started Tutorials for Version X.I
    - runs on Windows-8
    - Part 1 to Part 5 is updated
- Updated Tutorial for Windows-8
    - Object Location with TemplateFinder3 and PolygonMatch
    - Advanced Training - Creating a 3D Image with the Scorpion 3D Scanner
        - added demo video
- Status diodes in statusbars for IO systems
- Updated to latest OpenCV 2.4.6
- Utilities additions
    - TeamViewer Host Setup
    - Passmark system performance test
- IO-System
    - SetValue / GetValue works for tags under Actions
- ImageLogging
    - fixed missing logging error missing due to AfterInspect
        - This can be important and affect other part of a system
- SingleLineFinder has added point cloud generation
- Grab command supports binary 3D image Filename=<name>.arr

Camera Drivers

- support for Basler Pylon 3.2 and 4.0 - updated pylon 2.3
    - uses format settings instead of camera type to determine mono or color images
    - no need for initial grab after setting continous<>0
- added beta kinect driver
- added latest SickIVP drivers

**Critical Patches  to run older versions the same computer:**
    - The patch files should be copied to system32 on 32 bit computer or syswow64 on 64 bit computers
        - https://dl.dropboxusercontent.com/u/9419179/Eventlog3X%20-%20patch%20549.zip
    - If you have a startup error Abstract Error download the patch and read the instructions
        - applies only to upgraded computers
        - The batch should be copied to system32 or syswow64 directories
        - https://dl.dropbox.com/u/9419179/Scorpion%20Vision%20Version%20X%20patch%20SmpSch_2.zip

Support e-mail: support@tordivel.no

April 29, 2014

Note 1: Install all extensions to run all demos

Note 2: Click Setup and use password 911 to inspect configuration of all demonstrations


    
        
    
    
     

    
    

        






