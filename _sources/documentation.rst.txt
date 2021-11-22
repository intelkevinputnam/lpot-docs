Documentation
###############

Get Started
#############

* `Introduction <docs/api-introduction.md>`__ explains Intel® Neural Compressor's API.
* `Transform <docs/transform.md>`__ introduces how to utilize Intel® Neural Compressor's built-in data processing and how to develop a custom data processing method.
* `Dataset <docs/dataset.md>`__ introduces how to utilize Intel® Neural Compressor's built-in dataset and how to develop a custom dataset.
* `Metric <docs/metric.md>`__ introduces how to utilize Intel® Neural Compressor's built-in metrics and how to develop a custom metric.
* `Tutorial <docs/tutorial.md>`__ provides comprehensive instructions on how to utilize Intel® Neural Compressor's features with examples.
* `Examples <examples_readme.md>`__ are provided to demonstrate the usage of Intel® Neural Compressor in different frameworks: TensorFlow, PyTorch, MXNet, and ONNX Runtime.
* `UX <docs/ux.md>`__ is a web-based system used to simplify Intel® Neural Compressor usage.
* `Intel oneAPI AI Analytics Toolkit Get Started Guide <https://software.intel.com/content/www/us/en/develop/documentation/get-started-with-ai-linux/top.html>`__ explains the AI Kit components, installation and configuration guides, and instructions for building and running sample apps.
* `AI and Analytics Samples  <https://github.com/oneapi-src/oneAPI-samples/tree/master/AI-and-Analytics>`__ includes code samples for Intel oneAPI libraries.

.. toctree::
   :hidden:
   
   Introduction <README.md>
   APIs <docs/api-introduction.md>
   Transform <docs/transform.md>
   Dataset <docs/dataset.md>
   Metric <docs/metric.md>
   Tutorial <docs/tutorial.md>
   Examples <examples_readme.md>
   UX <docs/ux.md>

Deep Dive
############

* `Quantization <docs/Quantization.md>`__ are processes that enable inference and training by performing computations at low-precision data types, such as fixed-point integers. Intel® Neural Compressor supports Post-Training Quantization `PTQ <docs/PTQ.md>`__) with `different quantization capabilities <docs/backend_quant.md>`__ and Quantization-Aware Training (`QAT <docs/QAT.md)>`__). Note that (`Dynamic Quantization <docs/dynamic_quantization.md>`__) currently has limited support.
* `Pruning <docs/pruning.md>`__ provides a common method for introducing sparsity in weights and activations.
* `Benchmarking <docs/benchmark.md>`__ introduces how to utilize the benchmark interface of Intel® Neural Compressor.
* `Mixed precision <docs/mixed_precision.md>`__ introduces how to enable mixed precision, including BFP16 and int8 and FP32, on Intel platforms during tuning.
* `Graph Optimization <docs/graph_optimization.md>`__ introduces how to enable graph optimization for FP32 and auto-mixed precision.
* `Model Conversion <docs/model_conversion.md>`__ introduces how to convert TensorFlow QAT model to quantized model running on Intel platforms.
* `TensorBoard <docs/tensorboard.md>`__ provides tensor histograms and execution graphs for tuning debugging purposes.

.. toctree::
   :hidden:

   Quantization <docs/Quantization.md>
   Pruning <docs/pruning.md>
   Benchmarking <docs/benchmark.md
   Mixed precision <docs/mixed_precision.md
   Graph Optimization <docs/graph_optimization.md
   Model Conversion <docs/model_conversion.md>
   TensorBoard <docs/tensorboard.md>

Advanced Topics
##################


* `Adaptor <docs/adaptor.md>`__ is the interface between Intel® Neural Compressor and framework. The method to develop adaptor extension is introduced with ONNX Runtime as example.
* `Strategy <docs/tuning_strategies.md>`__ can automatically optimized low-precision recipes for deep learning models to achieve optimal product objectives like inference performance and memory usage with expected accuracy criteria. The method to develop a new strategy is introduced.

.. toctree::
   :hidden:

   Adaptor <docs/adaptor.md>
   Strategy <docs/tuning_strategies.md>

Publications
=============

* `MLPerf™ Performance Gains Abound with latest 3rd Generation Intel® Xeon® Scalable Processors <https://www.intel.com/content/www/us/en/artificial-intelligence/posts/3rd-gen-xeon-mlperf-performance-gains.html>`__ (Apr 2021)
* `3D Digital Face Reconstruction Solution enabled by 3rd Gen Intel® Xeon® Scalable Processors <https://www.intel.com/content/www/us/en/artificial-intelligence/posts/tencent-3d-digital-face-reconstruction.html>`__ (Apr 2021)
* `Accelerating Alibaba Transformer model performance with 3rd Gen Intel® Xeon® Scalable Processors (Ice Lake) and Intel® Deep Learning Boost <https://www.intel.com/content/www/us/en/artificial-intelligence/posts/alibaba-lpot.html>`__ (Apr 2021)
* `Using Low-Precision Optimizations for High-Performance DL Inference Applications <https://techdecoded.intel.io/essentials/using-low-precision-optimizations-for-high-performance-dl-inference-applications/#gs.z20k91>`__ (Apr 2021)
* `DL Boost Quantization with CERN's 3D-GANs model <https://www.nextplatform.com/2021/02/01/cern-uses-dlboost-oneapi-to-juice-inference-without-accuracy-loss/>`__ (Feb 2021)

Full publication list please refers to `here <docs/publication_list.md>`__
