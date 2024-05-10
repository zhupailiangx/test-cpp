# test-cpp



<!DOCTYPE html>

<html lang="en">
  <head>
    <meta charset="utf-8" />
    <meta name="viewport" content="width=device-width, initial-scale=1.0" /><meta content="Use the benchmark results for Intel® Distribution of OpenVINO™ toolkit, that may help you decide what hardware to use or how to plan the workload." name="description" />

    <title>Performance Benchmarks &#8212; OpenVINO™  documentation</title>

    
    
  <link href="../_static/css/theme.css" rel="stylesheet">
  <link href="../_static/css/index.ff1ffe594081f20da1ef19478df9384b.css" rel="stylesheet">

    
  <link rel="stylesheet"
    href="../_static/vendor/fontawesome/5.13.0/css/all.min.css">
  <link rel="preload" as="font" type="font/woff2" crossorigin
    href="../_static/vendor/fontawesome/5.13.0/webfonts/fa-solid-900.woff2">
  <link rel="preload" as="font" type="font/woff2" crossorigin
    href="../_static/vendor/fontawesome/5.13.0/webfonts/fa-brands-400.woff2">

    
      

    
    <link rel="stylesheet" type="text/css" href="../_static/pygments.css" />
    <link rel="stylesheet" type="text/css" href="../_static/css/blank.css" />
    <link rel="stylesheet" type="text/css" href="../_static/tabs.css" />
    <link rel="stylesheet" type="text/css" href="../_static/copybutton.css" />
    <link rel="stylesheet" type="text/css" href="../_static/panels-main.c949a650a448cc0ae9fd3441c0e17fb0.css" />
    <link rel="stylesheet" type="text/css" href="../_static/panels-variables.06eb56fa6e07937060861dad626602ad.css" />
    <link rel="stylesheet" type="text/css" href="../_static/design-style.4045f2051d55cab465a707391d5b2007.min.css" />
    
  <link rel="preload" as="script" href="../_static/js/index.be7d3bbb2ef33a8344ce.js">

    <link href="../_static/css/media/favicon.ico" rel="shortcut icon">
    <link rel="stylesheet" href="../_static/css/openvino_sphinx_theme.css" type="text/css" />
    <link rel="stylesheet" href="../_static/css/button.css" type="text/css" />
    <link rel="stylesheet" href="../_static/css/input.css" type="text/css" />
    <link rel="stylesheet" href="../_static/css/textfield.css" type="text/css" />
    <link rel="stylesheet" href="../_static/css/tabs.css" type="text/css" />
    <script src="../_static/js/openvino_sphinx_theme.js"></script>
    <script src="../_static/js/sortable_tables.js"></script>

<link href="https://cdn.jsdelivr.net/npm/@splidejs/splide@4.1.4/dist/css/splide.min.css" rel="stylesheet">
<script src="https://cdn.jsdelivr.net/npm/@splidejs/splide@4.1.4/dist/js/splide.min.js"></script>

<script type="module" src="https://static.cloud.coveo.com/atomic/v2/atomic.esm.js"></script> 
<link rel="stylesheet" href="https://static.cloud.coveo.com/atomic/v2/themes/coveo.css">

<link rel="stylesheet" href="../_static/css/viewer.min.css" type="text/css" />
<link rel="stylesheet" href="../_static/css/custom.css" type="text/css" />
<link rel="stylesheet" href="../_static/css/banner.css" type="text/css" />
<link rel="stylesheet" href="../_static/css/coveo_custom.css" type="text/css" />

<script src="https://cdn.jsdelivr.net/npm/chart.js@4.4.1/dist/chart.umd.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-datalabels"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/chartjs-plugin-annotation/0.5.7/chartjs-plugin-annotation.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-barchart-background@1.3.0/build/Plugin.Barchart.Background.min.js"></script>
<script src="https://cdn.jsdelivr.net/npm/chartjs-plugin-deferred@1"></script>
<script src="https://cdnjs.cloudflare.com/ajax/libs/PapaParse/5.3.1/papaparse.min.js"></script>
<script src="../_static/js/viewer.min.js"></script>
<script src="/assets/versions_raw.js"></script>

    <script data-url_root="../" id="documentation_options" src="../_static/documentation_options.js"></script>
    <script src="../_static/jquery.js"></script>
    <script src="../_static/underscore.js"></script>
    <script src="../_static/doctools.js"></script>
    <script src="../_static/tabs.js"></script>
    <script src="../_static/clipboard.min.js"></script>
    <script src="../_static/copybutton.js"></script>
    <script src="../_static/js/custom.js"></script>
    <script src="../_static/js/graphs.js"></script>
    <script src="../_static/js/newsletter.js"></script>
    <script src="../_static/js/open_sidebar.js"></script>
    <script src="../_static/design-tabs.js"></script>
    <link rel="shortcut icon" href="../_static/favicon.ico"/>
    <link rel="index" title="Index" href="../genindex.html" />
    <link rel="search" title="Search" href="../search.html" />
    <link rel="next" title="Performance Information F.A.Q." href="performance-benchmarks/performance-benchmarks-faq.html" />
    <link rel="prev" title="About OpenVINO" href="../about-openvino.html" />
    <meta name="viewport" content="width=device-width, initial-scale=1" />
    <meta name="docsearch:language" content="en">
    

    <!-- Google Analytics -->
    
  </head>
  <body data-spy="scroll" data-target="#bd-toc-nav" data-offset="80">
    

      <nav class="navbar navbar-light navbar-expand-lg bg-light fixed-top bd-navbar" id="navbar-main"><div class="container-xl">

  <div id="navbar-start">
    
    

<a class="navbar-brand" href="../index.html">
  <img src="../_static/logo.svg" class="logo" alt="logo">
</a>


    
  </div>

  <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbar-collapsible" aria-controls="navbar-collapsible" aria-expanded="false" aria-label="Toggle navigation">
    <span class="navbar-toggler-icon"></span>
  </button>

  
  <div id="navbar-collapsible" class="col-lg-9 collapse navbar-collapse">
    <div id="navbar-center" class="mr-auto">
      
      <div class="navbar-center-item">
        <ul id="navbar-main-elements" class="navbar-nav">
    <li class="toctree-l1 current active nav-item">
 <a class="reference internal nav-link" href="../home.html">
  OpenVINO 2024.1
 </a>
</li>

<li class="toctree-l1 nav-item">
 <a class="reference external nav-link" href="https://docs.openvino.ai/install">
  Install
 </a>
</li>

<li class="toctree-l1 nav-item">
 <a class="reference external nav-link" href="https://blog.openvino.ai/">
  Blog
 </a>
</li>

<li class="toctree-l1 nav-item">
 <a class="reference external nav-link" href="https://community.intel.com/t5/Intel-Distribution-of-OpenVINO/bd-p/distribution-openvino-toolkit">
  Forum
 </a>
</li>

<li class="toctree-l1 nav-item">
 <a class="reference external nav-link" href="https://www.intel.com/content/www/us/en/support/products/96066/software/development-software/openvino-toolkit.html">
  Support
 </a>
</li>

<li class="toctree-l1 nav-item">
 <a class="reference external nav-link" href="https://github.com/openvinotoolkit">
  GitHub
 </a>
</li>

    
</ul>
      </div>
      
    </div>

    <div id="navbar-end">
      
      <div class="navbar-end-item">
        <ul id="navbar-icon-links" class="navbar-nav" aria-label="Icon Links">
        <li class="nav-item">
          <a class="nav-link" href="https://github.com/openvinotoolkit/openvino" rel="noopener" target="_blank" title="GitHub">
            <span><i class="sst-github"></i></span>
            <label class="sr-only">GitHub</label>
          </a>
        </li>
</ul>
      </div>
      
      <div class="navbar-end-item">
        
<div class="dropdown sst-dropdown sst-dropdown-navbar">
  <button class="btn sst-btn dropdown-toggle" type="button" id="version-selector" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false"></button>
  <div class="dropdown-menu" aria-labelledby="version-selector">
  </div>
</div>
      </div>
      
      <div class="navbar-end-item">
        

<div class="dropdown sst-dropdown sst-dropdown-navbar">
  <button class="btn sst-btn dropdown-toggle" type="button" id="language-selector" data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">English</button>
  <div class="dropdown-menu" aria-labelledby="language-selector">
    
      
        <a class="dropdown-item font-weight-bold" href="/latest/index.html">English</a>
      
    
      
        <a  class="dropdown-item" href="/cn/latest/index.html">Chinese</a>
      
    
  </div>
</div>

      </div>
      
    </div>
  </div>
</div>
        <div id="collapse-nav-wrapper" class="container-xl">
          <button id="collapse-nav" class="button bttn-prm button-size-m" type="button" data-toggle="collapse" data-target="#nav-tree" aria-expanded="false" aria-controls="nav-tree">
            Documentation navigation <i class="fas fa-chevron-down"></i>
          </button>
        </div>
      </nav>
    
<div id="info-banner" class="transition-banner"></div>
<script src="../_static/js/hide_banner.js"></script>


    <div class="container-xl">
      <div class="row">
          
            
            <!-- Only show if we have sidebars configured, else just a small margin  -->
            <div class="col-12 col-md-3 bd-sidebar" id="nav-tree"><div>
<atomic-search-interface id="sa-search">
  <atomic-search-box redirection-url="search.html">
  </atomic-search-box>
</atomic-search-interface>
</div><nav class="bd-links" id="bd-docs-nav" aria-label="Main navigation">
    <div class="bd-toc-item active">
      
      
      <ul class="current nav bd-sidenav">
<li class="toctree-l1 has-children"><a class="reference internal" href="../get-started.html">GET STARTED</a><input class="toctree-checkbox" id="toctree-checkbox-1" name="toctree-checkbox-1" type="checkbox"/><label for="toctree-checkbox-1"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l2 has-children"><a class="reference internal" href="../get-started/install-openvino.html">Install OpenVINO</a><input class="toctree-checkbox" id="toctree-checkbox-2" name="toctree-checkbox-2" type="checkbox"/><label for="toctree-checkbox-2"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3 has-children"><a class="reference internal" href="../get-started/install-openvino/install-openvino-linux.html">OpenVINO Runtime on Linux</a><input class="toctree-checkbox" id="toctree-checkbox-3" name="toctree-checkbox-3" type="checkbox"/><label for="toctree-checkbox-3"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-archive-linux.html">Use Archive</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-pip.html">Use PyPI</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-apt.html">Use APT</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-yum.html">Use YUM</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-zypper.html">Use ZYPPER</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-conda.html">Use Conda Forge</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-vcpkg.html">Use vcpkg</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-brew.html">Use Homebrew</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-conan.html">Use Conan</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-docker-linux.html">Use Docker</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-npm.html">Use npm</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../get-started/install-openvino/install-openvino-windows.html">OpenVINO Runtime on Windows</a><input class="toctree-checkbox" id="toctree-checkbox-4" name="toctree-checkbox-4" type="checkbox"/><label for="toctree-checkbox-4"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-archive-windows.html">Use Archive</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-pip.html">Use PyPI</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-conda.html">Use Conda Forge</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-vcpkg.html">Use vcpkg</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-docker-linux.html">Use Docker</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-conan.html">Use Conan</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-npm.html">Use npm</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../get-started/install-openvino/install-openvino-macos.html">OpenVINO Runtime on macOS</a><input class="toctree-checkbox" id="toctree-checkbox-5" name="toctree-checkbox-5" type="checkbox"/><label for="toctree-checkbox-5"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-archive-macos.html">Use Archive</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-brew.html">Use Homebrew</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-pip.html">Use PyPI</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-conda.html">Use Conda Forge</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-vcpkg.html">Use vcpkg</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-conan.html">Use Conan</a></li>
<li class="toctree-l4"><a class="reference internal" href="../get-started/install-openvino/install-openvino-npm.html">Use npm</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../get-started/configurations.html">Additional Hardware Setup</a><input class="toctree-checkbox" id="toctree-checkbox-6" name="toctree-checkbox-6" type="checkbox"/><label for="toctree-checkbox-6"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../get-started/configurations/configurations-intel-gpu.html">For GPU</a></li>
<li class="toctree-l3"><a class="reference internal" href="../get-started/configurations/configurations-intel-npu.html">For NPU</a></li>
</ul>
</li>
<li class="toctree-l2"><a class="reference internal" href="../get-started/troubleshooting-install-config.html">Troubleshooting</a></li>
</ul>
</li>

<li class="toctree-l1 has-children"><a class="reference internal" href="../learn-openvino.html">LEARN OPENVINO</a><input class="toctree-checkbox" id="toctree-checkbox-7" name="toctree-checkbox-7" type="checkbox"/><label for="toctree-checkbox-7"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l2 has-children"><a class="reference internal" href="../learn-openvino/interactive-tutorials-python.html">Interactive Tutorials (Python)</a><input class="toctree-checkbox" id="toctree-checkbox-8" name="toctree-checkbox-8" type="checkbox"/><label for="toctree-checkbox-8"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/interactive-tutorials-python/notebooks-installation.html">Installation of OpenVINO™ Notebooks</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/3D-pose-estimation-with-output.html">Live 3D Human Pose Estimation with OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/3D-segmentation-point-clouds-with-output.html">Part Segmentation of 3D Point Clouds with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/action-recognition-webcam-with-output.html">Human Action Recognition with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/amused-lightweight-text-to-image-with-output.html">Lightweight image generation with aMUSEd and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/animate-anyone-with-output.html">Image-to-Video synthesis with AnimateAnyone and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/async-api-with-output.html">Asynchronous Inference with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/auto-device-with-output.html">Automatic Device Selection with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/bark-text-to-audio-with-output.html">Text-to-speech generation using Bark and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/blip-diffusion-subject-generation-with-output.html">Subject-driven image generation and editing using BLIP Diffusion and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/blip-visual-language-processing-with-output.html">Visual Question Answering and Image Captioning using BLIP and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/clip-language-saliency-map-with-output.html">Language-Visual Saliency with CLIP and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/clip-zero-shot-classification-with-output.html">Zero-shot Image Classification with OpenAI CLIP and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/code-language-id-with-output.html">Programming Language Classification with OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/controlnet-stable-diffusion-with-output.html">Text-to-Image Generation with ControlNet Conditioning</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/convert-to-openvino-with-output.html">OpenVINO™ Model conversion</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/convnext-classification-with-output.html">Classification with ConvNeXt and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/cross-lingual-books-alignment-with-output.html">Cross-lingual Books Alignment with Transformers and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/ct-scan-live-inference-with-output.html">Live Inference and Benchmark CT-scan Data with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/ct-segmentation-quantize-nncf-with-output.html">Quantize a Segmentation Model and Show Live Inference</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/decidiffusion-image-generation-with-output.html">Image generation with DeciDiffusion and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/deep-floyd-if-convert-with-output.html">Image generation with DeepFloyd IF and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/deep-floyd-if-optimize-with-output.html">Post-Training Quantization and Weights Compression of DeepFloyd IF model with NNCF</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/depth-anything-with-output.html">Depth estimation with DepthAnything and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/depth-estimation-videpth-with-output.html">Monocular Visual-Inertial Depth Estimation using OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/detectron2-to-openvino-with-output.html">Convert Detectron2 Models to OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/distil-whisper-asr-with-output.html">Automatic speech recognition using Distil-Whisper and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/distilbert-sequence-classification-with-output.html">Sentiment Analysis with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/dolly-2-instruction-following-with-output.html">Instruction following using Databricks Dolly 2.0 and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/efficient-sam-with-output.html">Object segmentations with EfficientSAM and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/encodec-audio-compression-with-output.html">Audio compression with EnCodec and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/fast-segment-anything-with-output.html">Object segmentations with FastSAM and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/fastcomposer-image-generation-with-output.html">FastComposer: Tuning-Free Multi-Subject Image Generation with Localized Attention</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/film-slowmo-with-output.html">Frame interpolation using FILM and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/gpu-device-with-output.html">Working with GPUs in OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/grammar-correction-with-output.html">Grammatical Error Correction with OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/grounded-segment-anything-with-output.html">Object detection and masking from prompts with GroundedSAM (GroundingDINO + SAM) and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/handwritten-ocr-with-output.html">Handwritten Chinese and Japanese OCR with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/hello-detection-with-output.html">Hello Object Detection</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/hello-segmentation-with-output.html">Hello Image Segmentation</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/hello-world-with-output.html">Hello Image Classification</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/hugging-face-hub-with-output.html">Hugging Face Model Hub with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/image-bind-with-output.html">Binding multimodal data using ImageBind and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/image-classification-quantization-with-output.html">Quantization of Image Classification Models</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/image-inpainting-with-output.html">Image In-painting with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/instant-id-with-output.html">InstantID: Zero-shot Identity-Preserving Generation using OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/instruct-pix2pix-image-editing-with-output.html">Image Editing with InstructPix2Pix and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/knowledge-graphs-conve-with-output.html">OpenVINO optimizations for Knowledge graphs</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/kosmos2-multimodal-large-language-model-with-output.html">Kosmos-2: Multimodal Large Language Model and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/language-quantize-bert-with-output.html">Quantize NLP models with Post-Training Quantization ​in NNCF</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/latency-tricks-with-output.html">Performance tricks in OpenVINO for latency mode</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/latent-consistency-models-image-generation-with-output.html">Image generation with Latent Consistency Model and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/latent-consistency-models-optimum-demo-with-output.html">Latent Consistency Model using Optimum-Intel OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/lcm-lora-controlnet-with-output.html">Text-to-Image Generation with LCM LoRA and ControlNet Conditioning</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/legacy-mo-convert-to-openvino-with-output.html">OpenVINO™ model conversion API</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/llava-multimodal-chatbot-with-output.html">Visual-language assistant with LLaVA and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/llava-next-multimodal-chatbot-with-output.html">Visual-language assistant with LLaVA Next and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/llm-agent-langchain-with-output.html">Create LLM Agent using OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/llm-chatbot-with-output.html">Create an LLM-powered Chatbot using OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/llm-question-answering-with-output.html">LLM Instruction-following pipeline with OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/llm-rag-langchain-with-output.html">Create a RAG system using OpenVINO and LangChain</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/lraspp-segmentation-with-output.html">Semantic segmentation with LRASPP MobileNet v3 and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/machine-translation-with-output.html">Machine translation demo</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/magika-content-type-recognition-with-output.html">Magika: AI powered fast and efficient file type identification using OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/meter-reader-with-output.html">Industrial Meter Reader</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/mms-massively-multilingual-speech-with-output.html">MMS: Scaling Speech Technology to 1000+ languages with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/mobileclip-video-search-with-output.html">Visual Content Search using MobileCLIP and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/mobilevlm-language-assistant-with-output.html">Mobile language assistant with MobileVLM and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/model-server-with-output.html">Hello Model Server</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/model-tools-with-output.html">Working with Open Model Zoo Models</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/music-generation-with-output.html">Controllable Music Generation with MusicGen and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/named-entity-recognition-with-output.html">Named entity recognition with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/object-detection-with-output.html">Live Object Detection with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/oneformer-segmentation-with-output.html">Universal Segmentation with OneFormer and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/openvino-api-with-output.html">OpenVINO™ Runtime API Tutorial</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/openvino-tokenizers-with-output.html">OpenVINO Tokenizers: Incorporate Text Processing Into OpenVINO Pipelines</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/openvoice-with-output.html">Voice tone cloning with OpenVoice and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/optical-character-recognition-with-output.html">Optical Character Recognition (OCR) with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/optimize-preprocessing-with-output.html">Optimize Preprocessing</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/paddle-ocr-webcam-with-output.html">PaddleOCR with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/paddle-to-openvino-classification-with-output.html">Convert a PaddlePaddle Model to OpenVINO™ IR</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/paint-by-example-with-output.html">Paint By Example: Exemplar-based Image Editing with Diffusion Models</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/person-tracking-with-output.html">Person Tracking with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/pix2struct-docvqa-with-output.html">Document Visual Question Answering Using Pix2Struct and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/pose-estimation-with-output.html">Live Human Pose Estimation with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/pyannote-speaker-diarization-with-output.html">Speaker diarization</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/pytorch-onnx-to-openvino-with-output.html">Convert a PyTorch Model to ONNX and OpenVINO™ IR</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/pytorch-post-training-quantization-nncf-with-output.html">Post-Training Quantization of PyTorch models with NNCF</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/pytorch-quantization-aware-training-with-output.html">Quantization Aware Training with NNCF, using PyTorch framework</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/pytorch-to-openvino-with-output.html">Convert a PyTorch Model to OpenVINO™ IR</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/qrcode-monster-with-output.html">Generate creative QR codes with ControlNet QR Code Monster and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/question-answering-with-output.html">Interactive question answering with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/riffusion-text-to-music-with-output.html">Text-to-Music generation using Riffusion and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/rmbg-background-removal-with-output.html">Background removal with RMBG v1.4 and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/sdxl-turbo-with-output.html">Single step image generation using SDXL-turbo and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/segment-anything-with-output.html">Object masks from prompts with SAM and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/segmenter-semantic-segmentation-with-output.html">Semantic Segmentation with OpenVINO™ using Segmenter</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/segmind-vegart-with-output.html">High-resolution image generation with Segmind-VegaRT and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/siglip-zero-shot-image-classification-with-output.html">Zero-shot Image Classification with SigLIP</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/slowfast-video-recognition-with-output.html">Video Recognition using SlowFast and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/softvc-voice-conversion-with-output.html">SoftVC VITS Singing Voice Conversion and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/sound-generation-audioldm2-with-output.html">Sound Generation with AudioLDM2 and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/sparsity-optimization-with-output.html">Accelerate Inference of Sparse Transformer Models with OpenVINO™ and 4th Gen Intel® Xeon® Scalable Processors</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/speculative-sampling-with-output.html">Text Generation via Speculative Sampling, KV Caching, and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/speech-recognition-quantization-data2vec-with-output.html">Quantize Data2Vec Speech Recognition Model using NNCF PTQ API</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/speech-recognition-quantization-wav2vec2-with-output.html">Quantize Wav2Vec Speech Recognition Model using NNCF PTQ API</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/speech-to-text-with-output.html">Speech to Text with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/ssd-b1-with-output.html">Image generation with Segmind Stable Diffusion 1B (SSD-1B) model and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-diffusion-ip-adapter-with-output.html">Image Generation with Stable Diffusion and IP-Adapter</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-diffusion-text-to-image-with-output.html">Text-to-Image Generation with Stable Diffusion and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-diffusion-torchdynamo-backend-with-output.html">Stable Diffusion v2.1 using OpenVINO TorchDynamo backend</a></li>

<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-diffusion-v2-infinite-zoom-with-output.html">Infinite Zoom Stable Diffusion v2 and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-diffusion-v2-optimum-demo-with-output.html">Stable Diffusion v2.1 using Optimum-Intel OpenVINO and multiple Intel Hardware</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-diffusion-v2-text-to-image-demo-with-output.html">Stable Diffusion Text-to-Image Demo</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-diffusion-v2-text-to-image-with-output.html">Text-to-Image Generation with Stable Diffusion v2 and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-diffusion-xl-with-output.html">Image generation with Stable Diffusion XL and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/stable-zephyr-3b-chatbot-with-output.html">LLM-powered chatbot using Stable-Zephyr-3b and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/style-transfer-with-output.html">Style Transfer with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/table-question-answering-with-output.html">Table Question Answering using TAPAS and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tensorflow-bit-image-classification-nncf-quantization-with-output.html">Big Transfer Image Classification Model Quantization pipeline with NNCF</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tensorflow-classification-to-openvino-with-output.html">Convert a TensorFlow Model to OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tensorflow-hub-with-output.html">Convert of TensorFlow Hub models to OpenVINO Intermediate Representation (IR)</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tensorflow-instance-segmentation-to-openvino-with-output.html">Convert a TensorFlow Instance Segmentation Model to OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tensorflow-object-detection-to-openvino-with-output.html">Convert a TensorFlow Object Detection Model to OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tensorflow-quantization-aware-training-with-output.html">Quantization Aware Training with NNCF, using TensorFlow Framework</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tensorflow-training-openvino-nncf-with-output.html">Post-Training Quantization with TensorFlow Classification Model</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tensorflow-training-openvino-with-output.html">From Training to Deployment with TensorFlow and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/text-prediction-with-output.html">Text Prediction with OpenVINO™</a></li>

<li class="toctree-l3"><a class="reference internal" href="../notebooks/tflite-selfie-segmentation-with-output.html">Selfie Segmentation using TFLite and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tflite-to-openvino-with-output.html">Convert a Tensorflow Lite Model to OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/throughput-tricks-with-output.html">Performance tricks in OpenVINO for throughput mode</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/tiny-sd-image-generation-with-output.html">Image Generation with Tiny-SD and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/triposr-3d-reconstruction-with-output.html">TripoSR feedforward 3D reconstruction from a single image and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/typo-detector-with-output.html">Typo Detector with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/vehicle-detection-and-recognition-with-output.html">Vehicle Detection And Recognition with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/videollava-multimodal-chatbot-with-output.html">Visual-language assistant with Video-LLaVA and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/vision-background-removal-with-output.html">Image Background Removal with U^2-Net and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/vision-image-colorization-with-output.html">Image Colorization with OpenVINO</a></li>

<li class="toctree-l3"><a class="reference internal" href="../notebooks/vision-monodepth-with-output.html">Monodepth Estimation with OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/vision-paddlegan-anime-with-output.html">Photos to Anime with PaddleGAN and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/vision-paddlegan-superresolution-with-output.html">Super Resolution with PaddleGAN and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/vision-superresolution-image-with-output.html">Single Image Super Resolution with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/vision-superresolution-video-with-output.html">Video Super Resolution with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/whisper-convert-with-output.html">Video Subtitle Generation using Whisper and OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/whisper-nncf-quantize-with-output.html">Post-Training Quantization of OpenAI Whisper model with NNCF</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/wuerstchen-image-generation-with-output.html">Image generation with Würstchen and OpenVINO</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/yolov7-optimization-with-output.html">Convert and Optimize YOLOv7 with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/yolov8-instance-segmentation-with-output.html">Convert and Optimize YOLOv8 instance segmentation model with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/yolov8-keypoint-detection-with-output.html">Convert and Optimize YOLOv8 keypoint detection model with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/yolov8-obb-with-output.html">YOLOv8 Oriented Bounding Boxes Object Detection with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/yolov8-object-detection-with-output.html">Convert and Optimize YOLOv8 real-time object detection with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/yolov8-quantization-with-accuracy-control-with-output.html">Convert and Optimize YOLOv8 with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/yolov9-optimization-with-output.html">Convert and Optimize YOLOv9 with OpenVINO™</a></li>
<li class="toctree-l3"><a class="reference internal" href="../notebooks/zeroscope-text2video-with-output.html">Video generation with ZeroScope and OpenVINO</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../learn-openvino/openvino-samples.html">Sample Applications (Python &amp; C++)</a><input class="toctree-checkbox" id="toctree-checkbox-9" name="toctree-checkbox-9" type="checkbox"/><label for="toctree-checkbox-9"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/get-started-demos.html">Get Started with Samples</a></li>





<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/hello-classification.html">Hello Classification Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/hello-nv12-input-classification.html">Hello NV12 Input Classification Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/hello-query-device.html">Hello Query Device Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/hello-reshape-ssd.html">Hello Reshape SSD Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/image-classification-async.html">Image Classification Async Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/model-creation.html">Model Creation Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/sync-benchmark.html">Sync Benchmark Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/throughput-benchmark.html">Throughput Benchmark Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/bert-benchmark.html">Bert Benchmark Python Sample</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/openvino-samples/benchmark-tool.html">Benchmark Tool</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../learn-openvino/llm_inference_guide.html">Large Language Model Inference Guide</a><input class="toctree-checkbox" id="toctree-checkbox-10" name="toctree-checkbox-10" type="checkbox"/><label for="toctree-checkbox-10"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/llm_inference_guide/llm-inference-hf.html">LLM Inference with Optimum Intel</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/llm_inference_guide/llm-inference-native-ov.html">LLM Inference with OpenVINO API</a></li>
<li class="toctree-l3"><a class="reference internal" href="../learn-openvino/llm_inference_guide/ov-tokenizers.html">OpenVINO Tokenizers</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l1 has-children"><a class="reference internal" href="../openvino-workflow.html">OPENVINO WORKFLOW</a><input class="toctree-checkbox" id="toctree-checkbox-11" name="toctree-checkbox-11" type="checkbox"/><label for="toctree-checkbox-11"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l2 has-children"><a class="reference internal" href="../openvino-workflow/model-preparation.html">Model Preparation</a><input class="toctree-checkbox" id="toctree-checkbox-12" name="toctree-checkbox-12" type="checkbox"/><label for="toctree-checkbox-12"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3 has-children"><a class="reference internal" href="../openvino-workflow/model-preparation/convert-model-to-ir.html">Convert to OpenVINO Model</a><input class="toctree-checkbox" id="toctree-checkbox-13" name="toctree-checkbox-13" type="checkbox"/><label for="toctree-checkbox-13"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-preparation/convert-model-pytorch.html">Convert from PyTorch</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-preparation/convert-model-tensorflow.html">Convert from TensorFlow</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-preparation/convert-model-onnx.html">Convert from ONNX</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-preparation/convert-model-tensorflow-lite.html">Convert from TensorFlow Lite</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-preparation/convert-model-paddle.html">Convert from PaddlePaddle</a></li>
</ul>
</li>
<li class="toctree-l3"><a class="reference internal" href="../openvino-workflow/model-preparation/conversion-parameters.html">Conversion Parameters</a></li>
<li class="toctree-l3"><a class="reference internal" href="../openvino-workflow/model-preparation/setting-input-shapes.html">Setting Input Shapes</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../openvino-workflow/model-optimization.html">Model Optimization and Compression</a><input class="toctree-checkbox" id="toctree-checkbox-14" name="toctree-checkbox-14" type="checkbox"/><label for="toctree-checkbox-14"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3 has-children"><a class="reference internal" href="../openvino-workflow/model-optimization-guide/quantizing-models-post-training.html">Quantizing Models Post-training</a><input class="toctree-checkbox" id="toctree-checkbox-15" name="toctree-checkbox-15" type="checkbox"/><label for="toctree-checkbox-15"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-optimization-guide/quantizing-models-post-training/basic-quantization-flow.html">Basic Quantization Flow</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-optimization-guide/quantizing-models-post-training/quantizing-with-accuracy-control.html">Quantizing with Accuracy Control</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../openvino-workflow/model-optimization-guide/compressing-models-during-training.html">Compressing Models During Training</a><input class="toctree-checkbox" id="toctree-checkbox-16" name="toctree-checkbox-16" type="checkbox"/><label for="toctree-checkbox-16"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-optimization-guide/compressing-models-during-training/quantization-aware-training.html">Quantization-aware Training (QAT)</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/model-optimization-guide/compressing-models-during-training/filter-pruning.html">Filter Pruning of Convolutional Models</a></li>
</ul>
</li>
<li class="toctree-l3"><a class="reference internal" href="../openvino-workflow/model-optimization-guide/weight-compression.html">Weight Compression</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../openvino-workflow/running-inference.html">Running Inference</a><input class="toctree-checkbox" id="toctree-checkbox-17" name="toctree-checkbox-17" type="checkbox"/><label for="toctree-checkbox-17"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/integrate-openvino-with-your-application.html">Integrate OpenVINO™ with Your Application</a><input class="toctree-checkbox" id="toctree-checkbox-18" name="toctree-checkbox-18" type="checkbox"/><label for="toctree-checkbox-18"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/integrate-openvino-with-your-application/model-representation.html">Model Representation in OpenVINO™ Runtime</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/integrate-openvino-with-your-application/inference-request.html">OpenVINO™ Inference Request</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/integrate-openvino-with-your-application/python-api-advanced-inference.html">OpenVINO™ Runtime Python API Advanced Inference</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/integrate-openvino-with-your-application/python-api-exclusives.html">OpenVINO™ Python API Exclusives</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes.html">Inference Devices and Modes</a><input class="toctree-checkbox" id="toctree-checkbox-19" name="toctree-checkbox-19" type="checkbox"/><label for="toctree-checkbox-19"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/cpu-device.html">CPU Device</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/gpu-device.html">GPU Device</a><input class="toctree-checkbox" id="toctree-checkbox-20" name="toctree-checkbox-20" type="checkbox"/><label for="toctree-checkbox-20"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/gpu-device/remote-tensor-api-gpu-plugin.html">Remote Tensor API of GPU Plugin</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/npu-device.html">NPU Device</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/auto-device-selection.html">Automatic Device Selection</a><input class="toctree-checkbox" id="toctree-checkbox-21" name="toctree-checkbox-21" type="checkbox"/><label for="toctree-checkbox-21"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/auto-device-selection/debugging-auto-device.html">Debugging Auto-Device Plugin</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/multi-device.html">Multi-device execution</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/hetero-execution.html">Heterogeneous execution</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/automatic-batching.html">Automatic Batching</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/inference-devices-and-modes/query-device-properties.html">Query Device Properties - Configuration</a></li>
</ul>
</li>
<li class="toctree-l3"><a class="reference internal" href="../openvino-workflow/running-inference/changing-input-shape.html">Changing Input Shapes</a></li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/dynamic-shapes.html">Dynamic Shapes</a><input class="toctree-checkbox" id="toctree-checkbox-22" name="toctree-checkbox-22" type="checkbox"/><label for="toctree-checkbox-22"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/dynamic-shapes/openvino-without-dynamic-shapes-api.html">When Dynamic Shapes API is Not Applicable</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/stateful-models.html">Stateful models and State API</a><input class="toctree-checkbox" id="toctree-checkbox-23" name="toctree-checkbox-23" type="checkbox"/><label for="toctree-checkbox-23"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/stateful-models/obtaining-stateful-openvino-model.html">Obtaining a Stateful OpenVINO Model</a></li>
</ul>
</li>
<li class="toctree-l3"><a class="reference internal" href="../openvino-workflow/running-inference/string-tensors.html">String Tensors</a></li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference.html">Optimize Inference</a><input class="toctree-checkbox" id="toctree-checkbox-24" name="toctree-checkbox-24" type="checkbox"/><label for="toctree-checkbox-24"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/general-optimizations.html">General Optimizations</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/high-level-performance-hints.html">High-level Performance Hints</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/precision-control.html">Precision Control</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimizing-latency.html">Optimizing for Latency</a><input class="toctree-checkbox" id="toctree-checkbox-25" name="toctree-checkbox-25" type="checkbox"/><label for="toctree-checkbox-25"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimizing-latency/model-caching-overview.html">Model Caching Overview</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimizing-throughput.html">Optimizing for Throughput</a><input class="toctree-checkbox" id="toctree-checkbox-26" name="toctree-checkbox-26" type="checkbox"/><label for="toctree-checkbox-26"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimizing-throughput/advanced_throughput_options.html">Advanced Throughput Options</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimize-preprocessing.html">Optimize Preprocessing</a><input class="toctree-checkbox" id="toctree-checkbox-27" name="toctree-checkbox-27" type="checkbox"/><label for="toctree-checkbox-27"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimize-preprocessing/preprocessing-api-details.html">Preprocessing API - details</a></li>
<li class="toctree-l5"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimize-preprocessing/layout-api-overview.html">Layout API Overview</a></li>
<li class="toctree-l5"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimize-preprocessing/integrate-save-preprocessing-use-case.html">Use Case - Integrate and Save Preprocessing Steps Into IR</a></li>
<li class="toctree-l5"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimize-preprocessing/torchvision-preprocessing-converter.html">Torchvision preprocessing converter</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimizing-low-level-implementation.html">Further Low-Level Implementation Details</a></li>
<li class="toctree-l4"><a class="reference internal" href="../openvino-workflow/running-inference/optimize-inference/optimizing-memory-usage.html">Optimizing memory usage</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../openvino-workflow/deployment-locally.html">Deployment on a Local System</a><input class="toctree-checkbox" id="toctree-checkbox-28" name="toctree-checkbox-28" type="checkbox"/><label for="toctree-checkbox-28"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../openvino-workflow/deployment-locally/local-distribution-libraries.html">Local Distribution Libraries</a></li>
<li class="toctree-l3"><a class="reference internal" href="../openvino-workflow/deployment-locally/optimial-binary-size-conditional-compilation.html">Optimize Binaries Size</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../ovms_what_is_openvino_model_server.html">Deployment on a Model Server</a><input class="toctree-checkbox" id="toctree-checkbox-29" name="toctree-checkbox-29" type="checkbox"/><label for="toctree-checkbox-29"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../ovms_docs_quick_start_guide.html">Quickstart Guide</a></li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../ovms_docs_serving_model.html">Setup Model Server</a><input class="toctree-checkbox" id="toctree-checkbox-30" name="toctree-checkbox-30" type="checkbox"/><label for="toctree-checkbox-30"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_models_repository.html">Prepare a Model Repository</a><input class="toctree-checkbox" id="toctree-checkbox-31" name="toctree-checkbox-31" type="checkbox"/><label for="toctree-checkbox-31"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_cloud_storage.html">Use Cloud Storage</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_parameters.html">Model Server Parameters</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_target_devices.html">Using AI Accelerators</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_security.html">Security Considerations</a></li>
</ul>
</li>
<li class="toctree-l3"><a class="reference internal" href="../ovms_docs_deploying_server.html">Deploy Model Server</a></li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../ovms_docs_server_app.html">Write a Client Application</a><input class="toctree-checkbox" id="toctree-checkbox-32" name="toctree-checkbox-32" type="checkbox"/><label for="toctree-checkbox-32"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_clients_tfs.html">TensorFlow Serving API</a><input class="toctree-checkbox" id="toctree-checkbox-33" name="toctree-checkbox-33" type="checkbox"/><label for="toctree-checkbox-33"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_grpc_api_tfs.html">gRPC API</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_rest_api_tfs.html">RESTful API</a></li>
<li class="toctree-l5"><a class="reference external" href="https://github.com/openvinotoolkit/model_server/blob/main/client/python/tensorflow-serving-api/samples/README.md">Examples</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_clients_kfs.html">KServe API</a><input class="toctree-checkbox" id="toctree-checkbox-34" name="toctree-checkbox-34" type="checkbox"/><label for="toctree-checkbox-34"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_grpc_api_kfs.html">gRPC API</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_rest_api_kfs.html">RESTful API</a></li>
<li class="toctree-l5"><a class="reference external" href="https://github.com/openvinotoolkit/model_server/tree/main/client/python/kserve-api/samples">Examples</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_c_api.html">OpenVINO Model Server C-API</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../ovms_docs_features.html">Model Server Features</a><input class="toctree-checkbox" id="toctree-checkbox-35" name="toctree-checkbox-35" type="checkbox"/><label for="toctree-checkbox-35"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_dag.html">Directed Acyclic Graph (DAG) Scheduler</a><input class="toctree-checkbox" id="toctree-checkbox-36" name="toctree-checkbox-36" type="checkbox"/><label for="toctree-checkbox-36"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_demultiplexing.html">Demultiplexing in DAG</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_custom_node_development.html">Custom Node Development Guide</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_mediapipe.html">Integration with mediapipe</a><input class="toctree-checkbox" id="toctree-checkbox-37" name="toctree-checkbox-37" type="checkbox"/><label for="toctree-checkbox-37"><i class="fas fa-chevron-down"></i></label><ul class="simple">
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_streaming_endpoints.html">gRPC Streaming API</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_python_support_reference.html">Python Execution in OpenVINO Model Server</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_stateful_models.html">Serving Stateful Models</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_binary_input.html">Support for Binary Encoded Image Input Data</a><input class="toctree-checkbox" id="toctree-checkbox-38" name="toctree-checkbox-38" type="checkbox"/><label for="toctree-checkbox-38"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_binary_input_layout_and_shape.html">Input Shape and Layout Considerations</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_binary_input_tfs.html">Predict on Binary Inputs via TensorFlow Serving API</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_binary_input_kfs.html">Predict on Binary Inputs via KServe API</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_demo_tensorflow_conversion.html">Convert TensorFlow Models to Accept Binary Inputs</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_text.html">Support for text data format</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_shape_batch_layout.html">Batch, Shape and Layout</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_dynamic_input.html">Dynamic Input Parameters</a><input class="toctree-checkbox" id="toctree-checkbox-39" name="toctree-checkbox-39" type="checkbox"/><label for="toctree-checkbox-39"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_dynamic_shape_dynamic_model.html">Dynamic Shape with dynamic IR/ONNX Model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_dynamic_shape_binary_inputs.html">Dynamic Shape with Binary Inputs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_dynamic_bs_auto_reload.html">Dynamic Batch Size with Automatic Model Reloading</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_dynamic_shape_auto_reload.html">Dynamic Shape with Automatic Model Reloading</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_dynamic_bs_demultiplexer.html">Dynamic batch size with OpenVINO™ Model Server Demultiplexer</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_dynamic_shape_custom_node.html">Dynamic Shape with a Custom Node</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_online_config_changes.html">Online Configuration Updates</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_model_version_policy.html">Model Version Policy</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_metrics.html">Metrics</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_c_api.html">OpenVINO Model Server C-API</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_advanced.html">Advanced Features</a><input class="toctree-checkbox" id="toctree-checkbox-40" name="toctree-checkbox-40" type="checkbox"/><label for="toctree-checkbox-40"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_sample_cpu_extension.html">CPU Extensions</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_model_cache.html">Model Cache</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_docs_custom_loader.html">Custom Model Loader</a></li>



