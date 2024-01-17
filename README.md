
![PNSTYLE_23png](https://github.com/ZHO-ZHO-ZHO/ComfyUI-PhotoMaker/assets/140084057/15f9ebaf-b205-4cbd-928e-eca1a0cacb7f)


# ComfyUI PhotoMaker

Unofficial implementation of [PhotoMaker](https://github.com/TencentARC/PhotoMaker) for ComfyUI

<!---
![Dingtalk_20240117150313](https://github.com/ZHO-ZHO-ZHO/ComfyUI-PhotoMaker/assets/140084057/da664c2b-cb30-44e2-85ec-d6070fcfa8f0)
--->

![Dingtalk_20240117161736](https://github.com/ZHO-ZHO-ZHO/ComfyUI-PhotoMaker/assets/140084057/07c924ab-3ee5-4919-87bc-ac49c28914f1)


## 项目介绍 | Info

- 来自对[PhotoMaker](https://github.com/TencentARC/PhotoMaker)的非官方实现
  
- 版本：V1.0


## 视频演示

https://github.com/ZHO-ZHO-ZHO/ComfyUI-PhotoMaker/assets/140084057/8718a70e-a5d7-463b-b36e-de1ffefad9ed


## 节点说明 | Features
- base_model_path：支持输入huggingface模型名称自动下载模型（如：SG161222/RealVisXL_V3.0）
- ref_images_path：支持批量读取参考图像，放入文件夹中即可
- ptompt、negative：正负提示词
- style_name：支持官方提供的10种风格
    - (No style)
    - Cinematic
    - Disney Charactor
    - Digital Art
    - Photographic (Default)
    - Fantasy art
    - Neonpunk
    - Enhance
    - Comic book
    - Lowpoly
    - Line art 
- style_strength_ratio：风格混合强度（高于30按30计算）
- step：步数，官方默认50步，但毕竟是基于SDXL模型，我实测下来30步足够了
- guidance_scale：提示词相关度，一般默认为5
- seed：种子


## 风格 | Styles

![PNSTYLE_2](https://github.com/ZHO-ZHO-ZHO/ComfyUI-PhotoMaker/assets/140084057/dc675478-47a0-456d-946b-0cf781aa4c28)


## 更新日志

- 20240117

  修复bug，初版上线

- 20240116

  创建项目


## 速度实测 | Speed

- A100 50步 23s

![image](https://github.com/ZHO-ZHO-ZHO/ComfyUI-PhotoMaker/assets/140084057/df6eacda-2640-425b-b5ca-1ab5a8a61a66)

- v100 50步 90s

![image](https://github.com/ZHO-ZHO-ZHO/ComfyUI-PhotoMaker/assets/140084057/973b8b6b-9195-4044-b75d-bd833bd6421e)


## Credits

感谢[@erLin](https://twitter.com/eviljer)对ComfyUI 的图像张量 Shape (N, H, W, C)的提醒，帮助我成功修复了bug！

[PhotoMaker](https://github.com/TencentARC/PhotoMaker)
