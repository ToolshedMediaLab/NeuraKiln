<h1 align="center">NeuraKiln v2.0.0 - Formerly Toolshed<br><sub>Dream. Think. Create.</sub></h1> <p align="center">Free, locally powered AI creation. Four labs. One application.</p>

---

https://github.com/user-attachments/assets/3c2dca6f-0f29-4bed-b397-895d878511a6

<details open>
  <summary><strong>Mesh Creation</strong></summary>
  
  <img width="880" height="496" alt="creation-zone-preview" src="https://github.com/user-attachments/assets/b01d78b1-829b-480b-8b4e-fe8b890384fc" />
 


  <p align="center">One prompt. Local LLM. Concept Art → 3D Generation → Blender Refinement → Export.</p>

  <p align="center"><sub>Demo Hardware: 2× RTX 3060 12GB, 1× RTX 5060 Ti 16GB</sub></p>
</details>

<details>
  <summary><strong>Media Restoration</strong></summary>

  <p align="center"><strong>Coming Soon</strong></p>
  <p align="center">Creation Zone — Media Restoration workflow demonstration.</p>
</details>

<details>
  <summary><strong>Image/Video Diffusion</strong></summary>

  <p align="center"><strong>Coming Soon</strong></p>
  <p align="center">Creation Zone — Diffusion workflow demonstration.</p>
</details>

<details>
  <summary><strong>Agentic Coding</strong></summary>

  <p align="center"><strong>Coming Soon</strong></p>
  <p align="center">Agent Space — Agentic Coding Demonstration.</p>
</details>

---

<h2 align="center">What is NeuraKiln?</h2>

<table>
  <tr>
    <td width="66%" valign="middle">
      <p><strong>NeuraKiln (formerly Toolshed)</strong> is a free-to-use, local-first AI workstation for Windows, built around NVIDIA GPU acceleration.</p>
      <p>It brings language models, AI-assisted media restoration, image and video generation, and 3D creation together in one application—without forcing you to manage a collection of disconnected tools.</p>
      <p><strong>Four specialized labs. One connected workspace.</strong></p>
    </td>
    <td width="34%" align="center" valign="middle">
      <img width="1344" height="1170" alt="neurakiln-logo" src="https://github.com/user-attachments/assets/c97db9cd-661c-47c8-94bc-62be4c00df68" />
    </td>
  </tr>
</table>

---

<h2 align="center">Explore the four labs</h2>


<table>
  <tr>
    <th align="left" width="50%">Llama Lab</th>
    <th align="left" width="50%">Diffusion Lab</th>
  </tr>
  <tr>
    <td valign="top">
      <strong>Local LLMs · Agents · Tools</strong>
      <br>
      <strong>Backend(s):</strong> llama.cpp · Strata
      <p>
        Run compatible language models on your own
        hardware. Chat, use integrated tools, and let
        agents coordinate multi-step tasks across
        supported workflows.
      </p>
    </td>
    <td valign="top">
      <strong>Image Generation · Video Generation</strong>
      <br>
      <strong>Backend(s):</strong> NKDiffusion · stablediffusion.cpp 
      <p>
        Create original images and video locally with
        compatible generative models and GPU-accelerated
        pipelines.
      </p>
    </td>
  </tr>
  <tr>
    <th align="left">Media Lab</th>
    <th align="left">Mesh Lab</th>
  </tr>
  <tr>
    <td valign="top">
      <strong>Restoration · Upscaling · Enhancement</strong>
      <br>
      <strong>Backend:</strong> NKMedia powered by ONNX
      <p>
        Restore and enhance existing videos and images
        with GPU-accelerated processing and configurable
        restoration workflows.
      </p>
    </td>
    <td valign="top">
      <strong>3D Generation · Texturing · Refinement</strong>
      <br>
      <strong>Backend(s):</strong> NKDiffusion · llama.cpp · stablediffusion.cpp  
      <p>
        Generate 3D assets, work with rigging and export
        tools, and use Blender-integrated workflows
        for further refinement.
      </p>
    </td>
  </tr>
</table>



---

<h2 align="center">Tools & Harnesses</h2>

<h3 align="center">Your Models. Your Hardware. Real Tools.</h3>

NeuraKiln extends local AI beyond traditional chat by providing agents with access to system utilities, browser automation, external integrations, and specialized creative workflows.

From navigating websites and executing code to generating 3D assets and restoring media, NeuraKiln connects language models to the tools they need to accomplish complex tasks.

---

### Agent Tools

<details>
<summary><strong>Browser — Web Navigation & Automation</strong></summary>

