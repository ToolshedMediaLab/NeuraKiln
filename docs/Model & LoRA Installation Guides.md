### Model & LoRA Installation Guides

NeuraKiln includes dedicated Model Tools for importing and organizing supported models and LoRAs. Follow the appropriate instructions below for the model type and backend you intend to use.

---

## Llama Lab

### llama.cpp Model Installation

#### Language Models

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Llama Lab**.
3. Select **llama.cpp GGUF Model** in the **Import Category** section.
4. Navigate to the **Source GGUF** box and select **Browse**.
5. Navigate to and select the GGUF model you intend to import.
6. Select **Import GGUF**.
7. Wait for the model import to complete.

**Done!** The model is now available to llama.cpp through NeuraKiln.

#### MTP Header

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Llama Lab**.
3. Select **llama.cpp MTP Header** in the **Import Category** section.
4. Navigate to the **Source GGUF** box and select **Browse**.
5. Navigate to and select the MTP Header model you intend to import.
6. Select **Import GGUF**.
7. Wait for the model import to complete.

**Done!**

#### MMPROJ Models

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Llama Lab**.
3. Select **llama.cpp MMPROJ** in the **Import Category** section.
4. In the **Source GGUF** section, select the language model the MMPROJ is intended for.
5. Select **Browse**.
6. Navigate to and select the MMPROJ model you intend to import.
7. Select **Import GGUF**.
8. Wait for the model import to complete.

**Done!**

> **Important:** MMPROJ files must be paired with a compatible base model. Import the base language model before importing its MMPROJ.

---

### Strata Model Installation

#### Language Models

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Llama Lab**.
3. Select **Strata GGUF Model** in the **Import Category** section.
4. Navigate to the **Source GGUF** box and select **Browse**.
5. Navigate to and select the GGUF model you intend to import.
6. Select **Import GGUF**.
7. Wait for the model import to complete.

**Done!** The model is now available to Strata through NeuraKiln.

#### MTP Header

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Llama Lab**.
3. Select **Strata MTP Header** in the **Import Category** section.
4. Navigate to the **Source GGUF** box and select **Browse**.
5. Navigate to and select the MTP Header model you intend to import.
6. Select **Import GGUF**.
7. Wait for the model import to complete.

**Done!**

#### MMPROJ Models

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Llama Lab**.
3. Select **Strata MMPROJ** in the **Import Category** section.
4. In the **Source GGUF** section, select the language model the MMPROJ is intended for.
5. Select **Browse**.
6. Navigate to and select the MMPROJ model you intend to import.
7. Select **Import GGUF**.
8. Wait for the model import to complete.

**Done!**

> **Important:** MMPROJ files must be compatible with the selected base model.

---

## Media Lab Model Installation

Media Lab supports compatible Python and ONNX restoration/upscaling models through the Model Importer.

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Media Lab**.
3. Select **Model Importer**.
4. Next to **Source ONNX Model**, select **Browse**.
5. Navigate to and select the model you intend to import.
6. Under **Media Lab Model Category**, configure the model's:
   - Source media type
   - Content type
   - Model scale
7. Verify that the selected categories accurately describe the model so NeuraKiln can organize and expose it correctly.
8. Select **Import Model**.
9. Wait for the model import to complete.

**Done!**

> **Important:** Selecting the correct media type, content type, and scale is necessary for NeuraKiln to categorize the imported model correctly.

---

## Diffusion Lab

### Text-to-Image Model Installation

NeuraKiln includes Qwen Image 2.1 as its supported base Text-to-Image configuration when installed through **Diffusion Lab Installation** or **Mesh Lab Installation**.

The **Text to Image Model Importer** is intended for importing additional `stable-diffusion.cpp`-compatible image models.

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Diffusion Lab**.
3. Select **Text to Image**.
4. In the **Model Bundle** section, select **Browse** next to **Diffusion GGUF**.
5. Navigate to and select the `stable-diffusion.cpp`-compatible diffusion GGUF you intend to import.
6. Select **Browse** next to **VAE** and select the VAE required by the model.
7. Add the text encoder or encoders required by the model.