<li class="toctree-l5"><a class="reference internal" href="../ovms_extras_nginx-mtls-auth-readme.html">Securing Model Server with NGINX</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l3"><a class="reference internal" href="../ovms_docs_performance_tuning.html">Performance tuning</a></li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../ovms_docs_demos.html">Demos</a><input class="toctree-checkbox" id="toctree-checkbox-41" name="toctree-checkbox-41" type="checkbox"/><label for="toctree-checkbox-41"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_clip_image_classification.html">CLIP image classification</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_age_gender_guide.html">Age and Gender Recognition via REST API</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_horizontal_text_detection.html">Horizontal Text Detection in Real-Time</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_optical_character_recognition.html">Optical Character Recognition with Directed Acyclic Graph</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_face_detection.html">Face Detection Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_face_blur_pipeline.html">Face Blur Pipeline Demo with OVMS</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_capi_inference_demo.html">C API inference demo (C/C++)</a></li>

<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_single_face_analysis_pipeline.html">Single Face Analysis Pipeline Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_multi_faces_analysis_pipeline.html">Multi Faces Analysis Pipeline Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_demo_ensemble.html">Model Ensemble Pipeline Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_demo_mediapipe_image_classification.html">MediaPipe Image Classification Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_demo_mediapipe_multi_model.html">MediaPipe Multi Model Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_demo_mediapipe_object_detection.html">MediaPipe Object Detection Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_demo_mediapipe_holistic.html">MediaPipe Holistic Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_docs_demo_mediapipe_iris.html">MediaPipe Iris Demo</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_docs_image_classification.html">Image Classification Demos</a><input class="toctree-checkbox" id="toctree-checkbox-42" name="toctree-checkbox-42" type="checkbox"/><label for="toctree-checkbox-42"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_demo_image_classification.html">Image Classification Demo (Python)</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_demo_image_classification_cpp.html">Image Classification Demo (C++)</a></li>