<br>

**Backend:** Playwright

NeuraKiln provides a dedicated browser automation environment for local AI agents. Browser sessions are isolated by runtime owner, allowing multiple agents to operate without sharing a single browser session.

| Tool | Description |
| --- | --- |
| **Navigate** | Open websites and navigate to URLs. |
| **Reload** | Refresh the current page. |
| **Page Snapshot** | Inspect page structure, text, and interactive elements. |
| **Click** | Interact with buttons, links, and other page elements. |
| **Type** | Enter text into forms and input fields. |
| **Keyboard Input** | Send keyboard commands and shortcuts. |
| **JavaScript Evaluation** | Execute JavaScript within the browser's page context. |
| **Browser Console** | Inspect console output for debugging and validation. |
| **Screenshot** | Capture visual representations of webpages. |
| **Close Browser** | Close the agent-owned browser session. |

**Supported workflows:** Web research, documentation browsing, form interaction, frontend testing, and browser-assisted development.

**Authentication:** Some services restrict automated sign-in. Authenticated browsing may require additional profile setup, which will be covered in the installation documentation.

</details>

<details>
<summary><strong>OpenTerminal — System & File Operations</strong></summary>

<br>

**Backend:** OpenTerminal

OpenTerminal provides agents with command execution, filesystem access, and process management capabilities through an isolated, managed tool service.

| Tool | Description |
| --- | --- |
| **Run Command** | Execute terminal commands, scripts, and development utilities. |
| **List Processes** | View running system processes. |
| **Get Process Status** | Inspect the state of a process. |
| **Send Process Input** | Send input to an active process. |
| **Kill Process** | Terminate a selected process. |
| **List Files** | Browse files and directories. |
| **Read File** | Read file contents for inspection or analysis. |
| **Write File** | Create or write files. |
| **Replace File Content** | Apply targeted changes to existing files. |
| **Grep Search** | Search file contents for matching text or patterns. |
| **Glob Search** | Discover files using filename patterns. |

**Supported workflows:** Software development, debugging, automation, scripting, filesystem management, and project maintenance.

Individual OpenTerminal tools can be enabled or disabled through the model's tool configuration.

</details>

<details>
<summary><strong>MCP Integrations — External Tools & Services</strong></summary>

<br>

**Integration:** Model Context Protocol (MCP)

NeuraKiln supports connecting local language models to external services through MCP-compatible tool providers.

| Integration | Description |
| --- | --- |
| **GitHub MCP** | Work with repositories, source code, issues, pull requests, and supported GitHub operations. |
| **Hugging Face MCP** | Access supported model hub and repository-related capabilities. |
| **Exa MCP** | Perform web searches and retrieve external information. |

Available tools depend on the connected MCP provider, configuration, and account permissions.

</details>

<details>
<summary><strong>Skill Tree — Structured Agent Procedures</strong></summary>

<br>

Skill Tree provides structured procedural guidance for models executing complex tasks.

Rather than requiring the model to repeatedly invent its own workflow, Skill Tree can route tasks through predefined instructions and specialized procedures.

| Capability | Description |
| --- | --- |
| **Task Routing** | Identify the appropriate procedural workflow for a task. |
| **Coding Procedures** | Guide development, inspection, modification, and validation workflows. |
| **Research Procedures** | Structure information gathering, investigation, and synthesis. |
| **Progressive Loading** | Load relevant instructions without placing every skill into the model's context. |
| **Workflow Transitions** | Move between procedures as a task progresses. |

Skill Tree is designed to complement execution tools such as OpenTerminal, Browser, and MCP rather than duplicate their functionality.

</details>

<details>
<summary><strong>Agent Space — Multi-Agent Coordination</strong></summary>

<br>

Agent Space provides a collaborative environment for multiple independently configured language-model participants.

Each participant maintains its own execution context while coordinating through shared workspace information.

| Capability | Description |
| --- | --- |
| **Independent Agents** | Run separately configured model participants. |
| **Shared Board** | Exchange plans, updates, and coordination information. |
| **Task Coordination** | Organize work and distribute responsibilities. |
| **Task Ownership** | Track assigned responsibilities across participants. |
| **Reviews & Handoffs** | Coordinate reviews, results, and transfers of work. |
| **Shared Workspace State** | Maintain information used for collaboration between agents. |
| **Tool Access** | Allow participants to use supported engineering and creation tools. |

Agent Space is designed for collaborative workflows involving multiple real model participants, rather than a single model simulating an entire team.

</details>

### Creative Tools & Lab Workflows

