Toolshed V1 Rev1.1

Toolshed V1 is a local Windows media restoration workflow built for NVIDIA RTX GPUs.

Rev1.1 is the complete public Toolshed V1 release and includes the full V1 feature set in a self-contained portable package.

Toolshed runs locally on your system and includes its required Python, CUDA, TensorRT RTX, and FFmpeg runtime components.

Requirements
Windows 10/11
NVIDIA RTX GPU
32 GB system RAM
Enough free disk space for the Toolshed package, temporary restoration files, and output media
7-Zip required to extract the multi-part download

A separate Python installation is not required.

Download

Toolshed V1 Rev1.1 is distributed as a multi-part 7-Zip archive because the full portable package is larger than GitHub's single-file release asset limit.

Download every part from the latest GitHub Release:

Toolshed V1 Rev1.1.7z.001
Toolshed V1 Rev1.1.7z.002
Toolshed V1 Rev1.1.7z.003
Toolshed V1 Rev1.1.7z.004
Toolshed V1 Rev1.1.7z.005
Toolshed V1 Rev1.1.7z.006
Toolshed V1 Rev1.1.7z.007

Keep all seven files together in the same folder.

After all parts are downloaded, extract only:

Toolshed V1 Rev1.1.7z.001

7-Zip will automatically read the remaining archive parts.

Do not extract each numbered file separately.

How to Run
Download all seven release archive parts.
Right-click Toolshed V1 Rev1.1.7z.001.
Extract it with 7-Zip.
Open the extracted toolshedV1 folder.
Run Launch Toolshed.bat.

Do not run Toolshed from inside the 7-Zip archive.

Toolshed uses the Python runtime included inside the application folder and does not require a system Python installation.

Included in Toolshed V1 Rev1.1

Toolshed V1 Rev1.1 includes the complete V1 workflow, including:

Toolshed Restore
Restore Batch Mode
SmartFrames / scan tools
Compare
PostEdit
Recompile
Pipeline+ workflows
Session / managed workflow functionality
Model Tools
Additional V1 workflow features previously reserved for Premium / Enterprise builds

There is no separate Free / Premium / Enterprise feature split in Rev1.1.

Rev1.1 Improvements

Rev1.1 includes fixes and packaging improvements made since the original public release, including:

Fixed TensorRT RTX tile handling when the selected tile size is larger than the source frame
Fixed the resulting TensorRT RTX input shape mismatch that could cause inference to fall back to CPU
Added a bundled Python 3.12 runtime
Removed the requirement for users to install Python separately
Updated the launcher to use Toolshed's bundled Python runtime directly
Cleaned up NVIDIA GPU detection dependencies
Bundled CUDA, TensorRT RTX, FFmpeg, FFprobe, and Python runtime components
General dependency and release packaging cleanup

Rev1.1 has been smoke-tested using the bundled portable runtime.

Issue Reports

When reporting an issue, please include:

GPU model
Windows version
Selected execution provider
Model used
Source media type and resolution
Console output or error message
Steps needed to reproduce the issue
Project Status

Toolshed V1 Rev1.1 is the final planned revision of Toolshed V1 in its current form.
