---
permalink: /projects/
layout: single
author_profile: false
---

My GoogleColab consists of 4 cells. Let's talk about what each cell does in this section.
The code in the first cell copies 3 files and a folder to /content.
Similar to the first cell, the second cell does not have much code. The second cell only has the following code: !nvidia-smi.
By running the code, I can know which device was assigned. In my case, a NVIDIA A100-SXM4-80GB was assigned. 
I do not yet know the internal of NVIDIA A100-SXM4-80GB. 

Before the training happens, the training dataset is loaded onto the ram (not onto the GPU).
Since the GPU will be used, the value of device.type will be "cuda".







