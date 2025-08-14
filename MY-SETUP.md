# My Setup

1. Fork and clone stable diffusion

   ```sh
   git@github.com:AUTOMATIC1111/stable-diffusion-webui.git

   git checkout dev

   git remote set-url origin https://github.com/dennis-gonzales/stable-diffusion-webui.git
   git remote add upstream https://github.com/AUTOMATIC1111/stable-diffusion-webui.git

   git remote -v

   ```

2. Run webui.(bat/py/sh)

3. Staying up to date

   Pull from upstream

   ```sh
   git pull upstream dev
   ```

   And set dev branch as default branch in Github