NeuraKiln integrates specialized tools for generating, restoring, enhancing, and manipulating creative assets.

<details>
<summary><strong>Media Lab — Restoration & Enhancement</strong></summary>

<br>

**Backend:** NKMedia Custom Backend / ONNX Runtime

| Tool / Workflow | Description |
| --- | --- |
| **Restore** | Restore or upscale individual media files using compatible AI models. |
| **Batch Restore** | Process multiple media files in a batch workflow. |
| **Pipeline+ Restore** | Apply configured restoration processing pipelines. |
| **Pipeline+ AFK Restore** | Run extended restoration workflows with reduced manual intervention. |
| **Smart Scan** | Analyze video material to assist restoration workflows. |
| **Photo Smart Scan** | Analyze images for supported photo-processing workflows. |
| **Compare** | Inspect and compare original and processed media. |
| **Postedit** | Perform additional processing on restoration results. |
| **Recompile** | Reassemble processed media into a final output. |

</details>

<details>
<summary><strong>Diffusion Lab — Image & Video Generation</strong></summary>

<br>

**Backends:** stable-diffusion.cpp / NKDiffusion Custom Backend

| Tool / Workflow | Description |
| --- | --- |
| **Text-to-Image** | Generate images from natural-language descriptions using supported models. |
| **Text-to-Video** | Generate video sequences from text prompts using compatible video-generation models. |
| **Model Configuration** | Configure supported generation models and execution settings. |
| **LoRA Support** | Apply compatible LoRA adapters where supported by the generation backend. |

</details>

<details>
<summary><strong>Mesh Lab — 3D Asset Creation</strong></summary>

<br>

**Integrations:** Hunyuan3D / Blender / NeuraKiln Creation Workflows

| Tool / Workflow | Description |
| --- | --- |
| **IdeaGen** | Generate visual concepts for downstream creative workflows. |
| **3DGen** | Generate 3D geometry from supported image or text-driven workflows. |
| **Texturing** | Produce textured assets using compatible 3D generation models. |
| **AutoRig** | Apply supported automated rigging operations to generated assets. |
| **Blender Integration** | Refine, inspect, and manipulate assets through Blender-assisted workflows. |
| **Asset Export** | Prepare and export generated assets for use in external applications. |

</details>

### Harnesses

**Tools perform operations. Harnesses organize those operations into workflows.**

NeuraKiln's harness system provides structured environments for local models to coordinate tools and complete multi-stage tasks.

<details>
<summary><strong>Creation Harnesses — Creative Workflows</strong></summary>

<br>

| Harness | Description |
| --- | --- |
| **Llama Lab Creator** | Coordinates supported tools and creative operations in model-driven workflows. |
| **Mesh Lab Assistant** | Assists with concept development, asset generation, and 3D creation workflows. |
| **IdeaGen** | Guides concept and image generation for supported creative tasks. |

Harness availability and supported operations depend on the configured model, installed components, and active tool integrations.

</details>

<details>
<summary><strong>Coding Harness — Software Engineering</strong></summary>

<br>

The Coding Harness equips local language models with development tools and structured workflows for software engineering, debugging, testing, and automation.

| Capability | Description |
| --- | --- |
| **Code Inspection** | Examine source files, dependencies, and project structures. |
| **Code Creation & Editing** | Create, modify, and refactor source code. |
| **Terminal Execution** | Execute scripts, development commands, and build utilities through OpenTerminal. |
| **Debugging** | Investigate failures, inspect logs, and apply targeted corrections. |
| **Testing & Validation** | Execute available tests, inspect results, and verify changes. |
| **Browser Testing** | Navigate, interact with, and inspect web applications using Playwright. |
| **Repository Integration** | Access supported GitHub operations through MCP. |
| **Skill Tree Integration** | Follow structured coding procedures for inspection, implementation, debugging, and verification. |
| **Multi-Agent Collaboration** | Coordinate development tasks between independent model participants through Agent Space. |

**Designed for:** Software development, debugging, code maintenance, automation, and multi-stage engineering workflows.

</details>

### One Environment. Connected Capabilities.

A local language model can combine supported capabilities into larger workflows rather than treating every tool as a separate application.

For example, a creation workflow may involve:

**User Request → Concept Generation → 3D Generation → Blender Refinement → Asset Export**

NeuraKiln's Creation Zone demonstration shows this type of multi-stage workflow being executed by a locally running model.

> **Tool availability:** Some integrations require additional model downloads, dependencies, accounts, or configuration. Agent access to individual creative workflows may vary by release version. Models must support the relevant tool-calling capabilities, and tool execution remains subject to the configured permissions and runtime environment.