<li class="toctree-l5"><a class="reference internal" href="../ovms_demo_image_classification_go.html">Image Classification Demo (Go)</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_using_onnx_model.html">Prediction Example with an ONNX Model</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_tf_classification.html">Model Server demo with a direct import of TensorFlow model</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_person_vehicle_bike_detection.html">Person, vehicle, bike detection with multiple data sources</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_vehicle_analysis_pipeline.html">Vehicle Analysis Pipeline Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_real_time_stream_analysis.html">Real Time Stream Analysis Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_using_paddlepaddle_model.html">Segmentation Example with a PaddlePaddle Model</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_bert.html">BERT Question Answering Demo</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_universal-sentence-encoder.html">Using inputs data in string format with universal-sentence-encoder model</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../ovms_demo_benchmark_client.html">Benchmark Client</a><input class="toctree-checkbox" id="toctree-checkbox-43" name="toctree-checkbox-43" type="checkbox"/><label for="toctree-checkbox-43"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../ovms_demo_benchmark_app.html">Benchmark Client (Python)</a></li>
<li class="toctree-l5"><a class="reference internal" href="../ovms_demo_benchmark_app_cpp.html">Benchmark Client (C++)</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_python_seq2seq.html">Seq2seq demo with python node</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_demo_python_stable_diffusion.html">Stable diffusion demo with python node</a></li>
<li class="toctree-l4"><a class="reference internal" href="../ovms_string_output_model_demo.html">String output model demo</a></li>
</ul>
</li>
<li class="toctree-l3"><a class="reference internal" href="../ovms_docs_troubleshooting.html">Troubleshooting</a></li>
</ul>
</li>
<li class="toctree-l2"><a class="reference internal" href="../openvino-workflow/torch-compile.html">PyTorch Deployment via “torch.compile”</a></li>
</ul>
</li>
<li class="toctree-l1 has-children"><a class="reference internal" href="../documentation.html">DOCUMENTATION</a><input class="toctree-checkbox" id="toctree-checkbox-44" name="toctree-checkbox-44" type="checkbox"/><label for="toctree-checkbox-44"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l2 has-children"><a class="reference internal" href="../api/api_reference.html">API Reference</a><input class="toctree-checkbox" id="toctree-checkbox-45" name="toctree-checkbox-45" type="checkbox"/><label for="toctree-checkbox-45"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3 has-children"><a class="reference internal" href="../api/ie_python_api/api.html">OpenVINO Python API</a><input class="toctree-checkbox" id="toctree-checkbox-46" name="toctree-checkbox-46" type="checkbox"/><label for="toctree-checkbox-46"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.html">openvino</a><input class="toctree-checkbox" id="toctree-checkbox-47" name="toctree-checkbox-47" type="checkbox"/><label for="toctree-checkbox-47"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.compile_model.html">openvino.compile_model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.convert_model.html">openvino.convert_model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.get_batch.html">openvino.get_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.get_version.html">openvino.get_version</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.save_model.html">openvino.save_model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.serialize.html">openvino.serialize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.set_batch.html">openvino.set_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.shutdown.html">openvino.shutdown</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.tensor_from_file.html">openvino.tensor_from_file</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.AsyncInferQueue.html">openvino.AsyncInferQueue</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.CompiledModel.html">openvino.CompiledModel</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Core.html">openvino.Core</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Dimension.html">openvino.Dimension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.InferRequest.html">openvino.InferRequest</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Layout.html">openvino.Layout</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Model.html">openvino.Model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.OVAny.html">openvino.OVAny</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.PartialShape.html">openvino.PartialShape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.RemoteContext.html">openvino.RemoteContext</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.RemoteTensor.html">openvino.RemoteTensor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Shape.html">openvino.Shape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Strides.html">openvino.Strides</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Symbol.html">openvino.Symbol</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Tensor.html">openvino.Tensor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.Type.html">openvino.Type</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.VAContext.html">openvino.VAContext</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.VASurfaceTensor.html">openvino.VASurfaceTensor</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.html">openvino.runtime</a><input class="toctree-checkbox" id="toctree-checkbox-48" name="toctree-checkbox-48" type="checkbox"/><label for="toctree-checkbox-48"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.compile_model.html">openvino.runtime.compile_model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.get_batch.html">openvino.runtime.get_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.get_version.html">openvino.runtime.get_version</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.save_model.html">openvino.runtime.save_model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.serialize.html">openvino.runtime.serialize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.set_batch.html">openvino.runtime.set_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.shutdown.html">openvino.runtime.shutdown</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.tensor_from_file.html">openvino.runtime.tensor_from_file</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.AsyncInferQueue.html">openvino.runtime.AsyncInferQueue</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.AxisSet.html">openvino.runtime.AxisSet</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.AxisVector.html">openvino.runtime.AxisVector</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.CompiledModel.html">openvino.runtime.CompiledModel</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.ConstOutput.html">openvino.runtime.ConstOutput</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Coordinate.html">openvino.runtime.Coordinate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.CoordinateDiff.html">openvino.runtime.CoordinateDiff</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Core.html">openvino.runtime.Core</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Dimension.html">openvino.runtime.Dimension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.DiscreteTypeInfo.html">openvino.runtime.DiscreteTypeInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Extension.html">openvino.runtime.Extension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.InferRequest.html">openvino.runtime.InferRequest</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Input.html">openvino.runtime.Input</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Layout.html">openvino.runtime.Layout</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Model.html">openvino.runtime.Model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Node.html">openvino.runtime.Node</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.OVAny.html">openvino.runtime.OVAny</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Output.html">openvino.runtime.Output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.PartialShape.html">openvino.runtime.PartialShape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.ProfilingInfo.html">openvino.runtime.ProfilingInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.RTMap.html">openvino.runtime.RTMap</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Shape.html">openvino.runtime.Shape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Strides.html">openvino.runtime.Strides</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Symbol.html">openvino.runtime.Symbol</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Tensor.html">openvino.runtime.Tensor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Type.html">openvino.runtime.Type</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.Version.html">openvino.runtime.Version</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.html">openvino.runtime.op</a><input class="toctree-checkbox" id="toctree-checkbox-49" name="toctree-checkbox-49" type="checkbox"/><label for="toctree-checkbox-49"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.Constant.html">openvino.runtime.op.Constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.Parameter.html">openvino.runtime.op.Parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.Result.html">openvino.runtime.op.Result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op._PagedAttentionExtension.html">openvino.runtime.op._PagedAttentionExtension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.assign.html">openvino.runtime.op.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.if_op.html">openvino.runtime.op.if_op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.loop.html">openvino.runtime.op.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.tensor_iterator.html">openvino.runtime.op.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.html">openvino.runtime.op.util</a><input class="toctree-checkbox" id="toctree-checkbox-50" name="toctree-checkbox-50" type="checkbox"/><label for="toctree-checkbox-50"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.ArithmeticReduction.html">openvino.runtime.op.util.ArithmeticReduction</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.BinaryElementwiseArithmetic.html">openvino.runtime.op.util.BinaryElementwiseArithmetic</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.BinaryElementwiseComparison.html">openvino.runtime.op.util.BinaryElementwiseComparison</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.BinaryElementwiseLogical.html">openvino.runtime.op.util.BinaryElementwiseLogical</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.BodyOutputDescription.html">openvino.runtime.op.util.BodyOutputDescription</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.ConcatOutputDescription.html">openvino.runtime.op.util.ConcatOutputDescription</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.IndexReduction.html">openvino.runtime.op.util.IndexReduction</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.InvariantInputDescription.html">openvino.runtime.op.util.InvariantInputDescription</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.MergedInputDescription.html">openvino.runtime.op.util.MergedInputDescription</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.SliceInputDescription.html">openvino.runtime.op.util.SliceInputDescription</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.UnaryElementwiseArithmetic.html">openvino.runtime.op.util.UnaryElementwiseArithmetic</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.Variable.html">openvino.runtime.op.util.Variable</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.op.util.VariableInfo.html">openvino.runtime.op.util.VariableInfo</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.html">openvino.runtime.opset1</a><input class="toctree-checkbox" id="toctree-checkbox-51" name="toctree-checkbox-51" type="checkbox"/><label for="toctree-checkbox-51"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.abs.html">openvino.runtime.opset1.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.absolute.html">openvino.runtime.opset1.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.acos.html">openvino.runtime.opset1.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.add.html">openvino.runtime.opset1.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.asin.html">openvino.runtime.opset1.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.atan.html">openvino.runtime.opset1.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.avg_pool.html">openvino.runtime.opset1.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.batch_norm_inference.html">openvino.runtime.opset1.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.binary_convolution.html">openvino.runtime.opset1.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.broadcast.html">openvino.runtime.opset1.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.ceil.html">openvino.runtime.opset1.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.ceiling.html">openvino.runtime.opset1.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.clamp.html">openvino.runtime.opset1.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.concat.html">openvino.runtime.opset1.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.constant.html">openvino.runtime.opset1.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.convert.html">openvino.runtime.opset1.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.convert_like.html">openvino.runtime.opset1.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.convolution.html">openvino.runtime.opset1.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.convolution_backprop_data.html">openvino.runtime.opset1.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.cos.html">openvino.runtime.opset1.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.cosh.html">openvino.runtime.opset1.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.ctc_greedy_decoder.html">openvino.runtime.opset1.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.deformable_convolution.html">openvino.runtime.opset1.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.deformable_psroi_pooling.html">openvino.runtime.opset1.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.depth_to_space.html">openvino.runtime.opset1.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.detection_output.html">openvino.runtime.opset1.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.divide.html">openvino.runtime.opset1.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.elu.html">openvino.runtime.opset1.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.equal.html">openvino.runtime.opset1.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.erf.html">openvino.runtime.opset1.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.exp.html">openvino.runtime.opset1.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.fake_quantize.html">openvino.runtime.opset1.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.floor.html">openvino.runtime.opset1.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.floor_mod.html">openvino.runtime.opset1.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.gather.html">openvino.runtime.opset1.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.gather_tree.html">openvino.runtime.opset1.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.greater.html">openvino.runtime.opset1.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.greater_equal.html">openvino.runtime.opset1.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.grn.html">openvino.runtime.opset1.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.group_convolution.html">openvino.runtime.opset1.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.group_convolution_backprop_data.html">openvino.runtime.opset1.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.hard_sigmoid.html">openvino.runtime.opset1.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.interpolate.html">openvino.runtime.opset1.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.less.html">openvino.runtime.opset1.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.less_equal.html">openvino.runtime.opset1.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.log.html">openvino.runtime.opset1.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.logical_and.html">openvino.runtime.opset1.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.logical_not.html">openvino.runtime.opset1.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.logical_or.html">openvino.runtime.opset1.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.logical_xor.html">openvino.runtime.opset1.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.lrn.html">openvino.runtime.opset1.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.lstm_cell.html">openvino.runtime.opset1.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.lstm_sequence.html">openvino.runtime.opset1.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.matmul.html">openvino.runtime.opset1.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.max_pool.html">openvino.runtime.opset1.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.maximum.html">openvino.runtime.opset1.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.minimum.html">openvino.runtime.opset1.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.mod.html">openvino.runtime.opset1.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.multiply.html">openvino.runtime.opset1.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.negative.html">openvino.runtime.opset1.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.non_max_suppression.html">openvino.runtime.opset1.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.normalize_l2.html">openvino.runtime.opset1.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.not_equal.html">openvino.runtime.opset1.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.one_hot.html">openvino.runtime.opset1.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.pad.html">openvino.runtime.opset1.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.parameter.html">openvino.runtime.opset1.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.power.html">openvino.runtime.opset1.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.prelu.html">openvino.runtime.opset1.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.prior_box.html">openvino.runtime.opset1.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.prior_box_clustered.html">openvino.runtime.opset1.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.proposal.html">openvino.runtime.opset1.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.psroi_pooling.html">openvino.runtime.opset1.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.range.html">openvino.runtime.opset1.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reduce_logical_and.html">openvino.runtime.opset1.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reduce_logical_or.html">openvino.runtime.opset1.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reduce_max.html">openvino.runtime.opset1.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reduce_mean.html">openvino.runtime.opset1.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reduce_min.html">openvino.runtime.opset1.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reduce_prod.html">openvino.runtime.opset1.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reduce_sum.html">openvino.runtime.opset1.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.region_yolo.html">openvino.runtime.opset1.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.relu.html">openvino.runtime.opset1.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reshape.html">openvino.runtime.opset1.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.result.html">openvino.runtime.opset1.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.reverse_sequence.html">openvino.runtime.opset1.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.select.html">openvino.runtime.opset1.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.selu.html">openvino.runtime.opset1.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.shape_of.html">openvino.runtime.opset1.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.sigmoid.html">openvino.runtime.opset1.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.sign.html">openvino.runtime.opset1.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.sin.html">openvino.runtime.opset1.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.sinh.html">openvino.runtime.opset1.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.softmax.html">openvino.runtime.opset1.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.space_to_depth.html">openvino.runtime.opset1.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.split.html">openvino.runtime.opset1.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.sqrt.html">openvino.runtime.opset1.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.squared_difference.html">openvino.runtime.opset1.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.squeeze.html">openvino.runtime.opset1.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.strided_slice.html">openvino.runtime.opset1.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.subtract.html">openvino.runtime.opset1.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.tan.html">openvino.runtime.opset1.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.tanh.html">openvino.runtime.opset1.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.tile.html">openvino.runtime.opset1.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.topk.html">openvino.runtime.opset1.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.transpose.html">openvino.runtime.opset1.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.unsqueeze.html">openvino.runtime.opset1.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.variadic_split.html">openvino.runtime.opset1.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset1.tensor_iterator.html">openvino.runtime.opset1.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.html">openvino.runtime.opset2</a><input class="toctree-checkbox" id="toctree-checkbox-52" name="toctree-checkbox-52" type="checkbox"/><label for="toctree-checkbox-52"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.abs.html">openvino.runtime.opset2.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.absolute.html">openvino.runtime.opset2.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.acos.html">openvino.runtime.opset2.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.add.html">openvino.runtime.opset2.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.asin.html">openvino.runtime.opset2.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.atan.html">openvino.runtime.opset2.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.avg_pool.html">openvino.runtime.opset2.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.batch_norm_inference.html">openvino.runtime.opset2.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.batch_to_space.html">openvino.runtime.opset2.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.binary_convolution.html">openvino.runtime.opset2.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.broadcast.html">openvino.runtime.opset2.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.ceil.html">openvino.runtime.opset2.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.ceiling.html">openvino.runtime.opset2.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.clamp.html">openvino.runtime.opset2.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.concat.html">openvino.runtime.opset2.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.constant.html">openvino.runtime.opset2.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.convert.html">openvino.runtime.opset2.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.convert_like.html">openvino.runtime.opset2.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.convolution.html">openvino.runtime.opset2.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.convolution_backprop_data.html">openvino.runtime.opset2.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.cos.html">openvino.runtime.opset2.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.cosh.html">openvino.runtime.opset2.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.ctc_greedy_decoder.html">openvino.runtime.opset2.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.deformable_convolution.html">openvino.runtime.opset2.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.deformable_psroi_pooling.html">openvino.runtime.opset2.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.depth_to_space.html">openvino.runtime.opset2.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.detection_output.html">openvino.runtime.opset2.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.divide.html">openvino.runtime.opset2.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.elu.html">openvino.runtime.opset2.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.equal.html">openvino.runtime.opset2.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.erf.html">openvino.runtime.opset2.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.exp.html">openvino.runtime.opset2.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.fake_quantize.html">openvino.runtime.opset2.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.floor.html">openvino.runtime.opset2.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.floor_mod.html">openvino.runtime.opset2.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.gather.html">openvino.runtime.opset2.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.gather_tree.html">openvino.runtime.opset2.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.gelu.html">openvino.runtime.opset2.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.greater.html">openvino.runtime.opset2.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.greater_equal.html">openvino.runtime.opset2.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.grn.html">openvino.runtime.opset2.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.group_convolution.html">openvino.runtime.opset2.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.group_convolution_backprop_data.html">openvino.runtime.opset2.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.hard_sigmoid.html">openvino.runtime.opset2.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.interpolate.html">openvino.runtime.opset2.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.less.html">openvino.runtime.opset2.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.less_equal.html">openvino.runtime.opset2.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.log.html">openvino.runtime.opset2.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.logical_and.html">openvino.runtime.opset2.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.logical_not.html">openvino.runtime.opset2.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.logical_or.html">openvino.runtime.opset2.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.logical_xor.html">openvino.runtime.opset2.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.lrn.html">openvino.runtime.opset2.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.lstm_cell.html">openvino.runtime.opset2.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.lstm_sequence.html">openvino.runtime.opset2.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.matmul.html">openvino.runtime.opset2.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.max_pool.html">openvino.runtime.opset2.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.maximum.html">openvino.runtime.opset2.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.minimum.html">openvino.runtime.opset2.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.mod.html">openvino.runtime.opset2.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.multiply.html">openvino.runtime.opset2.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.mvn.html">openvino.runtime.opset2.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.negative.html">openvino.runtime.opset2.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.non_max_suppression.html">openvino.runtime.opset2.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.normalize_l2.html">openvino.runtime.opset2.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.not_equal.html">openvino.runtime.opset2.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.one_hot.html">openvino.runtime.opset2.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.pad.html">openvino.runtime.opset2.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.parameter.html">openvino.runtime.opset2.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.power.html">openvino.runtime.opset2.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.prelu.html">openvino.runtime.opset2.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.prior_box.html">openvino.runtime.opset2.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.prior_box_clustered.html">openvino.runtime.opset2.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.proposal.html">openvino.runtime.opset2.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.psroi_pooling.html">openvino.runtime.opset2.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.range.html">openvino.runtime.opset2.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reduce_logical_and.html">openvino.runtime.opset2.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reduce_logical_or.html">openvino.runtime.opset2.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reduce_max.html">openvino.runtime.opset2.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reduce_mean.html">openvino.runtime.opset2.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reduce_min.html">openvino.runtime.opset2.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reduce_prod.html">openvino.runtime.opset2.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reduce_sum.html">openvino.runtime.opset2.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.region_yolo.html">openvino.runtime.opset2.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.relu.html">openvino.runtime.opset2.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reorg_yolo.html">openvino.runtime.opset2.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reshape.html">openvino.runtime.opset2.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.result.html">openvino.runtime.opset2.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.reverse_sequence.html">openvino.runtime.opset2.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.roi_pooling.html">openvino.runtime.opset2.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.select.html">openvino.runtime.opset2.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.selu.html">openvino.runtime.opset2.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.shape_of.html">openvino.runtime.opset2.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.sigmoid.html">openvino.runtime.opset2.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.sign.html">openvino.runtime.opset2.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.sin.html">openvino.runtime.opset2.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.sinh.html">openvino.runtime.opset2.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.softmax.html">openvino.runtime.opset2.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.space_to_batch.html">openvino.runtime.opset2.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.space_to_depth.html">openvino.runtime.opset2.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.split.html">openvino.runtime.opset2.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.sqrt.html">openvino.runtime.opset2.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.squared_difference.html">openvino.runtime.opset2.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.squeeze.html">openvino.runtime.opset2.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.strided_slice.html">openvino.runtime.opset2.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.subtract.html">openvino.runtime.opset2.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.tan.html">openvino.runtime.opset2.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.tanh.html">openvino.runtime.opset2.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.tile.html">openvino.runtime.opset2.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.topk.html">openvino.runtime.opset2.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.transpose.html">openvino.runtime.opset2.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.unsqueeze.html">openvino.runtime.opset2.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.variadic_split.html">openvino.runtime.opset2.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset2.tensor_iterator.html">openvino.runtime.opset2.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.html">openvino.runtime.opset3</a><input class="toctree-checkbox" id="toctree-checkbox-53" name="toctree-checkbox-53" type="checkbox"/><label for="toctree-checkbox-53"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.abs.html">openvino.runtime.opset3.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.absolute.html">openvino.runtime.opset3.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.acos.html">openvino.runtime.opset3.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.add.html">openvino.runtime.opset3.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.asin.html">openvino.runtime.opset3.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.assign.html">openvino.runtime.opset3.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.atan.html">openvino.runtime.opset3.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.avg_pool.html">openvino.runtime.opset3.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.batch_norm_inference.html">openvino.runtime.opset3.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.batch_to_space.html">openvino.runtime.opset3.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.binary_convolution.html">openvino.runtime.opset3.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.broadcast.html">openvino.runtime.opset3.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.bucketize.html">openvino.runtime.opset3.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.ceil.html">openvino.runtime.opset3.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.ceiling.html">openvino.runtime.opset3.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.clamp.html">openvino.runtime.opset3.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.concat.html">openvino.runtime.opset3.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.constant.html">openvino.runtime.opset3.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.convert.html">openvino.runtime.opset3.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.convert_like.html">openvino.runtime.opset3.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.convolution.html">openvino.runtime.opset3.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.convolution_backprop_data.html">openvino.runtime.opset3.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.cos.html">openvino.runtime.opset3.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.cosh.html">openvino.runtime.opset3.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.ctc_greedy_decoder.html">openvino.runtime.opset3.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.cum_sum.html">openvino.runtime.opset3.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.cumsum.html">openvino.runtime.opset3.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.deformable_convolution.html">openvino.runtime.opset3.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.deformable_psroi_pooling.html">openvino.runtime.opset3.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.depth_to_space.html">openvino.runtime.opset3.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.detection_output.html">openvino.runtime.opset3.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.divide.html">openvino.runtime.opset3.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.elu.html">openvino.runtime.opset3.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.embedding_bag_offsets_sum.html">openvino.runtime.opset3.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.embedding_bag_packed_sum.html">openvino.runtime.opset3.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.embedding_segments_sum.html">openvino.runtime.opset3.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.equal.html">openvino.runtime.opset3.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.erf.html">openvino.runtime.opset3.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.exp.html">openvino.runtime.opset3.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.extract_image_patches.html">openvino.runtime.opset3.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.fake_quantize.html">openvino.runtime.opset3.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.floor.html">openvino.runtime.opset3.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.floor_mod.html">openvino.runtime.opset3.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.gather.html">openvino.runtime.opset3.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.gather_tree.html">openvino.runtime.opset3.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.gelu.html">openvino.runtime.opset3.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.greater.html">openvino.runtime.opset3.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.greater_equal.html">openvino.runtime.opset3.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.grn.html">openvino.runtime.opset3.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.group_convolution.html">openvino.runtime.opset3.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.group_convolution_backprop_data.html">openvino.runtime.opset3.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.gru_cell.html">openvino.runtime.opset3.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.hard_sigmoid.html">openvino.runtime.opset3.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.interpolate.html">openvino.runtime.opset3.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.less.html">openvino.runtime.opset3.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.less_equal.html">openvino.runtime.opset3.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.log.html">openvino.runtime.opset3.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.logical_and.html">openvino.runtime.opset3.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.logical_not.html">openvino.runtime.opset3.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.logical_or.html">openvino.runtime.opset3.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.logical_xor.html">openvino.runtime.opset3.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.lrn.html">openvino.runtime.opset3.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.lstm_cell.html">openvino.runtime.opset3.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.lstm_sequence.html">openvino.runtime.opset3.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.matmul.html">openvino.runtime.opset3.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.max_pool.html">openvino.runtime.opset3.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.maximum.html">openvino.runtime.opset3.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.minimum.html">openvino.runtime.opset3.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.mod.html">openvino.runtime.opset3.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.multiply.html">openvino.runtime.opset3.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.mvn.html">openvino.runtime.opset3.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.negative.html">openvino.runtime.opset3.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.non_max_suppression.html">openvino.runtime.opset3.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.non_zero.html">openvino.runtime.opset3.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.normalize_l2.html">openvino.runtime.opset3.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.not_equal.html">openvino.runtime.opset3.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.one_hot.html">openvino.runtime.opset3.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.pad.html">openvino.runtime.opset3.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.parameter.html">openvino.runtime.opset3.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.power.html">openvino.runtime.opset3.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.prelu.html">openvino.runtime.opset3.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.prior_box.html">openvino.runtime.opset3.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.prior_box_clustered.html">openvino.runtime.opset3.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.proposal.html">openvino.runtime.opset3.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.psroi_pooling.html">openvino.runtime.opset3.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.range.html">openvino.runtime.opset3.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.read_value.html">openvino.runtime.opset3.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reduce_logical_and.html">openvino.runtime.opset3.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reduce_logical_or.html">openvino.runtime.opset3.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reduce_max.html">openvino.runtime.opset3.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reduce_mean.html">openvino.runtime.opset3.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reduce_min.html">openvino.runtime.opset3.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reduce_prod.html">openvino.runtime.opset3.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reduce_sum.html">openvino.runtime.opset3.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.region_yolo.html">openvino.runtime.opset3.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.relu.html">openvino.runtime.opset3.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reorg_yolo.html">openvino.runtime.opset3.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reshape.html">openvino.runtime.opset3.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.result.html">openvino.runtime.opset3.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.reverse_sequence.html">openvino.runtime.opset3.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.rnn_cell.html">openvino.runtime.opset3.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.roi_align.html">openvino.runtime.opset3.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.roi_pooling.html">openvino.runtime.opset3.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.scatter_elements_update.html">openvino.runtime.opset3.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.scatter_update.html">openvino.runtime.opset3.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.select.html">openvino.runtime.opset3.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.selu.html">openvino.runtime.opset3.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.shape_of.html">openvino.runtime.opset3.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.shuffle_channels.html">openvino.runtime.opset3.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.sigmoid.html">openvino.runtime.opset3.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.sign.html">openvino.runtime.opset3.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.sin.html">openvino.runtime.opset3.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.sinh.html">openvino.runtime.opset3.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.softmax.html">openvino.runtime.opset3.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.space_to_batch.html">openvino.runtime.opset3.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.space_to_depth.html">openvino.runtime.opset3.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.split.html">openvino.runtime.opset3.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.sqrt.html">openvino.runtime.opset3.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.squared_difference.html">openvino.runtime.opset3.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.squeeze.html">openvino.runtime.opset3.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.strided_slice.html">openvino.runtime.opset3.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.subtract.html">openvino.runtime.opset3.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.tan.html">openvino.runtime.opset3.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.tanh.html">openvino.runtime.opset3.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.tile.html">openvino.runtime.opset3.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.topk.html">openvino.runtime.opset3.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.transpose.html">openvino.runtime.opset3.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.unsqueeze.html">openvino.runtime.opset3.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.variadic_split.html">openvino.runtime.opset3.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset3.tensor_iterator.html">openvino.runtime.opset3.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.html">openvino.runtime.opset4</a><input class="toctree-checkbox" id="toctree-checkbox-54" name="toctree-checkbox-54" type="checkbox"/><label for="toctree-checkbox-54"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.abs.html">openvino.runtime.opset4.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.absolute.html">openvino.runtime.opset4.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.acos.html">openvino.runtime.opset4.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.acosh.html">openvino.runtime.opset4.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.add.html">openvino.runtime.opset4.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.asin.html">openvino.runtime.opset4.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.asinh.html">openvino.runtime.opset4.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.assign.html">openvino.runtime.opset4.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.atan.html">openvino.runtime.opset4.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.atanh.html">openvino.runtime.opset4.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.avg_pool.html">openvino.runtime.opset4.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.batch_norm_inference.html">openvino.runtime.opset4.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.batch_to_space.html">openvino.runtime.opset4.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.binary_convolution.html">openvino.runtime.opset4.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.broadcast.html">openvino.runtime.opset4.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.bucketize.html">openvino.runtime.opset4.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.ceil.html">openvino.runtime.opset4.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.ceiling.html">openvino.runtime.opset4.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.clamp.html">openvino.runtime.opset4.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.concat.html">openvino.runtime.opset4.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.constant.html">openvino.runtime.opset4.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.convert.html">openvino.runtime.opset4.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.convert_like.html">openvino.runtime.opset4.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.convolution.html">openvino.runtime.opset4.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.convolution_backprop_data.html">openvino.runtime.opset4.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.cos.html">openvino.runtime.opset4.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.cosh.html">openvino.runtime.opset4.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.ctc_greedy_decoder.html">openvino.runtime.opset4.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.ctc_loss.html">openvino.runtime.opset4.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.cum_sum.html">openvino.runtime.opset4.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.cumsum.html">openvino.runtime.opset4.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.deformable_convolution.html">openvino.runtime.opset4.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.deformable_psroi_pooling.html">openvino.runtime.opset4.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.depth_to_space.html">openvino.runtime.opset4.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.detection_output.html">openvino.runtime.opset4.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.divide.html">openvino.runtime.opset4.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.elu.html">openvino.runtime.opset4.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.embedding_bag_offsets_sum.html">openvino.runtime.opset4.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.embedding_bag_packed_sum.html">openvino.runtime.opset4.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.embedding_segments_sum.html">openvino.runtime.opset4.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.equal.html">openvino.runtime.opset4.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.erf.html">openvino.runtime.opset4.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.exp.html">openvino.runtime.opset4.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.extract_image_patches.html">openvino.runtime.opset4.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.fake_quantize.html">openvino.runtime.opset4.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.floor.html">openvino.runtime.opset4.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.floor_mod.html">openvino.runtime.opset4.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.gather.html">openvino.runtime.opset4.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.gather_tree.html">openvino.runtime.opset4.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.gelu.html">openvino.runtime.opset4.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.greater.html">openvino.runtime.opset4.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.greater_equal.html">openvino.runtime.opset4.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.grn.html">openvino.runtime.opset4.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.group_convolution.html">openvino.runtime.opset4.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.group_convolution_backprop_data.html">openvino.runtime.opset4.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.gru_cell.html">openvino.runtime.opset4.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.hard_sigmoid.html">openvino.runtime.opset4.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.hswish.html">openvino.runtime.opset4.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.interpolate.html">openvino.runtime.opset4.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.less.html">openvino.runtime.opset4.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.less_equal.html">openvino.runtime.opset4.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.log.html">openvino.runtime.opset4.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.logical_and.html">openvino.runtime.opset4.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.logical_not.html">openvino.runtime.opset4.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.logical_or.html">openvino.runtime.opset4.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.logical_xor.html">openvino.runtime.opset4.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.lrn.html">openvino.runtime.opset4.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.lstm_cell.html">openvino.runtime.opset4.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.lstm_sequence.html">openvino.runtime.opset4.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.matmul.html">openvino.runtime.opset4.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.max_pool.html">openvino.runtime.opset4.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.maximum.html">openvino.runtime.opset4.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.minimum.html">openvino.runtime.opset4.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.mish.html">openvino.runtime.opset4.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.mod.html">openvino.runtime.opset4.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.multiply.html">openvino.runtime.opset4.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.mvn.html">openvino.runtime.opset4.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.negative.html">openvino.runtime.opset4.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.non_max_suppression.html">openvino.runtime.opset4.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.non_zero.html">openvino.runtime.opset4.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.normalize_l2.html">openvino.runtime.opset4.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.not_equal.html">openvino.runtime.opset4.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.one_hot.html">openvino.runtime.opset4.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.pad.html">openvino.runtime.opset4.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.parameter.html">openvino.runtime.opset4.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.power.html">openvino.runtime.opset4.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.prelu.html">openvino.runtime.opset4.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.prior_box.html">openvino.runtime.opset4.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.prior_box_clustered.html">openvino.runtime.opset4.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.proposal.html">openvino.runtime.opset4.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.psroi_pooling.html">openvino.runtime.opset4.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.range.html">openvino.runtime.opset4.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.read_value.html">openvino.runtime.opset4.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_l1.html">openvino.runtime.opset4.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_l2.html">openvino.runtime.opset4.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_logical_and.html">openvino.runtime.opset4.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_logical_or.html">openvino.runtime.opset4.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_max.html">openvino.runtime.opset4.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_mean.html">openvino.runtime.opset4.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_min.html">openvino.runtime.opset4.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_prod.html">openvino.runtime.opset4.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reduce_sum.html">openvino.runtime.opset4.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.region_yolo.html">openvino.runtime.opset4.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.relu.html">openvino.runtime.opset4.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reorg_yolo.html">openvino.runtime.opset4.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reshape.html">openvino.runtime.opset4.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.result.html">openvino.runtime.opset4.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.reverse_sequence.html">openvino.runtime.opset4.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.rnn_cell.html">openvino.runtime.opset4.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.roi_align.html">openvino.runtime.opset4.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.roi_pooling.html">openvino.runtime.opset4.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.scatter_elements_update.html">openvino.runtime.opset4.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.scatter_nd_update.html">openvino.runtime.opset4.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.scatter_update.html">openvino.runtime.opset4.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.select.html">openvino.runtime.opset4.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.selu.html">openvino.runtime.opset4.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.shape_of.html">openvino.runtime.opset4.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.shuffle_channels.html">openvino.runtime.opset4.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.sigmoid.html">openvino.runtime.opset4.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.sign.html">openvino.runtime.opset4.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.sin.html">openvino.runtime.opset4.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.sinh.html">openvino.runtime.opset4.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.softmax.html">openvino.runtime.opset4.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.softplus.html">openvino.runtime.opset4.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.space_to_batch.html">openvino.runtime.opset4.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.space_to_depth.html">openvino.runtime.opset4.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.split.html">openvino.runtime.opset4.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.sqrt.html">openvino.runtime.opset4.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.squared_difference.html">openvino.runtime.opset4.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.squeeze.html">openvino.runtime.opset4.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.strided_slice.html">openvino.runtime.opset4.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.subtract.html">openvino.runtime.opset4.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.swish.html">openvino.runtime.opset4.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.tan.html">openvino.runtime.opset4.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.tanh.html">openvino.runtime.opset4.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.tile.html">openvino.runtime.opset4.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.topk.html">openvino.runtime.opset4.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.transpose.html">openvino.runtime.opset4.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.unsqueeze.html">openvino.runtime.opset4.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.variadic_split.html">openvino.runtime.opset4.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset4.tensor_iterator.html">openvino.runtime.opset4.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.html">openvino.runtime.opset5</a><input class="toctree-checkbox" id="toctree-checkbox-55" name="toctree-checkbox-55" type="checkbox"/><label for="toctree-checkbox-55"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.abs.html">openvino.runtime.opset5.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.absolute.html">openvino.runtime.opset5.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.acos.html">openvino.runtime.opset5.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.acosh.html">openvino.runtime.opset5.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.add.html">openvino.runtime.opset5.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.asin.html">openvino.runtime.opset5.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.asinh.html">openvino.runtime.opset5.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.assign.html">openvino.runtime.opset5.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.atan.html">openvino.runtime.opset5.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.atanh.html">openvino.runtime.opset5.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.avg_pool.html">openvino.runtime.opset5.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.batch_norm_inference.html">openvino.runtime.opset5.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.batch_to_space.html">openvino.runtime.opset5.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.binary_convolution.html">openvino.runtime.opset5.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.broadcast.html">openvino.runtime.opset5.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.bucketize.html">openvino.runtime.opset5.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.ceil.html">openvino.runtime.opset5.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.ceiling.html">openvino.runtime.opset5.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.clamp.html">openvino.runtime.opset5.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.concat.html">openvino.runtime.opset5.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.constant.html">openvino.runtime.opset5.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.convert.html">openvino.runtime.opset5.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.convert_like.html">openvino.runtime.opset5.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.convolution.html">openvino.runtime.opset5.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.convolution_backprop_data.html">openvino.runtime.opset5.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.cos.html">openvino.runtime.opset5.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.cosh.html">openvino.runtime.opset5.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.ctc_greedy_decoder.html">openvino.runtime.opset5.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.ctc_loss.html">openvino.runtime.opset5.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.cum_sum.html">openvino.runtime.opset5.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.cumsum.html">openvino.runtime.opset5.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.deformable_convolution.html">openvino.runtime.opset5.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.deformable_psroi_pooling.html">openvino.runtime.opset5.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.depth_to_space.html">openvino.runtime.opset5.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.detection_output.html">openvino.runtime.opset5.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.divide.html">openvino.runtime.opset5.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.elu.html">openvino.runtime.opset5.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.embedding_bag_offsets_sum.html">openvino.runtime.opset5.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.embedding_bag_packed_sum.html">openvino.runtime.opset5.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.embedding_segments_sum.html">openvino.runtime.opset5.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.equal.html">openvino.runtime.opset5.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.erf.html">openvino.runtime.opset5.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.exp.html">openvino.runtime.opset5.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.extract_image_patches.html">openvino.runtime.opset5.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.fake_quantize.html">openvino.runtime.opset5.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.floor.html">openvino.runtime.opset5.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.floor_mod.html">openvino.runtime.opset5.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.gather.html">openvino.runtime.opset5.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.gather_nd.html">openvino.runtime.opset5.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.gather_tree.html">openvino.runtime.opset5.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.gelu.html">openvino.runtime.opset5.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.greater.html">openvino.runtime.opset5.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.greater_equal.html">openvino.runtime.opset5.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.grn.html">openvino.runtime.opset5.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.group_convolution.html">openvino.runtime.opset5.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.group_convolution_backprop_data.html">openvino.runtime.opset5.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.gru_cell.html">openvino.runtime.opset5.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.gru_sequence.html">openvino.runtime.opset5.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.hard_sigmoid.html">openvino.runtime.opset5.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.hsigmoid.html">openvino.runtime.opset5.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.hswish.html">openvino.runtime.opset5.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.interpolate.html">openvino.runtime.opset5.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.less.html">openvino.runtime.opset5.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.less_equal.html">openvino.runtime.opset5.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.log.html">openvino.runtime.opset5.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.log_softmax.html">openvino.runtime.opset5.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.logical_and.html">openvino.runtime.opset5.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.logical_not.html">openvino.runtime.opset5.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.logical_or.html">openvino.runtime.opset5.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.logical_xor.html">openvino.runtime.opset5.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.lrn.html">openvino.runtime.opset5.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.lstm_cell.html">openvino.runtime.opset5.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.lstm_sequence.html">openvino.runtime.opset5.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.matmul.html">openvino.runtime.opset5.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.max_pool.html">openvino.runtime.opset5.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.maximum.html">openvino.runtime.opset5.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.minimum.html">openvino.runtime.opset5.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.mish.html">openvino.runtime.opset5.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.mod.html">openvino.runtime.opset5.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.multiply.html">openvino.runtime.opset5.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.mvn.html">openvino.runtime.opset5.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.negative.html">openvino.runtime.opset5.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.non_max_suppression.html">openvino.runtime.opset5.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.non_zero.html">openvino.runtime.opset5.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.normalize_l2.html">openvino.runtime.opset5.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.not_equal.html">openvino.runtime.opset5.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.one_hot.html">openvino.runtime.opset5.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.pad.html">openvino.runtime.opset5.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.parameter.html">openvino.runtime.opset5.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.power.html">openvino.runtime.opset5.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.prelu.html">openvino.runtime.opset5.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.prior_box.html">openvino.runtime.opset5.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.prior_box_clustered.html">openvino.runtime.opset5.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.proposal.html">openvino.runtime.opset5.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.psroi_pooling.html">openvino.runtime.opset5.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.range.html">openvino.runtime.opset5.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.read_value.html">openvino.runtime.opset5.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_l1.html">openvino.runtime.opset5.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_l2.html">openvino.runtime.opset5.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_logical_and.html">openvino.runtime.opset5.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_logical_or.html">openvino.runtime.opset5.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_max.html">openvino.runtime.opset5.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_mean.html">openvino.runtime.opset5.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_min.html">openvino.runtime.opset5.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_prod.html">openvino.runtime.opset5.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reduce_sum.html">openvino.runtime.opset5.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.region_yolo.html">openvino.runtime.opset5.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.relu.html">openvino.runtime.opset5.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reorg_yolo.html">openvino.runtime.opset5.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reshape.html">openvino.runtime.opset5.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.result.html">openvino.runtime.opset5.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.reverse_sequence.html">openvino.runtime.opset5.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.rnn_cell.html">openvino.runtime.opset5.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.rnn_sequence.html">openvino.runtime.opset5.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.roi_align.html">openvino.runtime.opset5.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.roi_pooling.html">openvino.runtime.opset5.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.round.html">openvino.runtime.opset5.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.scatter_elements_update.html">openvino.runtime.opset5.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.scatter_nd_update.html">openvino.runtime.opset5.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.scatter_update.html">openvino.runtime.opset5.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.select.html">openvino.runtime.opset5.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.selu.html">openvino.runtime.opset5.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.shape_of.html">openvino.runtime.opset5.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.shuffle_channels.html">openvino.runtime.opset5.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.sigmoid.html">openvino.runtime.opset5.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.sign.html">openvino.runtime.opset5.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.sin.html">openvino.runtime.opset5.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.sinh.html">openvino.runtime.opset5.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.softmax.html">openvino.runtime.opset5.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.softplus.html">openvino.runtime.opset5.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.space_to_batch.html">openvino.runtime.opset5.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.space_to_depth.html">openvino.runtime.opset5.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.split.html">openvino.runtime.opset5.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.sqrt.html">openvino.runtime.opset5.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.squared_difference.html">openvino.runtime.opset5.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.squeeze.html">openvino.runtime.opset5.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.strided_slice.html">openvino.runtime.opset5.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.subtract.html">openvino.runtime.opset5.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.swish.html">openvino.runtime.opset5.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.tan.html">openvino.runtime.opset5.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.tanh.html">openvino.runtime.opset5.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.tile.html">openvino.runtime.opset5.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.topk.html">openvino.runtime.opset5.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.transpose.html">openvino.runtime.opset5.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.unsqueeze.html">openvino.runtime.opset5.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.variadic_split.html">openvino.runtime.opset5.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.loop.html">openvino.runtime.opset5.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset5.tensor_iterator.html">openvino.runtime.opset5.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.html">openvino.runtime.opset6</a><input class="toctree-checkbox" id="toctree-checkbox-56" name="toctree-checkbox-56" type="checkbox"/><label for="toctree-checkbox-56"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.abs.html">openvino.runtime.opset6.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.absolute.html">openvino.runtime.opset6.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.acos.html">openvino.runtime.opset6.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.acosh.html">openvino.runtime.opset6.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.add.html">openvino.runtime.opset6.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.asin.html">openvino.runtime.opset6.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.asinh.html">openvino.runtime.opset6.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.atan.html">openvino.runtime.opset6.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.atanh.html">openvino.runtime.opset6.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.avg_pool.html">openvino.runtime.opset6.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.batch_norm_inference.html">openvino.runtime.opset6.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.batch_to_space.html">openvino.runtime.opset6.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.binary_convolution.html">openvino.runtime.opset6.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.broadcast.html">openvino.runtime.opset6.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.bucketize.html">openvino.runtime.opset6.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.ceil.html">openvino.runtime.opset6.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.ceiling.html">openvino.runtime.opset6.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.clamp.html">openvino.runtime.opset6.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.concat.html">openvino.runtime.opset6.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.constant.html">openvino.runtime.opset6.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.convert.html">openvino.runtime.opset6.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.convert_like.html">openvino.runtime.opset6.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.convolution.html">openvino.runtime.opset6.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.convolution_backprop_data.html">openvino.runtime.opset6.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.cos.html">openvino.runtime.opset6.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.cosh.html">openvino.runtime.opset6.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.ctc_greedy_decoder.html">openvino.runtime.opset6.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset6.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.ctc_loss.html">openvino.runtime.opset6.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.cum_sum.html">openvino.runtime.opset6.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.cumsum.html">openvino.runtime.opset6.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.deformable_convolution.html">openvino.runtime.opset6.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.deformable_psroi_pooling.html">openvino.runtime.opset6.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.depth_to_space.html">openvino.runtime.opset6.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.detection_output.html">openvino.runtime.opset6.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.divide.html">openvino.runtime.opset6.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.elu.html">openvino.runtime.opset6.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.embedding_bag_offsets_sum.html">openvino.runtime.opset6.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.embedding_bag_packed_sum.html">openvino.runtime.opset6.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.embedding_segments_sum.html">openvino.runtime.opset6.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.equal.html">openvino.runtime.opset6.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.erf.html">openvino.runtime.opset6.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.exp.html">openvino.runtime.opset6.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.extract_image_patches.html">openvino.runtime.opset6.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.fake_quantize.html">openvino.runtime.opset6.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.floor.html">openvino.runtime.opset6.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.floor_mod.html">openvino.runtime.opset6.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.gather.html">openvino.runtime.opset6.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.gather_elements.html">openvino.runtime.opset6.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.gather_nd.html">openvino.runtime.opset6.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.gather_tree.html">openvino.runtime.opset6.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.gelu.html">openvino.runtime.opset6.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.greater.html">openvino.runtime.opset6.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.greater_equal.html">openvino.runtime.opset6.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.grn.html">openvino.runtime.opset6.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.group_convolution.html">openvino.runtime.opset6.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.group_convolution_backprop_data.html">openvino.runtime.opset6.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.gru_cell.html">openvino.runtime.opset6.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.gru_sequence.html">openvino.runtime.opset6.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.hard_sigmoid.html">openvino.runtime.opset6.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.hsigmoid.html">openvino.runtime.opset6.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.hswish.html">openvino.runtime.opset6.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.interpolate.html">openvino.runtime.opset6.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.less.html">openvino.runtime.opset6.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.less_equal.html">openvino.runtime.opset6.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.log.html">openvino.runtime.opset6.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.log_softmax.html">openvino.runtime.opset6.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.logical_and.html">openvino.runtime.opset6.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.logical_not.html">openvino.runtime.opset6.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.logical_or.html">openvino.runtime.opset6.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.logical_xor.html">openvino.runtime.opset6.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.lrn.html">openvino.runtime.opset6.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.lstm_cell.html">openvino.runtime.opset6.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.lstm_sequence.html">openvino.runtime.opset6.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.matmul.html">openvino.runtime.opset6.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.max_pool.html">openvino.runtime.opset6.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.maximum.html">openvino.runtime.opset6.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.minimum.html">openvino.runtime.opset6.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.mish.html">openvino.runtime.opset6.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.mod.html">openvino.runtime.opset6.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.multiply.html">openvino.runtime.opset6.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.mvn.html">openvino.runtime.opset6.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.negative.html">openvino.runtime.opset6.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.non_max_suppression.html">openvino.runtime.opset6.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.non_zero.html">openvino.runtime.opset6.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.normalize_l2.html">openvino.runtime.opset6.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.not_equal.html">openvino.runtime.opset6.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.one_hot.html">openvino.runtime.opset6.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.pad.html">openvino.runtime.opset6.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.parameter.html">openvino.runtime.opset6.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.power.html">openvino.runtime.opset6.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.prelu.html">openvino.runtime.opset6.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.prior_box.html">openvino.runtime.opset6.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.prior_box_clustered.html">openvino.runtime.opset6.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.proposal.html">openvino.runtime.opset6.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.psroi_pooling.html">openvino.runtime.opset6.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.range.html">openvino.runtime.opset6.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.read_value.html">openvino.runtime.opset6.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_l1.html">openvino.runtime.opset6.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_l2.html">openvino.runtime.opset6.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_logical_and.html">openvino.runtime.opset6.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_logical_or.html">openvino.runtime.opset6.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_max.html">openvino.runtime.opset6.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_mean.html">openvino.runtime.opset6.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_min.html">openvino.runtime.opset6.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_prod.html">openvino.runtime.opset6.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reduce_sum.html">openvino.runtime.opset6.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.region_yolo.html">openvino.runtime.opset6.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.relu.html">openvino.runtime.opset6.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reorg_yolo.html">openvino.runtime.opset6.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reshape.html">openvino.runtime.opset6.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.result.html">openvino.runtime.opset6.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.reverse_sequence.html">openvino.runtime.opset6.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.rnn_cell.html">openvino.runtime.opset6.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.rnn_sequence.html">openvino.runtime.opset6.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.roi_align.html">openvino.runtime.opset6.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.roi_pooling.html">openvino.runtime.opset6.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.round.html">openvino.runtime.opset6.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.scatter_elements_update.html">openvino.runtime.opset6.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.scatter_nd_update.html">openvino.runtime.opset6.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.scatter_update.html">openvino.runtime.opset6.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.select.html">openvino.runtime.opset6.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.selu.html">openvino.runtime.opset6.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.shape_of.html">openvino.runtime.opset6.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.shuffle_channels.html">openvino.runtime.opset6.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.sigmoid.html">openvino.runtime.opset6.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.sign.html">openvino.runtime.opset6.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.sin.html">openvino.runtime.opset6.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.sinh.html">openvino.runtime.opset6.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.softmax.html">openvino.runtime.opset6.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.softplus.html">openvino.runtime.opset6.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.space_to_batch.html">openvino.runtime.opset6.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.space_to_depth.html">openvino.runtime.opset6.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.split.html">openvino.runtime.opset6.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.sqrt.html">openvino.runtime.opset6.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.squared_difference.html">openvino.runtime.opset6.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.squeeze.html">openvino.runtime.opset6.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.strided_slice.html">openvino.runtime.opset6.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.subtract.html">openvino.runtime.opset6.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.swish.html">openvino.runtime.opset6.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.tan.html">openvino.runtime.opset6.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.tanh.html">openvino.runtime.opset6.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.tile.html">openvino.runtime.opset6.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.topk.html">openvino.runtime.opset6.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.transpose.html">openvino.runtime.opset6.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.unsqueeze.html">openvino.runtime.opset6.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.variadic_split.html">openvino.runtime.opset6.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.assign.html">openvino.runtime.opset6.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.loop.html">openvino.runtime.opset6.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset6.tensor_iterator.html">openvino.runtime.opset6.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.html">openvino.runtime.opset7</a><input class="toctree-checkbox" id="toctree-checkbox-57" name="toctree-checkbox-57" type="checkbox"/><label for="toctree-checkbox-57"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.abs.html">openvino.runtime.opset7.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.absolute.html">openvino.runtime.opset7.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.acos.html">openvino.runtime.opset7.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.acosh.html">openvino.runtime.opset7.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.add.html">openvino.runtime.opset7.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.asin.html">openvino.runtime.opset7.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.asinh.html">openvino.runtime.opset7.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.atan.html">openvino.runtime.opset7.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.atanh.html">openvino.runtime.opset7.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.avg_pool.html">openvino.runtime.opset7.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.batch_norm_inference.html">openvino.runtime.opset7.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.batch_to_space.html">openvino.runtime.opset7.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.binary_convolution.html">openvino.runtime.opset7.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.broadcast.html">openvino.runtime.opset7.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.bucketize.html">openvino.runtime.opset7.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.ceil.html">openvino.runtime.opset7.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.ceiling.html">openvino.runtime.opset7.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.clamp.html">openvino.runtime.opset7.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.concat.html">openvino.runtime.opset7.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.constant.html">openvino.runtime.opset7.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.convert.html">openvino.runtime.opset7.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.convert_like.html">openvino.runtime.opset7.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.convolution.html">openvino.runtime.opset7.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.convolution_backprop_data.html">openvino.runtime.opset7.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.cos.html">openvino.runtime.opset7.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.cosh.html">openvino.runtime.opset7.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.ctc_greedy_decoder.html">openvino.runtime.opset7.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset7.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.ctc_loss.html">openvino.runtime.opset7.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.cum_sum.html">openvino.runtime.opset7.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.cumsum.html">openvino.runtime.opset7.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.deformable_convolution.html">openvino.runtime.opset7.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.deformable_psroi_pooling.html">openvino.runtime.opset7.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.depth_to_space.html">openvino.runtime.opset7.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.detection_output.html">openvino.runtime.opset7.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.dft.html">openvino.runtime.opset7.dft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.divide.html">openvino.runtime.opset7.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.einsum.html">openvino.runtime.opset7.einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.elu.html">openvino.runtime.opset7.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.embedding_bag_offsets_sum.html">openvino.runtime.opset7.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.embedding_bag_packed_sum.html">openvino.runtime.opset7.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.embedding_segments_sum.html">openvino.runtime.opset7.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.equal.html">openvino.runtime.opset7.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.erf.html">openvino.runtime.opset7.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.exp.html">openvino.runtime.opset7.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.extract_image_patches.html">openvino.runtime.opset7.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.fake_quantize.html">openvino.runtime.opset7.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.floor.html">openvino.runtime.opset7.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.floor_mod.html">openvino.runtime.opset7.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.gather.html">openvino.runtime.opset7.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.gather_elements.html">openvino.runtime.opset7.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.gather_nd.html">openvino.runtime.opset7.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.gather_tree.html">openvino.runtime.opset7.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.gelu.html">openvino.runtime.opset7.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.greater.html">openvino.runtime.opset7.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.greater_equal.html">openvino.runtime.opset7.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.grn.html">openvino.runtime.opset7.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.group_convolution.html">openvino.runtime.opset7.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.group_convolution_backprop_data.html">openvino.runtime.opset7.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.gru_cell.html">openvino.runtime.opset7.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.gru_sequence.html">openvino.runtime.opset7.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.hard_sigmoid.html">openvino.runtime.opset7.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.hsigmoid.html">openvino.runtime.opset7.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.hswish.html">openvino.runtime.opset7.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.idft.html">openvino.runtime.opset7.idft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.interpolate.html">openvino.runtime.opset7.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.less.html">openvino.runtime.opset7.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.less_equal.html">openvino.runtime.opset7.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.log.html">openvino.runtime.opset7.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.log_softmax.html">openvino.runtime.opset7.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.logical_and.html">openvino.runtime.opset7.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.logical_not.html">openvino.runtime.opset7.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.logical_or.html">openvino.runtime.opset7.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.logical_xor.html">openvino.runtime.opset7.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.lrn.html">openvino.runtime.opset7.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.lstm_cell.html">openvino.runtime.opset7.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.lstm_sequence.html">openvino.runtime.opset7.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.matmul.html">openvino.runtime.opset7.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.max_pool.html">openvino.runtime.opset7.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.maximum.html">openvino.runtime.opset7.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.minimum.html">openvino.runtime.opset7.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.mish.html">openvino.runtime.opset7.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.mod.html">openvino.runtime.opset7.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.multiply.html">openvino.runtime.opset7.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.mvn.html">openvino.runtime.opset7.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.negative.html">openvino.runtime.opset7.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.non_max_suppression.html">openvino.runtime.opset7.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.non_zero.html">openvino.runtime.opset7.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.normalize_l2.html">openvino.runtime.opset7.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.not_equal.html">openvino.runtime.opset7.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.one_hot.html">openvino.runtime.opset7.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.pad.html">openvino.runtime.opset7.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.parameter.html">openvino.runtime.opset7.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.power.html">openvino.runtime.opset7.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.prelu.html">openvino.runtime.opset7.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.prior_box.html">openvino.runtime.opset7.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.prior_box_clustered.html">openvino.runtime.opset7.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.proposal.html">openvino.runtime.opset7.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.psroi_pooling.html">openvino.runtime.opset7.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.range.html">openvino.runtime.opset7.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.read_value.html">openvino.runtime.opset7.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_l1.html">openvino.runtime.opset7.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_l2.html">openvino.runtime.opset7.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_logical_and.html">openvino.runtime.opset7.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_logical_or.html">openvino.runtime.opset7.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_max.html">openvino.runtime.opset7.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_mean.html">openvino.runtime.opset7.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_min.html">openvino.runtime.opset7.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_prod.html">openvino.runtime.opset7.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reduce_sum.html">openvino.runtime.opset7.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.region_yolo.html">openvino.runtime.opset7.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.relu.html">openvino.runtime.opset7.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reorg_yolo.html">openvino.runtime.opset7.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reshape.html">openvino.runtime.opset7.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.result.html">openvino.runtime.opset7.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.reverse_sequence.html">openvino.runtime.opset7.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.rnn_cell.html">openvino.runtime.opset7.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.rnn_sequence.html">openvino.runtime.opset7.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.roi_align.html">openvino.runtime.opset7.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.roi_pooling.html">openvino.runtime.opset7.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.roll.html">openvino.runtime.opset7.roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.round.html">openvino.runtime.opset7.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.scatter_elements_update.html">openvino.runtime.opset7.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.scatter_nd_update.html">openvino.runtime.opset7.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.scatter_update.html">openvino.runtime.opset7.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.select.html">openvino.runtime.opset7.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.selu.html">openvino.runtime.opset7.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.shape_of.html">openvino.runtime.opset7.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.shuffle_channels.html">openvino.runtime.opset7.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.sigmoid.html">openvino.runtime.opset7.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.sign.html">openvino.runtime.opset7.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.sin.html">openvino.runtime.opset7.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.sinh.html">openvino.runtime.opset7.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.softmax.html">openvino.runtime.opset7.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.softplus.html">openvino.runtime.opset7.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.space_to_batch.html">openvino.runtime.opset7.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.space_to_depth.html">openvino.runtime.opset7.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.split.html">openvino.runtime.opset7.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.sqrt.html">openvino.runtime.opset7.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.squared_difference.html">openvino.runtime.opset7.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.squeeze.html">openvino.runtime.opset7.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.strided_slice.html">openvino.runtime.opset7.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.subtract.html">openvino.runtime.opset7.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.swish.html">openvino.runtime.opset7.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.tan.html">openvino.runtime.opset7.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.tanh.html">openvino.runtime.opset7.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.tile.html">openvino.runtime.opset7.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.topk.html">openvino.runtime.opset7.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.transpose.html">openvino.runtime.opset7.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.unsqueeze.html">openvino.runtime.opset7.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.variadic_split.html">openvino.runtime.opset7.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.assign.html">openvino.runtime.opset7.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.loop.html">openvino.runtime.opset7.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset7.tensor_iterator.html">openvino.runtime.opset7.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.html">openvino.runtime.opset8</a><input class="toctree-checkbox" id="toctree-checkbox-58" name="toctree-checkbox-58" type="checkbox"/><label for="toctree-checkbox-58"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.abs.html">openvino.runtime.opset8.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.absolute.html">openvino.runtime.opset8.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.acos.html">openvino.runtime.opset8.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.acosh.html">openvino.runtime.opset8.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.adaptive_avg_pool.html">openvino.runtime.opset8.adaptive_avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.adaptive_max_pool.html">openvino.runtime.opset8.adaptive_max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.add.html">openvino.runtime.opset8.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.asin.html">openvino.runtime.opset8.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.asinh.html">openvino.runtime.opset8.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.atan.html">openvino.runtime.opset8.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.atanh.html">openvino.runtime.opset8.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.avg_pool.html">openvino.runtime.opset8.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.batch_norm_inference.html">openvino.runtime.opset8.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.batch_to_space.html">openvino.runtime.opset8.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.binary_convolution.html">openvino.runtime.opset8.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.broadcast.html">openvino.runtime.opset8.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.bucketize.html">openvino.runtime.opset8.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.ceil.html">openvino.runtime.opset8.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.ceiling.html">openvino.runtime.opset8.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.clamp.html">openvino.runtime.opset8.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.concat.html">openvino.runtime.opset8.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.constant.html">openvino.runtime.opset8.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.convert.html">openvino.runtime.opset8.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.convert_like.html">openvino.runtime.opset8.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.convolution.html">openvino.runtime.opset8.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.convolution_backprop_data.html">openvino.runtime.opset8.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.cos.html">openvino.runtime.opset8.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.cosh.html">openvino.runtime.opset8.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.ctc_greedy_decoder.html">openvino.runtime.opset8.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset8.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.ctc_loss.html">openvino.runtime.opset8.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.cum_sum.html">openvino.runtime.opset8.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.cumsum.html">openvino.runtime.opset8.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.deformable_convolution.html">openvino.runtime.opset8.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.deformable_psroi_pooling.html">openvino.runtime.opset8.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.depth_to_space.html">openvino.runtime.opset8.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.detection_output.html">openvino.runtime.opset8.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.dft.html">openvino.runtime.opset8.dft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.divide.html">openvino.runtime.opset8.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.einsum.html">openvino.runtime.opset8.einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.elu.html">openvino.runtime.opset8.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.embedding_bag_offsets_sum.html">openvino.runtime.opset8.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.embedding_bag_packed_sum.html">openvino.runtime.opset8.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.embedding_segments_sum.html">openvino.runtime.opset8.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.equal.html">openvino.runtime.opset8.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.erf.html">openvino.runtime.opset8.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.exp.html">openvino.runtime.opset8.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.extract_image_patches.html">openvino.runtime.opset8.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.fake_quantize.html">openvino.runtime.opset8.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.floor.html">openvino.runtime.opset8.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.floor_mod.html">openvino.runtime.opset8.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.gather.html">openvino.runtime.opset8.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.gather_elements.html">openvino.runtime.opset8.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.gather_nd.html">openvino.runtime.opset8.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.gather_tree.html">openvino.runtime.opset8.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.gelu.html">openvino.runtime.opset8.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.greater.html">openvino.runtime.opset8.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.greater_equal.html">openvino.runtime.opset8.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.grn.html">openvino.runtime.opset8.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.group_convolution.html">openvino.runtime.opset8.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.group_convolution_backprop_data.html">openvino.runtime.opset8.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.gru_cell.html">openvino.runtime.opset8.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.gru_sequence.html">openvino.runtime.opset8.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.hard_sigmoid.html">openvino.runtime.opset8.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.hsigmoid.html">openvino.runtime.opset8.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.hswish.html">openvino.runtime.opset8.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.i420_to_bgr.html">openvino.runtime.opset8.i420_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.i420_to_rgb.html">openvino.runtime.opset8.i420_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.idft.html">openvino.runtime.opset8.idft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.interpolate.html">openvino.runtime.opset8.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.less.html">openvino.runtime.opset8.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.less_equal.html">openvino.runtime.opset8.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.log.html">openvino.runtime.opset8.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.log_softmax.html">openvino.runtime.opset8.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.logical_and.html">openvino.runtime.opset8.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.logical_not.html">openvino.runtime.opset8.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.logical_or.html">openvino.runtime.opset8.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.logical_xor.html">openvino.runtime.opset8.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.lrn.html">openvino.runtime.opset8.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.lstm_cell.html">openvino.runtime.opset8.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.lstm_sequence.html">openvino.runtime.opset8.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.matmul.html">openvino.runtime.opset8.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.matrix_nms.html">openvino.runtime.opset8.matrix_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.max_pool.html">openvino.runtime.opset8.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.maximum.html">openvino.runtime.opset8.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.minimum.html">openvino.runtime.opset8.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.mish.html">openvino.runtime.opset8.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.mod.html">openvino.runtime.opset8.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.multiclass_nms.html">openvino.runtime.opset8.multiclass_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.multiply.html">openvino.runtime.opset8.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.mvn.html">openvino.runtime.opset8.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.negative.html">openvino.runtime.opset8.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.non_max_suppression.html">openvino.runtime.opset8.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.non_zero.html">openvino.runtime.opset8.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.normalize_l2.html">openvino.runtime.opset8.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.not_equal.html">openvino.runtime.opset8.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.nv12_to_bgr.html">openvino.runtime.opset8.nv12_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.nv12_to_rgb.html">openvino.runtime.opset8.nv12_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.one_hot.html">openvino.runtime.opset8.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.pad.html">openvino.runtime.opset8.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.parameter.html">openvino.runtime.opset8.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.power.html">openvino.runtime.opset8.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.prelu.html">openvino.runtime.opset8.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.prior_box.html">openvino.runtime.opset8.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.prior_box_clustered.html">openvino.runtime.opset8.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.proposal.html">openvino.runtime.opset8.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.psroi_pooling.html">openvino.runtime.opset8.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.random_uniform.html">openvino.runtime.opset8.random_uniform</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.range.html">openvino.runtime.opset8.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.read_value.html">openvino.runtime.opset8.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_l1.html">openvino.runtime.opset8.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_l2.html">openvino.runtime.opset8.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_logical_and.html">openvino.runtime.opset8.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_logical_or.html">openvino.runtime.opset8.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_max.html">openvino.runtime.opset8.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_mean.html">openvino.runtime.opset8.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_min.html">openvino.runtime.opset8.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_prod.html">openvino.runtime.opset8.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reduce_sum.html">openvino.runtime.opset8.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.region_yolo.html">openvino.runtime.opset8.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.relu.html">openvino.runtime.opset8.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reorg_yolo.html">openvino.runtime.opset8.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reshape.html">openvino.runtime.opset8.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.result.html">openvino.runtime.opset8.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.reverse_sequence.html">openvino.runtime.opset8.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.rnn_cell.html">openvino.runtime.opset8.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.rnn_sequence.html">openvino.runtime.opset8.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.roi_align.html">openvino.runtime.opset8.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.roi_pooling.html">openvino.runtime.opset8.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.roll.html">openvino.runtime.opset8.roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.round.html">openvino.runtime.opset8.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.scatter_elements_update.html">openvino.runtime.opset8.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.scatter_nd_update.html">openvino.runtime.opset8.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.scatter_update.html">openvino.runtime.opset8.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.select.html">openvino.runtime.opset8.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.selu.html">openvino.runtime.opset8.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.shape_of.html">openvino.runtime.opset8.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.shuffle_channels.html">openvino.runtime.opset8.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.sigmoid.html">openvino.runtime.opset8.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.sign.html">openvino.runtime.opset8.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.sin.html">openvino.runtime.opset8.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.sinh.html">openvino.runtime.opset8.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.slice.html">openvino.runtime.opset8.slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.softmax.html">openvino.runtime.opset8.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.softplus.html">openvino.runtime.opset8.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.space_to_batch.html">openvino.runtime.opset8.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.space_to_depth.html">openvino.runtime.opset8.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.split.html">openvino.runtime.opset8.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.sqrt.html">openvino.runtime.opset8.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.squared_difference.html">openvino.runtime.opset8.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.squeeze.html">openvino.runtime.opset8.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.strided_slice.html">openvino.runtime.opset8.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.subtract.html">openvino.runtime.opset8.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.swish.html">openvino.runtime.opset8.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.tan.html">openvino.runtime.opset8.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.tanh.html">openvino.runtime.opset8.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.tile.html">openvino.runtime.opset8.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.topk.html">openvino.runtime.opset8.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.transpose.html">openvino.runtime.opset8.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.unsqueeze.html">openvino.runtime.opset8.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.variadic_split.html">openvino.runtime.opset8.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.assign.html">openvino.runtime.opset8.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.if_op.html">openvino.runtime.opset8.if_op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.loop.html">openvino.runtime.opset8.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset8.tensor_iterator.html">openvino.runtime.opset8.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.html">openvino.runtime.opset9</a><input class="toctree-checkbox" id="toctree-checkbox-59" name="toctree-checkbox-59" type="checkbox"/><label for="toctree-checkbox-59"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.abs.html">openvino.runtime.opset9.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.absolute.html">openvino.runtime.opset9.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.acos.html">openvino.runtime.opset9.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.acosh.html">openvino.runtime.opset9.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.adaptive_avg_pool.html">openvino.runtime.opset9.adaptive_avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.adaptive_max_pool.html">openvino.runtime.opset9.adaptive_max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.add.html">openvino.runtime.opset9.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.asin.html">openvino.runtime.opset9.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.asinh.html">openvino.runtime.opset9.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.atan.html">openvino.runtime.opset9.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.atanh.html">openvino.runtime.opset9.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.avg_pool.html">openvino.runtime.opset9.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.batch_norm_inference.html">openvino.runtime.opset9.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.batch_to_space.html">openvino.runtime.opset9.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.binary_convolution.html">openvino.runtime.opset9.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.broadcast.html">openvino.runtime.opset9.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.bucketize.html">openvino.runtime.opset9.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.ceil.html">openvino.runtime.opset9.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.ceiling.html">openvino.runtime.opset9.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.clamp.html">openvino.runtime.opset9.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.concat.html">openvino.runtime.opset9.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.constant.html">openvino.runtime.opset9.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.convert.html">openvino.runtime.opset9.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.convert_like.html">openvino.runtime.opset9.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.convolution.html">openvino.runtime.opset9.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.convolution_backprop_data.html">openvino.runtime.opset9.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.cos.html">openvino.runtime.opset9.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.cosh.html">openvino.runtime.opset9.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.ctc_greedy_decoder.html">openvino.runtime.opset9.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset9.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.ctc_loss.html">openvino.runtime.opset9.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.cum_sum.html">openvino.runtime.opset9.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.cumsum.html">openvino.runtime.opset9.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.deformable_convolution.html">openvino.runtime.opset9.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.deformable_psroi_pooling.html">openvino.runtime.opset9.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.depth_to_space.html">openvino.runtime.opset9.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.detection_output.html">openvino.runtime.opset9.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.dft.html">openvino.runtime.opset9.dft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.divide.html">openvino.runtime.opset9.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.einsum.html">openvino.runtime.opset9.einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.elu.html">openvino.runtime.opset9.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.embedding_bag_offsets_sum.html">openvino.runtime.opset9.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.embedding_bag_packed_sum.html">openvino.runtime.opset9.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.embedding_segments_sum.html">openvino.runtime.opset9.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.equal.html">openvino.runtime.opset9.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.erf.html">openvino.runtime.opset9.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.exp.html">openvino.runtime.opset9.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.extract_image_patches.html">openvino.runtime.opset9.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.eye.html">openvino.runtime.opset9.eye</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.fake_quantize.html">openvino.runtime.opset9.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.floor.html">openvino.runtime.opset9.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.floor_mod.html">openvino.runtime.opset9.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.gather.html">openvino.runtime.opset9.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.gather_elements.html">openvino.runtime.opset9.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.gather_nd.html">openvino.runtime.opset9.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.gather_tree.html">openvino.runtime.opset9.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.gelu.html">openvino.runtime.opset9.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.generate_proposals.html">openvino.runtime.opset9.generate_proposals</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.greater.html">openvino.runtime.opset9.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.greater_equal.html">openvino.runtime.opset9.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.grid_sample.html">openvino.runtime.opset9.grid_sample</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.grn.html">openvino.runtime.opset9.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.group_convolution.html">openvino.runtime.opset9.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.group_convolution_backprop_data.html">openvino.runtime.opset9.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.gru_cell.html">openvino.runtime.opset9.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.gru_sequence.html">openvino.runtime.opset9.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.hard_sigmoid.html">openvino.runtime.opset9.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.hsigmoid.html">openvino.runtime.opset9.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.hswish.html">openvino.runtime.opset9.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.i420_to_bgr.html">openvino.runtime.opset9.i420_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.i420_to_rgb.html">openvino.runtime.opset9.i420_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.idft.html">openvino.runtime.opset9.idft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.interpolate.html">openvino.runtime.opset9.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.irdft.html">openvino.runtime.opset9.irdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.less.html">openvino.runtime.opset9.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.less_equal.html">openvino.runtime.opset9.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.log.html">openvino.runtime.opset9.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.log_softmax.html">openvino.runtime.opset9.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.logical_and.html">openvino.runtime.opset9.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.logical_not.html">openvino.runtime.opset9.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.logical_or.html">openvino.runtime.opset9.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.logical_xor.html">openvino.runtime.opset9.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.lrn.html">openvino.runtime.opset9.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.lstm_cell.html">openvino.runtime.opset9.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.lstm_sequence.html">openvino.runtime.opset9.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.matmul.html">openvino.runtime.opset9.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.matrix_nms.html">openvino.runtime.opset9.matrix_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.max_pool.html">openvino.runtime.opset9.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.maximum.html">openvino.runtime.opset9.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.minimum.html">openvino.runtime.opset9.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.mish.html">openvino.runtime.opset9.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.mod.html">openvino.runtime.opset9.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.multiclass_nms.html">openvino.runtime.opset9.multiclass_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.multiply.html">openvino.runtime.opset9.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.mvn.html">openvino.runtime.opset9.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.negative.html">openvino.runtime.opset9.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.non_max_suppression.html">openvino.runtime.opset9.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.non_zero.html">openvino.runtime.opset9.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.normalize_l2.html">openvino.runtime.opset9.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.not_equal.html">openvino.runtime.opset9.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.nv12_to_bgr.html">openvino.runtime.opset9.nv12_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.nv12_to_rgb.html">openvino.runtime.opset9.nv12_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.one_hot.html">openvino.runtime.opset9.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.pad.html">openvino.runtime.opset9.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.parameter.html">openvino.runtime.opset9.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.power.html">openvino.runtime.opset9.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.prelu.html">openvino.runtime.opset9.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.prior_box.html">openvino.runtime.opset9.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.prior_box_clustered.html">openvino.runtime.opset9.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.proposal.html">openvino.runtime.opset9.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.psroi_pooling.html">openvino.runtime.opset9.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.random_uniform.html">openvino.runtime.opset9.random_uniform</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.range.html">openvino.runtime.opset9.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.rdft.html">openvino.runtime.opset9.rdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.read_value.html">openvino.runtime.opset9.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_l1.html">openvino.runtime.opset9.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_l2.html">openvino.runtime.opset9.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_logical_and.html">openvino.runtime.opset9.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_logical_or.html">openvino.runtime.opset9.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_max.html">openvino.runtime.opset9.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_mean.html">openvino.runtime.opset9.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_min.html">openvino.runtime.opset9.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_prod.html">openvino.runtime.opset9.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reduce_sum.html">openvino.runtime.opset9.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.region_yolo.html">openvino.runtime.opset9.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.relu.html">openvino.runtime.opset9.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reorg_yolo.html">openvino.runtime.opset9.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reshape.html">openvino.runtime.opset9.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.result.html">openvino.runtime.opset9.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.reverse_sequence.html">openvino.runtime.opset9.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.rnn_cell.html">openvino.runtime.opset9.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.rnn_sequence.html">openvino.runtime.opset9.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.roi_align.html">openvino.runtime.opset9.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.roi_pooling.html">openvino.runtime.opset9.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.roll.html">openvino.runtime.opset9.roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.round.html">openvino.runtime.opset9.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.scatter_elements_update.html">openvino.runtime.opset9.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.scatter_nd_update.html">openvino.runtime.opset9.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.scatter_update.html">openvino.runtime.opset9.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.select.html">openvino.runtime.opset9.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.selu.html">openvino.runtime.opset9.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.shape_of.html">openvino.runtime.opset9.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.shuffle_channels.html">openvino.runtime.opset9.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.sigmoid.html">openvino.runtime.opset9.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.sign.html">openvino.runtime.opset9.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.sin.html">openvino.runtime.opset9.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.sinh.html">openvino.runtime.opset9.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.slice.html">openvino.runtime.opset9.slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.softmax.html">openvino.runtime.opset9.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.softplus.html">openvino.runtime.opset9.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.softsign.html">openvino.runtime.opset9.softsign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.space_to_batch.html">openvino.runtime.opset9.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.space_to_depth.html">openvino.runtime.opset9.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.split.html">openvino.runtime.opset9.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.sqrt.html">openvino.runtime.opset9.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.squared_difference.html">openvino.runtime.opset9.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.squeeze.html">openvino.runtime.opset9.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.strided_slice.html">openvino.runtime.opset9.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.subtract.html">openvino.runtime.opset9.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.swish.html">openvino.runtime.opset9.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.tan.html">openvino.runtime.opset9.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.tanh.html">openvino.runtime.opset9.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.tile.html">openvino.runtime.opset9.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.topk.html">openvino.runtime.opset9.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.transpose.html">openvino.runtime.opset9.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.unsqueeze.html">openvino.runtime.opset9.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.variadic_split.html">openvino.runtime.opset9.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.assign.html">openvino.runtime.opset9.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.if_op.html">openvino.runtime.opset9.if_op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.loop.html">openvino.runtime.opset9.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset9.tensor_iterator.html">openvino.runtime.opset9.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.html">openvino.runtime.opset10</a><input class="toctree-checkbox" id="toctree-checkbox-60" name="toctree-checkbox-60" type="checkbox"/><label for="toctree-checkbox-60"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.abs.html">openvino.runtime.opset10.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.absolute.html">openvino.runtime.opset10.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.acos.html">openvino.runtime.opset10.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.acosh.html">openvino.runtime.opset10.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.adaptive_avg_pool.html">openvino.runtime.opset10.adaptive_avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.adaptive_max_pool.html">openvino.runtime.opset10.adaptive_max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.add.html">openvino.runtime.opset10.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.asin.html">openvino.runtime.opset10.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.asinh.html">openvino.runtime.opset10.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.atan.html">openvino.runtime.opset10.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.atanh.html">openvino.runtime.opset10.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.avg_pool.html">openvino.runtime.opset10.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.batch_norm_inference.html">openvino.runtime.opset10.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.batch_to_space.html">openvino.runtime.opset10.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.binary_convolution.html">openvino.runtime.opset10.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.broadcast.html">openvino.runtime.opset10.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.bucketize.html">openvino.runtime.opset10.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.ceil.html">openvino.runtime.opset10.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.ceiling.html">openvino.runtime.opset10.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.clamp.html">openvino.runtime.opset10.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.concat.html">openvino.runtime.opset10.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.constant.html">openvino.runtime.opset10.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.convert.html">openvino.runtime.opset10.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.convert_like.html">openvino.runtime.opset10.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.convolution.html">openvino.runtime.opset10.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.convolution_backprop_data.html">openvino.runtime.opset10.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.cos.html">openvino.runtime.opset10.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.cosh.html">openvino.runtime.opset10.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.ctc_greedy_decoder.html">openvino.runtime.opset10.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset10.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.ctc_loss.html">openvino.runtime.opset10.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.cum_sum.html">openvino.runtime.opset10.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.cumsum.html">openvino.runtime.opset10.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.deformable_convolution.html">openvino.runtime.opset10.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.deformable_psroi_pooling.html">openvino.runtime.opset10.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.depth_to_space.html">openvino.runtime.opset10.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.detection_output.html">openvino.runtime.opset10.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.dft.html">openvino.runtime.opset10.dft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.divide.html">openvino.runtime.opset10.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.einsum.html">openvino.runtime.opset10.einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.elu.html">openvino.runtime.opset10.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.embedding_bag_offsets_sum.html">openvino.runtime.opset10.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.embedding_bag_packed_sum.html">openvino.runtime.opset10.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.embedding_segments_sum.html">openvino.runtime.opset10.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.equal.html">openvino.runtime.opset10.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.erf.html">openvino.runtime.opset10.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.exp.html">openvino.runtime.opset10.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.extract_image_patches.html">openvino.runtime.opset10.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.eye.html">openvino.runtime.opset10.eye</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.fake_quantize.html">openvino.runtime.opset10.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.floor.html">openvino.runtime.opset10.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.floor_mod.html">openvino.runtime.opset10.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.gather.html">openvino.runtime.opset10.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.gather_elements.html">openvino.runtime.opset10.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.gather_nd.html">openvino.runtime.opset10.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.gather_tree.html">openvino.runtime.opset10.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.gelu.html">openvino.runtime.opset10.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.generate_proposals.html">openvino.runtime.opset10.generate_proposals</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.greater.html">openvino.runtime.opset10.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.greater_equal.html">openvino.runtime.opset10.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.grid_sample.html">openvino.runtime.opset10.grid_sample</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.grn.html">openvino.runtime.opset10.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.group_convolution.html">openvino.runtime.opset10.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.group_convolution_backprop_data.html">openvino.runtime.opset10.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.gru_cell.html">openvino.runtime.opset10.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.gru_sequence.html">openvino.runtime.opset10.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.hard_sigmoid.html">openvino.runtime.opset10.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.hsigmoid.html">openvino.runtime.opset10.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.hswish.html">openvino.runtime.opset10.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.i420_to_bgr.html">openvino.runtime.opset10.i420_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.i420_to_rgb.html">openvino.runtime.opset10.i420_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.idft.html">openvino.runtime.opset10.idft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.interpolate.html">openvino.runtime.opset10.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.irdft.html">openvino.runtime.opset10.irdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.is_finite.html">openvino.runtime.opset10.is_finite</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.is_inf.html">openvino.runtime.opset10.is_inf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.is_nan.html">openvino.runtime.opset10.is_nan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.less.html">openvino.runtime.opset10.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.less_equal.html">openvino.runtime.opset10.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.log.html">openvino.runtime.opset10.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.log_softmax.html">openvino.runtime.opset10.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.logical_and.html">openvino.runtime.opset10.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.logical_not.html">openvino.runtime.opset10.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.logical_or.html">openvino.runtime.opset10.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.logical_xor.html">openvino.runtime.opset10.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.lrn.html">openvino.runtime.opset10.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.lstm_cell.html">openvino.runtime.opset10.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.lstm_sequence.html">openvino.runtime.opset10.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.matmul.html">openvino.runtime.opset10.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.matrix_nms.html">openvino.runtime.opset10.matrix_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.max_pool.html">openvino.runtime.opset10.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.maximum.html">openvino.runtime.opset10.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.minimum.html">openvino.runtime.opset10.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.mish.html">openvino.runtime.opset10.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.mod.html">openvino.runtime.opset10.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.multiclass_nms.html">openvino.runtime.opset10.multiclass_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.multiply.html">openvino.runtime.opset10.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.mvn.html">openvino.runtime.opset10.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.negative.html">openvino.runtime.opset10.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.non_max_suppression.html">openvino.runtime.opset10.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.non_zero.html">openvino.runtime.opset10.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.normalize_l2.html">openvino.runtime.opset10.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.not_equal.html">openvino.runtime.opset10.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.nv12_to_bgr.html">openvino.runtime.opset10.nv12_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.nv12_to_rgb.html">openvino.runtime.opset10.nv12_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.one_hot.html">openvino.runtime.opset10.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.pad.html">openvino.runtime.opset10.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.parameter.html">openvino.runtime.opset10.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.power.html">openvino.runtime.opset10.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.prelu.html">openvino.runtime.opset10.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.prior_box.html">openvino.runtime.opset10.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.prior_box_clustered.html">openvino.runtime.opset10.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.proposal.html">openvino.runtime.opset10.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.psroi_pooling.html">openvino.runtime.opset10.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.random_uniform.html">openvino.runtime.opset10.random_uniform</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.range.html">openvino.runtime.opset10.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.rdft.html">openvino.runtime.opset10.rdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.read_value.html">openvino.runtime.opset10.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_l1.html">openvino.runtime.opset10.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_l2.html">openvino.runtime.opset10.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_logical_and.html">openvino.runtime.opset10.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_logical_or.html">openvino.runtime.opset10.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_max.html">openvino.runtime.opset10.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_mean.html">openvino.runtime.opset10.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_min.html">openvino.runtime.opset10.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_prod.html">openvino.runtime.opset10.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reduce_sum.html">openvino.runtime.opset10.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.region_yolo.html">openvino.runtime.opset10.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.relu.html">openvino.runtime.opset10.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reorg_yolo.html">openvino.runtime.opset10.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reshape.html">openvino.runtime.opset10.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.result.html">openvino.runtime.opset10.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.reverse_sequence.html">openvino.runtime.opset10.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.rnn_cell.html">openvino.runtime.opset10.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.rnn_sequence.html">openvino.runtime.opset10.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.roi_align.html">openvino.runtime.opset10.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.roi_pooling.html">openvino.runtime.opset10.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.roll.html">openvino.runtime.opset10.roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.round.html">openvino.runtime.opset10.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.scatter_elements_update.html">openvino.runtime.opset10.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.scatter_nd_update.html">openvino.runtime.opset10.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.scatter_update.html">openvino.runtime.opset10.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.select.html">openvino.runtime.opset10.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.selu.html">openvino.runtime.opset10.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.shape_of.html">openvino.runtime.opset10.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.shuffle_channels.html">openvino.runtime.opset10.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.sigmoid.html">openvino.runtime.opset10.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.sign.html">openvino.runtime.opset10.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.sin.html">openvino.runtime.opset10.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.sinh.html">openvino.runtime.opset10.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.slice.html">openvino.runtime.opset10.slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.softmax.html">openvino.runtime.opset10.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.softplus.html">openvino.runtime.opset10.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.softsign.html">openvino.runtime.opset10.softsign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.space_to_batch.html">openvino.runtime.opset10.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.space_to_depth.html">openvino.runtime.opset10.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.split.html">openvino.runtime.opset10.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.sqrt.html">openvino.runtime.opset10.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.squared_difference.html">openvino.runtime.opset10.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.squeeze.html">openvino.runtime.opset10.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.strided_slice.html">openvino.runtime.opset10.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.subtract.html">openvino.runtime.opset10.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.swish.html">openvino.runtime.opset10.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.tan.html">openvino.runtime.opset10.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.tanh.html">openvino.runtime.opset10.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.tile.html">openvino.runtime.opset10.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.topk.html">openvino.runtime.opset10.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.transpose.html">openvino.runtime.opset10.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.unique.html">openvino.runtime.opset10.unique</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.unsqueeze.html">openvino.runtime.opset10.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.variadic_split.html">openvino.runtime.opset10.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.assign.html">openvino.runtime.opset10.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.if_op.html">openvino.runtime.opset10.if_op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.loop.html">openvino.runtime.opset10.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset10.tensor_iterator.html">openvino.runtime.opset10.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.html">openvino.runtime.opset11</a><input class="toctree-checkbox" id="toctree-checkbox-61" name="toctree-checkbox-61" type="checkbox"/><label for="toctree-checkbox-61"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.abs.html">openvino.runtime.opset11.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.absolute.html">openvino.runtime.opset11.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.acos.html">openvino.runtime.opset11.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.acosh.html">openvino.runtime.opset11.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.adaptive_avg_pool.html">openvino.runtime.opset11.adaptive_avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.adaptive_max_pool.html">openvino.runtime.opset11.adaptive_max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.add.html">openvino.runtime.opset11.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.asin.html">openvino.runtime.opset11.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.asinh.html">openvino.runtime.opset11.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.atan.html">openvino.runtime.opset11.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.atanh.html">openvino.runtime.opset11.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.avg_pool.html">openvino.runtime.opset11.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.batch_norm_inference.html">openvino.runtime.opset11.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.batch_to_space.html">openvino.runtime.opset11.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.binary_convolution.html">openvino.runtime.opset11.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.broadcast.html">openvino.runtime.opset11.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.bucketize.html">openvino.runtime.opset11.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.ceil.html">openvino.runtime.opset11.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.ceiling.html">openvino.runtime.opset11.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.clamp.html">openvino.runtime.opset11.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.concat.html">openvino.runtime.opset11.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.constant.html">openvino.runtime.opset11.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.convert.html">openvino.runtime.opset11.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.convert_like.html">openvino.runtime.opset11.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.convolution.html">openvino.runtime.opset11.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.convolution_backprop_data.html">openvino.runtime.opset11.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.cos.html">openvino.runtime.opset11.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.cosh.html">openvino.runtime.opset11.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.ctc_greedy_decoder.html">openvino.runtime.opset11.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset11.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.ctc_loss.html">openvino.runtime.opset11.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.cum_sum.html">openvino.runtime.opset11.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.cumsum.html">openvino.runtime.opset11.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.deformable_convolution.html">openvino.runtime.opset11.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.deformable_psroi_pooling.html">openvino.runtime.opset11.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.depth_to_space.html">openvino.runtime.opset11.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.detection_output.html">openvino.runtime.opset11.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.dft.html">openvino.runtime.opset11.dft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.divide.html">openvino.runtime.opset11.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.einsum.html">openvino.runtime.opset11.einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.elu.html">openvino.runtime.opset11.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.embedding_bag_offsets_sum.html">openvino.runtime.opset11.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.embedding_bag_packed_sum.html">openvino.runtime.opset11.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.embedding_segments_sum.html">openvino.runtime.opset11.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.equal.html">openvino.runtime.opset11.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.erf.html">openvino.runtime.opset11.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.exp.html">openvino.runtime.opset11.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.extract_image_patches.html">openvino.runtime.opset11.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.eye.html">openvino.runtime.opset11.eye</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.fake_quantize.html">openvino.runtime.opset11.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.floor.html">openvino.runtime.opset11.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.floor_mod.html">openvino.runtime.opset11.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.gather.html">openvino.runtime.opset11.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.gather_elements.html">openvino.runtime.opset11.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.gather_nd.html">openvino.runtime.opset11.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.gather_tree.html">openvino.runtime.opset11.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.gelu.html">openvino.runtime.opset11.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.generate_proposals.html">openvino.runtime.opset11.generate_proposals</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.greater.html">openvino.runtime.opset11.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.greater_equal.html">openvino.runtime.opset11.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.grid_sample.html">openvino.runtime.opset11.grid_sample</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.grn.html">openvino.runtime.opset11.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.group_convolution.html">openvino.runtime.opset11.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.group_convolution_backprop_data.html">openvino.runtime.opset11.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.gru_cell.html">openvino.runtime.opset11.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.gru_sequence.html">openvino.runtime.opset11.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.hard_sigmoid.html">openvino.runtime.opset11.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.hsigmoid.html">openvino.runtime.opset11.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.hswish.html">openvino.runtime.opset11.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.i420_to_bgr.html">openvino.runtime.opset11.i420_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.i420_to_rgb.html">openvino.runtime.opset11.i420_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.idft.html">openvino.runtime.opset11.idft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.interpolate.html">openvino.runtime.opset11.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.irdft.html">openvino.runtime.opset11.irdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.is_finite.html">openvino.runtime.opset11.is_finite</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.is_inf.html">openvino.runtime.opset11.is_inf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.is_nan.html">openvino.runtime.opset11.is_nan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.less.html">openvino.runtime.opset11.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.less_equal.html">openvino.runtime.opset11.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.log.html">openvino.runtime.opset11.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.log_softmax.html">openvino.runtime.opset11.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.logical_and.html">openvino.runtime.opset11.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.logical_not.html">openvino.runtime.opset11.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.logical_or.html">openvino.runtime.opset11.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.logical_xor.html">openvino.runtime.opset11.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.lrn.html">openvino.runtime.opset11.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.lstm_cell.html">openvino.runtime.opset11.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.lstm_sequence.html">openvino.runtime.opset11.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.matmul.html">openvino.runtime.opset11.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.matrix_nms.html">openvino.runtime.opset11.matrix_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.max_pool.html">openvino.runtime.opset11.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.maximum.html">openvino.runtime.opset11.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.minimum.html">openvino.runtime.opset11.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.mish.html">openvino.runtime.opset11.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.mod.html">openvino.runtime.opset11.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.multiclass_nms.html">openvino.runtime.opset11.multiclass_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.multiply.html">openvino.runtime.opset11.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.mvn.html">openvino.runtime.opset11.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.negative.html">openvino.runtime.opset11.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.non_max_suppression.html">openvino.runtime.opset11.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.non_zero.html">openvino.runtime.opset11.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.normalize_l2.html">openvino.runtime.opset11.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.not_equal.html">openvino.runtime.opset11.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.nv12_to_bgr.html">openvino.runtime.opset11.nv12_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.nv12_to_rgb.html">openvino.runtime.opset11.nv12_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.one_hot.html">openvino.runtime.opset11.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.pad.html">openvino.runtime.opset11.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.parameter.html">openvino.runtime.opset11.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.power.html">openvino.runtime.opset11.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.prelu.html">openvino.runtime.opset11.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.prior_box.html">openvino.runtime.opset11.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.prior_box_clustered.html">openvino.runtime.opset11.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.proposal.html">openvino.runtime.opset11.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.psroi_pooling.html">openvino.runtime.opset11.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.random_uniform.html">openvino.runtime.opset11.random_uniform</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.range.html">openvino.runtime.opset11.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.rdft.html">openvino.runtime.opset11.rdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.read_value.html">openvino.runtime.opset11.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_l1.html">openvino.runtime.opset11.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_l2.html">openvino.runtime.opset11.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_logical_and.html">openvino.runtime.opset11.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_logical_or.html">openvino.runtime.opset11.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_max.html">openvino.runtime.opset11.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_mean.html">openvino.runtime.opset11.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_min.html">openvino.runtime.opset11.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_prod.html">openvino.runtime.opset11.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reduce_sum.html">openvino.runtime.opset11.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.region_yolo.html">openvino.runtime.opset11.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.relu.html">openvino.runtime.opset11.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reorg_yolo.html">openvino.runtime.opset11.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reshape.html">openvino.runtime.opset11.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.result.html">openvino.runtime.opset11.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.reverse_sequence.html">openvino.runtime.opset11.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.rnn_cell.html">openvino.runtime.opset11.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.rnn_sequence.html">openvino.runtime.opset11.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.roi_align.html">openvino.runtime.opset11.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.roi_pooling.html">openvino.runtime.opset11.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.roll.html">openvino.runtime.opset11.roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.round.html">openvino.runtime.opset11.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.scatter_elements_update.html">openvino.runtime.opset11.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.scatter_nd_update.html">openvino.runtime.opset11.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.scatter_update.html">openvino.runtime.opset11.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.select.html">openvino.runtime.opset11.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.selu.html">openvino.runtime.opset11.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.shape_of.html">openvino.runtime.opset11.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.shuffle_channels.html">openvino.runtime.opset11.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.sigmoid.html">openvino.runtime.opset11.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.sign.html">openvino.runtime.opset11.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.sin.html">openvino.runtime.opset11.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.sinh.html">openvino.runtime.opset11.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.slice.html">openvino.runtime.opset11.slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.softmax.html">openvino.runtime.opset11.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.softplus.html">openvino.runtime.opset11.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.softsign.html">openvino.runtime.opset11.softsign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.space_to_batch.html">openvino.runtime.opset11.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.space_to_depth.html">openvino.runtime.opset11.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.split.html">openvino.runtime.opset11.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.sqrt.html">openvino.runtime.opset11.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.squared_difference.html">openvino.runtime.opset11.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.squeeze.html">openvino.runtime.opset11.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.strided_slice.html">openvino.runtime.opset11.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.subtract.html">openvino.runtime.opset11.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.swish.html">openvino.runtime.opset11.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.tan.html">openvino.runtime.opset11.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.tanh.html">openvino.runtime.opset11.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.tile.html">openvino.runtime.opset11.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.topk.html">openvino.runtime.opset11.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.transpose.html">openvino.runtime.opset11.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.unique.html">openvino.runtime.opset11.unique</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.unsqueeze.html">openvino.runtime.opset11.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.variadic_split.html">openvino.runtime.opset11.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.assign.html">openvino.runtime.opset11.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.if_op.html">openvino.runtime.opset11.if_op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.loop.html">openvino.runtime.opset11.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset11.tensor_iterator.html">openvino.runtime.opset11.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.html">openvino.runtime.opset12</a><input class="toctree-checkbox" id="toctree-checkbox-62" name="toctree-checkbox-62" type="checkbox"/><label for="toctree-checkbox-62"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.abs.html">openvino.runtime.opset12.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.absolute.html">openvino.runtime.opset12.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.acos.html">openvino.runtime.opset12.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.acosh.html">openvino.runtime.opset12.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.adaptive_avg_pool.html">openvino.runtime.opset12.adaptive_avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.adaptive_max_pool.html">openvino.runtime.opset12.adaptive_max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.add.html">openvino.runtime.opset12.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.asin.html">openvino.runtime.opset12.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.asinh.html">openvino.runtime.opset12.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.atan.html">openvino.runtime.opset12.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.atanh.html">openvino.runtime.opset12.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.avg_pool.html">openvino.runtime.opset12.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.batch_norm_inference.html">openvino.runtime.opset12.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.batch_to_space.html">openvino.runtime.opset12.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.binary_convolution.html">openvino.runtime.opset12.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.broadcast.html">openvino.runtime.opset12.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.bucketize.html">openvino.runtime.opset12.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.ceil.html">openvino.runtime.opset12.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.ceiling.html">openvino.runtime.opset12.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.clamp.html">openvino.runtime.opset12.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.concat.html">openvino.runtime.opset12.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.constant.html">openvino.runtime.opset12.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.convert.html">openvino.runtime.opset12.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.convert_like.html">openvino.runtime.opset12.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.convolution.html">openvino.runtime.opset12.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.convolution_backprop_data.html">openvino.runtime.opset12.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.cos.html">openvino.runtime.opset12.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.cosh.html">openvino.runtime.opset12.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.ctc_greedy_decoder.html">openvino.runtime.opset12.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset12.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.ctc_loss.html">openvino.runtime.opset12.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.cum_sum.html">openvino.runtime.opset12.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.cumsum.html">openvino.runtime.opset12.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.deformable_convolution.html">openvino.runtime.opset12.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.deformable_psroi_pooling.html">openvino.runtime.opset12.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.depth_to_space.html">openvino.runtime.opset12.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.detection_output.html">openvino.runtime.opset12.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.dft.html">openvino.runtime.opset12.dft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.divide.html">openvino.runtime.opset12.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.einsum.html">openvino.runtime.opset12.einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.elu.html">openvino.runtime.opset12.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.embedding_bag_offsets_sum.html">openvino.runtime.opset12.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.embedding_bag_packed_sum.html">openvino.runtime.opset12.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.embedding_segments_sum.html">openvino.runtime.opset12.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.equal.html">openvino.runtime.opset12.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.erf.html">openvino.runtime.opset12.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.exp.html">openvino.runtime.opset12.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.extract_image_patches.html">openvino.runtime.opset12.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.eye.html">openvino.runtime.opset12.eye</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.fake_quantize.html">openvino.runtime.opset12.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.floor.html">openvino.runtime.opset12.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.floor_mod.html">openvino.runtime.opset12.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.gather.html">openvino.runtime.opset12.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.gather_elements.html">openvino.runtime.opset12.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.gather_nd.html">openvino.runtime.opset12.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.gather_tree.html">openvino.runtime.opset12.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.gelu.html">openvino.runtime.opset12.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.generate_proposals.html">openvino.runtime.opset12.generate_proposals</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.greater.html">openvino.runtime.opset12.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.greater_equal.html">openvino.runtime.opset12.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.grid_sample.html">openvino.runtime.opset12.grid_sample</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.grn.html">openvino.runtime.opset12.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.group_convolution.html">openvino.runtime.opset12.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.group_convolution_backprop_data.html">openvino.runtime.opset12.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.group_normalization.html">openvino.runtime.opset12.group_normalization</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.gru_cell.html">openvino.runtime.opset12.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.gru_sequence.html">openvino.runtime.opset12.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.hard_sigmoid.html">openvino.runtime.opset12.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.hsigmoid.html">openvino.runtime.opset12.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.hswish.html">openvino.runtime.opset12.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.i420_to_bgr.html">openvino.runtime.opset12.i420_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.i420_to_rgb.html">openvino.runtime.opset12.i420_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.idft.html">openvino.runtime.opset12.idft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.interpolate.html">openvino.runtime.opset12.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.irdft.html">openvino.runtime.opset12.irdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.is_finite.html">openvino.runtime.opset12.is_finite</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.is_inf.html">openvino.runtime.opset12.is_inf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.is_nan.html">openvino.runtime.opset12.is_nan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.less.html">openvino.runtime.opset12.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.less_equal.html">openvino.runtime.opset12.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.log.html">openvino.runtime.opset12.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.log_softmax.html">openvino.runtime.opset12.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.logical_and.html">openvino.runtime.opset12.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.logical_not.html">openvino.runtime.opset12.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.logical_or.html">openvino.runtime.opset12.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.logical_xor.html">openvino.runtime.opset12.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.lrn.html">openvino.runtime.opset12.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.lstm_cell.html">openvino.runtime.opset12.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.lstm_sequence.html">openvino.runtime.opset12.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.matmul.html">openvino.runtime.opset12.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.matrix_nms.html">openvino.runtime.opset12.matrix_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.max_pool.html">openvino.runtime.opset12.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.maximum.html">openvino.runtime.opset12.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.minimum.html">openvino.runtime.opset12.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.mish.html">openvino.runtime.opset12.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.mod.html">openvino.runtime.opset12.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.multiclass_nms.html">openvino.runtime.opset12.multiclass_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.multiply.html">openvino.runtime.opset12.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.mvn.html">openvino.runtime.opset12.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.negative.html">openvino.runtime.opset12.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.non_max_suppression.html">openvino.runtime.opset12.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.non_zero.html">openvino.runtime.opset12.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.normalize_l2.html">openvino.runtime.opset12.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.not_equal.html">openvino.runtime.opset12.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.nv12_to_bgr.html">openvino.runtime.opset12.nv12_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.nv12_to_rgb.html">openvino.runtime.opset12.nv12_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.one_hot.html">openvino.runtime.opset12.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.pad.html">openvino.runtime.opset12.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.parameter.html">openvino.runtime.opset12.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.power.html">openvino.runtime.opset12.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.prelu.html">openvino.runtime.opset12.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.prior_box.html">openvino.runtime.opset12.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.prior_box_clustered.html">openvino.runtime.opset12.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.proposal.html">openvino.runtime.opset12.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.psroi_pooling.html">openvino.runtime.opset12.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.random_uniform.html">openvino.runtime.opset12.random_uniform</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.range.html">openvino.runtime.opset12.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.rdft.html">openvino.runtime.opset12.rdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.read_value.html">openvino.runtime.opset12.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_l1.html">openvino.runtime.opset12.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_l2.html">openvino.runtime.opset12.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_logical_and.html">openvino.runtime.opset12.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_logical_or.html">openvino.runtime.opset12.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_max.html">openvino.runtime.opset12.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_mean.html">openvino.runtime.opset12.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_min.html">openvino.runtime.opset12.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_prod.html">openvino.runtime.opset12.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reduce_sum.html">openvino.runtime.opset12.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.region_yolo.html">openvino.runtime.opset12.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.relu.html">openvino.runtime.opset12.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reorg_yolo.html">openvino.runtime.opset12.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reshape.html">openvino.runtime.opset12.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.result.html">openvino.runtime.opset12.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.reverse_sequence.html">openvino.runtime.opset12.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.rnn_cell.html">openvino.runtime.opset12.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.rnn_sequence.html">openvino.runtime.opset12.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.roi_align.html">openvino.runtime.opset12.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.roi_pooling.html">openvino.runtime.opset12.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.roll.html">openvino.runtime.opset12.roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.round.html">openvino.runtime.opset12.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.scatter_elements_update.html">openvino.runtime.opset12.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.scatter_nd_update.html">openvino.runtime.opset12.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.scatter_update.html">openvino.runtime.opset12.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.select.html">openvino.runtime.opset12.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.selu.html">openvino.runtime.opset12.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.shape_of.html">openvino.runtime.opset12.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.shuffle_channels.html">openvino.runtime.opset12.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.sigmoid.html">openvino.runtime.opset12.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.sign.html">openvino.runtime.opset12.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.sin.html">openvino.runtime.opset12.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.sinh.html">openvino.runtime.opset12.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.slice.html">openvino.runtime.opset12.slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.softmax.html">openvino.runtime.opset12.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.softplus.html">openvino.runtime.opset12.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.softsign.html">openvino.runtime.opset12.softsign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.space_to_batch.html">openvino.runtime.opset12.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.space_to_depth.html">openvino.runtime.opset12.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.split.html">openvino.runtime.opset12.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.sqrt.html">openvino.runtime.opset12.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.squared_difference.html">openvino.runtime.opset12.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.squeeze.html">openvino.runtime.opset12.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.strided_slice.html">openvino.runtime.opset12.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.subtract.html">openvino.runtime.opset12.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.swish.html">openvino.runtime.opset12.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.tan.html">openvino.runtime.opset12.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.tanh.html">openvino.runtime.opset12.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.tile.html">openvino.runtime.opset12.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.topk.html">openvino.runtime.opset12.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.transpose.html">openvino.runtime.opset12.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.unique.html">openvino.runtime.opset12.unique</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.unsqueeze.html">openvino.runtime.opset12.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.variadic_split.html">openvino.runtime.opset12.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.assign.html">openvino.runtime.opset12.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.if_op.html">openvino.runtime.opset12.if_op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.loop.html">openvino.runtime.opset12.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset12.tensor_iterator.html">openvino.runtime.opset12.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.html">openvino.runtime.opset13</a><input class="toctree-checkbox" id="toctree-checkbox-63" name="toctree-checkbox-63" type="checkbox"/><label for="toctree-checkbox-63"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.abs.html">openvino.runtime.opset13.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.absolute.html">openvino.runtime.opset13.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.acos.html">openvino.runtime.opset13.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.acosh.html">openvino.runtime.opset13.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.adaptive_avg_pool.html">openvino.runtime.opset13.adaptive_avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.adaptive_max_pool.html">openvino.runtime.opset13.adaptive_max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.add.html">openvino.runtime.opset13.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.asin.html">openvino.runtime.opset13.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.asinh.html">openvino.runtime.opset13.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.atan.html">openvino.runtime.opset13.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.atanh.html">openvino.runtime.opset13.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.avg_pool.html">openvino.runtime.opset13.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.batch_norm_inference.html">openvino.runtime.opset13.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.batch_to_space.html">openvino.runtime.opset13.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.binary_convolution.html">openvino.runtime.opset13.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.bitwise_and.html">openvino.runtime.opset13.bitwise_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.bitwise_not.html">openvino.runtime.opset13.bitwise_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.bitwise_or.html">openvino.runtime.opset13.bitwise_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.bitwise_xor.html">openvino.runtime.opset13.bitwise_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.broadcast.html">openvino.runtime.opset13.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.bucketize.html">openvino.runtime.opset13.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.ceil.html">openvino.runtime.opset13.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.ceiling.html">openvino.runtime.opset13.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.clamp.html">openvino.runtime.opset13.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.concat.html">openvino.runtime.opset13.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.constant.html">openvino.runtime.opset13.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.convert.html">openvino.runtime.opset13.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.convert_like.html">openvino.runtime.opset13.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.convolution.html">openvino.runtime.opset13.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.convolution_backprop_data.html">openvino.runtime.opset13.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.cos.html">openvino.runtime.opset13.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.cosh.html">openvino.runtime.opset13.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.ctc_greedy_decoder.html">openvino.runtime.opset13.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset13.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.ctc_loss.html">openvino.runtime.opset13.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.cum_sum.html">openvino.runtime.opset13.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.cumsum.html">openvino.runtime.opset13.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.deformable_convolution.html">openvino.runtime.opset13.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.deformable_psroi_pooling.html">openvino.runtime.opset13.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.depth_to_space.html">openvino.runtime.opset13.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.detection_output.html">openvino.runtime.opset13.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.dft.html">openvino.runtime.opset13.dft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.divide.html">openvino.runtime.opset13.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.einsum.html">openvino.runtime.opset13.einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.elu.html">openvino.runtime.opset13.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.embedding_bag_offsets_sum.html">openvino.runtime.opset13.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.embedding_bag_packed_sum.html">openvino.runtime.opset13.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.embedding_segments_sum.html">openvino.runtime.opset13.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.equal.html">openvino.runtime.opset13.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.erf.html">openvino.runtime.opset13.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.exp.html">openvino.runtime.opset13.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.extract_image_patches.html">openvino.runtime.opset13.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.eye.html">openvino.runtime.opset13.eye</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.fake_convert.html">openvino.runtime.opset13.fake_convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.fake_quantize.html">openvino.runtime.opset13.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.floor.html">openvino.runtime.opset13.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.floor_mod.html">openvino.runtime.opset13.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.gather.html">openvino.runtime.opset13.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.gather_elements.html">openvino.runtime.opset13.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.gather_nd.html">openvino.runtime.opset13.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.gather_tree.html">openvino.runtime.opset13.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.gelu.html">openvino.runtime.opset13.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.generate_proposals.html">openvino.runtime.opset13.generate_proposals</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.greater.html">openvino.runtime.opset13.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.greater_equal.html">openvino.runtime.opset13.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.grid_sample.html">openvino.runtime.opset13.grid_sample</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.grn.html">openvino.runtime.opset13.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.group_convolution.html">openvino.runtime.opset13.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.group_convolution_backprop_data.html">openvino.runtime.opset13.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.group_normalization.html">openvino.runtime.opset13.group_normalization</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.gru_cell.html">openvino.runtime.opset13.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.gru_sequence.html">openvino.runtime.opset13.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.hard_sigmoid.html">openvino.runtime.opset13.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.hsigmoid.html">openvino.runtime.opset13.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.hswish.html">openvino.runtime.opset13.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.i420_to_bgr.html">openvino.runtime.opset13.i420_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.i420_to_rgb.html">openvino.runtime.opset13.i420_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.idft.html">openvino.runtime.opset13.idft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.interpolate.html">openvino.runtime.opset13.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.irdft.html">openvino.runtime.opset13.irdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.is_finite.html">openvino.runtime.opset13.is_finite</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.is_inf.html">openvino.runtime.opset13.is_inf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.is_nan.html">openvino.runtime.opset13.is_nan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.less.html">openvino.runtime.opset13.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.less_equal.html">openvino.runtime.opset13.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.log.html">openvino.runtime.opset13.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.log_softmax.html">openvino.runtime.opset13.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.logical_and.html">openvino.runtime.opset13.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.logical_not.html">openvino.runtime.opset13.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.logical_or.html">openvino.runtime.opset13.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.logical_xor.html">openvino.runtime.opset13.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.lrn.html">openvino.runtime.opset13.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.lstm_cell.html">openvino.runtime.opset13.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.lstm_sequence.html">openvino.runtime.opset13.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.matmul.html">openvino.runtime.opset13.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.matrix_nms.html">openvino.runtime.opset13.matrix_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.max_pool.html">openvino.runtime.opset13.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.maximum.html">openvino.runtime.opset13.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.minimum.html">openvino.runtime.opset13.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.mish.html">openvino.runtime.opset13.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.mod.html">openvino.runtime.opset13.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.multiclass_nms.html">openvino.runtime.opset13.multiclass_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.multinomial.html">openvino.runtime.opset13.multinomial</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.multiply.html">openvino.runtime.opset13.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.mvn.html">openvino.runtime.opset13.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.negative.html">openvino.runtime.opset13.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.nms_rotated.html">openvino.runtime.opset13.nms_rotated</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.non_max_suppression.html">openvino.runtime.opset13.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.non_zero.html">openvino.runtime.opset13.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.normalize_l2.html">openvino.runtime.opset13.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.not_equal.html">openvino.runtime.opset13.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.nv12_to_bgr.html">openvino.runtime.opset13.nv12_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.nv12_to_rgb.html">openvino.runtime.opset13.nv12_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.one_hot.html">openvino.runtime.opset13.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.pad.html">openvino.runtime.opset13.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.parameter.html">openvino.runtime.opset13.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.power.html">openvino.runtime.opset13.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.prelu.html">openvino.runtime.opset13.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.prior_box.html">openvino.runtime.opset13.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.prior_box_clustered.html">openvino.runtime.opset13.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.proposal.html">openvino.runtime.opset13.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.psroi_pooling.html">openvino.runtime.opset13.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.random_uniform.html">openvino.runtime.opset13.random_uniform</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.range.html">openvino.runtime.opset13.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.rdft.html">openvino.runtime.opset13.rdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.read_value.html">openvino.runtime.opset13.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_l1.html">openvino.runtime.opset13.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_l2.html">openvino.runtime.opset13.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_logical_and.html">openvino.runtime.opset13.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_logical_or.html">openvino.runtime.opset13.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_max.html">openvino.runtime.opset13.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_mean.html">openvino.runtime.opset13.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_min.html">openvino.runtime.opset13.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_prod.html">openvino.runtime.opset13.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reduce_sum.html">openvino.runtime.opset13.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.region_yolo.html">openvino.runtime.opset13.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.relu.html">openvino.runtime.opset13.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reorg_yolo.html">openvino.runtime.opset13.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reshape.html">openvino.runtime.opset13.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.result.html">openvino.runtime.opset13.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.reverse_sequence.html">openvino.runtime.opset13.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.rnn_cell.html">openvino.runtime.opset13.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.rnn_sequence.html">openvino.runtime.opset13.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.roi_align.html">openvino.runtime.opset13.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.roi_pooling.html">openvino.runtime.opset13.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.roll.html">openvino.runtime.opset13.roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.round.html">openvino.runtime.opset13.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.scaled_dot_product_attention.html">openvino.runtime.opset13.scaled_dot_product_attention</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.scatter_elements_update.html">openvino.runtime.opset13.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.scatter_nd_update.html">openvino.runtime.opset13.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.scatter_update.html">openvino.runtime.opset13.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.select.html">openvino.runtime.opset13.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.selu.html">openvino.runtime.opset13.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.shape_of.html">openvino.runtime.opset13.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.shuffle_channels.html">openvino.runtime.opset13.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.sigmoid.html">openvino.runtime.opset13.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.sign.html">openvino.runtime.opset13.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.sin.html">openvino.runtime.opset13.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.sinh.html">openvino.runtime.opset13.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.slice.html">openvino.runtime.opset13.slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.softmax.html">openvino.runtime.opset13.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.softplus.html">openvino.runtime.opset13.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.softsign.html">openvino.runtime.opset13.softsign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.space_to_batch.html">openvino.runtime.opset13.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.space_to_depth.html">openvino.runtime.opset13.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.split.html">openvino.runtime.opset13.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.sqrt.html">openvino.runtime.opset13.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.squared_difference.html">openvino.runtime.opset13.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.squeeze.html">openvino.runtime.opset13.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.strided_slice.html">openvino.runtime.opset13.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.subtract.html">openvino.runtime.opset13.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.swish.html">openvino.runtime.opset13.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.tan.html">openvino.runtime.opset13.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.tanh.html">openvino.runtime.opset13.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.tile.html">openvino.runtime.opset13.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.topk.html">openvino.runtime.opset13.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.transpose.html">openvino.runtime.opset13.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.unique.html">openvino.runtime.opset13.unique</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.unsqueeze.html">openvino.runtime.opset13.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.variadic_split.html">openvino.runtime.opset13.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.assign.html">openvino.runtime.opset13.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.if_op.html">openvino.runtime.opset13.if_op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.loop.html">openvino.runtime.opset13.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset13.tensor_iterator.html">openvino.runtime.opset13.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.html">openvino.runtime.opset14</a><input class="toctree-checkbox" id="toctree-checkbox-64" name="toctree-checkbox-64" type="checkbox"/><label for="toctree-checkbox-64"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.abs.html">openvino.runtime.opset14.abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.absolute.html">openvino.runtime.opset14.absolute</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.acos.html">openvino.runtime.opset14.acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.acosh.html">openvino.runtime.opset14.acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.adaptive_avg_pool.html">openvino.runtime.opset14.adaptive_avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.adaptive_max_pool.html">openvino.runtime.opset14.adaptive_max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.add.html">openvino.runtime.opset14.add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.asin.html">openvino.runtime.opset14.asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.asinh.html">openvino.runtime.opset14.asinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.atan.html">openvino.runtime.opset14.atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.atanh.html">openvino.runtime.opset14.atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.avg_pool.html">openvino.runtime.opset14.avg_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.batch_norm_inference.html">openvino.runtime.opset14.batch_norm_inference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.batch_to_space.html">openvino.runtime.opset14.batch_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.binary_convolution.html">openvino.runtime.opset14.binary_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.bitwise_and.html">openvino.runtime.opset14.bitwise_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.bitwise_not.html">openvino.runtime.opset14.bitwise_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.bitwise_or.html">openvino.runtime.opset14.bitwise_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.bitwise_xor.html">openvino.runtime.opset14.bitwise_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.broadcast.html">openvino.runtime.opset14.broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.bucketize.html">openvino.runtime.opset14.bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.ceil.html">openvino.runtime.opset14.ceil</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.ceiling.html">openvino.runtime.opset14.ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.clamp.html">openvino.runtime.opset14.clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.concat.html">openvino.runtime.opset14.concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.constant.html">openvino.runtime.opset14.constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.convert.html">openvino.runtime.opset14.convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.convert_like.html">openvino.runtime.opset14.convert_like</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.convert_promote_types.html">openvino.runtime.opset14.convert_promote_types</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.convolution.html">openvino.runtime.opset14.convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.convolution_backprop_data.html">openvino.runtime.opset14.convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.cos.html">openvino.runtime.opset14.cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.cosh.html">openvino.runtime.opset14.cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.ctc_greedy_decoder.html">openvino.runtime.opset14.ctc_greedy_decoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.ctc_greedy_decoder_seq_len.html">openvino.runtime.opset14.ctc_greedy_decoder_seq_len</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.ctc_loss.html">openvino.runtime.opset14.ctc_loss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.cum_sum.html">openvino.runtime.opset14.cum_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.cumsum.html">openvino.runtime.opset14.cumsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.deformable_convolution.html">openvino.runtime.opset14.deformable_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.deformable_psroi_pooling.html">openvino.runtime.opset14.deformable_psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.depth_to_space.html">openvino.runtime.opset14.depth_to_space</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.detection_output.html">openvino.runtime.opset14.detection_output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.dft.html">openvino.runtime.opset14.dft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.divide.html">openvino.runtime.opset14.divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.einsum.html">openvino.runtime.opset14.einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.elu.html">openvino.runtime.opset14.elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.embedding_bag_offsets_sum.html">openvino.runtime.opset14.embedding_bag_offsets_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.embedding_bag_packed_sum.html">openvino.runtime.opset14.embedding_bag_packed_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.embedding_segments_sum.html">openvino.runtime.opset14.embedding_segments_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.equal.html">openvino.runtime.opset14.equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.erf.html">openvino.runtime.opset14.erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.exp.html">openvino.runtime.opset14.exp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.extract_image_patches.html">openvino.runtime.opset14.extract_image_patches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.eye.html">openvino.runtime.opset14.eye</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.fake_convert.html">openvino.runtime.opset14.fake_convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.fake_quantize.html">openvino.runtime.opset14.fake_quantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.floor.html">openvino.runtime.opset14.floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.floor_mod.html">openvino.runtime.opset14.floor_mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.gather.html">openvino.runtime.opset14.gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.gather_elements.html">openvino.runtime.opset14.gather_elements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.gather_nd.html">openvino.runtime.opset14.gather_nd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.gather_tree.html">openvino.runtime.opset14.gather_tree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.gelu.html">openvino.runtime.opset14.gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.generate_proposals.html">openvino.runtime.opset14.generate_proposals</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.greater.html">openvino.runtime.opset14.greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.greater_equal.html">openvino.runtime.opset14.greater_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.grid_sample.html">openvino.runtime.opset14.grid_sample</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.grn.html">openvino.runtime.opset14.grn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.group_convolution.html">openvino.runtime.opset14.group_convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.group_convolution_backprop_data.html">openvino.runtime.opset14.group_convolution_backprop_data</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.group_normalization.html">openvino.runtime.opset14.group_normalization</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.gru_cell.html">openvino.runtime.opset14.gru_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.gru_sequence.html">openvino.runtime.opset14.gru_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.hard_sigmoid.html">openvino.runtime.opset14.hard_sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.hsigmoid.html">openvino.runtime.opset14.hsigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.hswish.html">openvino.runtime.opset14.hswish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.i420_to_bgr.html">openvino.runtime.opset14.i420_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.i420_to_rgb.html">openvino.runtime.opset14.i420_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.idft.html">openvino.runtime.opset14.idft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.interpolate.html">openvino.runtime.opset14.interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.inverse.html">openvino.runtime.opset14.inverse</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.irdft.html">openvino.runtime.opset14.irdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.is_finite.html">openvino.runtime.opset14.is_finite</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.is_inf.html">openvino.runtime.opset14.is_inf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.is_nan.html">openvino.runtime.opset14.is_nan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.less.html">openvino.runtime.opset14.less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.less_equal.html">openvino.runtime.opset14.less_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.log.html">openvino.runtime.opset14.log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.log_softmax.html">openvino.runtime.opset14.log_softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.logical_and.html">openvino.runtime.opset14.logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.logical_not.html">openvino.runtime.opset14.logical_not</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.logical_or.html">openvino.runtime.opset14.logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.logical_xor.html">openvino.runtime.opset14.logical_xor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.lrn.html">openvino.runtime.opset14.lrn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.lstm_cell.html">openvino.runtime.opset14.lstm_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.lstm_sequence.html">openvino.runtime.opset14.lstm_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.matmul.html">openvino.runtime.opset14.matmul</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.matrix_nms.html">openvino.runtime.opset14.matrix_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.max_pool.html">openvino.runtime.opset14.max_pool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.maximum.html">openvino.runtime.opset14.maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.minimum.html">openvino.runtime.opset14.minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.mish.html">openvino.runtime.opset14.mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.mod.html">openvino.runtime.opset14.mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.multiclass_nms.html">openvino.runtime.opset14.multiclass_nms</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.multinomial.html">openvino.runtime.opset14.multinomial</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.multiply.html">openvino.runtime.opset14.multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.mvn.html">openvino.runtime.opset14.mvn</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.negative.html">openvino.runtime.opset14.negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.nms_rotated.html">openvino.runtime.opset14.nms_rotated</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.non_max_suppression.html">openvino.runtime.opset14.non_max_suppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.non_zero.html">openvino.runtime.opset14.non_zero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.normalize_l2.html">openvino.runtime.opset14.normalize_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.not_equal.html">openvino.runtime.opset14.not_equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.nv12_to_bgr.html">openvino.runtime.opset14.nv12_to_bgr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.nv12_to_rgb.html">openvino.runtime.opset14.nv12_to_rgb</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.one_hot.html">openvino.runtime.opset14.one_hot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.pad.html">openvino.runtime.opset14.pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.parameter.html">openvino.runtime.opset14.parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.power.html">openvino.runtime.opset14.power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.prelu.html">openvino.runtime.opset14.prelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.prior_box.html">openvino.runtime.opset14.prior_box</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.prior_box_clustered.html">openvino.runtime.opset14.prior_box_clustered</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.proposal.html">openvino.runtime.opset14.proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.psroi_pooling.html">openvino.runtime.opset14.psroi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.random_uniform.html">openvino.runtime.opset14.random_uniform</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.range.html">openvino.runtime.opset14.range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.rdft.html">openvino.runtime.opset14.rdft</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.read_value.html">openvino.runtime.opset14.read_value</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_l1.html">openvino.runtime.opset14.reduce_l1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_l2.html">openvino.runtime.opset14.reduce_l2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_logical_and.html">openvino.runtime.opset14.reduce_logical_and</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_logical_or.html">openvino.runtime.opset14.reduce_logical_or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_max.html">openvino.runtime.opset14.reduce_max</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_mean.html">openvino.runtime.opset14.reduce_mean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_min.html">openvino.runtime.opset14.reduce_min</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_prod.html">openvino.runtime.opset14.reduce_prod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reduce_sum.html">openvino.runtime.opset14.reduce_sum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.region_yolo.html">openvino.runtime.opset14.region_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.relu.html">openvino.runtime.opset14.relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reorg_yolo.html">openvino.runtime.opset14.reorg_yolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reshape.html">openvino.runtime.opset14.reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.result.html">openvino.runtime.opset14.result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.reverse_sequence.html">openvino.runtime.opset14.reverse_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.rnn_cell.html">openvino.runtime.opset14.rnn_cell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.rnn_sequence.html">openvino.runtime.opset14.rnn_sequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.roi_align.html">openvino.runtime.opset14.roi_align</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.roi_pooling.html">openvino.runtime.opset14.roi_pooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.roll.html">openvino.runtime.opset14.roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.round.html">openvino.runtime.opset14.round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.scaled_dot_product_attention.html">openvino.runtime.opset14.scaled_dot_product_attention</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.scatter_elements_update.html">openvino.runtime.opset14.scatter_elements_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.scatter_nd_update.html">openvino.runtime.opset14.scatter_nd_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.scatter_update.html">openvino.runtime.opset14.scatter_update</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.select.html">openvino.runtime.opset14.select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.selu.html">openvino.runtime.opset14.selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.shape_of.html">openvino.runtime.opset14.shape_of</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.shuffle_channels.html">openvino.runtime.opset14.shuffle_channels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.sigmoid.html">openvino.runtime.opset14.sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.sign.html">openvino.runtime.opset14.sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.sin.html">openvino.runtime.opset14.sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.sinh.html">openvino.runtime.opset14.sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.slice.html">openvino.runtime.opset14.slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.softmax.html">openvino.runtime.opset14.softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.softplus.html">openvino.runtime.opset14.softplus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.softsign.html">openvino.runtime.opset14.softsign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.space_to_batch.html">openvino.runtime.opset14.space_to_batch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.space_to_depth.html">openvino.runtime.opset14.space_to_depth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.split.html">openvino.runtime.opset14.split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.sqrt.html">openvino.runtime.opset14.sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.squared_difference.html">openvino.runtime.opset14.squared_difference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.squeeze.html">openvino.runtime.opset14.squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.strided_slice.html">openvino.runtime.opset14.strided_slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.subtract.html">openvino.runtime.opset14.subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.swish.html">openvino.runtime.opset14.swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.tan.html">openvino.runtime.opset14.tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.tanh.html">openvino.runtime.opset14.tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.tile.html">openvino.runtime.opset14.tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.topk.html">openvino.runtime.opset14.topk</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.transpose.html">openvino.runtime.opset14.transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.unique.html">openvino.runtime.opset14.unique</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.unsqueeze.html">openvino.runtime.opset14.unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.variadic_split.html">openvino.runtime.opset14.variadic_split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.assign.html">openvino.runtime.opset14.assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.if_op.html">openvino.runtime.opset14.if_op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.loop.html">openvino.runtime.opset14.loop</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.opset14.tensor_iterator.html">openvino.runtime.opset14.tensor_iterator</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.html">openvino.runtime.passes</a><input class="toctree-checkbox" id="toctree-checkbox-65" name="toctree-checkbox-65" type="checkbox"/><label for="toctree-checkbox-65"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.consumers_count.html">openvino.runtime.passes.consumers_count</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.has_static_dim.html">openvino.runtime.passes.has_static_dim</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.has_static_dims.html">openvino.runtime.passes.has_static_dims</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.has_static_rank.html">openvino.runtime.passes.has_static_rank</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.has_static_shape.html">openvino.runtime.passes.has_static_shape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.rank_equals.html">openvino.runtime.passes.rank_equals</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.type_matches.html">openvino.runtime.passes.type_matches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.type_matches_any.html">openvino.runtime.passes.type_matches_any</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.AnyInput.html">openvino.runtime.passes.AnyInput</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.BackwardGraphRewrite.html">openvino.runtime.passes.BackwardGraphRewrite</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.ConstantFolding.html">openvino.runtime.passes.ConstantFolding</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.ConvertFP32ToFP16.html">openvino.runtime.passes.ConvertFP32ToFP16</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.GraphRewrite.html">openvino.runtime.passes.GraphRewrite</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.LowLatency2.html">openvino.runtime.passes.LowLatency2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.MakeStateful.html">openvino.runtime.passes.MakeStateful</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.Manager.html">openvino.runtime.passes.Manager</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.Matcher.html">openvino.runtime.passes.Matcher</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.MatcherPass.html">openvino.runtime.passes.MatcherPass</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.ModelPass.html">openvino.runtime.passes.ModelPass</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.Optional.html">openvino.runtime.passes.Optional</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.Or.html">openvino.runtime.passes.Or</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.PassBase.html">openvino.runtime.passes.PassBase</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.Serialize.html">openvino.runtime.passes.Serialize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.Version.html">openvino.runtime.passes.Version</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.VisualizeTree.html">openvino.runtime.passes.VisualizeTree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.runtime.passes.WrapType.html">openvino.runtime.passes.WrapType</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.html">openvino.preprocess</a><input class="toctree-checkbox" id="toctree-checkbox-66" name="toctree-checkbox-66" type="checkbox"/><label for="toctree-checkbox-66"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.get_version.html">openvino.preprocess.get_version</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.ColorFormat.html">openvino.preprocess.ColorFormat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.InputInfo.html">openvino.preprocess.InputInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.InputModelInfo.html">openvino.preprocess.InputModelInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.InputTensorInfo.html">openvino.preprocess.InputTensorInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.OutputInfo.html">openvino.preprocess.OutputInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.OutputModelInfo.html">openvino.preprocess.OutputModelInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.OutputTensorInfo.html">openvino.preprocess.OutputTensorInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.PostProcessSteps.html">openvino.preprocess.PostProcessSteps</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.PrePostProcessor.html">openvino.preprocess.PrePostProcessor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.PreProcessSteps.html">openvino.preprocess.PreProcessSteps</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.preprocess.ResizeAlgorithm.html">openvino.preprocess.ResizeAlgorithm</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.html">openvino.properties</a><input class="toctree-checkbox" id="toctree-checkbox-67" name="toctree-checkbox-67" type="checkbox"/><label for="toctree-checkbox-67"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.Affinity.html">openvino.properties.Affinity</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.CacheMode.html">openvino.properties.CacheMode</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.device.html">openvino.properties.device</a><input class="toctree-checkbox" id="toctree-checkbox-68" name="toctree-checkbox-68" type="checkbox"/><label for="toctree-checkbox-68"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.device.Capability.html">openvino.properties.device.Capability</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.device.Type.html">openvino.properties.device.Type</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.hint.html">openvino.properties.hint</a><input class="toctree-checkbox" id="toctree-checkbox-69" name="toctree-checkbox-69" type="checkbox"/><label for="toctree-checkbox-69"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.hint.ExecutionMode.html">openvino.properties.hint.ExecutionMode</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.hint.ModelDistributionPolicy.html">openvino.properties.hint.ModelDistributionPolicy</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.hint.PerformanceMode.html">openvino.properties.hint.PerformanceMode</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.hint.Priority.html">openvino.properties.hint.Priority</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.hint.SchedulingCoreType.html">openvino.properties.hint.SchedulingCoreType</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.intel_auto.html">openvino.properties.intel_auto</a><input class="toctree-checkbox" id="toctree-checkbox-70" name="toctree-checkbox-70" type="checkbox"/><label for="toctree-checkbox-70"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.intel_auto.SchedulePolicy.html">openvino.properties.intel_auto.SchedulePolicy</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.intel_cpu.html">openvino.properties.intel_cpu</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.intel_gpu.html">openvino.properties.intel_gpu</a><input class="toctree-checkbox" id="toctree-checkbox-71" name="toctree-checkbox-71" type="checkbox"/><label for="toctree-checkbox-71"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.intel_gpu.CapabilityGPU.html">openvino.properties.intel_gpu.CapabilityGPU</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.intel_gpu.MemoryType.html">openvino.properties.intel_gpu.MemoryType</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.intel_gpu.hint.html">openvino.properties.intel_gpu.hint</a><input class="toctree-checkbox" id="toctree-checkbox-72" name="toctree-checkbox-72" type="checkbox"/><label for="toctree-checkbox-72"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.intel_gpu.hint.ThrottleLevel.html">openvino.properties.intel_gpu.hint.ThrottleLevel</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.log.html">openvino.properties.log</a><input class="toctree-checkbox" id="toctree-checkbox-73" name="toctree-checkbox-73" type="checkbox"/><label for="toctree-checkbox-73"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.log.Level.html">openvino.properties.log.Level</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.streams.html">openvino.properties.streams</a><input class="toctree-checkbox" id="toctree-checkbox-74" name="toctree-checkbox-74" type="checkbox"/><label for="toctree-checkbox-74"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.properties.streams.Num.html">openvino.properties.streams.Num</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.html">openvino.frontend</a><input class="toctree-checkbox" id="toctree-checkbox-75" name="toctree-checkbox-75" type="checkbox"/><label for="toctree-checkbox-75"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.get_version.html">openvino.frontend.get_version</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.ConversionExtension.html">openvino.frontend.ConversionExtension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.DecoderTransformationExtension.html">openvino.frontend.DecoderTransformationExtension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.FrontEnd.html">openvino.frontend.FrontEnd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.FrontEndManager.html">openvino.frontend.FrontEndManager</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.InputModel.html">openvino.frontend.InputModel</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.NodeContext.html">openvino.frontend.NodeContext</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.OpExtension.html">openvino.frontend.OpExtension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.Place.html">openvino.frontend.Place</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.ProgressReporterExtension.html">openvino.frontend.ProgressReporterExtension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.TelemetryExtension.html">openvino.frontend.TelemetryExtension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.GeneralFailure.html">openvino.frontend.GeneralFailure</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.InitializationFailure.html">openvino.frontend.InitializationFailure</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.NotImplementedFailure.html">openvino.frontend.NotImplementedFailure</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.OpConversionFailure.html">openvino.frontend.OpConversionFailure</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/ie_python_api/_autosummary/openvino.frontend.OpValidationFailure.html">openvino.frontend.OpValidationFailure</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__cpp__api.html">Group OpenVINO Runtime C++ API</a><input class="toctree-checkbox" id="toctree-checkbox-76" name="toctree-checkbox-76" type="checkbox"/><label for="toctree-checkbox-76"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__model__cpp__api.html">Basics</a><input class="toctree-checkbox" id="toctree-checkbox-77" name="toctree-checkbox-77" type="checkbox"/><label for="toctree-checkbox-77"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__layout__cpp__api.html">Layout</a><input class="toctree-checkbox" id="toctree-checkbox-78" name="toctree-checkbox-78" type="checkbox"/><label for="toctree-checkbox-78"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_layout.html">ov::Layout</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__element__cpp__api.html">Element types</a><input class="toctree-checkbox" id="toctree-checkbox-79" name="toctree-checkbox-79" type="checkbox"/><label for="toctree-checkbox-79"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1element_1_1_type.html">ov::element::Type</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_dimension.html">ov::Dimension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_extension.html">ov::Extension</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_model.html">ov::Model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_node.html">ov::Node</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_partial_shape.html">ov::PartialShape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1preprocess_1_1_pre_post_processor.html">ov::preprocess::PrePostProcessor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_shape.html">ov::Shape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_symbol.html">ov::Symbol</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov_1_1_discrete_type_info.html">ov::DiscreteTypeInfo</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__ops__cpp__api.html">Operations</a><input class="toctree-checkbox" id="toctree-checkbox-80" name="toctree-checkbox-80" type="checkbox"/><label for="toctree-checkbox-80"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1internal_1_1_a_u_g_r_u_cell.html">ov::op::internal::AUGRUCell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1internal_1_1_a_u_g_r_u_sequence.html">ov::op::internal::AUGRUSequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1internal_1_1_r_p_e.html">ov::op::internal::RPE</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_abs.html">ov::op::v0::Abs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_acos.html">ov::op::v0::Acos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_acosh.html">ov::op::v3::Acosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_adaptive_avg_pool.html">ov::op::v8::AdaptiveAvgPool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_adaptive_max_pool.html">ov::op::v8::AdaptiveMaxPool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_add.html">ov::op::v1::Add</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_asin.html">ov::op::v0::Asin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_assign.html">ov::op::v3::Assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_assign.html">ov::op::v6::Assign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_atan.html">ov::op::v0::Atan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_atanh.html">ov::op::v3::Atanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_avg_pool.html">ov::op::v1::AvgPool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v14_1_1_avg_pool.html">ov::op::v14::AvgPool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_batch_norm_inference.html">ov::op::v0::BatchNormInference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_batch_norm_inference.html">ov::op::v5::BatchNormInference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_batch_to_space.html">ov::op::v1::BatchToSpace</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_binary_convolution.html">ov::op::v1::BinaryConvolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v13_1_1_bitwise_and.html">ov::op::v13::BitwiseAnd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v13_1_1_bitwise_not.html">ov::op::v13::BitwiseNot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v13_1_1_bitwise_or.html">ov::op::v13::BitwiseOr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v13_1_1_bitwise_xor.html">ov::op::v13::BitwiseXor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_broadcast.html">ov::op::v3::Broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_broadcast.html">ov::op::v1::Broadcast</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_bucketize.html">ov::op::v3::Bucketize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_ceiling.html">ov::op::v0::Ceiling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_clamp.html">ov::op::v0::Clamp</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_concat.html">ov::op::v0::Concat</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_constant.html">ov::op::v0::Constant</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_convert.html">ov::op::v0::Convert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_convert_like.html">ov::op::v1::ConvertLike</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v14_1_1_convert_promote_types.html">ov::op::v14::ConvertPromoteTypes</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_convolution.html">ov::op::v1::Convolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_convolution_backprop_data.html">ov::op::v1::ConvolutionBackpropData</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_cos.html">ov::op::v0::Cos</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_cosh.html">ov::op::v0::Cosh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_c_t_c_greedy_decoder.html">ov::op::v0::CTCGreedyDecoder</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_c_t_c_greedy_decoder_seq_len.html">ov::op::v6::CTCGreedyDecoderSeqLen</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_c_t_c_loss.html">ov::op::v4::CTCLoss</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_cum_sum.html">ov::op::v0::CumSum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_deformable_convolution.html">ov::op::v1::DeformableConvolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_deformable_convolution.html">ov::op::v8::DeformableConvolution</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_deformable_p_s_r_o_i_pooling.html">ov::op::v1::DeformablePSROIPooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_depth_to_space.html">ov::op::v0::DepthToSpace</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v7_1_1_d_f_t.html">ov::op::v7::DFT</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_divide.html">ov::op::v1::Divide</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v7_1_1_einsum.html">ov::op::v7::Einsum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_elu.html">ov::op::v0::Elu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_embedding_segments_sum.html">ov::op::v3::EmbeddingSegmentsSum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_embedding_bag_offsets_sum.html">ov::op::v3::EmbeddingBagOffsetsSum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_embedding_bag_packed_sum.html">ov::op::v3::EmbeddingBagPackedSum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_equal.html">ov::op::v1::Equal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_erf.html">ov::op::v0::Erf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_exp.html">ov::op::v0::Exp</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_experimental_detectron_detection_output.html">ov::op::v6::ExperimentalDetectronDetectionOutput</a><input class="toctree-checkbox" id="toctree-checkbox-81" name="toctree-checkbox-81" type="checkbox"/><label for="toctree-checkbox-81"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v6_1_1_experimental_detectron_detection_output_1_1_attributes.html">ov::op::v6::ExperimentalDetectronDetectionOutput::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_experimental_detectron_generate_proposals_single_image.html">ov::op::v6::ExperimentalDetectronGenerateProposalsSingleImage</a><input class="toctree-checkbox" id="toctree-checkbox-82" name="toctree-checkbox-82" type="checkbox"/><label for="toctree-checkbox-82"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v6_1_1_experimental_detectron_generate_proposals_single_image_1_1_attributes.html">ov::op::v6::ExperimentalDetectronGenerateProposalsSingleImage::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_experimental_detectron_prior_grid_generator.html">ov::op::v6::ExperimentalDetectronPriorGridGenerator</a><input class="toctree-checkbox" id="toctree-checkbox-83" name="toctree-checkbox-83" type="checkbox"/><label for="toctree-checkbox-83"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v6_1_1_experimental_detectron_prior_grid_generator_1_1_attributes.html">ov::op::v6::ExperimentalDetectronPriorGridGenerator::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_experimental_detectron_r_o_i_feature_extractor.html">ov::op::v6::ExperimentalDetectronROIFeatureExtractor</a><input class="toctree-checkbox" id="toctree-checkbox-84" name="toctree-checkbox-84" type="checkbox"/><label for="toctree-checkbox-84"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v6_1_1_experimental_detectron_r_o_i_feature_extractor_1_1_attributes.html">ov::op::v6::ExperimentalDetectronROIFeatureExtractor::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_experimental_detectron_top_k_r_o_is.html">ov::op::v6::ExperimentalDetectronTopKROIs</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_extract_image_patches.html">ov::op::v3::ExtractImagePatches</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v9_1_1_eye.html">ov::op::v9::Eye</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v13_1_1_fake_convert.html">ov::op::v13::FakeConvert</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_fake_quantize.html">ov::op::v0::FakeQuantize</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_floor.html">ov::op::v0::Floor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_floor_mod.html">ov::op::v1::FloorMod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_gather.html">ov::op::v1::Gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v7_1_1_gather.html">ov::op::v7::Gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_gather.html">ov::op::v8::Gather</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_gather_elements.html">ov::op::v6::GatherElements</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_gather_n_d.html">ov::op::v5::GatherND</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_gather_n_d.html">ov::op::v8::GatherND</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_gather_tree.html">ov::op::v1::GatherTree</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_gelu.html">ov::op::v0::Gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v7_1_1_gelu.html">ov::op::v7::Gelu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_greater.html">ov::op::v1::Greater</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_greater_equal.html">ov::op::v1::GreaterEqual</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v9_1_1_grid_sample.html">ov::op::v9::GridSample</a><input class="toctree-checkbox" id="toctree-checkbox-85" name="toctree-checkbox-85" type="checkbox"/><label for="toctree-checkbox-85"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v9_1_1_grid_sample_1_1_attributes.html">ov::op::v9::GridSample::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v12_1_1_group_normalization.html">ov::op::v12::GroupNormalization</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_g_r_u_cell.html">ov::op::v3::GRUCell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_g_r_u_sequence.html">ov::op::v5::GRUSequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_hard_sigmoid.html">ov::op::v0::HardSigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_h_sigmoid.html">ov::op::v5::HSigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_h_swish.html">ov::op::v4::HSwish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_i420to_b_g_r.html">ov::op::v8::I420toBGR</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_i420to_r_g_b.html">ov::op::v8::I420toRGB</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v7_1_1_i_d_f_t.html">ov::op::v7::IDFT</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_if.html">ov::op::v8::If</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_interpolate.html">ov::op::v0::Interpolate</a><input class="toctree-checkbox" id="toctree-checkbox-86" name="toctree-checkbox-86" type="checkbox"/><label for="toctree-checkbox-86"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v0_1_1_interpolate_1_1_attributes.html">ov::op::v0::Interpolate::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_interpolate.html">ov::op::v4::Interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v11_1_1_interpolate.html">ov::op::v11::Interpolate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v14_1_1_inverse.html">ov::op::v14::Inverse</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v10_1_1_is_finite.html">ov::op::v10::IsFinite</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v10_1_1_is_inf.html">ov::op::v10::IsInf</a><input class="toctree-checkbox" id="toctree-checkbox-87" name="toctree-checkbox-87" type="checkbox"/><label for="toctree-checkbox-87"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v10_1_1_is_inf_1_1_attributes.html">ov::op::v10::IsInf::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v10_1_1_is_na_n.html">ov::op::v10::IsNaN</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_less.html">ov::op::v1::Less</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_less_equal.html">ov::op::v1::LessEqual</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_log.html">ov::op::v0::Log</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_log_softmax.html">ov::op::v5::LogSoftmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_logical_and.html">ov::op::v1::LogicalAnd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_logical_not.html">ov::op::v1::LogicalNot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_logical_or.html">ov::op::v1::LogicalOr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_logical_xor.html">ov::op::v1::LogicalXor</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_loop.html">ov::op::v5::Loop</a><input class="toctree-checkbox" id="toctree-checkbox-88" name="toctree-checkbox-88" type="checkbox"/><label for="toctree-checkbox-88"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v5_1_1_loop_1_1_special_body_ports.html">ov::op::v5::Loop::SpecialBodyPorts</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_l_r_n.html">ov::op::v0::LRN</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_l_s_t_m_cell.html">ov::op::v0::LSTMCell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_l_s_t_m_cell.html">ov::op::v4::LSTMCell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_l_s_t_m_sequence.html">ov::op::v0::LSTMSequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_l_s_t_m_sequence.html">ov::op::v5::LSTMSequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_mat_mul.html">ov::op::v0::MatMul</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_matrix_nms.html">ov::op::v8::MatrixNms</a><input class="toctree-checkbox" id="toctree-checkbox-89" name="toctree-checkbox-89" type="checkbox"/><label for="toctree-checkbox-89"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v8_1_1_matrix_nms_1_1_attributes.html">ov::op::v8::MatrixNms::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_max_pool.html">ov::op::v1::MaxPool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_max_pool.html">ov::op::v8::MaxPool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v14_1_1_max_pool.html">ov::op::v14::MaxPool</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_maximum.html">ov::op::v1::Maximum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_minimum.html">ov::op::v1::Minimum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_mish.html">ov::op::v4::Mish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_mod.html">ov::op::v1::Mod</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v13_1_1_multinomial.html">ov::op::v13::Multinomial</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_multiply.html">ov::op::v1::Multiply</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_m_v_n.html">ov::op::v0::MVN</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_m_v_n.html">ov::op::v6::MVN</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_negative.html">ov::op::v0::Negative</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_non_max_suppression.html">ov::op::v1::NonMaxSuppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_non_max_suppression.html">ov::op::v3::NonMaxSuppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_non_max_suppression.html">ov::op::v4::NonMaxSuppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_non_max_suppression.html">ov::op::v5::NonMaxSuppression</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_non_zero.html">ov::op::v3::NonZero</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_normalize_l2.html">ov::op::v0::NormalizeL2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_not_equal.html">ov::op::v1::NotEqual</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_n_v12to_b_g_r.html">ov::op::v8::NV12toBGR</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_n_v12to_r_g_b.html">ov::op::v8::NV12toRGB</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_one_hot.html">ov::op::v1::OneHot</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1_op.html">ov::op::Op</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_pad.html">ov::op::v1::Pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v12_1_1_pad.html">ov::op::v12::Pad</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_parameter.html">ov::op::v0::Parameter</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_power.html">ov::op::v1::Power</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_p_relu.html">ov::op::v0::PRelu</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_prior_box.html">ov::op::v0::PriorBox</a><input class="toctree-checkbox" id="toctree-checkbox-90" name="toctree-checkbox-90" type="checkbox"/><label for="toctree-checkbox-90"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v0_1_1_prior_box_1_1_attributes.html">ov::op::v0::PriorBox::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_prior_box.html">ov::op::v8::PriorBox</a><input class="toctree-checkbox" id="toctree-checkbox-91" name="toctree-checkbox-91" type="checkbox"/><label for="toctree-checkbox-91"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v8_1_1_prior_box_1_1_attributes.html">ov::op::v8::PriorBox::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_prior_box_clustered.html">ov::op::v0::PriorBoxClustered</a><input class="toctree-checkbox" id="toctree-checkbox-92" name="toctree-checkbox-92" type="checkbox"/><label for="toctree-checkbox-92"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v0_1_1_prior_box_clustered_1_1_attributes.html">ov::op::v0::PriorBoxClustered::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_proposal.html">ov::op::v0::Proposal</a><input class="toctree-checkbox" id="toctree-checkbox-93" name="toctree-checkbox-93" type="checkbox"/><label for="toctree-checkbox-93"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1op_1_1v0_1_1_proposal_1_1_attributes.html">ov::op::v0::Proposal::Attributes</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_proposal.html">ov::op::v4::Proposal</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_p_s_r_o_i_pooling.html">ov::op::v0::PSROIPooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_random_uniform.html">ov::op::v8::RandomUniform</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_range.html">ov::op::v4::Range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_range.html">ov::op::v0::Range</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_read_value.html">ov::op::v3::ReadValue</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v6_1_1_read_value.html">ov::op::v6::ReadValue</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_reduce_l1.html">ov::op::v4::ReduceL1</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_reduce_l2.html">ov::op::v4::ReduceL2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reduce_logical_and.html">ov::op::v1::ReduceLogicalAnd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reduce_logical_or.html">ov::op::v1::ReduceLogicalOr</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reduce_max.html">ov::op::v1::ReduceMax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reduce_mean.html">ov::op::v1::ReduceMean</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reduce_min.html">ov::op::v1::ReduceMin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reduce_prod.html">ov::op::v1::ReduceProd</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reduce_sum.html">ov::op::v1::ReduceSum</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_region_yolo.html">ov::op::v0::RegionYolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_relu.html">ov::op::v0::Relu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_reorg_yolo.html">ov::op::v0::ReorgYolo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reshape.html">ov::op::v1::Reshape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_result.html">ov::op::v0::Result</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_reverse.html">ov::op::v1::Reverse</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_reverse_sequence.html">ov::op::v0::ReverseSequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_r_n_n_cell.html">ov::op::v0::RNNCell</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_r_n_n_sequence.html">ov::op::v5::RNNSequence</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_r_o_i_align.html">ov::op::v3::ROIAlign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_r_o_i_pooling.html">ov::op::v0::ROIPooling</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v7_1_1_roll.html">ov::op::v7::Roll</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v5_1_1_round.html">ov::op::v5::Round</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v13_1_1_scaled_dot_product_attention.html">ov::op::v13::ScaledDotProductAttention</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_scatter_elements_update.html">ov::op::v3::ScatterElementsUpdate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_scatter_n_d_update.html">ov::op::v3::ScatterNDUpdate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_scatter_update.html">ov::op::v3::ScatterUpdate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_select.html">ov::op::v1::Select</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_selu.html">ov::op::v0::Selu</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_shape_of.html">ov::op::v3::ShapeOf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_shape_of.html">ov::op::v0::ShapeOf</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_shuffle_channels.html">ov::op::v0::ShuffleChannels</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_sigmoid.html">ov::op::v0::Sigmoid</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_sign.html">ov::op::v0::Sign</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_sin.html">ov::op::v0::Sin</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_sinh.html">ov::op::v0::Sinh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1_sink.html">ov::op::Sink</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_slice.html">ov::op::v8::Slice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_softmax.html">ov::op::v1::Softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v8_1_1_softmax.html">ov::op::v8::Softmax</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_soft_plus.html">ov::op::v4::SoftPlus</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_space_to_batch.html">ov::op::v1::SpaceToBatch</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_space_to_depth.html">ov::op::v0::SpaceToDepth</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_split.html">ov::op::v1::Split</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_sqrt.html">ov::op::v0::Sqrt</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_squared_difference.html">ov::op::v0::SquaredDifference</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_squeeze.html">ov::op::v0::Squeeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_strided_slice.html">ov::op::v1::StridedSlice</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_subtract.html">ov::op::v1::Subtract</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v4_1_1_swish.html">ov::op::v4::Swish</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_tan.html">ov::op::v0::Tan</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_tanh.html">ov::op::v0::Tanh</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_tensor_iterator.html">ov::op::v0::TensorIterator</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_tile.html">ov::op::v0::Tile</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_top_k.html">ov::op::v1::TopK</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v3_1_1_top_k.html">ov::op::v3::TopK</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v11_1_1_top_k.html">ov::op::v11::TopK</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_transpose.html">ov::op::v1::Transpose</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v10_1_1_unique.html">ov::op::v10::Unique</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_unsqueeze.html">ov::op::v0::Unsqueeze</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v1_1_1_variadic_split.html">ov::op::v1::VariadicSplit</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1op_1_1v0_1_1_xor.html">ov::op::v0::Xor</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__opset__cpp__api.html">Operation sets</a><input class="toctree-checkbox" id="toctree-checkbox-94" name="toctree-checkbox-94" type="checkbox"/><label for="toctree-checkbox-94"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_op_set.html">ov::OpSet</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__pass__cpp__api.html">Transformation passes</a><input class="toctree-checkbox" id="toctree-checkbox-95" name="toctree-checkbox-95" type="checkbox"/><label for="toctree-checkbox-95"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_constant_folding.html">ov::pass::ConstantFolding</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_f_p32_to_f_p16.html">ov::pass::ConvertFP32ToFP16</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_matcher_pass.html">ov::pass::MatcherPass</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_graph_rewrite.html">ov::pass::GraphRewrite</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_low_latency2.html">ov::pass::LowLatency2</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_make_stateful.html">ov::pass::MakeStateful</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_manager.html">ov::pass::Manager</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pass_base.html">ov::pass::PassBase</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_model_pass.html">ov::pass::ModelPass</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pass_config.html">ov::pass::PassConfig</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_serialize.html">ov::pass::Serialize</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_stream_serialize.html">ov::pass::StreamSerialize</a><input class="toctree-checkbox" id="toctree-checkbox-96" name="toctree-checkbox-96" type="checkbox"/><label for="toctree-checkbox-96"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1pass_1_1_stream_serialize_1_1_data_header.html">ov::pass::StreamSerialize::DataHeader</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_validate.html">ov::pass::Validate</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_visualize_tree.html">ov::pass::VisualizeTree</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__runtime__cpp__api.html">Inference</a><input class="toctree-checkbox" id="toctree-checkbox-97" name="toctree-checkbox-97" type="checkbox"/><label for="toctree-checkbox-97"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/group__ov__runtime__cpu__prop__cpp__api.html">Intel CPU specific properties</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__runtime__ocl__gpu__cpp__api.html">Intel GPU OpenCL interoperability</a><input class="toctree-checkbox" id="toctree-checkbox-98" name="toctree-checkbox-98" type="checkbox"/><label for="toctree-checkbox-98"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_d3_d_buffer_tensor.html">ov::intel_gpu::ocl::D3DBufferTensor</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_d3_d_surface2_d_tensor.html">ov::intel_gpu::ocl::D3DSurface2DTensor</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_d3_d_context.html">ov::intel_gpu::ocl::D3DContext</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_cl_buffer_tensor.html">ov::intel_gpu::ocl::ClBufferTensor</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_cl_image2_d_tensor.html">ov::intel_gpu::ocl::ClImage2DTensor</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_u_s_m_tensor.html">ov::intel_gpu::ocl::USMTensor</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_cl_context.html">ov::intel_gpu::ocl::ClContext</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_v_a_surface_tensor.html">ov::intel_gpu::ocl::VASurfaceTensor</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/classov_1_1intel__gpu_1_1ocl_1_1_v_a_context.html">ov::intel_gpu::ocl::VAContext</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/group__ov__runtime__ocl__gpu__prop__cpp__api.html">Intel GPU OpenCL specific properties</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/group__ov__runtime__npu__prop__cpp__api.html">Intel NPU specific properties</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__runtime__cpp__prop__api.html">Device properties</a><input class="toctree-checkbox" id="toctree-checkbox-99" name="toctree-checkbox-99" type="checkbox"/><label for="toctree-checkbox-99"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1device_1_1_priorities.html">ov::device::Priorities</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1device_1_1_properties.html">ov::device::Properties</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1device_1_1_u_u_i_d.html">ov::device::UUID</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1device_1_1_l_u_i_d.html">ov::device::LUID</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1streams_1_1_num.html">ov::streams::Num</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_allocator.html">ov::Allocator</a><input class="toctree-checkbox" id="toctree-checkbox-100" name="toctree-checkbox-100" type="checkbox"/><label for="toctree-checkbox-100"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1_allocator_1_1_base.html">ov::Allocator::Base</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/structov_1_1_allocator_1_1_impl.html">ov::Allocator::Impl</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_tensor.html">ov::Tensor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_compiled_model.html">ov::CompiledModel</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_core.html">ov::Core</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_cancelled.html">ov::Cancelled</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_busy.html">ov::Busy</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_infer_request.html">ov::InferRequest</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_remote_context.html">ov::RemoteContext</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_remote_tensor.html">ov::RemoteTensor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_variable_state.html">ov::VariableState</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov_1_1_profiling_info.html">ov::ProfilingInfo</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__c__api.html">Group OpenVINO Runtime C API</a><input class="toctree-checkbox" id="toctree-checkbox-101" name="toctree-checkbox-101" type="checkbox"/><label for="toctree-checkbox-101"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../api/c_cpp_api/group__ov__base__c__api.html">Basics</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__compiled__model__c__api.html">Compiled Model</a><input class="toctree-checkbox" id="toctree-checkbox-102" name="toctree-checkbox-102" type="checkbox"/><label for="toctree-checkbox-102"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__compiled__model__t.html">ov_compiled_model_t</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__core__c__api.html">Core</a><input class="toctree-checkbox" id="toctree-checkbox-103" name="toctree-checkbox-103" type="checkbox"/><label for="toctree-checkbox-103"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__core__t.html">ov_core_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__version.html">ov_version</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__core__version.html">ov_core_version</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__core__version__list.html">ov_core_version_list</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__available__devices__t.html">ov_available_devices_t</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dimension__c__api.html">Dimension</a><input class="toctree-checkbox" id="toctree-checkbox-104" name="toctree-checkbox-104" type="checkbox"/><label for="toctree-checkbox-104"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__dimension.html">ov_dimension</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__infer__request__c__api.html">Infer Request</a><input class="toctree-checkbox" id="toctree-checkbox-105" name="toctree-checkbox-105" type="checkbox"/><label for="toctree-checkbox-105"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__infer__request__t.html">ov_infer_request_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__callback__t.html">ov_callback_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov___profiling_info__t.html">ov_ProfilingInfo_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__profiling__info__list__t.html">ov_profiling_info_list_t</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__layout__c__api.html">Layout</a><input class="toctree-checkbox" id="toctree-checkbox-106" name="toctree-checkbox-106" type="checkbox"/><label for="toctree-checkbox-106"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__layout__t.html">ov_layout_t</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__model__c__api.html">Model</a><input class="toctree-checkbox" id="toctree-checkbox-107" name="toctree-checkbox-107" type="checkbox"/><label for="toctree-checkbox-107"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__model__t.html">ov_model_t</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__node__c__api.html">Node</a><input class="toctree-checkbox" id="toctree-checkbox-108" name="toctree-checkbox-108" type="checkbox"/><label for="toctree-checkbox-108"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__output__const__port__t.html">ov_output_const_port_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__output__port__t.html">ov_output_port_t</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__partial__shape__c__api.html">Partial Shape</a><input class="toctree-checkbox" id="toctree-checkbox-109" name="toctree-checkbox-109" type="checkbox"/><label for="toctree-checkbox-109"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__partial__shape.html">ov_partial_shape</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__prepostprocess__c__api.html">Pre Post Process</a><input class="toctree-checkbox" id="toctree-checkbox-110" name="toctree-checkbox-110" type="checkbox"/><label for="toctree-checkbox-110"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__preprocess__prepostprocessor__t.html">ov_preprocess_prepostprocessor_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__preprocess__input__info__t.html">ov_preprocess_input_info_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__preprocess__input__tensor__info__t.html">ov_preprocess_input_tensor_info_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__preprocess__output__info__t.html">ov_preprocess_output_info_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__preprocess__output__tensor__info__t.html">ov_preprocess_output_tensor_info_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__preprocess__input__model__info__t.html">ov_preprocess_input_model_info_t</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__preprocess__preprocess__steps__t.html">ov_preprocess_preprocess_steps_t</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../api/c_cpp_api/group__ov__property__c__api.html">Property</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__rank__c__api.html">Rank</a><input class="toctree-checkbox" id="toctree-checkbox-111" name="toctree-checkbox-111" type="checkbox"/><label for="toctree-checkbox-111"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__rank__t.html">ov_rank_t</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__shape__c__api.html">Shape</a><input class="toctree-checkbox" id="toctree-checkbox-112" name="toctree-checkbox-112" type="checkbox"/><label for="toctree-checkbox-112"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__shape__t.html">ov_shape_t</a></li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__tensor__c__api.html">Tensor</a><input class="toctree-checkbox" id="toctree-checkbox-113" name="toctree-checkbox-113" type="checkbox"/><label for="toctree-checkbox-113"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/c_cpp_api/structov__tensor__t.html">ov_tensor_t</a></li>
</ul>
</li>
<li class="toctree-l4"><a class="reference internal" href="../api/c_cpp_api/group__ov__remote__context__c__api.html">Remote Context</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../api/nodejs_api/nodejs_api.html">OpenVINO Node.js API</a><input class="toctree-checkbox" id="toctree-checkbox-114" name="toctree-checkbox-114" type="checkbox"/><label for="toctree-checkbox-114"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4 has-children"><a class="reference internal" href="../api/nodejs_api/addon.html">addon</a><input class="toctree-checkbox" id="toctree-checkbox-115" name="toctree-checkbox-115" type="checkbox"/><label for="toctree-checkbox-115"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/enums/element.html">element</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/enums/resizeAlgorithm.html">resizeAlgorithm</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/CompiledModel.html">CompiledModel</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/Core.html">Core</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/CoreConstructor.html">CoreConstructor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/InferRequest.html">InferRequest</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/InputInfo.html">InputInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/InputModelInfo.html">InputModelInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/InputTensorInfo.html">InputTensorInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/Model.html">Model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/Output.html">Output</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/OutputInfo.html">OutputInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/OutputTensorInfo.html">OutputTensorInfo</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/PartialShape.html">PartialShape</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/PartialShapeConstructor.html">PartialShapeConstructor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/PrePostProcessor.html">PrePostProcessor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/PrePostProcessorConstructor.html">PrePostProcessorConstructor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/PreProcessSteps.html">PreProcessSteps</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/Tensor.html">Tensor</a></li>
<li class="toctree-l5"><a class="reference internal" href="../api/nodejs_api/openvino-node/interfaces/TensorConstructor.html">TensorConstructor</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../documentation/openvino-ir-format.html">OpenVINO IR format and Operation Sets</a><input class="toctree-checkbox" id="toctree-checkbox-116" name="toctree-checkbox-116" type="checkbox"/><label for="toctree-checkbox-116"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets.html">Operation Sets in OpenVINO</a></li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets.html">Available Operation Sets</a><input class="toctree-checkbox" id="toctree-checkbox-117" name="toctree-checkbox-117" type="checkbox"/><label for="toctree-checkbox-117"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset14.html">opset14</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset13.html">opset13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset12.html">opset12</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset11.html">opset11</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset10.html">opset10</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset9.html">opset9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset8.html">opset8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset7.html">opset7</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset6.html">opset6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset5.html">opset5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset4.html">opset4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset3.html">opset3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset2.html">opset2</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/available-opsets/opset1.html">opset1</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs.html">Operation Specifications</a><input class="toctree-checkbox" id="toctree-checkbox-118" name="toctree-checkbox-118" type="checkbox"/><label for="toctree-checkbox-118"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/abs-1.html">Abs-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/acos-1.html">Acos-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/acosh-3.html">Acosh-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/pooling/adaptive-avg-pool-8.html">AdaptiveAvgPool-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/pooling/adaptive-max-pool-8.html">AdaptiveMaxPool-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/add-1.html">Add-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/asin-1.html">Asin-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/asinh-3.html">Asinh-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/assign-3.html">Assign-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/assign-6.html">Assign-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/atan-1.html">Atan-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/atanh-3.html">Atanh-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/pooling/avg-pool-1.html">AvgPool-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/pooling/avg-pool-14.html">AvgPool-14</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/normalization/batch-norm-inference-1.html">BatchNormInference-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/normalization/batch-norm-inference-5.html">BatchNormInference-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/batch-to-space-2.html">BatchToSpace-2</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/convolution/binary-convolution-1.html">BinaryConvolution-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/bitwise/bitwise-and-13.html">BitwiseAnd-13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/bitwise/bitwise-not-13.html">BitwiseNot-13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/bitwise/bitwise-or-13.html">BitwiseOr-13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/bitwise/bitwise-xor-13.html">BitwiseXor-13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/broadcast-1.html">Broadcast-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/broadcast-3.html">Broadcast-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/condition/bucketize-3.html">Bucketize-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/ctc-greedy-decoder-1.html">CTCGreedyDecoder-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/ctc-greedy-decoder-seq-len-6.html">CTCGreedyDecoderSeqLen-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/ceiling-1.html">Ceiling-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/clamp-1.html">Clamp-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/concat-1.html">Concat-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/constant-1.html">Constant-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/type/convert-like-1.html">ConvertLike-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/type/convert-promote-types-14.html">ConvertPromoteTypes-14</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/type/convert-1.html">Convert-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/convolution/convolution-backprop-data-1.html">ConvolutionBackpropData-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/convolution/convolution-1.html">Convolution-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/cos-1.html">Cos-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/cosh-1.html">Cosh-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/ctc-loss-4.html">CTCLoss-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/cumsum-3.html">CumSum-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/convolution/deformable-convolution-1.html">DeformableConvolution-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/convolution/deformable-convolution-8.html">DeformableConvolution-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/deformable-psroi-pooling-1.html">DeformablePSROIPooling-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/depth-to-space-1.html">DepthToSpace-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/detectionoutput-1.html">DetectionOutput-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/detectionoutput-8.html">DetectionOutput-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/signals/dft-7.html">DFT-7</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/divide-1.html">Divide-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/matrix/einsum-7.html">Einsum-7</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/elu-1.html">Elu-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sparse/embedding-bag-offsets-sum-3.html">EmbeddingBagOffsetsSum-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sparse/embedding-bag-packed-sum-3.html">EmbeddingBagPackedSum-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sparse/embedding-segments-sum-3.html">EmbeddingSegmentsSum-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/equal-1.html">Equal-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/erf-1.html">Erf-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/exp-1.html">Exp-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/experimental-detectron-detection-output-6.html">ExperimentalDetectronDetectionOutput-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/experimental-detectron-generate-proposals-single-image-6.html">ExperimentalDetectronGenerateProposalsSingleImage-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/experimental-detectron-prior-grid-generator-6.html">ExperimentalDetectronPriorGridGenerator-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/experimental-detectron-roi-feature-extractor-6.html">ExperimentalDetectronROIFeatureExtractor-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/experimental-detectron-top-krois-6.html">ExperimentalDetectronTopKROIs-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/extract-image-patches-3.html">ExtractImagePatches-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/generation/eye-9.html">Eye-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/quantization/fake-convert-13.html">FakeConvert-13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/quantization/fake-quantize-1.html">FakeQuantize-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/floormod-1.html">FloorMod-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/floor-1.html">Floor-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/image/grid-sample-9.html">GridSample-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/normalization/grn-1.html">GRN-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/gru-cell-3.html">GRUCell-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/gru-sequence-5.html">GRUSequence-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/gather-tree-1.html">GatherTree-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/gather-1.html">Gather-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/gather-7.html">Gather-7</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/gather-8.html">Gather-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/gather-elements-6.html">GatherElements-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/gather-nd-5.html">GatherND-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/gather-nd-8.html">GatherND-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/gelu-2.html">GELU-2</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/gelu-7.html">GELU-7</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/generate-proposals-9.html">GenerateProposals-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/greater-equal-1.html">GreaterEqual-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/greater-1.html">Greater-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/convolution/group-convolution-backprop-data-1.html">GroupConvolutionBackpropData-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/convolution/group-convolution-1.html">GroupConvolution-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/normalization/group-normalization-12.html">GroupNormalization-12</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/hard-sigmoid-1.html">HardSigmoid-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/hsigmoid-5.html">HSigmoid-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/hswish-4.html">HSwish-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/image/i420-to-bgr-8.html">I420toBGR-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/image/i420-to-rgb-8.html">I420toRGB-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/signals/idft-7.html">IDFT-7</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/signals/irdft-9.html">IRDFT-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/condition/if-8.html">If-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/image/interpolate-1.html">Interpolate-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/image/interpolate-4.html">Interpolate-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/image/interpolate-11.html">Interpolate-11</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/isfinite-10.html">IsFinite-10</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/isinf-10.html">IsInf-10</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/isnan-10.html">IsNaN-10</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/normalization/lrn-1.html">LRN-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/lstm-cell-1.html">LSTMCell-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/lstm-sequence-1.html">LSTMSequence-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/lessequal-1.html">LessEqual-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/less-1.html">Less-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/log-1.html">Log-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/logical/logical-and-1.html">LogicalAnd-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/logical/logical-not-1.html">LogicalNot-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/logical/logical-or-1.html">LogicalOr-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/logical/logical-xor-1.html">LogicalXor-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/log-soft-max-5.html">LogSoftmax-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/loop-5.html">Loop-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/normalization/mvn-1.html">MVN-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/normalization/mvn-6.html">MVN-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/matrix/matmul-1.html">MatMul-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/matrix-non-max-suppression-8.html">MatrixNms-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/pooling/max-pool-1.html">MaxPool-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/pooling/max-pool-8.html">MaxPool-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/pooling/max-pool-14.html">MaxPool-14</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/maximum-1.html">Maximum-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/minimum-1.html">Minimum-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/mish-4.html">Mish-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/mod-1.html">Mod-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/multiclass-non-max-suppression-8.html">MulticlassNonMaxSuppression-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/multiclass-non-max-suppression-9.html">MulticlassNonMaxSuppression-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/generation/multinomial-13.html">Multinomial-13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/multiply-1.html">Multiply-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/negative-1.html">Negative-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/nms-rotated-13.html">NMSRotated-13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/non-max-suppression-1.html">NonMaxSuppression-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/non-max-suppression-3.html">NonMaxSuppression-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/non-max-suppression-4.html">NonMaxSuppression-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/no-max-suppression-5.html">NonMaxSuppression-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/non-max-suppression-9.html">NonMaxSuppression-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/condition/nonzero-3.html">NonZero-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/normalization/normalize-l2-1.html">NormalizeL2-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/comparison/notequal-1.html">NotEqual-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/image/nv12-to-bgr-8.html">NV12toBGR-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/image/nv12-to-rgb-8.html">NV12toRGB-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/one-hot-1.html">OneHot-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/prelu-1.html">PReLU-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/psroi-pooling-1.html">PSROIPooling-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/pad-1.html">Pad-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/pad-12.html">Pad-12</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/parameter-1.html">Parameter-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/power-1.html">Power-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/prior-box-clustered-1.html">PriorBoxClustered-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/prior-box-1.html">PriorBox-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/prior-box-8.html">PriorBox-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/proposal-1.html">Proposal-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/proposal-4.html">Proposal-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/generation/random-uniform-8.html">RandomUniform-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/generation/range-1.html">Range-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/generation/range-4.html">Range-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/signals/rdft-9.html">RDFT-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/read-value-3.html">ReadValue-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/read-value-6.html">ReadValue-6</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/relu-1.html">ReLU-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-l1-4.html">ReduceL1-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-l2-4.html">ReduceL2-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-logical-and-1.html">ReduceLogicalAnd-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-logical-or-1.html">ReduceLogicalOr-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-max-1.html">ReduceMax-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-mean-1.html">ReduceMean-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-min-1.html">ReduceMin-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-prod-1.html">ReduceProd-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/reduction/reduce-sum-1.html">ReduceSum-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/region-yolo-1.html">RegionYolo-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/reorg-yolo-1.html">ReorgYolo-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/shape/reshape-1.html">Reshape-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/result-1.html">Result-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/reverse-1.html">Reverse-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/reverse-sequence-1.html">ReverseSequence-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/rnn-cell-3.html">RNNCell-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/rnn-sequence-5.html">RNNSequence-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/roi-align-3.html">ROIAlign-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/roi-align-9.html">ROIAlign-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/detection/roi-pooling-1.html">ROIPooling-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/roll-7.html">Roll-7</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/round-5.html">Round-5</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sequence/scaled-dot-product-attention.html">ScaledDotProductAttention-13</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/scatter-elements-update-3.html">ScatterElementsUpdate-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/scatter-elements-update-12.html">ScatterElementsUpdate-12</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/scatter-nd-update-3.html">ScatterNDUpdate-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/scatter-update-3.html">ScatterUpdate-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/condition/select-1.html">Select-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/selu-1.html">Selu-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/shape/shape-of-1.html">ShapeOf-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/shape/shape-of-3.html">ShapeOf-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/shuffle-channels-1.html">ShuffleChannels-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/sigmoid-1.html">Sigmoid-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/sign-1.html">Sign-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/sin-1.html">Sin-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/sinh-1.html">Sinh-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/slice-8.html">Slice-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/softmax-1.html">SoftMax-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/softmax-8.html">SoftMax-8</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/softplus-4.html">SoftPlus-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/softsign-9.html">SoftSign-9</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/space-to-batch-2.html">SpaceToBatch-2</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/space-to-depth-1.html">SpaceToDepth-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/split-1.html">Split-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/sqrt-1.html">Sqrt-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/squared-difference-1.html">SquaredDifference-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/shape/squeeze-1.html">Squeeze-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/strided-slice-1.html">StridedSlice-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/subtract-1.html">Subtract-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/activation/swish-4.html">Swish-4</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/tan-1.html">Tan-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/arithmetic/tanh-1.html">Tanh-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/infrastructure/tensor-iterator-1.html">TensorIterator-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/tile-1.html">Tile-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/top-k-1.html">TopK-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/top-k-3.html">TopK-3</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/sort/top-k-11.html">TopK-11</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/transpose-1.html">Transpose-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/unique-10.html">Unique-10</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/shape/unsqueeze-1.html">Unsqueeze-1</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/operation-specs/movement/variadic-split-1.html">VariadicSplit-1</a></li>
</ul>
</li>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-ir-format/operation-sets/broadcast-rules.html">Broadcast Rules For Elementwise Operations</a></li>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-ir-format/intermediate-representation-int8-inference.html">Intermediate Representation Suitable for INT8 Inference</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../documentation/legacy-features.html">Legacy Features</a><input class="toctree-checkbox" id="toctree-checkbox-119" name="toctree-checkbox-119" type="checkbox"/><label for="toctree-checkbox-119"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../documentation/legacy-features/install-dev-tools.html">OpenVINO Development Tools package</a></li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api.html">Model Optimizer / Conversion API</a><input class="toctree-checkbox" id="toctree-checkbox-120" name="toctree-checkbox-120" type="checkbox"/><label for="toctree-checkbox-120"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4 has-children"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api.html">Legacy Conversion API</a><input class="toctree-checkbox" id="toctree-checkbox-121" name="toctree-checkbox-121" type="checkbox"/><label for="toctree-checkbox-121"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-setting-input-shapes.html">Setting Input Shapes</a></li>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-troubleshooting-reshape-errors.html">Troubleshooting Reshape Errors</a></li>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-cutting-parts-of-a-model.html">Cutting Off Parts of a Model</a></li>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-embedding-preprocessing-computation.html">Embedding Preprocessing Computation</a></li>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-compressing-model-to-fp16.html">Compressing a Model to FP16</a></li>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-convert-models-as-python-objects.html">Convert Models Represented as Python Objects</a></li>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-model-optimizer-faq.html">Model Optimizer Frequently Asked Questions</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats.html">Supported Model Formats</a><input class="toctree-checkbox" id="toctree-checkbox-122" name="toctree-checkbox-122" type="checkbox"/><label for="toctree-checkbox-122"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-convert-tensorflow.html">Converting a TensorFlow Model</a></li>
<li class="toctree-l6"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-convert-onnx.html">Converting an ONNX Model</a></li>
<li class="toctree-l6"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-convert-pytorch.html">Converting a PyTorch Model</a></li>
<li class="toctree-l6"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-convert-tensorflow-lite.html">Converting a TensorFlow Lite Model</a></li>
<li class="toctree-l6"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-convert-paddle.html">Converting a PaddlePaddle Model</a></li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials.html">Model Conversion Tutorials</a><input class="toctree-checkbox" id="toctree-checkbox-123" name="toctree-checkbox-123" type="checkbox"/><label for="toctree-checkbox-123"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-attention-ocr.html">Converting a TensorFlow Attention OCR Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-bert.html">Converting a TensorFlow BERT Model</a></li>

