# stylegan3
Base for create our own stylegan3 / Alias Free Gan generating faces!

`$cd stylegan3`

`$conda env create -f environment.yml`

`$conda activate stylegan3`

`$conda list`

`$conda uninstall *torch*`

`$conda install pytorch torchvision torchaudio cudatoolkit=11.3 -c pytorch`

#### Generate an image using pre-trained AFHQv2 model ("Ours" in Figure 1, left).
`python gen_images.py --outdir=out --trunc=1 --seeds=2 --network=https://api.ngc.nvidia.com/v2/models/nvidia/research/stylegan3/versions/1/files/stylegan3-t-ffhq-1024x1024.pkl`

#### Render a 4x2 grid of interpolations for seeds 0 through 31.
`python gen_video.py --output=lerp.mp4 --trunc=1 --seeds=0-31 --grid=4x2 --network=https://api.ngc.nvidia.com/v2/models/nvidia/research/stylegan3/versions/1/files/stylegan3-t-ffhq-1024x1024.pkl`

### Version of torch
![Pytorch version for w11](https://user-images.githubusercontent.com/107881653/184113915-90ec3827-8c51-4e29-869a-46139e7da43d.png)
