---
license: other
tags:
  - lora
  - detail-slider
  - scene-complexity
  - stylized
  - trash-mode
pipeline_tag: text-to-image
---

# 🟣 Simple_DTS — Detail / Trash Slider LoRA  
**ZIT & FLUX compatible · Safe · Stylized detail-level manipulation**

---

## ⚡ Quick Links

<table>
<tr>

<td width="50%" valign="top">

### ZIT  
[Download Weights](https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/ZIT/Simple_Trash_S.safetensors)

<br>

<img src="https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/ZIT/2026-01-16-2.png" width="220"><br>
<img src="https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/ZIT/2026-01-16-3.png" width="220"><br>
<img src="https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/ZIT/2026-01-16-4.png" width="220"><br>
<img src="https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/ZIT/2026-01-16.png" width="220">

</td>

<td width="50%" valign="top">

### FLUX (dev)  
[Download Weights](https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/FLUX%20(dev)/Simple_Trash_S.safetensors)

<br>

<img src="https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/FLUX%20(dev)/2026-01-16-13.png" width="220"><br>
<img src="https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/FLUX%20(dev)/2026-01-20-1.png" width="220"><br>
<img src="https://huggingface.co/dmsnoa/Simple_DTS/resolve/main/FLUX%20(dev)/2026-01-20.png" width="220">

</td>

</tr>
</table>


## 🔍 Overview
**Simple_DTS** is an artistic scene-complexity LoRA that modifies **only the stylized amount of visual detail and clutter**, without touching:

- identity  
- anatomy  
- age  
- body proportions  
- realism-critical features  

It controls **props, accessories, textures, clutter, micro-details**, and the overall scene complexity — while keeping characters fully intact.

All effects remain **safe, non-realistic, purely stylistic**.

---

## ⚙️ How the Slider Works

Adjust `network_multiplier` to control scene detail & clutter amount:

| Multiplier | Effect |
|-----------:|--------|
| `-2 → -0.7` | cleaner image · minimal props · reduced clutter |
| `-0.6 → -0.2` | slightly simplified scene |
| `0` | neutral (no modification) |
| `+0.2 → +0.7` | added detail · extra props · richer textures |
| `+0.8 → +2` | heavy stylized clutter · “trash mode” · maximal visual noise |

The slider affects *only* scene complexity — **not identity or anatomy**.

---

## 🧩 Example Usage (ComfyUI / AITS Toolkit)

```yaml
lora:
  name: "dmsnoa/jix/Simple_DTS"
  multiplier: 0.7   # increased stylized detail
```

### Recommended Base Prompt
```
portrait or full-body, clean lighting,
realistic skin texture, professional photography style,
detailed clothing, soft shadows
```

💡 No need to describe “detail / clutter / props” —  
the LoRA applies stylization automatically.

---

## 🔐 Safety Notice
- Stylized detail-level modification only  
- Does NOT affect identity or anatomy  
- Not intended for biometric or forensic usage  
- Commercial + non-commercial use allowed under the license

---


## 🧾 License
**CreativeML OpenRAIL-M**

---

## ✏️ Author  
Created by **dmsnoa / jix**

⭐ If this model helped you — consider starring the repository!