<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-crnn.html">Converting a TensorFlow CRNN Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-deep-speech.html">Converting a TensorFlow DeepSpeech Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-efficient-det.html">Converting TensorFlow EfficientDet Models</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-face-net.html">Converting TensorFlow FaceNet Models</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-gnmt.html">Converting a TensorFlow GNMT Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-language-1b.html">Converting a TensorFlow Language Model on One Billion Word Benchmark</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-ncf.html">Converting a TensorFlow Neural Collaborative Filtering Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-object-detection.html">Converting TensorFlow Object Detection API Models</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-retina-net.html">Converting a TensorFlow RetinaNet Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-slim-library.html">Converting TensorFlow Slim Image Classification Model Library Models</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-wide-and-deep-family.html">Converting TensorFlow Wide and Deep Family Models</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-xlnet.html">Converting a TensorFlow XLNet Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-tensorflow-yolo.html">Converting TensorFlow YOLO Models</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-onnx-faster-r-cnn.html">Converting an ONNX Faster R-CNN Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-onnx-gpt-2.html">Converting an ONNX GPT-2 Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-onnx-mask-r-cnn.html">Converting an ONNX Mask R-CNN Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-pytorch-bert-ner.html">Converting a PyTorch BERT-NER Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-pytorch-cascade-rcnn-r-101.html">Converting a PyTorch Cascade RCNN R-101 Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-pytorch-f3-net.html">Converting a PyTorch F3Net Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-pytorch-quartz-net.html">Converting a PyTorch QuartzNet Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-pytorch-rcan.html">Converting a PyTorch RCAN Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-pytorch-rnn-t.html">Converting a PyTorch RNN-T Model</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-conversion-api/%5Blegacy%5D-supported-model-formats/%5Blegacy%5D-conversion-tutorials/convert-pytorch-yolact.html">Converting a PyTorch YOLACT Model</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-model-optimizer-extensibility.html">Legacy Model Optimizer Extensibility</a><input class="toctree-checkbox" id="toctree-checkbox-124" name="toctree-checkbox-124" type="checkbox"/><label for="toctree-checkbox-124"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-model-optimizer-extensibility/%5Blegacy%5D-graph-traversal-and-modification.html">[LEGACY] Graph Traversal and Modification</a></li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-model-optimizer-extensibility/%5Blegacy%5D-model-optimizer-extensions.html">[LEGACY] Model Optimizer Extensions</a><input class="toctree-checkbox" id="toctree-checkbox-125" name="toctree-checkbox-125" type="checkbox"/><label for="toctree-checkbox-125"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-model-optimizer-extensibility/%5Blegacy%5D-model-optimizer-extensions/%5Blegacy%5D-model-optimizer-operation.html">[LEGACY] Model Optimizer Operation</a></li>
<li class="toctree-l6"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-model-optimizer-extensibility/%5Blegacy%5D-model-optimizer-extensions/%5Blegacy%5D-optimizer-extractor.html">[LEGACY] Operation Extractor</a></li>
<li class="toctree-l6"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-model-optimizer-extensibility/%5Blegacy%5D-model-optimizer-extensions/%5Blegacy%5D-graph-transformation-extensions.html">[LEGACY] Graph Transformation Extensions</a></li>
</ul>
</li>
<li class="toctree-l5"><a class="reference internal" href="../documentation/legacy-features/transition-legacy-conversion-api/legacy-model-optimizer-extensibility/%5Blegacy%5D-extending-model-optimizer-with-caffe-python-layers.html">[LEGACY] Extending Model Optimizer with Caffe Python Layers</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../documentation/legacy-features/model-zoo.html">Open Model ZOO</a><input class="toctree-checkbox" id="toctree-checkbox-126" name="toctree-checkbox-126" type="checkbox"/><label for="toctree-checkbox-126"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../omz_models_group_intel.html">Overview of OpenVINO™ Toolkit Intel’s Pre-Trained Models</a></li>
<li class="toctree-l4"><a class="reference internal" href="../omz_models_group_public.html">Overview of OpenVINO™ Toolkit Public Pre-Trained Models</a></li>
<li class="toctree-l4"><a class="reference internal" href="../omz_tools_downloader.html">Model Downloader and other automation tools</a></li>
<li class="toctree-l4"><a class="reference internal" href="../omz_tools_accuracy_checker.html">Deep Learning accuracy validation framework</a></li>
<li class="toctree-l4"><a class="reference internal" href="../omz_data_datasets.html">Dataset Preparation Guide</a></li>
<li class="toctree-l4"><a class="reference internal" href="../omz_demos.html">Open Model Zoo Demos</a></li>
<li class="toctree-l4"><a class="reference internal" href="../omz_model_api_ovms_adapter.html">OpenVINO Model Server Adapter</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../documentation/openvino-ecosystem.html">Tool Ecosystem</a><input class="toctree-checkbox" id="toctree-checkbox-127" name="toctree-checkbox-127" type="checkbox"/><label for="toctree-checkbox-127"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-ecosystem/openvino-training-extensions.html">OpenVINO™ Training Extensions</a></li>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-ecosystem/datumaro.html">Datumaro</a></li>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-ecosystem/openvino-security-add-on.html">OpenVINO™ Security Add-on</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../documentation/openvino-extensibility.html">OpenVINO Extensibility</a><input class="toctree-checkbox" id="toctree-checkbox-128" name="toctree-checkbox-128" type="checkbox"/><label for="toctree-checkbox-128"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-extensibility/custom-openvino-operations.html">Custom OpenVINO Operations</a></li>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-extensibility/frontend-extensions.html">Frontend Extensions</a></li>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-extensibility/custom-gpu-operations.html">How to Implement Custom GPU Operations</a></li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/transformation-api.html">Overview of Transformations API</a><input class="toctree-checkbox" id="toctree-checkbox-129" name="toctree-checkbox-129" type="checkbox"/><label for="toctree-checkbox-129"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/transformation-api/model-pass.html">OpenVINO Model Pass</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/transformation-api/matcher-pass.html">OpenVINO Matcher Pass</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/transformation-api/graph-rewrite-pass.html">OpenVINO Graph Rewrite Pass</a></li>
</ul>
</li>
<li class="toctree-l3 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library.html">OpenVINO Plugin Developer Guide</a><input class="toctree-checkbox" id="toctree-checkbox-130" name="toctree-checkbox-130" type="checkbox"/><label for="toctree-checkbox-130"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/plugin.html">Implement Plugin Functionality</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/compiled-model.html">Implement Compiled Model Functionality</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/synch-inference-request.html">Implement Synchronous Inference Request</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/asynch-inference-request.html">Implement Asynchronous Inference Request</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/plugin-properties.html">Provide Plugin Specific Properties</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/remote-context.html">Implement Remote Context</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/remote-tensor.html">Implement Remote Tensor</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/build-plugin-using-cmake.html">Build Plugin Using CMake</a></li>
<li class="toctree-l4"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/plugin-testing.html">Plugin Testing</a></li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides.html">Advanced Topics</a><input class="toctree-checkbox" id="toctree-checkbox-131" name="toctree-checkbox-131" type="checkbox"/><label for="toctree-checkbox-131"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/quantized-models.html">Quantized models compute and restrictions</a><input class="toctree-checkbox" id="toctree-checkbox-132" name="toctree-checkbox-132" type="checkbox"/><label for="toctree-checkbox-132"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/quantized-models/low-precision-model-representation.html">Representation of low-precision models</a></li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations.html">OpenVINO™ Low Precision Transformations</a><input class="toctree-checkbox" id="toctree-checkbox-133" name="toctree-checkbox-133" type="checkbox"/><label for="toctree-checkbox-133"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/lpt-attributes.html">Attributes</a><input class="toctree-checkbox" id="toctree-checkbox-134" name="toctree-checkbox-134" type="checkbox"/><label for="toctree-checkbox-134"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/lpt-attributes/avg-pool-precision-preserved.html">AvgPoolPrecisionPreserved</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/lpt-attributes/intervals-alignment.html">IntervalsAlignment</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/lpt-attributes/precision-preserved.html">PrecisionPreserved</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/lpt-attributes/precisions.html">Precisions</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/lpt-attributes/quantization-alignment.html">QuantizationAlignment</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/lpt-attributes/quantization-granularity.html">QuantizationGranularity</a></li>
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step1-prerequisites.html">Step 1. Prerequisites transformations</a><input class="toctree-checkbox" id="toctree-checkbox-135" name="toctree-checkbox-135" type="checkbox"/><label for="toctree-checkbox-135"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step1-prerequisites/pull-reshape-through-dequantization.html">PullReshapeThroughDequantization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step1-prerequisites/pull-transpose-through-dequantization.html">PullTransposeThroughDequantization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step1-prerequisites/lin-op-sequence-fusion.html">LinOpSequenceFusion</a></li>
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup.html">Step 2. Markup transformations</a><input class="toctree-checkbox" id="toctree-checkbox-136" name="toctree-checkbox-136" type="checkbox"/><label for="toctree-checkbox-136"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/markup-bias.html">MarkupBias</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/markup-can-be-quantized.html">MarkupCanBeQuantized</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/markup-precisions.html">MarkupPrecisions</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/markup-per-tensor-quantization.html">MarkupPerTensorQuantization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/markup-avg-pool-precision-preserved.html">MarkupAvgPoolPrecisionPreserved</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/propagate-precisions.html">PropagatePrecisions</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/align-quantization-intervals.html">AlignQuantizationIntervals</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/align-quantization-parameters.html">AlignQuantizationParameters</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/create-attribute.html">CreateAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/create-precisions-dependent-attribute.html">CreatePrecisionsDependentAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/propagate-through-precision-preserved.html">PropagateThroughPrecisionPreserved</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/propagate-to-input.html">PropagateToInput</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step2-markup/update-shared-precision-preserved.html">UpdateSharedPrecisionPreserved</a></li>
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main.html">Step 3. Main transformations</a><input class="toctree-checkbox" id="toctree-checkbox-137" name="toctree-checkbox-137" type="checkbox"/><label for="toctree-checkbox-137"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/arithmetic/add.html">AddTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/pooling/avg-pool.html">AvgPoolTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/shape/batch-to-space.html">BatchToSpaceTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/activation/clamp.html">ClampTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/movement/concat.html">ConcatTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/convolution/convolution.html">ConvolutionTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/convolution/convolution-backprop-data.html">ConvolutionBackpropDataTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step4-cleanup/fake-quantize-decomposition.html">FakeQuantizeDecompositionTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/quantization/fake-quantize.html">FakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/image/interpolate.html">InterpolateTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/convolution/group-convolution.html">GroupConvolutionTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/movement/gather.html">GatherTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/matrix/mat-mul.html">MatMulTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/pooling/max-pool.html">MaxPoolTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/arithmetic/multiply-partial.html">MultiplyPartialTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/normalization/mvn.html">MVNTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/normalization/normalize-l2.html">NormalizeL2Transformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/movement/pad.html">PadTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/activation/prelu.html">PReluTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/reduction/reduce-max.html">ReduceMaxTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/reduction/reduce-mean.html">ReduceMeanTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/reduction/reduce-min.html">ReduceMinTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/reduction/reduce-sum.html">ReduceSumTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/activation/relu.html">ReluTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/shape/reshape.html">ReshapeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/shape/space-to-batch.html">SpaceToBatchTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/shape/squeeze.html">SqueezeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/movement/shuffle-channels.html">ShuffleChannelsTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/movement/split.html">SplitTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/movement/strided-slice.html">StridedSliceTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/movement/transpose.html">TransposeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/shape/unsqueeze.html">UnsqueezeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/movement/variadic-split.html">VariadicSplitTransformation</a></li>
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step4-cleanup.html">Step 4. Cleanup transformations</a><input class="toctree-checkbox" id="toctree-checkbox-138" name="toctree-checkbox-138" type="checkbox"/><label for="toctree-checkbox-138"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step4-cleanup/eliminate-fake-quantize.html">EliminateFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step4-cleanup/fold-convert.html">FoldConvertTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step3-main/quantization/fold-fake-quantize.html">FoldFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step4-cleanup/fuse-convert.html">FuseConvertTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step4-cleanup/fuse-multiply-to-fake-quantize.html">FuseMultiplyToFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step4-cleanup/fuse-subtract-to-fake-quantize.html">FuseSubtractToFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/advanced-guides/low-precision-transformations/step4-cleanup/multiply-to-group-convolution.html">MultiplyToGroupConvolutionTransformation</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l4 has-children"><a class="reference internal" href="../documentation/openvino-extensibility/openvino-plugin-library/plugin-api-references.html">Plugin API Reference</a><input class="toctree-checkbox" id="toctree-checkbox-139" name="toctree-checkbox-139" type="checkbox"/><label for="toctree-checkbox-139"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api.html">Group OpenVINO Plugin API</a><input class="toctree-checkbox" id="toctree-checkbox-140" name="toctree-checkbox-140" type="checkbox"/><label for="toctree-checkbox-140"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__plugin__api.html">Plugin base classes</a><input class="toctree-checkbox" id="toctree-checkbox-141" name="toctree-checkbox-141" type="checkbox"/><label for="toctree-checkbox-141"><i class="fas fa-chevron-down"></i></label><ul class="simple">
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__compiled__model__api.html">Compiled Model base classes</a><input class="toctree-checkbox" id="toctree-checkbox-142" name="toctree-checkbox-142" type="checkbox"/><label for="toctree-checkbox-142"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_i_compiled_model.html">ov::ICompiledModel</a></li>
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__infer__request__api.html">Inference Request common classes</a><input class="toctree-checkbox" id="toctree-checkbox-143" name="toctree-checkbox-143" type="checkbox"/><label for="toctree-checkbox-143"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_i_infer_request.html">ov::IInferRequest</a></li>
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__sync__infer__request__api.html">Inference Request base classes</a><input class="toctree-checkbox" id="toctree-checkbox-144" name="toctree-checkbox-144" type="checkbox"/><label for="toctree-checkbox-144"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_i_sync_infer_request.html">ov::ISyncInferRequest</a><input class="toctree-checkbox" id="toctree-checkbox-145" name="toctree-checkbox-145" type="checkbox"/><label for="toctree-checkbox-145"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/structov_1_1_i_sync_infer_request_1_1_found_port.html">ov::ISyncInferRequest::FoundPort</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__async__infer__request__api.html">Asynchronous Inference Request base classes</a><input class="toctree-checkbox" id="toctree-checkbox-146" name="toctree-checkbox-146" type="checkbox"/><label for="toctree-checkbox-146"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_i_async_infer_request.html">ov::IAsyncInferRequest</a><input class="toctree-checkbox" id="toctree-checkbox-147" name="toctree-checkbox-147" type="checkbox"/><label for="toctree-checkbox-147"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/structov_1_1_i_async_infer_request_1_1_disable_callback_guard.html">ov::IAsyncInferRequest::DisableCallbackGuard</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__variable__state__api.html">Variable state base classes</a><input class="toctree-checkbox" id="toctree-checkbox-148" name="toctree-checkbox-148" type="checkbox"/><label for="toctree-checkbox-148"><i class="fas fa-chevron-down"></i></label><ul class="simple">
</ul>
</li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__threading.html">Threading utilities</a><input class="toctree-checkbox" id="toctree-checkbox-149" name="toctree-checkbox-149" type="checkbox"/><label for="toctree-checkbox-149"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1threading_1_1_immediate_executor.html">ov::threading::ImmediateExecutor</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1threading_1_1_c_p_u_streams_executor.html">ov::threading::CPUStreamsExecutor</a></li>
</ul>
</li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__system__conf.html">System configuration utilities</a></li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__exec__model.html">Execution model utilities</a><input class="toctree-checkbox" id="toctree-checkbox-150" name="toctree-checkbox-150" type="checkbox"/><label for="toctree-checkbox-150"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1exec__model__info_1_1_execution_node.html">ov::exec_model_info::ExecutionNode</a></li>
</ul>
</li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__api__error__debug.html">Error handling and debug helpers</a></li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__dev__profiling.html">ITT profiling utilities</a><input class="toctree-checkbox" id="toctree-checkbox-151" name="toctree-checkbox-151" type="checkbox"/><label for="toctree-checkbox-151"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/structopenvino_1_1itt_1_1_scoped_task.html">openvino::itt::ScopedTask</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classopenvino_1_1itt_1_1_task_chain.html">openvino::itt::TaskChain</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l5 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ie__transformation__api.html">Group OpenVINO Transformation API</a><input class="toctree-checkbox" id="toctree-checkbox-152" name="toctree-checkbox-152" type="checkbox"/><label for="toctree-checkbox-152"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/group__ie__runtime__attr__api.html">Runtime information</a></li>
<li class="toctree-l6 has-children"><a class="reference internal" href="../api/c_cpp_api/group__ov__transformation__common__api.html">Common optimization passes</a><input class="toctree-checkbox" id="toctree-checkbox-153" name="toctree-checkbox-153" type="checkbox"/><label for="toctree-checkbox-153"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_add_transformation.html">ov::pass::low_precision::AddTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_align_quantization_intervals.html">ov::pass::low_precision::AlignQuantizationIntervals</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_align_quantization_parameters.html">ov::pass::low_precision::AlignQuantizationParameters</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_avg_pool_transformation.html">ov::pass::low_precision::AvgPoolTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_batch_to_space_transformation.html">ov::pass::low_precision::BatchToSpaceTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_clamp_transformation.html">ov::pass::low_precision::ClampTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_cleanup_transformation.html">ov::pass::low_precision::CleanupTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_concat_transformation.html">ov::pass::low_precision::ConcatTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_convert_subtract_constant.html">ov::pass::low_precision::ConvertSubtractConstant</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_convolution_transformation.html">ov::pass::low_precision::ConvolutionTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_convolution_backprop_data_transformation.html">ov::pass::low_precision::ConvolutionBackpropDataTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_create_attribute.html">ov::pass::low_precision::CreateAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_create_precisions_dependent_attribute.html">ov::pass::low_precision::CreatePrecisionsDependentAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_depth_to_space_transformation.html">ov::pass::low_precision::DepthToSpaceTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_eliminate_fake_quantize_transformation.html">ov::pass::low_precision::EliminateFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_eltwise_base_transformation.html">ov::pass::low_precision::EltwiseBaseTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_fake_quantize_transformation.html">ov::pass::low_precision::FakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_fake_quantize_decomposition_transformation.html">ov::pass::low_precision::FakeQuantizeDecompositionTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_fold_convert_transformation.html">ov::pass::low_precision::FoldConvertTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_fold_fake_quantize_transformation.html">ov::pass::low_precision::FoldFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_fuse_convert_transformation.html">ov::pass::low_precision::FuseConvertTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_fuse_elementwise_to_fake_quantize_transformation.html">ov::pass::low_precision::FuseElementwiseToFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_fuse_multiply_to_fake_quantize_transformation.html">ov::pass::low_precision::FuseMultiplyToFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_fuse_subtract_to_fake_quantize_transformation.html">ov::pass::low_precision::FuseSubtractToFakeQuantizeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_group_convolution_transformation.html">ov::pass::low_precision::GroupConvolutionTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_interpolate_transformation.html">ov::pass::low_precision::InterpolateTransformation</a></li>
<li class="toctree-l7 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_layer_transformation.html">ov::pass::low_precision::LayerTransformation</a><input class="toctree-checkbox" id="toctree-checkbox-154" name="toctree-checkbox-154" type="checkbox"/><label for="toctree-checkbox-154"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_params.html">ov::pass::low_precision::LayerTransformation::Params</a></li>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_layer_transformation_1_1_precision_details.html">ov::pass::low_precision::LayerTransformation::PrecisionDetails</a></li>
</ul>
</li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_markup_avg_pool_precision_preserved.html">ov::pass::low_precision::MarkupAvgPoolPrecisionPreserved</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_markup_bias.html">ov::pass::low_precision::MarkupBias</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_markup_can_be_quantized.html">ov::pass::low_precision::MarkupCanBeQuantized</a></li>
<li class="toctree-l7 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_markup_precisions.html">ov::pass::low_precision::MarkupPrecisions</a><input class="toctree-checkbox" id="toctree-checkbox-155" name="toctree-checkbox-155" type="checkbox"/><label for="toctree-checkbox-155"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_markup_precisions_1_1_restriction.html">ov::pass::low_precision::MarkupPrecisions::Restriction</a></li>
</ul>
</li>
<li class="toctree-l7 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_markup_quantization_granularity.html">ov::pass::low_precision::MarkupQuantizationGranularity</a><input class="toctree-checkbox" id="toctree-checkbox-156" name="toctree-checkbox-156" type="checkbox"/><label for="toctree-checkbox-156"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_markup_quantization_granularity_1_1_per_tensor_quantization.html">ov::pass::low_precision::MarkupQuantizationGranularity::PerTensorQuantization</a></li>
</ul>
</li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_mat_mul_transformation.html">ov::pass::low_precision::MatMulTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_max_pool_transformation.html">ov::pass::low_precision::MaxPoolTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_multiply_transformation.html">ov::pass::low_precision::MultiplyTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_multiply_partial_transformation.html">ov::pass::low_precision::MultiplyPartialTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_multiply_to_group_convolution_transformation.html">ov::pass::low_precision::MultiplyToGroupConvolutionTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_m_v_n_transformation.html">ov::pass::low_precision::MVNTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_normalize_l2_transformation.html">ov::pass::low_precision::NormalizeL2Transformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_pad_transformation.html">ov::pass::low_precision::PadTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_p_relu_transformation.html">ov::pass::low_precision::PReluTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_propagate_precisions.html">ov::pass::low_precision::PropagatePrecisions</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_propagate_shared_value.html">ov::pass::low_precision::PropagateSharedValue</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_propagate_through_precision_preserved.html">ov::pass::low_precision::PropagateThroughPrecisionPreserved</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_propagate_to_input.html">ov::pass::low_precision::PropagateToInput</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_pull_reshape_through_dequantization.html">ov::pass::low_precision::PullReshapeThroughDequantization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_pull_transpose_through_dequantization.html">ov::pass::low_precision::PullTransposeThroughDequantization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_reduce_base_transformation.html">ov::pass::low_precision::ReduceBaseTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_reduce_max_transformation.html">ov::pass::low_precision::ReduceMaxTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_reduce_mean_transformation.html">ov::pass::low_precision::ReduceMeanTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_reduce_min_transformation.html">ov::pass::low_precision::ReduceMinTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_reduce_sum_transformation.html">ov::pass::low_precision::ReduceSumTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_relu_transformation.html">ov::pass::low_precision::ReluTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_reshape_transformation.html">ov::pass::low_precision::ReshapeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_avg_pool_precision_preserved_attribute.html">ov::AvgPoolPrecisionPreservedAttribute</a></li>
<li class="toctree-l7 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_intervals_alignment_shared_value.html">ov::IntervalsAlignmentSharedValue</a><input class="toctree-checkbox" id="toctree-checkbox-157" name="toctree-checkbox-157" type="checkbox"/><label for="toctree-checkbox-157"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_intervals_alignment_shared_value_1_1_interval.html">ov::IntervalsAlignmentSharedValue::Interval</a></li>
</ul>
</li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_intervals_alignment_attribute.html">ov::IntervalsAlignmentAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_precision_preserved_attribute.html">ov::PrecisionPreservedAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_precisions_attribute.html">ov::PrecisionsAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_quantization_alignment_attribute.html">ov::QuantizationAlignmentAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1_quantization_granularity_attribute.html">ov::QuantizationGranularityAttribute</a></li>
<li class="toctree-l7 has-children"><a class="reference internal" href="../api/c_cpp_api/class_shared_attribute_1_1_shared_value_attribute.html">SharedAttribute::SharedValueAttribute</a><input class="toctree-checkbox" id="toctree-checkbox-158" name="toctree-checkbox-158" type="checkbox"/><label for="toctree-checkbox-158"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/struct_shared_attribute_1_1_shared_value_attribute_1_1_shared_value.html">SharedAttribute::SharedValueAttribute::SharedValue</a></li>
</ul>
</li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_shuffle_channels_transformation.html">ov::pass::low_precision::ShuffleChannelsTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_space_to_batch_transformation.html">ov::pass::low_precision::SpaceToBatchTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_split_transformation.html">ov::pass::low_precision::SplitTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_squeeze_transformation.html">ov::pass::low_precision::SqueezeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_strided_slice_transformation.html">ov::pass::low_precision::StridedSliceTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_subtract_transformation.html">ov::pass::low_precision::SubtractTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_transformation_context.html">ov::pass::low_precision::TransformationContext</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_transparent_base_transformation.html">ov::pass::low_precision::TransparentBaseTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_transpose_transformation.html">ov::pass::low_precision::TransposeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_unsqueeze_transformation.html">ov::pass::low_precision::UnsqueezeTransformation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_update_shared_precision_preserved.html">ov::pass::low_precision::UpdateSharedPrecisionPreserved</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_variadic_split_transformation.html">ov::pass::low_precision::VariadicSplitTransformation</a></li>
<li class="toctree-l7 has-children"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1low__precision_1_1_weightable_layer_transformation.html">ov::pass::low_precision::WeightableLayerTransformation</a><input class="toctree-checkbox" id="toctree-checkbox-159" name="toctree-checkbox-159" type="checkbox"/><label for="toctree-checkbox-159"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l8"><a class="reference internal" href="../api/c_cpp_api/structov_1_1pass_1_1low__precision_1_1_weightable_layer_transformation_1_1_can_be_transformed_params.html">ov::pass::low_precision::WeightableLayerTransformation::CanBeTransformedParams</a></li>
</ul>
</li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_init_masks.html">ov::pass::InitMasks</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_init_const_mask.html">ov::pass::InitConstMask</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_propagate_masks.html">ov::pass::PropagateMasks</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_shrink_weights.html">ov::pass::ShrinkWeights</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pruning.html">ov::pass::Pruning</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_adaptive_pool_to_reduce.html">ov::pass::AdaptivePoolToReduce</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_add_fake_quantize_fusion.html">ov::pass::AddFakeQuantizeFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_a_u_g_r_u_cell_fusion.html">ov::pass::AUGRUCellFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_batch_to_space_fusion.html">ov::pass::BatchToSpaceFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_binarize_weights.html">ov::pass::BinarizeWeights</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_broadcast_elementwise_fusion.html">ov::pass::BroadcastElementwiseFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_broadcast_transition.html">ov::pass::BroadcastTransition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_clamp_fusion.html">ov::pass::ClampFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_compress_float_constants_impl.html">ov::pass::CompressFloatConstantsImpl</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_compress_float_constants.html">ov::pass::CompressFloatConstants</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_concat_fusion.html">ov::pass::ConcatFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_replace_concat_reduce_by_min_or_max.html">ov::pass::ReplaceConcatReduceByMinOrMax</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pull_squeeze_through_eltwise.html">ov::pass::PullSqueezeThroughEltwise</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_concat_reduce_fusion.html">ov::pass::ConcatReduceFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_conv_to_binary_conv.html">ov::pass::ConvToBinaryConv</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_nms_gather_path_to_unsigned.html">ov::pass::ConvertNmsGatherPathToUnsigned</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_quantize_dequantize.html">ov::pass::ConvertQuantizeDequantize</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_u4_weights_zero_point_to_scalar.html">ov::pass::ConvertU4WeightsZeroPointToScalar</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convolution_to_group_convolution_fusion.html">ov::pass::ConvolutionToGroupConvolutionFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_depth_to_space_fusion.html">ov::pass::DepthToSpaceFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_dilated_convolution_converter.html">ov::pass::DilatedConvolutionConverter</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_disable_random_uniform_constant_folding.html">ov::pass::DisableRandomUniformConstantFolding</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_divide_fusion.html">ov::pass::DivideFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_dropout_with_random_uniform_replacer.html">ov::pass::DropoutWithRandomUniformReplacer</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_unsqueeze_gather.html">ov::pass::EliminateUnsqueezeGather</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_gather_unsqueeze.html">ov::pass::EliminateGatherUnsqueeze</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_enable_shape_of_constant_folding.html">ov::pass::EnableShapeOfConstantFolding</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_fake_quantize_mul_fusion.html">ov::pass::FakeQuantizeMulFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_fake_quantize_reshape_fusion.html">ov::pass::FakeQuantizeReshapeFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_r_p_e___fusion.html">ov::pass::RPE_Fusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_fused_names_cleanup.html">ov::pass::FusedNamesCleanup</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gelu_fusion_with_erf_one.html">ov::pass::GeluFusionWithErfOne</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gelu_fusion_with_erf_two.html">ov::pass::GeluFusionWithErfTwo</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gelu_fusion_with_erf_three.html">ov::pass::GeluFusionWithErfThree</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gelu_fusion_with_erf_four.html">ov::pass::GeluFusionWithErfFour</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gelu_fusion_with_tanh.html">ov::pass::GeluFusionWithTanh</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gelu_fusion_with_tanh_no_power.html">ov::pass::GeluFusionWithTanhNoPower</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gelu_fusion.html">ov::pass::GeluFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_g_r_u_cell_fusion.html">ov::pass::GRUCellFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_sigmoid_fusion_with_relu_div.html">ov::pass::HSigmoidFusionWithReluDiv</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_sigmoid_fusion_with_relu_mul.html">ov::pass::HSigmoidFusionWithReluMul</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_sigmoid_fusion_without_relu.html">ov::pass::HSigmoidFusionWithoutRelu</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_sigmoid_fusion_with_clamp_mul.html">ov::pass::HSigmoidFusionWithClampMul</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_sigmoid_fusion_with_clamp_div.html">ov::pass::HSigmoidFusionWithClampDiv</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_sigmoid_fusion.html">ov::pass::HSigmoidFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_swish_fusion_with_relu_div.html">ov::pass::HSwishFusionWithReluDiv</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_swish_fusion_with_relu_mul.html">ov::pass::HSwishFusionWithReluMul</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_swish_fusion_with_h_sigmoid.html">ov::pass::HSwishFusionWithHSigmoid</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_swish_fusion_with_clamp.html">ov::pass::HSwishFusionWithClamp</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_swish_fusion.html">ov::pass::HSwishFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_interpolate_sequence_fusion.html">ov::pass::InterpolateSequenceFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_leaky_relu_fusion.html">ov::pass::LeakyReluFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_lin_op_sequence_fusion.html">ov::pass::LinOpSequenceFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_l_s_t_m_cell_fusion.html">ov::pass::LSTMCellFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mark_precision_sensitive_shape_of_subgraphs.html">ov::pass::MarkPrecisionSensitiveShapeOfSubgraphs</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mark_shape_of_subgraphs.html">ov::pass::MarkShapeOfSubgraphs</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mark_precision_sensitive_constants.html">ov::pass::MarkPrecisionSensitiveConstants</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mark_divides_in_shape_subgraphs.html">ov::pass::MarkDividesInShapeSubgraphs</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mat_mul_multiply_fusion.html">ov::pass::MatMulMultiplyFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mish_fusion.html">ov::pass::MishFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_multiply_convolution_fusion.html">ov::pass::MultiplyConvolutionFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mul_fake_quantize_fusion.html">ov::pass::MulFakeQuantizeFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_m_v_n_fusion_without_constants.html">ov::pass::MVNFusionWithoutConstants</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_m_v_n_fusion_with_constants_inside.html">ov::pass::MVNFusionWithConstantsInside</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_m_v_n_fusion.html">ov::pass::MVNFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_nearest_neighbor_upsampling_fusion.html">ov::pass::NearestNeighborUpsamplingFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_non_zero_horizontal_fusion.html">ov::pass::NonZeroHorizontalFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_pad.html">ov::pass::EliminatePad</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_convert.html">ov::pass::EliminateConvert</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_convert_non_zero.html">ov::pass::EliminateConvertNonZero</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_concat.html">ov::pass::EliminateConcat</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_split.html">ov::pass::EliminateSplit</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_squeeze.html">ov::pass::EliminateSqueeze</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_transpose.html">ov::pass::EliminateTranspose</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_eltwise.html">ov::pass::EliminateEltwise</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_scatter_update.html">ov::pass::EliminateScatterUpdate</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_split_concat.html">ov::pass::EliminateSplitConcat</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eliminate_nop_broadcast.html">ov::pass::EliminateNopBroadcast</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_nop_slice_before_gather_elements.html">ov::pass::NopSliceBeforeGatherElements</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_normalize_l2_fusion.html">ov::pass::NormalizeL2Fusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_useless_slice_eraser.html">ov::pass::UselessSliceEraser</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_grouped_strided_slice_optimizer.html">ov::pass::GroupedStridedSliceOptimizer</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_grouped_slice_to_v_split_optimization.html">ov::pass::GroupedSliceToVSplitOptimization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_strided_slice_optimization.html">ov::pass::StridedSliceOptimization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pad_fusion_avg_pool.html">ov::pass::PadFusionAvgPool</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pad_fusion_convolution.html">ov::pass::PadFusionConvolution</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pad_fusion_convolution_backprop_data.html">ov::pass::PadFusionConvolutionBackpropData</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pad_fusion_group_convolution.html">ov::pass::PadFusionGroupConvolution</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pad_fusion_group_convolution_backprop_data.html">ov::pass::PadFusionGroupConvolutionBackpropData</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_p_relu_fusion_negative_add.html">ov::pass::PReluFusionNegativeAdd</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_p_relu_fusion_negative_sub.html">ov::pass::PReluFusionNegativeSub</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_p_relu_fusion_multiply_add.html">ov::pass::PReluFusionMultiplyAdd</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_p_relu_fusion_multiply_sub.html">ov::pass::PReluFusionMultiplySub</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_p_relu_fusion_abs_sub_mul_mul_add.html">ov::pass::PReluFusionAbsSubMulMulAdd</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_p_relu_fusion_neg_relu_mul_add.html">ov::pass::PReluFusionNegReluMulAdd</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_p_relu_fusion.html">ov::pass::PReluFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pull_unsqueeze_through_reduce.html">ov::pass::PullUnsqueezeThroughReduce</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pull_reshape_through_reduce.html">ov::pass::PullReshapeThroughReduce</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_pull_through_reduce.html">ov::pass::PullThroughReduce</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_push_constant_to_subgraph.html">ov::pass::PushConstantToSubgraph</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_random_uniform_fusion.html">ov::pass::RandomUniformFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reduce_merge.html">ov::pass::ReduceMerge</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reduce_reshape_fusion.html">ov::pass::ReduceReshapeFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_relu_fake_quantize_fusion.html">ov::pass::ReluFakeQuantizeFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_remove_concat_zero_dim_input.html">ov::pass::RemoveConcatZeroDimInput</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reshape_p_relu.html">ov::pass::ReshapePRelu</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reshape_sequence_fusion.html">ov::pass::ReshapeSequenceFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reverse_input_channels_fusion.html">ov::pass::ReverseInputChannelsFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_select_with_one_value_condition.html">ov::pass::SelectWithOneValueCondition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_sequence_fusion.html">ov::pass::SequenceFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_shared_op_optimization.html">ov::pass::SharedOpOptimization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_shuffle_channels_fusion.html">ov::pass::ShuffleChannelsFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_grouped_gather_elimination.html">ov::pass::GroupedGatherElimination</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gather_nop_elimination.html">ov::pass::GatherNopElimination</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_skip_gather_before_transpose_and_reshape.html">ov::pass::SkipGatherBeforeTransposeAndReshape</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_softmax_fusion.html">ov::pass::SoftmaxFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_soft_plus_fusion.html">ov::pass::SoftPlusFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_soft_plus_to_mish_fusion.html">ov::pass::SoftPlusToMishFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_space_to_batch_fusion.html">ov::pass::SpaceToBatchFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_split_concat_pair_to_interpolate_fusion.html">ov::pass::SplitConcatPairToInterpolateFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_split_squeeze_concat_fusion.html">ov::pass::SplitSqueezeConcatFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_conv_strides_propagation.html">ov::pass::ConvStridesPropagation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_supported_nodes_strides_propagation.html">ov::pass::SupportedNodesStridesPropagation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_unsupported_nodes_strides_propagation.html">ov::pass::UnsupportedNodesStridesPropagation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_strides_optimization.html">ov::pass::StridesOptimization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_subtract_fusion.html">ov::pass::SubtractFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_swish_fusion_with_sigmoid.html">ov::pass::SwishFusionWithSigmoid</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_swish_fusion_with_sigmoid_with_beta.html">ov::pass::SwishFusionWithSigmoidWithBeta</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_swish_fusion_with_beta.html">ov::pass::SwishFusionWithBeta</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_swish_fusion_without_beta.html">ov::pass::SwishFusionWithoutBeta</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_swish_fusion.html">ov::pass::SwishFusion</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_transpose_reshape_elimination_for_matmul.html">ov::pass::TransposeReshapeEliminationForMatmul</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_transpose_reduction.html">ov::pass::TransposeReduction</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_transpose_f_q_reduction.html">ov::pass::TransposeFQReduction</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_transpose_convert.html">ov::pass::TransposeConvert</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_transpose_eltwise.html">ov::pass::TransposeEltwise</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_transpose_fuse.html">ov::pass::TransposeFuse</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_transpose_sinking.html">ov::pass::TransposeSinking</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_transpose_to_reshape.html">ov::pass::TransposeToReshape</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_weights_dequantize_to_fake_quantize.html">ov::pass::WeightsDequantizeToFakeQuantize</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_wrap_interpolate_into_transposes.html">ov::pass::WrapInterpolateIntoTransposes</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_unroll_if.html">ov::pass::UnrollIf</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_unroll_tensor_iterator.html">ov::pass::UnrollTensorIterator</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/struct_enum_class_hash.html">EnumClassHash</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_align_mixed_f_p32_f_p16_types.html">ov::pass::AlignMixedFP32FP16Types</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_compressed_only_to_legacy.html">ov::pass::ConvertCompressedOnlyToLegacy</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_enable_decompression_convert_constant_folding.html">ov::pass::EnableDecompressionConvertConstantFolding</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_disable_decompression_convert_constant_folding.html">ov::pass::DisableDecompressionConvertConstantFolding</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_keep_const_and_decompression.html">ov::pass::KeepConstAndDecompression</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_keep_constants_precision_and_add_converts.html">ov::pass::KeepConstantsPrecisionAndAddConverts</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mark_compressed_float_constants.html">ov::pass::MarkCompressedFloatConstants</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_init_node_info.html">ov::pass::InitNodeInfo</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_mark_dequantization_subgraph.html">ov::pass::MarkDequantizationSubgraph</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_bidirectional_l_s_t_m_sequence_decomposition.html">ov::pass::BidirectionalLSTMSequenceDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_bidirectional_g_r_u_sequence_decomposition.html">ov::pass::BidirectionalGRUSequenceDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_bidirectional_r_n_n_sequence_decomposition.html">ov::pass::BidirectionalRNNSequenceDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_bidirectional_sequence_decomposition.html">ov::pass::BidirectionalSequenceDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_batch_to_space.html">ov::pass::ConvertBatchToSpace</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/class_convert_bitwise_to_logical.html">ConvertBitwiseToLogical</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_deformable_conv8_to1.html">ov::pass::ConvertDeformableConv8To1</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_gather0_d.html">ov::pass::ConvertGather0D</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_gather7_to_gather1.html">ov::pass::ConvertGather7ToGather1</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_gather8_to_gather7.html">ov::pass::ConvertGather8ToGather7</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_gather1_to_gather7.html">ov::pass::ConvertGather1ToGather7</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_gather7_to_gather8.html">ov::pass::ConvertGather7ToGather8</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_interpolate11_to_interpolate4.html">ov::pass::ConvertInterpolate11ToInterpolate4</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_interpolate1_to_interpolate4.html">ov::pass::ConvertInterpolate1ToInterpolate4</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_max_pool8_to_max_pool1.html">ov::pass::ConvertMaxPool8ToMaxPool1</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_max_pool1_to_max_pool8.html">ov::pass::ConvertMaxPool1ToMaxPool8</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_m_v_n1_to_m_v_n6.html">ov::pass::ConvertMVN1ToMVN6</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_pad12_to_pad1.html">ov::pass::ConvertPad12ToPad1</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_pad_to_group_convolution.html">ov::pass::ConvertPadToGroupConvolution</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_prior_box8_to0.html">ov::pass::ConvertPriorBox8To0</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_r_o_i_align3_to9.html">ov::pass::ConvertROIAlign3To9</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_r_o_i_align9_to3.html">ov::pass::ConvertROIAlign9To3</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_scatter_elements_to_scatter.html">ov::pass::ConvertScatterElementsToScatter</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_scatter_elements_update12_to_scatter_elements_update3.html">ov::pass::ConvertScatterElementsUpdate12ToScatterElementsUpdate3</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_r_n_n_sequence_to_tensor_iterator.html">ov::pass::ConvertRNNSequenceToTensorIterator</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_g_r_u_sequence_to_tensor_iterator.html">ov::pass::ConvertGRUSequenceToTensorIterator</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_l_s_t_m_sequence_to_tensor_iterator.html">ov::pass::ConvertLSTMSequenceToTensorIterator</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_slice_to_strided_slice.html">ov::pass::SliceToStridedSlice</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_soft_max8_to_soft_max1.html">ov::pass::ConvertSoftMax8ToSoftMax1</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_soft_max1_to_soft_max8.html">ov::pass::ConvertSoftMax1ToSoftMax8</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_space_to_batch.html">ov::pass::ConvertSpaceToBatch</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_tensor_iterator_to_l_s_t_m_sequence.html">ov::pass::ConvertTensorIteratorToLSTMSequence</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_tensor_iterator_to_r_n_n_sequence.html">ov::pass::ConvertTensorIteratorToRNNSequence</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_tensor_iterator_to_g_r_u_sequence.html">ov::pass::ConvertTensorIteratorToGRUSequence</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_loop_to_l_s_t_m_sequence.html">ov::pass::ConvertLoopToLSTMSequence</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_fuse_reverse_l_s_t_m_sequence.html">ov::pass::FuseReverseLSTMSequence</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_fuse_l_s_t_m_sequences_to_bidirectional_l_s_t_m_sequence.html">ov::pass::FuseLSTMSequencesToBidirectionalLSTMSequence</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_top_k11_to_top_k3.html">ov::pass::ConvertTopK11ToTopK3</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_xor_to_logical_xor.html">ov::pass::ConvertXorToLogicalXor</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_detection_output8_to_detection_output1.html">ov::pass::ConvertDetectionOutput8ToDetectionOutput1</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_convert_detection_output1_to_detection_output8.html">ov::pass::ConvertDetectionOutput1ToDetectionOutput8</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_einsum_decomposition.html">ov::pass::EinsumDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_eye_decomposition.html">ov::pass::EyeDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_fake_quantize_decomposition.html">ov::pass::FakeQuantizeDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_gelu7_downgrade.html">ov::pass::Gelu7Downgrade</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_g_r_u_cell_decomposition.html">ov::pass::GRUCellDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_sigmoid_decomposition.html">ov::pass::HSigmoidDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_h_swish_decomposition.html">ov::pass::HSwishDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_log_softmax_decomposition.html">ov::pass::LogSoftmaxDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_l_s_t_m_cell_decomposition.html">ov::pass::LSTMCellDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_m_v_n6_decomposition.html">ov::pass::MVN6Decomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_normalize_l2_decomposition.html">ov::pass::NormalizeL2Decomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reduce_l1_decomposition.html">ov::pass::ReduceL1Decomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reduce_l2_decomposition.html">ov::pass::ReduceL2Decomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_r_n_n_cell_decomposition.html">ov::pass::RNNCellDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_softmax_decomposition.html">ov::pass::SoftmaxDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_soft_plus_decomposition.html">ov::pass::SoftPlusDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_soft_sign_decomposition.html">ov::pass::SoftSignDecomposition</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_resolve_name_collisions.html">ov::pass::ResolveNameCollisions</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_broadcast_const_range_replacement.html">ov::pass::BroadcastConstRangeReplacement</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_l_s_t_m_states_broadcast.html">ov::pass::LSTMStatesBroadcast</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reshape_a_mat_mul.html">ov::pass::ReshapeAMatMul</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_proposal1_scales.html">ov::pass::Proposal1Scales</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reshape_sinking_mat_mul.html">ov::pass::ReshapeSinkingMatMul</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reshape_to1_d.html">ov::pass::ReshapeTo1D</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_shape_of_const_folding.html">ov::pass::ShapeOfConstFolding</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_strided_slice_squeeze.html">ov::pass::StridedSliceSqueeze</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_squeeze_strided_slice.html">ov::pass::SqueezeStridedSlice</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_chained_maximum_optimization.html">ov::pass::ChainedMaximumOptimization</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_de_reshape_mat_mul.html">ov::pass::DeReshapeMatMul</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_de_reshape_fully_connected.html">ov::pass::DeReshapeFullyConnected</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_nop_broadcast.html">ov::pass::NopBroadcast</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_reshape_optimizations.html">ov::pass::ReshapeOptimizations</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_apply_symbol_equivalence.html">ov::pass::ApplySymbolEquivalence</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_optimize_symbols_used_as_values.html">ov::pass::OptimizeSymbolsUsedAsValues</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_symbolic_optimizations.html">ov::pass::SymbolicOptimizations</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_symbolic_propagation.html">ov::pass::SymbolicPropagation</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1_label_resolving_through_select.html">ov::pass::LabelResolvingThroughSelect</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_forward_base.html">ov::pass::transpose_sinking::TSForwardBase</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_binary_forward.html">ov::pass::transpose_sinking::TSBinaryForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_binary_backward.html">ov::pass::transpose_sinking::TSBinaryBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_concat_forward.html">ov::pass::transpose_sinking::TSConcatForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_concat_backward.html">ov::pass::transpose_sinking::TSConcatBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_cum_sum_forward.html">ov::pass::transpose_sinking::TSCumSumForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_cum_sum_backward.html">ov::pass::transpose_sinking::TSCumSumBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_data_movement_forward.html">ov::pass::transpose_sinking::TSDataMovementForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_data_movement_backward.html">ov::pass::transpose_sinking::TSDataMovementBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_fuse.html">ov::pass::transpose_sinking::TSFuse</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_gather_forward.html">ov::pass::transpose_sinking::TSGatherForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_gather_backward.html">ov::pass::transpose_sinking::TSGatherBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_general_forward.html">ov::pass::transpose_sinking::TSGeneralForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_general_backward.html">ov::pass::transpose_sinking::TSGeneralBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_general.html">ov::pass::transpose_sinking::TSGeneral</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_interpolate_forward.html">ov::pass::transpose_sinking::TSInterpolateForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_interpolate_backward.html">ov::pass::transpose_sinking::TSInterpolateBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_reduction_forward.html">ov::pass::transpose_sinking::TSReductionForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_reduction_backward.html">ov::pass::transpose_sinking::TSReductionBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_reset_no_sinking_attribute.html">ov::pass::transpose_sinking::TSResetNoSinkingAttribute</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_shape_of_forward.html">ov::pass::transpose_sinking::TSShapeOfForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_split_forward.html">ov::pass::transpose_sinking::TSSplitForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_split_backward.html">ov::pass::transpose_sinking::TSSplitBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_squeeze_forward.html">ov::pass::transpose_sinking::TSSqueezeForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_squeeze_backward.html">ov::pass::transpose_sinking::TSSqueezeBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_tile_forward.html">ov::pass::transpose_sinking::TSTileForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_tile_backward.html">ov::pass::transpose_sinking::TSTileBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_unary_forward.html">ov::pass::transpose_sinking::TSUnaryForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_unary_backward.html">ov::pass::transpose_sinking::TSUnaryBackward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_unsqueeze_forward.html">ov::pass::transpose_sinking::TSUnsqueezeForward</a></li>
<li class="toctree-l7"><a class="reference internal" href="../api/c_cpp_api/classov_1_1pass_1_1transpose__sinking_1_1_t_s_unsqueeze_backward.html">ov::pass::transpose_sinking::TSUnsqueezeBackward</a></li>
</ul>
</li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/group__ie__transformation__to__opset2__api.html">Conversion from opset3 to opset2</a></li>
<li class="toctree-l6"><a class="reference internal" href="../api/c_cpp_api/group__ie__transformation__to__opset1__api.html">Conversion from opset2 to opset1</a></li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="../documentation/openvino-security.html">OpenVINO™ Security</a><input class="toctree-checkbox" id="toctree-checkbox-160" name="toctree-checkbox-160" type="checkbox"/><label for="toctree-checkbox-160"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="../documentation/openvino-security/openvino-encrypted-models.html">Using Encrypted Models with OpenVINO</a></li>
</ul>
</li>
</ul>
</li>
<li class="toctree-l1 current active has-children"><a class="reference internal" href="../about-openvino.html">ABOUT OPENVINO</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-161" name="toctree-checkbox-161" type="checkbox"/><label for="toctree-checkbox-161"><i class="fas fa-chevron-down"></i></label><ul class="current">
<li class="toctree-l2 current active has-children"><a class="current reference internal" href="#">Performance Benchmarks</a><input checked="" class="toctree-checkbox" id="toctree-checkbox-162" name="toctree-checkbox-162" type="checkbox"/><label for="toctree-checkbox-162"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="performance-benchmarks/performance-benchmarks-faq.html">Performance Information F.A.Q.</a></li>
<li class="toctree-l3"><a class="reference internal" href="performance-benchmarks/model-accuracy-int8-fp32.html">OpenVINO Accuracy</a></li>
<li class="toctree-l3"><a class="reference internal" href="performance-benchmarks/getting-performance-numbers.html">Getting Performance Numbers</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="compatibility-and-support.html">Compatibility and Support</a><input class="toctree-checkbox" id="toctree-checkbox-163" name="toctree-checkbox-163" type="checkbox"/><label for="toctree-checkbox-163"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="compatibility-and-support/supported-devices.html">Inference Device Support</a></li>
<li class="toctree-l3"><a class="reference internal" href="compatibility-and-support/supported-operations-inference-devices.html">Supported Operations - by Inference Devices</a></li>
<li class="toctree-l3"><a class="reference internal" href="compatibility-and-support/supported-operations-framework-frontend.html">Supported Operations - by Framework Frontend</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="release-notes-openvino.html">Release Notes</a><input class="toctree-checkbox" id="toctree-checkbox-164" name="toctree-checkbox-164" type="checkbox"/><label for="toctree-checkbox-164"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="release-notes-openvino/system-requirements.html">System Requirements</a></li>
<li class="toctree-l3"><a class="reference internal" href="release-notes-openvino/release-policy.html">Release Policy</a></li>
</ul>
</li>
<li class="toctree-l2 has-children"><a class="reference internal" href="additional-resources.html">Additional Resources</a><input class="toctree-checkbox" id="toctree-checkbox-165" name="toctree-checkbox-165" type="checkbox"/><label for="toctree-checkbox-165"><i class="fas fa-chevron-down"></i></label><ul>
<li class="toctree-l3"><a class="reference internal" href="additional-resources/glossary.html">Glossary</a></li>
<li class="toctree-l3"><a class="reference internal" href="additional-resources/legal-information.html">Legal Information</a></li>
<li class="toctree-l3"><a class="reference internal" href="additional-resources/telemetry.html">OpenVINO™ Telemetry</a></li>
<li class="toctree-l3"><a class="reference external" href="https://www.intel.com/openvino-success-stories">Case Studies</a></li>
</ul>
</li>
</ul>
</li>
</ul>

    </div>
  </nav>
  
            </div>
            
          

          
          <div class="d-none d-xl-block col-xl-2 bd-toc">
            
              
              <div class="toc-item">
                

