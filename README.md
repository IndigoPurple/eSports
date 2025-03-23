# 🎮 eSports Broadcasts with Event Cameras

This repository contains the dataset and relevant code for our paper:

> Yaping Zhao, Rongzhou Chen, Chutian Wang, and Edmund Y. Lam,  
> “eSports Broadcasts with Event Cameras,”  
> *International Conference on Neural Information Processing (ICONIP)*, Springer, 2024.
<table class="center" align="center">
    <thead class="center">
        <tr>
            <th>Scene</th>
            <th>Fine Motor Skills</th>
        </tr>
    </thead>
    <tbody class="center" align="center">
        <tr>
            <td rowspan=4><img src="img/frame.gif" raw=true></td>
            <td>with a traditional camera</td>
        </tr>
        <tr>
            <td class="center" align="center"><img src="img/frame_crop.gif" raw=true></td>
        </tr>
        <tr>
            <td>with an event camera</td>
        </tr>
        <tr>
            <td><img src="img/event.gif" raw=true></td>
        </tr>
    </tbody>
</table>

---

## 📁 Dataset Overview

👉 <a href="https://connecthkuhk-my.sharepoint.com/:f:/g/personal/zhaoyp_connect_hku_hk/Em14pK42rO9Lshv2rVNu9vsBaHIsc5CpEzgUY_tbqAfYOA?e=6PBVQG" target="_blank"><strong>Download the dataset here</strong></a>

The following folders are included:

- `davis_data/`:  
  The primary dataset used in our paper. Captured with a DAVIS346 event camera during the eSports tournaments.

- `davis_data_b/`:  
  Backup data captured during the eSports tournaments. These samples were not included in the dataset for experiments and final paper due to lower image quality.

- `frame.zip`:  
  Video frames reconstructed from raw event data using [E2VID](https://github.com/uzh-rpg/rpg_e2vid).

- `pick/`:  
  Materials and image assets used in the figures of the paper.

---

## 🧠 Code Implementation

- **Reconstruction**:  
  We adopt the <a href="https://github.com/uzh-rpg/rpg_e2vid" target="_blank">E2VID</a> model to convert event streams into video frames.

- **Region of Interest Extraction**:  
  Please refer to the pseudocode in our paper for the ROI extraction algorithm.

---

## 📌 Citation

Cite our paper if you find this project interesting!

```bibtex
@inproceedings{zhao2024esports,
  title     = {eSports Broadcasts with Event Cameras},
  author    = {Zhao, Yaping and Chen, Rongzhou and Wang, Chutian and Lam, Edmund Y.},
  booktitle = {International Conference on Neural Information Processing (ICONIP)},
  year      = {2024},
  publisher = {Springer}
}

