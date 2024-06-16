# Abstract[En]
  Object-aware systems such as Deep Shape Prior SLAM (DSP-SLAM), provide a feasible technique for creating environment-sparse maps on the fly while representing scene objects as complete 3D models. Such systems provide a compelling solution for improving the intelligence of care robots by offering a means to develop spatial-model-knowledge of objects and the environment. Also, user experience in augmented and virtual reality therapy applications can be further enriched with such systems. However, due to abrupt and unpredictable movements exhibited by users during virtual therapy engagements and real-time robot responses to changes in situation and commands, robustness and speed of sensor data processing are imperative.
  
  DSP-SLAM suffers from a low-performance speed of 10 - 15 fps, even with ORB-SLAM2 as a backbone which can run at 30 fps. Mainly, this is because its instance segmentation approach has an average latency of 53ms(18.86fps). To improve camera tracking robustness, keyframes must be processed at a fast rate.
  
  This work introduces the use of a state-of-the-art one-stage deep learning detector and implements a fast method for real-time keyframe creation and object data association that significantly reduces the wait time for detection-based data association during keyframe creation. The method presented in this work is denoted as Real-time Deep Shape Prior SLAM (RDSP-SLAM).
  
  Results show that segmentations are performed at 20ms (50fps), while the object 3D reconstruction quality is the same as that of DSP-SLAM. RDSP-SLAM accepts RGB sequential images at 30fps and tracks them at a mean latency of 38fps.

Key Words: Deep shape priors, Instance segmentation, Object-aware SLAM, Object representation, Object Reconstruction

# Abstrct[Ch]

  具有深度形状先验的目标感知 SLAM(DSP-SLAM)，是一种具有物体预感知能力的 同步定位与建图视觉系统。它提供了一种能够实时创建环境稀疏地图，并将环境中的对象 完整呈现为 3D 模型的方法。此系统可提高护理机器人的智能水平使它能对物体和环境空 间模型有了更高的感知，并且为增强用户在现实和虚拟环境下理疗的舒适体验感提供了解 决方案。然而，在虚拟现实疗法中，难以预测的用户行为动作以及机器人实时响应情况和 接受指令变化，对传感器数据处理的稳健性和速度至关重要。
  
  现有算法 DSP-SLAM 的图像处理效率较低，虽然使用了处理速度能达到 30 fps 的 ORB-SLAM2 作为基础框架，但也仅能达到 10-15 fps。主要原因在于其实例分割方法的平 均延迟为 53ms(18.86fps)，为了在目标定位和环境建图时提高相机跟踪的稳健性，需要 以较快速率处理关键帧。
  
  本研究采用了一种最先进的单阶段深度学习检测器，提出了一种实时创建关键帧和处 理物体数据关联方法，在视觉同步定位与建图过程中，大幅度缩短了相机每帧的跟踪时间， 提高了相机随机与剧烈运动时检测速度和跟踪鲁棒性。本文研究 Real-time Deep Shape Prior SLAM(RDSP-SLAM)。
  
  结果显示，图像分割时间缩小到 20ms(50fps)，而对象的 3D 重建质量与 DSP-SLAM 相当。 RDSP-SLAM 是一个单目视觉物体感知 SLAM 系统。它能接受以 30fps 的速度输 入的 RGB 序列图像，并以 38fps 的平均延迟进行跟踪。

关键词:深度先验，图片实例分割，目标感知 SLAM，目标表示法，目标模型重建
