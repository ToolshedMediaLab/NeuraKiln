# Initial Installation & Setup Guide

## Requirements

- Windows 10/11 64-bit
- NVIDIA GPU
- Current NVIDIA graphics driver
- 7-Zip
- At least 30 GB of free disk space

## Initial Installation & Setup

### First...

- Download **ALL 4 PARTS** of `NeuraKiln-v2.0.0`.
- Download **ALL 3 PARTS** of the `NK Setup Bundle`.

### Then...

- On your Desktop, right-click and create a folder named `NK`, then create another folder named `Setup`.
- Place **ALL 4 PARTS** of `NeuraKiln-v2.0.0` into the `NK` folder.
- Place **ALL 3 PARTS** of the `NK Setup Bundle` into the `Setup` folder.
- Open the `Setup` folder.
- Right-click **PART ONE** of the NK Setup Bundle.
- Select "Show More Options"
- Navigate to 7Zip in the listed options
- Select **Extract Here**.
- You will now have a .zip named `NK Setup Bundle`.
- Right click `NK Setup Bundle.zip`
- Select "Extract Here"
- You will now have a folder named `NK Setup Bundle`. Leave it inside the `Setup` folder for now.
- Exit the `Setup` folder.
- Open the `NK` folder.
- Right-click **PART ONE** of `NeuraKiln-v2.0.0`.
- Select "Show More Options"
- Navigate to 7Zip in the listed options
- Select **Extract Here**.

### After extraction finishes...

- You will now have a ZIP file named `NeuraKiln-v2.0.0.zip`.
- Right-click `NeuraKiln-v2.0.0.zip`.
- Select **Extract Here**.
- You will now have a folder named `NeuraKiln-v2.0.0`. This is the portable NeuraKiln application.
- Move the `NeuraKiln-v2.0.0` folder to your Desktop or directly to `C:\`.
- Open the `NeuraKiln-v2.0.0` folder.
- Double-click `Launch_NK.bat`.
- Click **Run** if prompted by Windows.

### After NeuraKiln starts and reaches the Home screen...

- Click **Model Tools**.
- Click **NeuraKiln v2.0.0 Initial Setup**.
- Browse to your Desktop and open the `Setup` folder you created earlier.
- Select the `NK Setup Bundle` folder.
- Click **Open**.
- Allow the installer to finish completely.

## Initial Installation Complete

Congratulations! NeuraKiln v2.0.0 is now installed and ready for its included workflows.

> **IMPORTANT NOTE:** Due to third-party licensing requirements, **Mesh Lab** and **Diffusion Lab** require additional model setup beyond the initial NeuraKiln installation. NeuraKiln provides guided in-app installers for the standard Mesh Lab and Diffusion Lab components. **MiniMax H3 is handled separately and must be obtained independently through its provider's licensing process before using NeuraKiln's local H3 installer.**

---

# Mesh Lab

## Requirements

- Active internet connection
- At least 60 GB of free disk space
- Review and acceptance of the applicable third-party model licenses

Mesh Lab uses several third-party AI models, including **Hunyuan3D 2.1**, **Qwen Image 2.1**, and the **Mesh Lab Assistant model**. These models are **not included with or redistributed by NeuraKiln**.

Instead of downloading and arranging the model files manually, NeuraKiln provides a guided installer that downloads the required components directly from their respective providers, verifies them, and installs them into the correct Mesh Lab directories automatically.

> **IMPORTANT:** Third-party models remain subject to their own licenses and terms. NeuraKiln does not grant additional rights to those models or their outputs. NK Mesh Lab is intended for non-commercial and research use. Review the complete disclosure and provider license links presented by NeuraKiln before installation.

## Installation & Setup

### Step 1 — Open the Mesh Lab component installer

1. Launch NeuraKiln.
2. From the Home screen, open **Model Tools**.
3. Select **Install Mesh Lab Components**.

NeuraKiln will perform a pre-installation check for available disk space and the current state of any Mesh Lab components already present on your system.

### Step 2 — Review the third-party model disclosure

Before any third-party model files are downloaded, NeuraKiln will display the **Third-Party Models & License Disclosure**.

The installer will identify each required model, its provider, and the applicable license, including:

- **Hunyuan3D 2.1** — Tencent
- **Qwen Image 2.1** — Qwen / Alibaba
- **Mesh Lab Assistant model** — provider and license shown in the installer

Use the **View License** or **View Notice** links provided in the installer to review the complete upstream terms.

#### Hunyuan3D 2.1 geographic restriction

The standard Tencent Hunyuan 3D 2.1 Community License does not authorize use in the **European Union, United Kingdom, or South Korea**. The Mesh Lab installer will present this restriction before installation.

If your intended use is within an excluded territory, do not install or use Hunyuan3D 2.1 through NeuraKiln unless you have obtained separate authorization that permits that use.

#### Qwen Image 2.1 use restriction

Qwen Image 2.1 is provided under its own third-party license. The installer will present the current license information and require you to acknowledge the applicable terms before the model can be installed.

NeuraKiln does not determine whether a particular use is permitted under a third-party license. You are responsible for ensuring that your intended use complies with the provider's terms.

### Step 3 — Accept the applicable terms

Each required model has its own acknowledgment in the installer.

1. Review the disclosure for each model.
2. Review the linked upstream license or notice.
3. Check the required acknowledgment box for each model.
4. Check the final NeuraKiln third-party model acknowledgment.
5. Click **Accept & Install**.

**Accept & Install** remains unavailable until all required acknowledgments have been completed.

NeuraKiln stores a local record of the license information presented and the time of acceptance. This record remains on your computer and is used to determine whether a license acknowledgment must be shown again later.

### Step 4 — Allow NeuraKiln to download and install the components

After you select **Accept & Install**, NeuraKiln will automatically:

1. Download the required Mesh Lab components directly from their respective providers or authorized distribution sources.
2. Stage the downloaded files before placing them into the live Mesh Lab model directories.
3. Verify the downloaded files and required model structure.
4. Install each component into the correct NeuraKiln directory.
5. Validate the completed Mesh Lab installation.

The installation window displays the status of each component while the process runs.

Example:

```text
Installing Mesh Lab Components

