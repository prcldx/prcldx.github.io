---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I'm a third-year Ph.D student from Shanghai Jiaotong University. My research interest includes dexterous prosthetic hand control, robot learning, and wearable sensing. I am very fortunate to be advised by [Prof. Peter Shull](http://www.wearablesystems.org/peter-shull) of Wearable systems Lab. You can find my [CV](../assets/CV_Dongxuan_Li.pdf) here. If you want to have a nice talk with me, don't hesitate to [email](mailto:sjtu_dongxuanli@sjtu.edu.cn) me.

<h2 id="Research" style="scroll-margin-top: 80px;">Research</h2>

<h3>面向多自由度仿生手的神经驱动控制方法</h3>

<p>
面向仿生手自然操作与多自由度连续控制场景，开发基于高密度肌电和运动单位放电信息的
<strong>神经驱动实时控制系统</strong>。
设计运动神经元在线解码与动作映射算法，实现腕屈伸、旋前/旋后及手部开合的
<strong>3-DoF 同步比例控制</strong>，并在截肢者中完成抓取、旋转、放置及多类日常操作任务验证。
项目重点体现了
<strong>人体运动意图感知、实时神经解码与机器人闭环控制</strong>
能力。
</p>

<video controls
       playsinline
       preload="metadata"
       style="display: block; width: 100%; max-width: 900px; height: auto;">
  <source src="/files/life3.mp4" type="video/mp4">
  Your browser does not support HTML5 video.
  <a href="/files/life3.mp4">点击此处查看视频</a>
</video>

<h3>面向腕手联合操作中动态腕部运动与抓握力意图解码方法</h3>

<p>
面向腕手协同操作中的<strong>运动位置与作用力联合感知</strong>需求，构建基于高密度肌电、IMU与力传感的多模态运动意图解码框架，
实现动态腕部角度与抓握力的同步连续预测。
设计<strong>GCN-LSTM 时空多任务网络</strong>，利用图卷积建模高密度肌电通道间的空间关联、LSTM提取时序依赖，
并通过共享特征与独立回归头联合解码腕部运动与抓握力。
进一步优化传感器配置与实时推理流程，将输入电极由192个减少至40个，在保持相近预测性能的同时实现<strong>300 ms以内的端到端在线解码</strong>。
</p>

<h3>面向多指协同运动的神经表征学习与在线人机交互接口</h3>

<p>
面向精细手指运动识别与机器人交互场景，开发基于高密度肌电和运动单位放电信息的
<strong>神经表征学习与实时控制接口</strong>。
构建个体神经特征与群体协同表征，并设计基于机器学习的多指动作识别模型，实现10类独立及协同手指运动识别，
离线准确率达到 <strong>97.8%</strong>。
项目进一步完成虚拟场景中的人在环闭环控制以及机械臂抓取实时验证，
重点体现了<strong>精细运动意图感知、神经特征建模与在线交互控制</strong>能力。
</p>

<div style="display: flex; flex-wrap: wrap; gap: 16px; margin-top: 20px;">

  <figure style="flex: 1 1 260px; min-width: 0; margin: 0;">
    <video controls playsinline preload="none"
           style="width: 100%; height: auto; border-radius: 6px;">
      <source src="/files/finger11.mp4" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption style="text-align: center; margin-top: 6px;">
      多指运动实时识别演示
    </figcaption>
  </figure>

  <figure style="flex: 1 1 260px; min-width: 0; margin: 0;">
    <video controls playsinline preload="none"
           style="width: 100%; height: auto; border-radius: 6px;">
      <source src="/files/finger22.mp4" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption style="text-align: center; margin-top: 6px;">
      在线人机交互与机械臂控制演示
    </figcaption>
  </figure>

</div>



<h2 id="project" style="scroll-margin-top: 80px;">Project</h2>

<h3>基于可穿戴肌电腕带的手写识别技术 | 华为技术有限公司 | 2026.04–至今</h3>

<p>
面向可穿戴设备自然交互场景，研发基于EMG与IMU多模态感知的腕带式手写识别系统。
完成30名用户、36类数字与字母手写数据采集，并设计基于TCN的跨用户时序识别模型。
在无需目标用户训练数据的条件下，跨用户识别准确率达到72.47%；通过少量个性化校准后提升至92.42%。
项目进一步完成多日测试与在线Demo验证，重点解决可穿戴手写交互中的跨用户泛化与快速个性化适配问题。
</p>

<video controls
       playsinline
       preload="none"
       loading="lazy"
       width="1280"
       height="720"
       style="display: block; width: 100%; max-width: 900px; height: auto;">
  <source src="/files/huawei_video.mp4" type="video/mp4">
  Your browser does not support HTML5 video.
</video>

<h3>运动单位放电序列非侵入式记录仪器 </h3>

<p>
面向神经接口与智能假肢中的高通量神经信息获取需求，参与研发
<strong>运动单位放电序列非侵入式实时记录仪器</strong>，
构建高密度表面肌电采集、运动单位放电实时解码与在线交互验证的一体化技术链。
负责运动单位放电序列实时解码算法研发，设计基于
<strong>3D-CNN的端到端时空解码网络</strong>，
并针对低信噪比条件下的神经放电识别与实时计算需求进行网络轻量化优化。
优化后单运动单位单窗推理时间由28.2 ms降低至约<strong>2.0 ms</strong>，
支持约<strong>40个运动单位同步解码</strong>，并在自研256通道HD-sEMG系统上完成腕手动作识别验证。
</p>

<h3>基于霍尔效应的力传感器设计与精细手势识别 | PICO / 字节跳动</h3>

<p>
面向VR/AR等可穿戴交互场景，研发基于<strong>柔性Hall Effect力传感</strong>的腕带式人机交互系统，
通过感知腕部肌腱形变产生的法向力与切向力变化，实现精细手指动作识别与握力连续感知。
参与磁体--柔性介质--三轴Hall传感单元及腕带结构设计，并结合腕部肌腱解剖位置开展传感区域灵敏度分析，
优化双模块传感器布局。
进一步开发<strong>轻量化实时手势识别算法</strong>，结合动作起始检测、时域/频域特征提取、
XGBoost等机器学习模型及时序后处理，实现点击、双击、滑动等精细手势的跨用户在线识别，
未见用户实时识别准确率达到<strong>84.8%</strong>，并实现0--10 kg范围内的连续握力估计。
</p>