<div class="tocsection onthispage pt-5 pb-3">
    On this page
</div>

<nav id="bd-toc-nav">
    
</nav>
              </div>
              
              <div class="toc-item">
                <div class="tocsection download-docs">
  <div class="dropdown sst-dropdown">
    <button class="button bttn-prm button-size-m" data-display="static" type="button" id="download-options"
      data-toggle="dropdown" aria-haspopup="true" aria-expanded="false">
      Download Docs
    </button>
    <div class="dropdown-menu" aria-labelledby="download-options">
      <a class="dropdown-item" href="#" onclick="window.print()">.pdf</a>
      <a id="download-zip-btn" class="dropdown-item" href="#">.zip</a>
    </div>
  </div>
</div>
              </div>
              
            
          </div>
          

          
          
              
          
          <main class="col-12 col-md-9 col-xl-7 py-md-5 pl-md-5 pr-md-4 bd-content" role="main">
            
                <div>
                  
  <div class="section" id="performance-benchmarks">
<h1>Performance Benchmarks<a class="headerlink" href="#performance-benchmarks" title="Permalink to this headline">¶</a></h1>
<div class="toctree-wrapper compound">
</div>
<p>This page presents benchmark results for
<a class="reference external" href="https://software.intel.com/content/www/us/en/develop/tools/openvino-toolkit.html">Intel® Distribution of OpenVINO™ toolkit</a>
and <a class="reference internal" href="../ovms_what_is_openvino_model_server.html"><span class="doc">OpenVINO Model Server</span></a>, for a representative
selection of public neural networks and Intel® devices. The results may help you decide which
hardware to use in your applications or plan AI workload for the hardware you have already
implemented in your solutions. Click the buttons below to see the chosen benchmark data.</p>
<div class="sd-container-fluid sd-sphinx-override sd-mb-4 docutils">
<div class="sd-row sd-row-cols-1 sd-row-cols-xs-1 sd-row-cols-sm-1 sd-row-cols-md-2 sd-row-cols-lg-2 sd-g-4 sd-g-xs-4 sd-g-sm-4 sd-g-md-4 sd-g-lg-4 docutils">
<div class="sd-col sd-d-flex-column docutils">
<p><span class="sd-d-grid"><a class="sd-sphinx-override sd-btn sd-text-wrap sd-btn-outline-primary ov-toolkit-benchmark-results reference external" href="#"><span><svg version="4.0.0.63c5cb3" width="1.4em" height="1.4em" class="sd-material-icon sd-material-icon-bar_chart" viewBox="0 0 24 24" aria-hidden="true"><path d="M0 0h24v24H0z" fill="none"></path><path d="M5 9.2h3V19H5zM10.6 5h2.8v14h-2.8zm5.6 8H19v6h-2.8z"></path></svg> OpenVINO Benchmark Graphs</span></a></span></p>
</div>
<div class="sd-col sd-d-flex-column docutils">
<p><span class="sd-d-grid"><a class="sd-sphinx-override sd-btn sd-text-wrap sd-btn-outline-primary ovms-toolkit-benchmark-results reference external" href="#"><span><svg version="4.0.0.63c5cb3" width="1.4em" height="1.4em" class="sd-material-icon sd-material-icon-bar_chart" viewBox="0 0 24 24" aria-hidden="true"><path d="M0 0h24v24H0z" fill="none"></path><path d="M5 9.2h3V19H5zM10.6 5h2.8v14h-2.8zm5.6 8H19v6h-2.8z"></path></svg> OVMS Benchmark Graphs</span></a></span></p>
</div>
</div>
</div>
<p>Please visit the tabs below for more information on key performance indicators and workload parameters.</p>
<div class="sd-tab-set docutils">
<input checked="checked" id="sd-tab-item-0" name="sd-tab-set-0" type="radio">
</input><label class="sd-tab-label" data-sync-id="throughput" for="sd-tab-item-0">
Throughput</label><div class="sd-tab-content docutils">
<p>Measures the number of inferences delivered within a latency threshold
(for example, number of Frames Per Second - FPS). When deploying a system with
deep learning inference, select the throughput that delivers the best trade-off
between latency and power for the price and performance that meets your requirements.</p>
</div>
<input id="sd-tab-item-1" name="sd-tab-set-0" type="radio">
</input><label class="sd-tab-label" data-sync-id="value" for="sd-tab-item-1">
Value</label><div class="sd-tab-content docutils">
<p>While throughput is important, what is more critical in edge AI deployments is
the performance efficiency or performance-per-cost. Application performance in
throughput per dollar of system cost is the best measure of value. The value KPI is
calculated as “Throughput measured as inferences per second / price of inference engine”.
This means for a 2 socket system 2x the price of a CPU is used. Prices are as per
date of benchmarking and sources can be found as links in the Hardware Platforms (PDF)
description below.</p>
</div>
<input id="sd-tab-item-2" name="sd-tab-set-0" type="radio">
</input><label class="sd-tab-label" data-sync-id="efficiency" for="sd-tab-item-2">
Efficiency</label><div class="sd-tab-content docutils">
<p>System power is a key consideration from the edge to the data center. When selecting
deep learning solutions, power efficiency (throughput/watt) is a critical factor to
consider. Intel designs provide excellent power efficiency for running deep learning
workloads. The efficiency KPI is calculated as “Throughput measured as inferences per
second / TDP of inference engine”. This means for a 2 socket system 2x the power
dissipation (TDP) of a CPU is used. TDP-values are as per date of benchmarking and sources
can be found as links in the Hardware Platforms (PDF) description below.</p>
</div>
<input id="sd-tab-item-3" name="sd-tab-set-0" type="radio">
</input><label class="sd-tab-label" data-sync-id="latency" for="sd-tab-item-3">
Latency</label><div class="sd-tab-content docutils">
<p>This measures the synchronous execution of inference requests and is reported in
milliseconds. Each inference request (for example: preprocess, infer, postprocess) is
allowed to complete before the next is started. This performance metric is relevant in
usage scenarios where a single image input needs to be acted upon as soon as possible. An
example would be the healthcare sector where medical personnel only request analysis of a
single ultra sound scanning image or in real-time or near real-time applications for
example an industrial robot’s response to actions in its environment or obstacle avoidance
for autonomous vehicles.</p>
</div>
<input id="sd-tab-item-4" name="sd-tab-set-0" type="radio">
</input><label class="sd-tab-label" data-sync-id="workloadparameters" for="sd-tab-item-4">
Workload Parameters</label><div class="sd-tab-content docutils">
<p>The workload parameters affect the performance results of the different models we use for
benchmarking. Image processing models have different image size definitions and the
Natural Language Processing models have different max token list lengths. All these can
be found in detail in the <a class="reference internal" href="performance-benchmarks/performance-benchmarks-faq.html"><span class="doc">FAQ section</span></a>.
All models are executed using a batch size of 1. Below are the parameters for the GenAI
models we display.</p>
<ul class="simple">
<li><p>Input tokens: 1024,</p></li>
<li><p>Output tokens: 128,</p></li>
<li><p>number of beams: 1</p></li>
</ul>
<p>For text to image:</p>
<ul class="simple">
<li><p>iteration steps: 20,</p></li>
<li><p>image size (HxW): 256 x 256,</p></li>
<li><p>input token length: 1024 (the tokens for GenAI models are in English).</p></li>
</ul>
</div>
</div>
<h2>Platforms, Configurations, Methodology</h2><p>For a listing of all platforms and configurations used for testing, refer to the following:</p>
<div class="sd-container-fluid sd-sphinx-override sd-mb-4 docutils">
<div class="sd-row sd-row-cols-1 sd-row-cols-xs-1 sd-row-cols-sm-1 sd-row-cols-md-2 sd-row-cols-lg-2 sd-g-4 sd-g-xs-4 sd-g-sm-4 sd-g-md-4 sd-g-lg-4 docutils">
<div class="sd-col sd-d-flex-column docutils">
<p><span class="sd-d-grid"><a class="sd-sphinx-override sd-btn sd-text-wrap sd-btn-outline-primary reference external" href="../_static/benchmarks_files/OV-2024.1-platform_list.pdf"><span><svg version="4.0.0.63c5cb3" width="1.5em" height="1.5em" class="sd-material-icon sd-material-icon-download" viewBox="0 0 24 24" aria-hidden="true"><g><rect fill="none" height="24" width="24"></rect></g><g><path d="M5,20h14v-2H5V20z M19,9h-4V3H9v6H5l7,7L19,9z"></path></g></svg> Click for Hardware Platforms [PDF]</span></a></span></p>
<p><span class="sd-d-grid"><a class="sd-sphinx-override sd-btn sd-text-wrap sd-btn-outline-primary reference external" href="../_static/benchmarks_files/OV-2024.1-system-info-detailed.xlsx"><span><svg version="4.0.0.63c5cb3" width="1.5em" height="1.5em" class="sd-material-icon sd-material-icon-download" viewBox="0 0 24 24" aria-hidden="true"><g><rect fill="none" height="24" width="24"></rect></g><g><path d="M5,20h14v-2H5V20z M19,9h-4V3H9v6H5l7,7L19,9z"></path></g></svg> Click for Configuration Details [XLSX]</span></a></span></p>
<p><span class="sd-d-grid"><a class="sd-sphinx-override sd-btn sd-text-wrap sd-btn-outline-primary reference external" href="../_static/benchmarks_files/OV-2024.1-Performance-Data.xlsx"><span><svg version="4.0.0.63c5cb3" width="1.5em" height="1.5em" class="sd-material-icon sd-material-icon-download" viewBox="0 0 24 24" aria-hidden="true"><g><rect fill="none" height="24" width="24"></rect></g><g><path d="M5,20h14v-2H5V20z M19,9h-4V3H9v6H5l7,7L19,9z"></path></g></svg> Click for Performance Data [XLSX]</span></a></span></p>
</div>
</div>
</div>
<p>The OpenVINO benchmark setup includes a single system with OpenVINO™, as well as the benchmark
application installed. It measures the time spent on actual inference (excluding any pre or post
processing) and then reports on the inferences per second (or Frames Per Second).</p>
<p>OpenVINO™ Model Server (OVMS) employs the Intel® Distribution of OpenVINO™ toolkit runtime
libraries and exposes a set of models via a convenient inference API over gRPC or HTTP/REST.
Its benchmark results are measured with the configuration of multiple-clients-single-server,
using two hardware platforms connected by ethernet. Network bandwidth depends on both, platforms
and models under investigation. It is set not to be a bottleneck for workload intensity. The
connection is dedicated only to measuring performance.</p>
<details class="sd-sphinx-override sd-dropdown sd-card sd-mb-3">
<summary class="sd-summary-title sd-card-header">
See more details about OVMS benchmark setup<div class="sd-summary-down docutils">
<svg version="1.1" width="1.5em" height="1.5em" class="sd-octicon sd-octicon-chevron-down" viewBox="0 0 24 24" aria-hidden="true"><path fill-rule="evenodd" d="M5.22 8.72a.75.75 0 000 1.06l6.25 6.25a.75.75 0 001.06 0l6.25-6.25a.75.75 0 00-1.06-1.06L12 14.44 6.28 8.72a.75.75 0 00-1.06 0z"></path></svg></div>
<div class="sd-summary-up docutils">
<svg version="1.1" width="1.5em" height="1.5em" class="sd-octicon sd-octicon-chevron-up" viewBox="0 0 24 24" aria-hidden="true"><path fill-rule="evenodd" d="M18.78 15.28a.75.75 0 000-1.06l-6.25-6.25a.75.75 0 00-1.06 0l-6.25 6.25a.75.75 0 101.06 1.06L12 9.56l5.72 5.72a.75.75 0 001.06 0z"></path></svg></div>
</summary><div class="sd-summary-content sd-card-body docutils">
<p class="sd-card-text">The benchmark setup for OVMS consists of four main parts:</p>
<img alt="OVMS Benchmark Setup Diagram" src="../_images/performance_benchmarks_ovms_02.png" />
<ul class="simple">
<li><p class="sd-card-text"><strong>OpenVINO™ Model Server</strong> is launched as a docker container on the server platform and it
listens to (and answers) requests from clients. OpenVINO™ Model Server is run on the same
system as the OpenVINO™ toolkit benchmark application in corresponding benchmarking. Models
served by OpenVINO™ Model Server are located in a local file system mounted into the docker
container. The OpenVINO™ Model Server instance communicates with other components via ports
over a dedicated docker network.</p></li>
<li><p class="sd-card-text"><strong>Clients</strong> are run in separated physical machine referred to as client platform. Clients
are implemented in Python3 programming language based on TensorFlow* API and they work as
parallel processes. Each client waits for a response from OpenVINO™ Model Server before it
will send a new next request. The role played by the clients is also verification of
responses.</p></li>
<li><p class="sd-card-text"><strong>Load balancer</strong> works on the client platform in a docker container. HAProxy is used for
this purpose. Its main role is counting of requests forwarded from clients to OpenVINO™
Model Server, estimating its latency, and sharing this information by Prometheus service.
The reason of locating the load balancer on the client site is to simulate real life
scenario that includes impact of physical network on reported metrics.</p></li>
<li><p class="sd-card-text"><strong>Execution Controller</strong> is launched on the client platform. It is responsible for
synchronization of the whole measurement process, downloading metrics from the load
balancer, and presenting the final report of the execution.</p></li>
</ul>
</div>
</details><h2>Test performance yourself</h2><p>You can also test performance for your system yourself, following the guide on
<a class="reference internal" href="performance-benchmarks/getting-performance-numbers.html"><span class="doc">getting performance numbers</span></a>.</p>
<p>Performance of a particular application can also be evaluated virtually using
<a class="reference external" href="https://devcloud.intel.com/edge/">Intel® DevCloud for the Edge</a>.
It is a remote development environment with access to Intel® hardware and the latest versions
of the Intel® Distribution of the OpenVINO™ Toolkit. To learn more about it, visit
<a class="reference external" href="https://www.intel.com/content/www/us/en/developer/tools/devcloud/edge/overview.html">the website</a>
or
<a class="reference external" href="https://www.intel.com/content/www/us/en/secure/forms/devcloud-enrollment/account-provisioning.html">create an account</a>.</p>
<h2>Disclaimers</h2><ul class="simple">
<li><p>Intel® Distribution of OpenVINO™ toolkit performance results are based on release
2024.1, as of April 17, 2024.</p></li>
<li><p>OpenVINO Model Server performance results are based on release
2024.0, as of March 15, 2024.</p></li>
</ul>
<p>The results may not reflect all publicly available updates. Intel technologies’ features and
benefits depend on system configuration and may require enabled hardware, software, or service
activation. Learn more at intel.com, or from the OEM or retailer.</p>
<p>See configuration disclosure for details. No product can be absolutely secure.
Performance varies by use, configuration and other factors. Learn more at
<a class="reference external" href="https://www.intel.com/PerformanceIndex">www.intel.com/PerformanceIndex</a>.
Your costs and results may vary.
Intel optimizations, for Intel compilers or other products, may not optimize to the same degree
for non-Intel products.</p>
<link rel="stylesheet" type="text/css" href="../_static/css/benchmark-banner.css"><div class="benchmark-banner docutils container">
<p>Results may vary. For more information, see
<a class="reference internal" href="performance-benchmarks/performance-benchmarks-faq.html"><span class="doc">F.A.Q.</span></a>
See <a class="reference internal" href="additional-resources/legal-information.html"><span class="doc">Legal Information</span></a>.</p>
</div>
</div>


                </div>
            
            
          </main>
          

      </div>
    </div>
  
  <script src="../_static/js/index.be7d3bbb2ef33a8344ce.js"></script>
<footer class="footer mt-5 mt-md-0">
</footer>
  </body>
</html>
