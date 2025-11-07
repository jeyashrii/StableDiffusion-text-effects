# Stable Diffusion Text Effects

Inspired by Adobe Firefly's text effects, Stable Diffusion Text Effects allows you to create mesmerizing and unique text effects with the power of stable diffusion algorithms.

![](assets/example_2.png)

## Prerequisites

1. Install Stable Diffusion Web UI by AUTOMATIC1111. [Follow these steps.](https://github.com/AUTOMATIC1111/stable-diffusion-webui#installation-and-running)
2. Download the [MeinaMix](https://civitai.com/models/7240/meinamix) model and place it inside `stable-diffusion-webui/models/Stable-diffusion`
3. Download the [lineart ControlNet model](https://huggingface.co/ControlNet-1-1-preview/control_v11p_sd15_lineart) and place it inside `stable-diffusion-webui/extensions/sd-webui-controlnet/models`

## Steps to Install

1.Set COMMANDLINE_ARGS in stable-diffusion-webui\webui-user.bat as `set COMMANDLINE_ARGS=--api --nowebui --use-cpu all --no-half --precision full --cors-allow-origins "http://localhost:3000" --api-log --skip-torch-cuda-test` 2. Install the dependencies using `yarn`. 3. `cd` into `stable-diffusion-webui` and run the following command to start the Stable Diffusion API:

````
.\webui-user.bat --api --listen --cors-allow-origins="http://localhost:3000" --no-half --use-cpu all --precision full --skip-torch-cuda-test ``` (or)
``` ./webui.sh --nowebui --cors-allow-origins http://localhost:3000 --api-log
````

4.Run the frontend app in the root directory

```
yarn start
```

5.App will be hosted on [localhost:3000](http://localhost:3000).