✓ Hunyuan3D 2.1       Installed
→ Qwen Image 2.1      Downloading...
○ Mesh Lab Assistant  Waiting
```

Large model downloads may take some time depending on your internet connection. NeuraKiln supports recovery from interrupted installations and will preserve resumable download data where supported.

### Step 5 — Wait for Mesh Lab validation

After all downloads finish, NeuraKiln will validate the installed components.

A successful installation will report that the required Mesh Lab components are present and ready.

```text
Hunyuan3D 2.1       ✓
Qwen Image 2.1      ✓
Mesh Lab Assistant  ✓

Mesh Lab Ready
```

If a required component is missing or fails validation, NeuraKiln will identify the affected component and provide an option to retry or repair the installation.

## Existing or Partial Installations

If compatible Mesh Lab components are already present, NeuraKiln will detect and validate them rather than automatically downloading duplicate copies.

Depending on the state of the installation, Model Tools may display:

- **Install Mesh Lab Components** — required components are not installed.
- **Continue Installation** — some components are already present.
- **Manage Mesh Lab Components** — all required components are installed.
- **Repair Mesh Lab Components** — one or more installed components failed validation.

An existing third-party model may still require license acknowledgment if NeuraKiln does not already have a local acceptance record for the current license revision.

## Verify Mesh Lab

1. Return to the NeuraKiln Home screen.
2. Open **Mesh Lab**.
3. Confirm that Mesh Lab reports its required components as ready.
4. Select the NVIDIA GPU or GPU configuration you want to use.
5. Run a small test workflow before beginning a larger Mesh Lab project.

Mesh Lab setup is now complete.

---

# Diffusion Lab

## Requirements

- Active internet connection for the guided Diffusion Lab installation
- Review and acceptance of the applicable third-party model licenses
- Sufficient free disk space for the selected models, temporary files, and generated media

The standard NeuraKiln Diffusion Lab installation uses:

- **Qwen Image 2.1** for Text-to-Image
- **LTX 2.5** for Text-to-Video

These third-party model files are **not included with or redistributed by NeuraKiln**. NeuraKiln's guided installer downloads the required components directly from their respective providers or authorized distribution sources, verifies them, and places them into the correct Diffusion Lab directories automatically.

> **IMPORTANT:** MiniMax H3 is **not** downloaded by the Diffusion Lab installer. MiniMax H3 requires a separate third-party licensing and model-acquisition process. NeuraKiln provides only a local installer for users who have independently obtained compatible MiniMax H3 files.

## Standard Diffusion Lab Installation

### Step 1 — Open the Diffusion Lab component installer

1. Launch NeuraKiln.
2. From the Home screen, open **Model Tools**.
3. Select **Diffusion Lab Installation**.

The **Diffusion Lab Installation** button is located alongside **Mesh Lab Installation** in Model Tools.

NeuraKiln will perform a pre-installation check for available disk space and determine whether any required Diffusion Lab components are already present on your system.

### Step 2 — Review the third-party model disclosure

Before any third-party model files are downloaded, NeuraKiln will display its **Third-Party Models & License Disclosure**.

The installer will identify the standard Diffusion Lab models, their providers, and the applicable license information, including:

- **Qwen Image 2.1** — Text-to-Image
- **LTX 2.5** — Text-to-Video

Use the **View License** or other provider links presented by NeuraKiln to review the complete upstream terms before continuing.

NeuraKiln does not include, redistribute, sublicense, or grant additional rights to these third-party models. Your installation and use of each model remain subject to the applicable provider's terms.

### Step 3 — Accept the applicable terms

Each required model has its own acknowledgment in the installer.

1. Review the disclosure for each model.
2. Review the linked upstream license information.
3. Check the required acknowledgment box for **Qwen Image 2.1**.
4. Check the required acknowledgment box for **LTX 2.5**.
5. Check the final NeuraKiln third-party model acknowledgment.
6. Click **Accept & Install**.

**Accept & Install** remains unavailable until all required acknowledgments have been completed.

NeuraKiln stores a local record of the license information presented and the time of acceptance. This record remains on your computer and is used to determine whether a license acknowledgment must be shown again later.

### Step 4 — Allow NeuraKiln to download and install the components

After you select **Accept & Install**, NeuraKiln will automatically:

1. Download the required Qwen Image 2.1 components directly from the applicable third-party source.
2. Install and register Qwen Image 2.1 for **Diffusion Lab → Text-to-Image**.
3. Download the validated LTX 2.5 components directly from the applicable third-party source.
4. Install and register LTX 2.5 for **Diffusion Lab → Text-to-Video**.
5. Stage and verify downloaded files before placing them into the live model directories.
6. Validate the completed Diffusion Lab installation.

The installation window displays the status of each component while the process runs.

Example:

```text
Installing Diffusion Lab Components

