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

<h3>面向多自由度仿生手的神经驱动控制方法</h3>

<p>
面向仿生手自然操作与多自由度连续控制场景，开发基于高密度肌电和运动单位放电信息的
<strong>神经驱动实时控制系统</strong>。
设计运动神经元在线解码与动作映射算法，实现腕屈伸、旋前/旋后及手部开合的
<strong>3-DoF 同步比例控制</strong>，并在截肢者中完成抓取、旋转、放置及多类日常操作任务验证。
项目重点体现了<strong>人体运动意图感知、实时神经解码与机器人闭环控制</strong>能力。
</p>

<h3>面向多指协同运动的神经表征学习与在线人机交互接口</h3>

<p>
面向精细手指运动的人机交互与机器人控制需求，构建基于高密度肌电与运动单位放电信息的
<strong>多层级神经表征学习与在线交互框架</strong>。
通过建模独立及协同手指运动中的个体神经特征与群体协同表征，比较不同神经表征的信息保真度与识别性能，
并进一步开发基于机器学习的实时手指动作识别接口。
系统可实现10类独立及协同手指运动识别，离线识别准确率达到
<strong>97.8%</strong>，
并完成虚拟场景中的人在环闭环控制及机械臂抓取实时验证，展示了神经表征从
<strong>运动意图解析到在线交互控制</strong>的应用潜力。
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
