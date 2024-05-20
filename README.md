# yolov8seg_onn_rknn_horizon_tensorRT_dfl

yolov8seg 部署版本，便于移植不同平台（onnx、tensorRT、rknn、Horizon），全网部署最简单、速度最快的部署方式。


yolov8seg_onnx：onnx模型、测试图像、测试结果、测试demo脚本

yolov8seg_TensorRT：TensorRT版本模型、测试图像、测试结果、测试demo脚本、onnx模型、onnx2tensorRT脚本(tensorRT-7.2.3.4)

yolov8seg_rknn：rknn模型、测试（量化）图像、测试结果、onnx2rknn转换测试脚本

yolov8seg_horizon：地平线模型、测试（量化）图像、测试结果、转换测试脚本、测试量化后onnx模型脚本

# 导出onnx参考

本示例提供的代码只适用按照参考博文导出的方式，其它导出方式自行写后处理。![导出onnx参考](https://blog.csdn.net/zhangqian_1/article/details/139066553)


# 测试结果
![images](https://github.com/cqu20160901/yolov8seg_onn_rknn_horizon_tensorRT_dfl/blob/main/yolov8seg_onnx/test_onnx_result.jpg)

说明：推理测试预处理没有考虑等比率缩放，训练时激活函数 SiLU 用 Relu 进行了替换。由于使用的是coco128数据进行训练的，且迭代的次数不多，效果并不是很好，仅供测试流程用。