---


<h2 align="center">Built Around Your Hardware</h2>

---

<p align="center"><strong>NeuraKiln isn't here to replace your creative tools. It's here to bring them together.</strong></p>

| Local-first | NVIDIA accelerated | Connected workflows |
| :--- | :--- | :--- |
| Run supported models and processing tasks on your own PC. | Take advantage of CUDA, TensorRT, and multiple NVIDIA GPUs where supported. | Use Model Tools to manage compatible models and let supported agents work across labs. |

---

<p align="center">
  <strong>NeuraKiln is free, and I intend to keep it that way.</strong>
</p>

<p align="center">
  <a href="https://buymeacoffee.com/toolshedmedialabs">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me a Coffee" width="200">
  </a>
</p>

<p align="center">
  If NeuraKiln has saved you a headache, improved your workflow, or helped bring your creative ideas to life, please consider buying me a coffee!
</p>

<p align="center">
  Every donation helps support continued development, improvements, and the growth of NeuraKiln.
</p>

---

<h2 align="center">System Requirements</h2>

<p>
  NeuraKiln is designed for NVIDIA RTX-powered systems.
  Hardware requirements vary depending on the selected
  lab, AI model, and workload.
</p>

<h3>System Memory (RAM)</h3>

<table>
  <tr>
    <th align="center" width="50%">Minimum</th>
    <th align="center" width="50%">Recommended</th>
  </tr>
  <tr>
    <td align="center"><strong>32 GB RAM</strong></td>
    <td align="center"><strong>64 GB RAM</strong></td>
  </tr>
</table>

<h3>GPU Requirements</h3>

<table>
  <tr>
    <th align="left">Lab / Workload</th>
    <th align="center">Minimum VRAM</th>
    <th align="center">Recommended VRAM</th>
  </tr>
  <tr>
    <td><strong>Llama Lab</strong></td>
    <td align="center">8 GB</td>
    <td align="center">16 GB</td>
  </tr>
  <tr>
    <td><strong>Media Lab</strong></td>
    <td align="center">12 GB</td>
    <td align="center">16 GB</td>
  </tr>
  <tr>
    <td><strong>Mesh Lab</strong></td>
    <td align="center">16 GB</td>
    <td align="center">16 GB</td>
  </tr>
  <tr>
    <td><strong>Diffusion Lab</strong><br>
    <sub>Text-to-Image</sub></td>
    <td align="center">12 GB</td>
    <td align="center">16 GB</td>
  </tr>
  <tr>
    <td><strong>Diffusion Lab</strong><br>
    <sub>Text-to-Video</sub></td>
    <td align="center">32 GB</td>
    <td align="center">32 GB</td>
  </tr>
</table>

<p>
  <strong>Multi-GPU Compatible Workloads:</strong>
  Llama Lab, Diffusion Lab Text-to-Image, and
  Diffusion Lab Text-to-Video.
</p>

<p>
  <strong>Important:</strong> All listed GPU requirements
  refer to NVIDIA RTX hardware. Actual VRAM consumption
  depends on model size, precision, resolution, and
  workload configuration. Multi-GPU support depends
  on the selected backend and does not necessarily
  combine GPU memory into one shared pool.
</p>

---

<h2 align="center">Installation, Setup & Guides</h2>




<h2 align="center">Join the NeuraKiln Community</h2>

<p align="center">
  Connect with the NeuraKiln community through the
  official Discord server!
</p>

<p align="center">
  Follow development progress, discuss features,
  share your creations, ask questions, and stay
  informed about upcoming releases.
</p>

<p align="center">
  <a href="https://discord.gg/KxXHZMmdZ7">
    <img
      src="https://img.shields.io/badge/Discord-Join%20the%20Community-5865F2?style=for-the-badge&logo=discord&logoColor=white"
      alt="Join the Official NeuraKiln Discord"
    />
  </a>
</p>

<p align="center">
  <strong>Bug Reporting</strong>
</p>

<p align="center">
  Found a bug or encountered an issue?
  Join the Discord and submit your report in
  <strong>#bug-report</strong>.
</p>

<p align="center">
  For reporting guidelines, see
  <a href="CONTRIBUTING.md">Contributing & Bug Reporting</a>.
</p>

<p align="center">
  <sub>Official NeuraKiln Discord Server</sub>
</p>

---

<h2 align="center">Credits & Acknowledgments</h2>

<p align="center">
  <strong>NeuraKiln is independently developed by ToolshedMediaLabs.</strong>
</p>

