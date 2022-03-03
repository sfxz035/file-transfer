## SR
-----

- LapSRN  
  - 多层金字塔结构  
  - MSE损失平滑细节，使用Charbonnier损失  
- edvr     
  - BN对于超分任务效果不佳    
  - 残差结构    
- Deep Back-Projection Networks For Super-Resolution   
  - 通过反复上采样下采样方式，学习准确低分辨率到高分辨率映射   
  - 上采样单元/下采样单元采用误差反馈结构，简单说就是学习上/下采样的残差信息  
  - 每阶段高分辨率信息的concat  
  - Dense结构    
- Recovering Realistic Texture in Image Super-resolution by
Deep Spatial Feature Transform  
  - loss改进：mse平滑细节，运用对抗损失。  
    - 局部纹理匹配损失local texture matching loss（ EnhanceNet: Single image super-resolution through automated texture synthesis）  
  - 采用仿射参数，调节网络结构中间层特征  
  - 利用语义分割概率图作为放射单元输入，先验纹理类别提升细节  

- Revisiting Global Statistics Aggregation for Improving Image Restoration
  - 利用局部统计信息提高图像恢复质量。聚焦于训练/测试统计信息差别。  
  
- Temporally Deformable Alignment Network for Video Super-Resolution   
  - DCN提出文章，利用可形变卷积对齐
  - 有显式的对齐损失
  
- Self-Supervised Adaptation for Video Super-Resolution
  - 利用视频帧不断运动具有不同尺度的重复patch,较大的patch有利于恢复细节信息