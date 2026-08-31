---
permalink: /
title: "About"
excerpt: "About me"
author_profile: true
redirect_from:
  - /about/
  - /about.html
---

<style>
.section-title {
  margin-top: 3.5rem;
  margin-bottom: 1.8rem;
  padding-bottom: 0.55rem;
  border-bottom: 3px solid #326891;
  font-size: 2.3rem;
  font-weight: 700;
  line-height: 1.2;
}

.content-divider {
  margin: 2.8rem 0;
  border: 0;
  border-top: 1px solid #d8dde3;
}

.content-video {
  display: block;
  width: 100%;
  max-width: 900px;
  height: auto;
  border-radius: 6px;
}

.video-grid {
  display: flex;
  flex-wrap: wrap;
  gap: 16px;
  margin-top: 20px;
}

.video-grid figure {
  flex: 1 1 260px;
  min-width: 0;
  margin: 0;
}

.video-grid video {
  display: block;
  width: 100%;
  height: auto;
  border-radius: 6px;
}

.video-grid figcaption {
  margin-top: 6px;
  text-align: center;
  color: #555;
  font-size: 0.95rem;
}

@media (max-width: 600px) {
  .section-title {
    font-size: 1.85rem;
  }

  .content-divider {
    margin: 2.2rem 0;
  }
}
</style>