✓ Qwen Image 2.1   Installed
→ LTX 2.5          Downloading...
```

Large model downloads may take some time depending on your internet connection. NeuraKiln supports recovery from interrupted installations and preserves resumable download data where supported.

### Shared Qwen Image 2.1 installation

Qwen Image 2.1 is shared between **Mesh Lab** and **Diffusion Lab**.

If Qwen Image 2.1 was already installed and validated through **Mesh Lab Installation**, the Diffusion Lab installer will reuse that installation instead of downloading another copy.

Likewise, if Qwen Image 2.1 is installed first through **Diffusion Lab Installation**, the Mesh Lab installer can detect and reuse the same compatible installation.

When an existing valid installation is found, the Diffusion Lab installer may display:

```text
Qwen Image 2.1   ✓ Already installed and verified
LTX 2.5          ○ Not installed
```

Only missing components will be downloaded.

If the current Qwen Image 2.1 license acknowledgment has already been accepted for the same license revision, NeuraKiln may reuse that local acceptance record rather than asking you to accept the identical terms again.

### Step 5 — Wait for Diffusion Lab validation

After all required downloads finish, NeuraKiln will validate the installed components.

A successful standard installation will report:

```text
Qwen Image 2.1   ✓
LTX 2.5          ✓

Diffusion Lab Ready
```

If a required component is missing or fails validation, NeuraKiln will identify the affected component and provide an option to retry or repair the installation.

## Existing or Partial Installations

If compatible Diffusion Lab components are already present, NeuraKiln will detect and validate them rather than automatically downloading duplicate copies.

Depending on the current state, Model Tools may display:

- **Diffusion Lab Installation** — required standard components are not installed.
- **Continue Diffusion Lab Installation** — some components are already present.
- **Manage Diffusion Lab Components** — all standard components are installed.
- **Repair Diffusion Lab Components** — one or more installed components failed validation.

An existing third-party model may still require license acknowledgment if NeuraKiln does not already have a local acceptance record for the current license revision.

## Other Text-to-Image Models

Qwen Image 2.1 is the standard Text-to-Image model installed by **Diffusion Lab Installation**, but Diffusion Lab is not limited to Qwen Image 2.1.

Advanced users may continue to import other compatible image models supported by `stable-diffusion.cpp` through the appropriate Model Tools import workflow.

Because component requirements vary by architecture, do not assume that a VAE, text encoder, or other companion component from one model family is interchangeable with another.

---

## MiniMax H3 — Local Installation Only

MiniMax H3 is intentionally excluded from NeuraKiln's automatic Diffusion Lab downloader.

MiniMax H3 requires a separate third-party licensing and model-acquisition process. **NeuraKiln does not provide, host, redistribute, or automatically download MiniMax H3 model files.**

If you want to use MiniMax H3, you must first obtain the required model files independently and ensure that your use complies with the applicable MiniMax licensing terms.

Once you have independently obtained compatible MiniMax H3 files, NeuraKiln's existing local installer can install them for Diffusion Lab.

### Prepare the MiniMax H3 source folder

The folder you select in NeuraKiln can have **any name**. What matters is the folder structure inside it.

Place the MiniMax H3 files into a folder containing the following subfolders directly inside it:

```text
Your folder\
├── diffusion_models\
│   └── MiniMax_H3_Ref2VA_pruned_int8_convrot.safetensors
├── text_encoder\
│   └── qwen3vl_32b_minimax_h3_int8_convrot.safetensors
└── vae\
    ├── minimax_h3_video_vae_fp16.safetensors
    └── minimax_h3_audio_vae_fp32.safetensors
