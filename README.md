🐣 Please follow me for new updates https://twitter.com/camenduru <br />
🔥 Please join our discord server https://discord.gg/k5BwmmvJJU <br />
🥳 Please join my patreon community https://patreon.com/camenduru <br />

## Tutorial
https://www.youtube.com/watch?v=NJ-uV5GHN8g <br />

## Jupyter Notebooks
[![Run in Saturn Cloud](https://saturncloud.io/images/embed/run-in-saturn-cloud.svg)](https://app.community.saturnenterprise.io/dash/o/community/resources?templateId=582c3235bbfc4140b1decea53fbbaf15)

| Jupyter Notebook | Info
| --- | --- |
[docto_gpt_text_webui_saturncloud](docto_gpt_text_webui_saturncloud.md) | [llSourcell/medllama2_7b](https://huggingface.co/llSourcell/medllama2_7b)

#### Jupyter Notebook (medllama2_7b)
```py
%cd /home/jovyan/workspace
!git clone -b v2.1 https://github.com/camenduru/text-generation-webui

!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/resolve/main/model-00001-of-00002.safetensors -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o model-00001-of-00002.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/resolve/main/model-00002-of-00002.safetensors -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o model-00002-of-00002.safetensors
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/raw/main/model.safetensors.index.json -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o model.safetensors.index.json
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/raw/main/special_tokens_map.json -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o special_tokens_map.json
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/raw/main/tokenizer.json -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o tokenizer.json
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/raw/main/tokenizer_config.json -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o tokenizer_config.json
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/raw/main/config.json -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o config.json
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/raw/main/generation_config.json -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o generation_config.json
!aria2c --console-log-level=error -c -x 16 -s 16 -k 1M https://huggingface.co/4bit/medllama2_7b_s/resolve/main/tokenizer.model -d /home/jovyan/workspace/text-generation-webui/models/medllama2_7b -o tokenizer.model

%cd /home/jovyan/workspace/text-generation-webui
!python server.py --listen --listen-port 8000 --model /home/jovyan/workspace/text-generation-webui/models/medllama2_7b
```

![Screenshot 2023-08-09 021455](https://github.com/camenduru/stable-diffusion-webui-saturncloud/assets/54370274/10e001b9-397c-45b6-851d-b4dc67612ee9)

## Text Generation Web UI
https://github.com/oobabooga/text-generation-webui (Thanks to @oobabooga ❤)

## Documentation
https://github.com/oobabooga/text-generation-webui/tree/main/docs