我是上海交通大学机械工程专业机器人研究所博士三年级学生，师从陈晨副教授、朱向阳教授，预计于2027年毕业。此前于上海交通大学机器人研究所获得机械工程硕士学位，硕士阶段师从 [Peter B. Shull 教授](http://www.wearablesystems.org/peter-shull)。

我的研究主要围绕**人机交互神经接口、人体运动意图解码与多自由度仿生手控制**展开，同时关注**灵巧操作、机器人学习、共享控制**。目前希望进一步将人体神经与运动信息感知同智能机器人技术相结合，探索更加自然、直观的人机交互与机器人控制方法。

如果你对我的研究、潜在合作或相关工作机会感兴趣，欢迎通过[邮件](mailto:sjtu_dongxuanli@sjtu.edu.cn)与我联系。

<h2 id="research"
    class="section-title"
    style="scroll-margin-top: 80px;">
  Research
</h2>

<h3>1. 面向多自由度仿生手的神经驱动控制方法</h3>

<p>
面向仿生手自然操作与多自由度连续控制场景，开发基于高密度肌电和运动单位放电信息的
<strong>神经驱动实时控制系统</strong>。
设计运动神经元在线解码与动作映射算法，实现腕屈伸、旋前/旋后及手部开合的
<strong>3-DoF 同步比例控制</strong>，
并在截肢者中完成抓取、旋转、放置及多类日常操作任务验证。
</p>

<p>
  <a href="https://doi.org/10.1126/sciadv.aej0245"
     target="_blank"
     rel="noopener noreferrer">
    论文：A motoneuron discharge-driven interface realizing simultaneous and proportional control of prosthetics in end-users
  </a>
</p>

<video controls
       playsinline
       preload="metadata"
       class="content-video">
  <source src="/files/life3.mp4" type="video/mp4">
  Your browser does not support HTML5 video.
  <a href="/files/life3.mp4">点击此处查看视频</a>
</video>

<hr class="content-divider">

<h3>2. 面向腕手联合操作中动态腕部运动与抓握力意图解码方法</h3>

<p>
面向腕手协同操作中的
<strong>运动位置与作用力联合感知</strong>
需求，构建基于高密度肌电、IMU与力传感的多模态运动意图解码框架，
实现动态腕部角度与抓握力的同步连续预测。
设计
<strong>GCN-LSTM 时空多任务网络</strong>，
利用图卷积建模高密度肌电通道间的空间关联、LSTM提取时序依赖，
并通过共享特征与独立回归头联合解码腕部运动与抓握力。
进一步优化传感器配置与实时推理流程，将输入电极由192个减少至40个，
在保持相近预测性能的同时实现
<strong>300 ms以内的端到端在线解码</strong>。
</p>

<p>
  <a href="https://doi.org/10.1109/JBHI.2024.3373432"
     target="_blank"
     rel="noopener noreferrer">
    Graph-Driven Simultaneous and Proportional Estimation of Wrist Angle and Grasp Force via High-Density EMG
  </a>
</p>

<hr class="content-divider">

<h3>3. 面向多指协同运动的神经表征学习与在线人机交互接口</h3>

<p>
面向精细手指运动识别与机器人交互场景，开发基于高密度肌电和运动单位放电信息的
<strong>神经表征学习与实时控制接口</strong>。
构建个体神经特征与群体协同表征，并设计基于机器学习的多指动作识别模型，
实现10类独立及协同手指运动识别，离线准确率达到
<strong>97.8%</strong>。
项目进一步完成虚拟场景中的人在环闭环控制以及机械臂抓取实时验证，
重点体现了
<strong>精细运动意图感知、神经特征建模与在线交互控制</strong>
能力。
</p>

<div class="video-grid">

  <figure>
    <video controls playsinline preload="metadata">
      <source src="/files/finger11.mp4" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption>多指运动实时识别演示</figcaption>
  </figure>

  <figure>
    <video controls playsinline preload="metadata">
      <source src="/files/finger22.mp4" type="video/mp4">
      Your browser does not support HTML5 video.
    </video>
    <figcaption>在线人机交互与机械臂控制演示</figcaption>
  </figure>

</div>

<h2 id="project"
    class="section-title"
    style="scroll-margin-top: 80px;">
  Project
</h2>

<h3>1. 基于可穿戴肌电腕带的手写识别技术 | 华为技术有限公司 | 2026.04–至今</h3>

<p>
面向可穿戴设备自然交互场景，研发基于EMG与IMU多模态感知的腕带式手写识别系统。
完成30名用户、36类数字与字母手写数据采集，并设计基于TCN的跨用户时序识别模型。
在无需目标用户训练数据的条件下，跨用户识别准确率达到72.47%；
通过少量个性化校准后提升至92.42%。
项目进一步完成多日测试与在线Demo验证，
重点解决可穿戴手写交互中的跨用户泛化与快速个性化适配问题。
</p>

<video controls
       playsinline
       preload="metadata"
       width="1280"
       height="720"
       class="content-video">
  <source src="/files/huawei_video.mp4" type="video/mp4">
  Your browser does not support HTML5 video.
  <a href="/files/huawei_video.mp4">点击此处查看视频</a>
</video>

<hr class="content-divider">

<h3>2. 运动单位放电序列非侵入式记录仪器</h3>

<p>
面向神经接口与智能假肢中的高通量神经信息获取需求，参与研发
<strong>运动单位放电序列非侵入式实时记录仪器</strong>，
构建高密度表面肌电采集、运动单位放电实时解码与在线交互验证的一体化技术链。
负责运动单位放电序列实时解码算法研发，设计基于
<strong>3D-CNN的端到端时空解码网络</strong>，
并针对低信噪比条件下的神经放电识别与实时计算需求进行网络轻量化优化。
优化后单运动单位单窗推理时间由28.2 ms降低至约
<strong>2.0 ms</strong>，
支持约
<strong>40个运动单位同步解码</strong>，
并在自研256通道HD-sEMG系统上完成腕手动作识别验证。
</p>

<video controls
       playsinline
       preload="metadata"
       width="1280"
       height="720"
       class="content-video">
  <source src="/files/mu_decomp.mp4" type="video/mp4">
  Your browser does not support HTML5 video.
  <a href="/files/huawei_video.mp4">点击此处查看视频</a>
</video>

<hr class="content-divider">

<h3>3. 基于霍尔效应的力传感器设计与精细手势识别 | PICO / 字节跳动</h3>

<p>
面向VR/AR等可穿戴交互场景，研发基于
<strong>柔性Hall Effect力传感</strong>
的腕带式人机交互系统，
通过感知腕部肌腱形变产生的法向力与切向力变化，
实现精细手指动作识别与握力连续感知。
参与磁体、柔性介质、三轴Hall传感单元及腕带结构设计，
并结合腕部肌腱解剖位置开展传感区域灵敏度分析，优化双模块传感器布局。
进一步开发
<strong>轻量化实时手势识别算法</strong>，
结合动作起始检测、时域/频域特征提取、
XGBoost等机器学习模型及时序后处理，
实现点击、双击、滑动等精细手势的跨用户在线识别，
未见用户实时识别准确率达到
<strong>84.8%</strong>，
并实现0–10 kg范围内的连续握力估计。
</p>