```

> **IMPORTANT:** The folder is named `text_encoder` — singular — not `text_encoders`.

For the transformer, NeuraKiln supports either of the following compatible filenames:

```text
MiniMax_H3_Ref2VA_pruned_int8_convrot.safetensors
```

or:

```text
MiniMax_H3_Ref2VA_nvfp4_mixed.safetensors
```

At least one supported transformer must be present inside `diffusion_models`.

NeuraKiln does not provide download links for these files. Obtain them through the appropriate MiniMax licensing and distribution process before continuing.

### Install MiniMax H3 from the prepared folder

1. Launch NeuraKiln.
2. Open **Model Tools**.
3. Open the existing **MiniMax H3** local installer.
4. When prompted for the MiniMax H3 source, select the folder that directly contains:
   - `diffusion_models`
   - `text_encoder`
   - `vae`
5. **Do not select the parent folder above it.** Select the folder containing those three subfolders directly.
6. Allow NeuraKiln to validate the folder structure and required files.
7. NeuraKiln will install the MiniMax H3 components into its managed Diffusion Lab model directory.
8. Open **Diffusion Lab → Text-to-Video**, select **MiniMax H3**, choose your GPU configuration, and run a short test generation.

For a NeuraKiln installation located at `C:\NeuraKiln-v2.0.0`, the installed MiniMax H3 directory is:

```text
C:\NeuraKiln-v2.0.0\models\Diffusion_Lab\TextToVideo\MiniMaxH3
```

If NeuraKiln is installed somewhere else, the same relative model path is used under your NeuraKiln installation directory:

```text
models\Diffusion_Lab\TextToVideo\MiniMaxH3
```

MiniMax H3 local setup is now complete.

## Verify Diffusion Lab

1. Return to the NeuraKiln Home screen.
2. Open **Diffusion Lab**.
3. Confirm that the standard installed components report as ready.
4. Open **Text-to-Image** and confirm that Qwen Image 2.1 is available if you installed the standard Text-to-Image component.
5. Open **Text-to-Video** and confirm that LTX 2.5 is available.
6. If you independently installed MiniMax H3, confirm that it also appears as an available Text-to-Video option.
7. Select the NVIDIA GPU or GPU configuration you want to use and run a short test generation before attempting a larger workflow.

Diffusion Lab setup is now complete.

---

# Setup Complete

NeuraKiln v2.0.0 and the optional labs you selected are now ready to use.

If a guided installation reports a missing or invalid component, use the applicable **Repair** option in Model Tools. For locally installed MiniMax H3 or other manually imported models, verify that all required companion components were selected and validated before restarting NeuraKiln.
[NeuraKiln_Install_Guide_v5.md](https://github.com/user-attachments/files/34451616/NeuraKiln_Install_Guide_v5.md)

