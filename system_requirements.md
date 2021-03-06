# System Requirements

Intel® Neural Compressor supports systems based on [Intel 64 architecture or compatible processors](https://en.wikipedia.org/wiki/X86-64), specially optimized for the following CPUs:

* Intel Xeon Scalable processor (formerly Skylake, Cascade Lake, Cooper Lake, and Icelake)
* future Intel Xeon Scalable processor (code name Sapphire Rapids)

Intel® Neural Compressor requires installing the pertinent Intel-optimized framework version for TensorFlow, PyTorch, MXNet, and ONNX runtime.

## Validated Hardware/Software Environment

<table class="docutils">
<thead>
  <tr>
    <th class="tg-bobw">Platform</th>
    <th class="tg-bobw">OS</th>
    <th class="tg-bobw">Python</th>
    <th class="tg-bobw">Framework</th>
    <th class="tg-bobw">Version</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td class="tg-nrix" rowspan="20">Cascade Lake<br><br>Cooper Lake<br><br>Skylake<br><br>Ice Lake</td>
    <td class="tg-nrix" rowspan="20">CentOS 8.3<br><br>Ubuntu 18.04</td>
    <td class="tg-nrix" rowspan="20">3.6<br><br>3.7<br><br>3.8<br><br>3.9</td>
    <td class="tg-cly1" rowspan="10">TensorFlow</td>
    <td class="tg-7zrl">2.6.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">2.5.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">2.4.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">2.3.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">2.2.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">2.1.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.15.0 UP1</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.15.0 UP2</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.15.0 UP3</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.15.2</td>
  </tr>
  <tr>
    <td class="tg-7zrl" rowspan="4">PyTorch</td>
    <td class="tg-7zrl">1.5.0+cpu</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.6.0+cpu</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.8.0+cpu</td>
  </tr>
  <tr>
    <td class="tg-7zrl">IPEX</td>
  </tr>
  <tr>
    <td class="tg-cly1" rowspan="2">MXNet</td>
    <td class="tg-7zrl">1.8.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.7.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.6.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl" rowspan="3">ONNX Runtime</td>
    <td class="tg-7zrl">1.6.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.7.0</td>
  </tr>
  <tr>
    <td class="tg-7zrl">1.8.0</td>
  </tr>
</tbody>
</table>

## Validated Models

Intel® Neural Compressor provides numerous examples to show promising accuracy loss with the best performance gain. A full quantized model list on various frameworks is available in the [Model List](docs/full_model_list.md).

### Validated MLPerf Models

<table>
<thead>
  <tr>
    <th>Model</th>
    <th>Framework</th>
    <th>Support</th>
    <th>Example</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td rowspan="2">ResNet50 v1.5</td>
    <td>TensorFlow</td>
    <td>Yes</td>
    <td><a href="https://github.com/intel/neural-compressor/tree/master/examples/tensorflow/image_recognition">Link</a></td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="https://github.com/intel/neural-compressor/tree/master/examples/pytorch/ipex/image_recognition/imagenet/cpu/ptq">Link</a></td>
  </tr>
  <tr>
    <td>DLRM</td>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="https://github.com/intel/neural-compressor/tree/master/examples/pytorch/fx/recommendation">Link</a></td>
  </tr>
  <tr>
    <td rowspan="2">BERT-large</td>
    <td>TensorFlow</td>
    <td>Yes</td>
    <td><a href="https://github.com/intel/neural-compressor/tree/master/examples/tensorflow/nlp/bert_large_squad">Link</a></td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="https://github.com/intel/neural-compressor/tree/master/examples/pytorch/eager/language_translation/ptq">Link</a></td>
  </tr>
  <tr>
    <td rowspan="2">SSD-ResNet34</td>
    <td>TensorFlow</td>
    <td>WIP</td>
    <td></td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="https://github.com/intel/neural-compressor/tree/master/examples/pytorch/fx/object_detection/ssd_resnet34/ptq">Link</a></td>
  </tr>
  <tr>
    <td>RNN-T</td>
    <td>PyTorch</td>
    <td>WIP</td>
    <td></td>
  </tr>
  <tr>
    <td rowspan="2">3D-UNet</td>
    <td>TensorFlow</td>
    <td>WIP</td>
    <td></td>
  </tr>
  <tr>
    <td>PyTorch</td>
    <td>Yes</td>
    <td><a href="https://github.com/intel/neural-compressor/tree/master/examples/pytorch/eager/medical_imaging/3d-unet">Link</a></td>
  </tr>
</tbody>
</table>

### Validated Quantized Models

<table>
<thead>
  <tr>
    <th rowspan="2">Framework</th>
    <th rowspan="2">Version</th>
    <th rowspan="2">Model</th>
    <th colspan="3">Accuracy</th>
    <th colspan="3">Performance</th>
  </tr>
  <tr>
    <th>INT8 Tuning Accuracy</th>
    <th>FP32 Accuracy Baseline</th>
    <th>Acc Ratio [(INT8-FP32)/FP32]</th>
    <th>INT8 realtime(ms)<br> CLX8280 1s 4c per instance</th>
    <th>FP32 realtime(ms)<br> CLX8280 1s 4c per instance</th>
    <th>Realtime Latency Ratio[FP32/INT8]</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>resnet50v1.0</td>
    <td>74.24%</td>
    <td>74.27%</td>
    <td>-0.04%</td>
    <td>7.64</td>
    <td>21.54</td>
    <td>2.82x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>resnet50v1.5</td>
    <td>76.94%</td>
    <td>76.46%</td>
    <td>0.63%</td>
    <td>9.54</td>
    <td>24.28</td>
    <td>2.54x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>resnet101</td>
    <td>77.21%</td>
    <td>76.45%</td>
    <td>0.99%</td>
    <td>12.92</td>
    <td>30.65</td>
    <td>2.37x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>inception_v1</td>
    <td>70.30%</td>
    <td>69.74%</td>
    <td>0.80%</td>
    <td>5.58</td>
    <td>10.13</td>
    <td>1.82x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>inception_v2</td>
    <td>74.27%</td>
    <td>73.97%</td>
    <td>0.41%</td>
    <td>6.78</td>
    <td>12.42</td>
    <td>1.83x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>inception_v3</td>
    <td>77.29%</td>
    <td>76.75%</td>
    <td>0.70%</td>
    <td>12.90</td>
    <td>27.74</td>
    <td>2.15x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>inception_v4</td>
    <td>80.36%</td>
    <td>80.27%</td>
    <td>0.11%</td>
    <td>21.00</td>
    <td>54.42</td>
    <td>2.59x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>inception_resnet_v2</td>
    <td>80.42%</td>
    <td>80.40%</td>
    <td>0.02%</td>
    <td>44.72</td>
    <td>87.62</td>
    <td>1.96x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>mobilenetv1</td>
    <td>73.93%</td>
    <td>70.96%</td>
    <td>4.19%</td>
    <td>2.96</td>
    <td>9.88</td>
    <td>3.34x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>mobilenetv2</td>
    <td>71.96%</td>
    <td>71.76%</td>
    <td>0.28%</td>
    <td>4.95</td>
    <td>10.71</td>
    <td>2.16x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>ssd_resnet50_v1</td>
    <td>37.91%</td>
    <td>38.00%</td>
    <td>-0.24%</td>
    <td>145.96</td>
    <td>422.11</td>
    <td>2.89x</td>
  </tr>
  <tr>
    <td>tensorflow</td>
    <td>2.5.0</td>
    <td>ssd_mobilenet_v1</td>
    <td>23.02%</td>
    <td>23.13%</td>
    <td>-0.48%</td>
    <td>12.19</td>
    <td>26.85</td>
    <td>2.20x</td>
  </tr>
</tbody>
</table>


<table class="docutils">
<thead>
  <tr>
    <th rowspan="2">Framework</th>
    <th rowspan="2">Version</th>
    <th rowspan="2">Model</th>
    <th colspan="3">Accuracy</th>
    <th colspan="3">Performance</th>
  </tr>
  <tr>
    <th>INT8 Tuning Accuracy</th>
    <th>FP32 Accuracy Baseline</th>
    <th>Acc Ratio [(INT8-FP32)/FP32]</th>
    <th>INT8 realtime(ms)<br> CLX8280 1s 4c per instance</th>
    <th>FP32 realtime(ms)<br> CLX8280 1s 4c per instance</th>
    <th>Realtime Latency Ratio[FP32/INT8]</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>resnet18</td>
    <td>69.58%</td>
    <td>69.76%</td>
    <td>-0.26%</td>
    <td>13.59</td>
    <td>24.97</td>
    <td>1.84x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>resnet50</td>
    <td>75.87%</td>
    <td>76.13%</td>
    <td>-0.34%</td>
    <td>25.67</td>
    <td>54.12</td>
    <td>2.11x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>resnext101_32x8d</td>
    <td>79.09%</td>
    <td>79.31%</td>
    <td>-0.28%</td>
    <td>62.44</td>
    <td>147.88</td>
    <td>2.37x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_base_mrpc</td>
    <td>88.16%</td>
    <td>88.73%</td>
    <td>-0.64%</td>
    <td>41.33</td>
    <td>81.93</td>
    <td>1.98x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_base_cola</td>
    <td>58.29%</td>
    <td>58.84%</td>
    <td>-0.93%</td>
    <td>39.30</td>
    <td>86.58</td>
    <td>2.20x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_base_sts-b</td>
    <td>88.65%</td>
    <td>89.27%</td>
    <td>-0.70%</td>
    <td>39.46</td>
    <td>86.97</td>
    <td>2.20x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_base_sst-2</td>
    <td>91.63%</td>
    <td>91.86%</td>
    <td>-0.25%</td>
    <td>39.12</td>
    <td>82.59</td>
    <td>2.11x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_base_rte</td>
    <td>69.31%</td>
    <td>69.68%</td>
    <td>-0.52%</td>
    <td>39.81</td>
    <td>81.98</td>
    <td>2.06x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_large_mrpc</td>
    <td>87.48%</td>
    <td>88.33%</td>
    <td>-0.95%</td>
    <td>112.61</td>
    <td>287.44</td>
    <td>2.55x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_large_squad</td>
    <td>92.79</td>
    <td>93.05</td>
    <td>-0.28%</td>
    <td>497.79</td>
    <td>953.74</td>
    <td>1.92x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_large_qnli</td>
    <td>91.12%</td>
    <td>91.82%</td>
    <td>-0.76%</td>
    <td>112.43</td>
    <td>291.10</td>
    <td>2.59x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_large_rte</td>
    <td>72.92%</td>
    <td>72.56%</td>
    <td>0.50%</td>
    <td>148.60</td>
    <td>287.03</td>
    <td>1.93x</td>
  </tr>
  <tr>
    <td>pytorch</td>
    <td>1.9.0+cpu</td>
    <td>bert_large_cola</td>
    <td>62.85%</td>
    <td>62.57%</td>
    <td>0.45%</td>
    <td>112.54</td>
    <td>283.38</td>
    <td>2.52x</td>
  </tr>
</tbody>
</table>

### Validated Pruning Models

<table>
<thead>
  <tr>
    <th rowspan="2">Tasks</th>
    <th rowspan="2">FWK</th>
    <th rowspan="2">Model</th>
    <th rowspan="2">fp32 baseline</th>
    <th colspan="3">gradient sensitivity with 20% sparsity</th>
    <th colspan="3">+onnx dynamic quantization on pruned model</th>
  </tr>
  <tr>
    <td>accuracy%</td>
    <td> drop%</td>
    <td>perf gain (sample/s)</td>
    <td>accuracy%</td>
    <td> drop%</td>
    <td>perf gain (sample/s)</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td>SST-2</td>
    <td>pytorch</td>
    <td>bert-base</td>
    <td>accuracy = 92.32</td>
    <td>accuracy = 91.97</td>
    <td>-0.38</td>
    <td>1.30x</td>
    <td>accuracy = 92.20</td>
    <td>-0.13</td>
    <td>1.86x</td>
  </tr>
  <tr>
    <td>QQP</td>
    <td>pytorch</td>
    <td>bert-base</td>
    <td>[accuracy, f1] = [91.10, 88.05]</td>
    <td>[accuracy, f1] = [89.97, 86.54]</td>
    <td>[-1.24, -1.71]</td>
    <td>1.32x</td>
    <td>[accuracy, f1] = [89.75, 86.60]</td>
    <td>[-1.48, -1.65]</td>
    <td>1.81x</td>
  </tr>
</tbody>
</table>

<table>
<thead>
  <tr>
    <th rowspan="2">Tasks</th>
    <th rowspan="2">FWK</th>
    <th rowspan="2">Model</th>
    <th rowspan="2">fp32 baseline</th>
    <th colspan="2">Pattern Lock on 70% Unstructured Sparsity</th>
    <th colspan="2">Pattern Lock on 50% 1:2 Structured Sparsity</th>
  </tr>
  <tr>
    <td>accuracy%</td>
    <td> drop%</td>
    <td>accuracy%</td>
    <td> drop%</td>
  </tr>
</thead>
<tbody>
  <tr>
    <td>MNLI</td>
    <td>pytorch</td>
    <td>bert-base</td>
    <td>[m, mm] = [84.57, 84.79]</td>
    <td>[m, mm] = [82.45, 83.27]</td>
    <td>[-2.51, -1.80]</td>
    <td>[m, mm] = [83.20, 84.11]</td>
    <td>[-1.62, -0.80]</td>
  </tr>
  <tr>
    <td>SST-2</td>
    <td>pytorch</td>
    <td>bert-base</td>
    <td>accuracy = 92.32</td>
    <td>accuracy = 91.51</td>
    <td>-0.88</td>
    <td>accuracy = 92.20</td>
    <td>-0.13</td>
  </tr>
  <tr>
    <td>QQP</td>
    <td>pytorch</td>
    <td>bert-base</td>
    <td>[accuracy, f1] = [91.10, 88.05]</td>
    <td>[accuracy, f1] = [90.48, 87.06]</td>
    <td>[-0.68, -1.12]</td>
    <td>[accuracy, f1] = [90.92, 87.78]</td>
    <td>[-0.20, -0.31]</td>
  </tr>
  <tr>
    <td>QNLI</td>
    <td>pytorch</td>
    <td>bert-base</td>
    <td>accuracy = 91.54</td>
    <td>accuracy = 90.39</td>
    <td>-1.26</td>
    <td>accuracy = 90.87</td>
    <td>-0.73</td>
  </tr>
  <tr>
    <td>QnA</td>
    <td>pytorch</td>
    <td>bert-base</td>
    <td>[em, f1] = [79.34, 87.10]</td>
    <td>[em, f1] = [77.27, 85.75]</td>
    <td>[-2.61, -1.54]</td>
    <td>[em, f1] = [78.03, 86.50]</td>
    <td>[-1.65, -0.69]</td>
  </tr>
</tbody>
</table>

<table>
<thead>
  <tr>
    <th>Framework</th>
    <th>Model</th>
    <th>fp32 baseline</th>
    <th>Compression</th>
    <th>dataset</th>
    <th>acc(drop)%</th>
  </tr>
</thead>
<tbody>
  <tr>
    <td>Pytorch</td>
    <td>resnet18</td>
    <td>69.76</td>
    <td>30% sparsity on magnitude</td>
    <td>ImageNet</td>
    <td>69.47(-0.42)</td>
  </tr>
  <tr>
    <td>Pytorch</td>
    <td>resnet18</td>
    <td>69.76</td>
    <td>30% sparsity on gradient sensitivity</td>
    <td>ImageNet</td>
    <td>68.85(-1.30)</td>
  </tr>
  <tr>
    <td>Pytorch</td>
    <td>resnet50</td>
    <td>76.13</td>
    <td>30% sparsity on magnitude</td>
    <td>ImageNet</td>
    <td>76.11(-0.03)</td>
  </tr>
  <tr>
    <td>Pytorch</td>
    <td>resnet50</td>
    <td>76.13</td>
    <td>30% sparsity on magnitude and post training quantization</td>
    <td>ImageNet</td>
    <td>76.01(-0.16)</td>
  </tr>
  <tr>
    <td>Pytorch</td>
    <td>resnet50</td>
    <td>76.13</td>
    <td>30% sparsity on magnitude and quantization aware training</td>
    <td>ImageNet</td>
    <td>75.90(-0.30)</td>
  </tr>
</tbody>
</table>