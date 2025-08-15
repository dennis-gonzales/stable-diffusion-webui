# My Setup

1.  Fork and clone stable diffusion

    ```sh
    git@github.com:AUTOMATIC1111/stable-diffusion-webui.git

    git checkout dev

    git remote set-url origin https://github.com/dennis-gonzales/stable-diffusion-webui.git
    git remote add upstream https://github.com/AUTOMATIC1111/stable-diffusion-webui.git

    git remote -v
    ```

    Note: you need python 3.10.6

2.  Install stuff (Optional if you didn't encounter any errors)

    [Install Pytorch for Nvidia Blackwell 50XX GPU (method 2)](https://github.com/AUTOMATIC1111/stable-diffusion-webui/issues/16824)

    Switch to dev branch if you haven't already

    ```sh
    git checkout dev # or git switch dev
    ```

    Add --reinstall-torch to COMMANDLINE_ARGS to tell webui to reinstall PyTorch thereafter launch webui

    ```sh
    # webuirc/modules/paths_internal.py
    commandline_args = os.environ.get('COMMANDLINE_ARGS', "")
    commandline_args += " --reinstall-torch"
    ```

    > remember to remove--reinstall-torch from COMMANDLINE_ARGS after it's done reinstalling PyTorch

3.  Run webui.(bat/py/sh)

4.  Staying up to date

    Pull from upstream

    ```sh
    git pull upstream dev
    ```

    And set dev branch as default branch in Github