Available encoder roles include:

- **LLM**
- **CLIP-L**
- **CLIP-G**
- **T5XXL**

Only provide the encoder roles required by the model you are importing. Refer to that model's `stable-diffusion.cpp` instructions to determine the correct components.

8. Review the automatically generated **Import Destination**.
9. Select **Import Model Bundle**.
10. Wait for NeuraKiln to copy, validate, and register the model bundle.
11. Confirm that the new model appears under **Installed Text to Image Models**.

**Done!**

> **Important:** Different diffusion architectures require different combinations of VAEs and text encoders. Do not assume components from one model family are compatible with another.

> The **LLM** field is used for models whose `stable-diffusion.cpp` configuration requires `--llm`. Other architectures may instead require CLIP-L, CLIP-G, T5XXL, or a combination of those encoders.

Imported Text-to-Image models are stored under:

```text
models\Diffusion_Lab\TextToImage\<model name>
```

---

### Text-to-Video LoRA Installation

Text-to-Video LoRAs are installed directly against a compatible Text-to-Video model.

1. Navigate to **Model Tools** from the NeuraKiln Home Menu.
2. Select **Diffusion Lab**.
3. Select **Text to Video LoRAs**.
4. Under **Target Model**, select **Select Model**.
5. Choose the installed Text-to-Video model the LoRA is intended for.
6. Confirm that the correct model appears next to **Selected model**.
7. Under **Source LoRA**, select **Browse**.
8. Navigate to and select the LoRA file you intend to import.
9. Review the automatically generated destination path.
10. Select **Import LoRA**.
11. Wait for the import to complete.
12. Select **Refresh List** if necessary and confirm that the LoRA appears under **Installed LoRAs**.

**Done!**

Imported Text-to-Video LoRAs are stored under:

```text
models\Diffusion_Lab\TextToVideo\<selected model>\loras
```

> **Important:** LoRAs are model-specific. Only install a LoRA to the model or model family it was created for. A LoRA intended for one Text-to-Video architecture may not function correctly with another.

#### Removing an Installed Text-to-Video LoRA

1. Navigate to **Model Tools → Diffusion Lab → Text to Video LoRAs**.
2. Select the appropriate **Target Model**.
3. Select the LoRA you want to remove from the **Installed LoRAs** list.
4. Select **Remove Selected LoRA**.
5. Refresh the list and verify that the LoRA has been removed.

---

## Default Mesh & Diffusion Lab Models

Users who only want NeuraKiln's supported default Mesh Lab and Diffusion Lab configurations do **not** need to manually import Qwen Image 2.1, Hunyuan3D 2.1, LTX 2.5, or the Mesh Lab Assistant model.

For Mesh Lab, use:

**Model Tools → Mesh Lab Installation**

For Diffusion Lab, use:

**Model Tools → Diffusion Lab Installation**

NeuraKiln will present the applicable third-party disclosures and then download, verify, install, and register the supported components automatically after acceptance.

### MiniMax H3

MiniMax H3 remains a separate local installation workflow and is **not downloaded or distributed by NeuraKiln**.

Users who have independently obtained compatible MiniMax H3 files can install them using NeuraKiln's local MiniMax H3 installer.

The source folder can have any name, but it must directly contain:

```text
Your Folder/
├── diffusion_models/
│   └── MiniMax_H3_Ref2VA_pruned_int8_convrot.safetensors
│      OR
│      MiniMax_H3_Ref2VA_nvfp4_mixed.safetensors
├── text_encoder/
│   └── qwen3vl_32b_minimax_h3_int8_convrot.safetensors
└── vae/
    ├── minimax_h3_video_vae_fp16.safetensors
    └── minimax_h3_audio_vae_fp32.safetensors
```

> **Important:** `text_encoder` is singular. Select the folder containing `diffusion_models`, `text_encoder`, and `vae`, not its parent folder.

NeuraKiln installs MiniMax H3 into:

```text
models\Diffusion_Lab\TextToVideo\MiniMaxH3
```
