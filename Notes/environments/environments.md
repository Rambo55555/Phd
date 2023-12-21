# 环境配置

## conda安装

```bash
https://docs.conda.io/projects/miniconda/en/latest/

~/miniconda3/bin/conda init
conda create --name d2l python=3.9 -y
conda activate d2l
pip install torch==1.12.0
pip install torchvision==0.13.0
pip install d2l==0.17.6

git config --global user.name "Mona Lisa"
git config --global user.email "YOUR_EMAIL"

# generate ssh
ssh-keygen -o
cat ~/.ssh/id_rsa.pub

#~/.ssh/config
Host github.com
  Hostname ssh.github.com
  Port 443
```

## Hugging face internet problem
```python
    os.environ["http_proxy"] = "http://127.0.0.1:7890"
    os.environ["https_proxy"] = "http://127.0.0.1:7890"
```
