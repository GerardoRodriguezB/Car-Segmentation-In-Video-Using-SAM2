# Car-Segmentation-In-Video-Using-SAM2

In this repository is used SAM2 to segment cars in a traffic road video. In each frame, cars are detected using YOLOv8 small, and then the boxes are passed to SAM2 to segment the cars. It is also used [SORT](https://github.com/abewley/sort) to track cars in the scene.

If you have a GPU compatible with CUDA install

```bash
pip install torch==2.7.1 torchvision==0.22.1 torchaudio==2.7.1 --index-url https://download.pytorch.org/whl/cu118
```

otherwise install the versions for CPU

```bash
pip install torch==2.7.1 torchvision==0.22.1 torchaudio==2.7.1
```

Then, install SAM2

```bash
git clone https://github.com/facebookresearch/sam2.git && cd sam2
pip install .
```

Move to the root folder of the project and install requeriments

```bash
pip install -r requeriments.txt
```

Clone the SORT repository

```bash
git clone https://github.com/abewley/sort.git
```
And replace the `sort.py` file with the file of the same name in the folder `SORT FILE UPDATED` included in this repository. Then, download the [SAM2 small checkpoint](https://dl.fbaipublicfiles.com/segment_anything_2/092824/sam2.1_hiera_small.pt) and its [configuration file](https://github.com/facebookresearch/sam2/blob/main/sam2/configs/sam2.1/sam2.1_hiera_s.yaml), and put them in a folder named `sam2_model`






Video cars
https://www.youtube.com/watch?v=zOq2XdwHGT0