<p align="center">
  NeuraKiln brings together original software, custom
  backends, and integrations with established AI
  technologies. The following projects and their
  contributors deserve recognition for their work.
</p>

<h3>Core Technologies & Backends</h3>

<table>
  <tr>
    <th align="left" width="50%">
      <a href="https://github.com/ggml-org/llama.cpp">llama.cpp</a>
    </th>
    <th align="left" width="50%">
      <a href="https://github.com/Niko1221/Strata">Strata</a>
    </th>
  </tr>
  <tr>
    <td>Local language model inference and GGUF support. Developed by the llama.cpp contributors.</td>
    <td>Alternative local LLM inference engine. Developed by Niko1221 and contributors.</td>
  </tr>

  <tr>
    <th align="left">
      <a href="https://github.com/leejet/stable-diffusion.cpp">stable-diffusion.cpp</a>
    </th>
    <th align="left">
      <a href="https://github.com/microsoft/onnxruntime">ONNX Runtime</a>
    </th>
  </tr>
  <tr>
    <td>Local generative model inference using C/C++ implementations.</td>
    <td>Cross-platform machine learning inference framework used in Media Lab processing.</td>
  </tr>

  <tr>
    <th align="left">
      <a href="https://www.blender.org/">Blender</a>
    </th>
    <th align="left">
      <a href="https://ffmpeg.org/">FFmpeg</a>
    </th>
  </tr>
  <tr>
    <td>Professional 3D creation and refinement tools. Developed by the Blender community.</td>
    <td>Multimedia processing, encoding, decoding, and video handling.</td>
  </tr>

  <tr>
    <th align="left">
      <a href="https://developer.nvidia.com/cuda-toolkit">NVIDIA CUDA</a> /
      <a href="https://developer.nvidia.com/tensorrt">TensorRT</a>
    </th>
    <th align="left">
      <a href="https://huggingface.co/">Hugging Face</a>
    </th>
  </tr>
  <tr>
    <td>GPU computing and optimized AI inference technologies powering supported NVIDIA workloads.</td>
    <td>AI model ecosystem and model discovery services.</td>
  </tr>
</table>

<h3>AI Models & Research</h3>

<table>
  <tr>
    <th align="left">Project</th>
    <th align="left">Developer</th>
  </tr>
  <tr>
    <td><a href="https://github.com/QwenLM">Qwen Models</a></td>
    <td>Qwen Team / Alibaba</td>
  </tr>
  <tr>
    <td><a href="https://github.com/tencent-hunyuan/hunyuan3d-2.1">Hunyuan3D</a></td>
    <td>Tencent Hunyuan</td>
  </tr>
  <tr>
    <td><a href="https://github.com/Lightricks/LTX-Video">LTX-Video</a></td>
    <td>Lightricks</td>
  </tr>
</table>

<p>
  NeuraKiln supports an expanding ecosystem of
  independently developed AI models. Credit for these
  models belongs to their respective creators,
  researchers, and contributors.
</p>

<h3>Original NeuraKiln Development</h3>

<p>
  The NeuraKiln application, its original user interface,
  integrated workflows, model management systems,
  agent tooling, and proprietary NKMedia and NKDiffusion
  backend components are developed by
  <strong>ToolshedMediaLabs</strong>.
</p>

<h3>Licensing & Third-Party Rights</h3>

<p>
  All third-party projects, libraries, frameworks,
  and AI models retain their respective copyrights,
  licenses, and terms of use.
</p>

<p>
  Recognition in this section does not imply
  affiliation, sponsorship, or endorsement by
  the credited projects or organizations.
</p>

<p>
  NeuraKiln's proprietary licensing applies only
  to components owned by its copyright holder
  and does not supersede third-party licenses.
</p>

---

<p align="center">
  <strong>Special thanks to the developers, researchers,
  and open-source communities advancing local AI.</strong>
</p>

<p align="center">
  <sub>NeuraKiln — Dream. Think. Create.</sub>
</p>

---

<h2 align="center">Support NeuraKiln Development</h2>

<p align="center">
  <strong>NeuraKiln is free, and I intend to keep it that way.</strong>
</p>

<p align="center">
  <a href="https://buymeacoffee.com/toolshedmedialabs">
    <img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me a Coffee" width="200">
  </a>
</p>

<p align="center">
  If NeuraKiln has saved you a headache, improved your workflow, or helped bring your creative ideas to life, please consider buying me a coffee!
</p>

<p align="center">
  Every donation helps support continued development, improvements, and the growth of NeuraKiln.
</p>

<p align="center">
  <em>Your support is entirely optional, but always appreciated.</em>
</p>

---

