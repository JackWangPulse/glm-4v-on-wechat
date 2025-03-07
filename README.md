# 本项目说明文档

## Introduction
利用GLM4V图生文模型进行图识别分析,将个人微信当作机器人，并通过wechat群聊天方式进行使用(使用gewechat，基于ipad协议)

## Run  

首先，从 [Gewechat](https://github.com/Devo919/Gewechat) 拉取最新 Docker 镜像并运行容器。具体命令请参考该仓库的说明。之后，可在本仓库进行运行。  

### 1. 配置 Gewechat  
在 `config.py` 或 `config.json` 中进行以下设置：  

```json
{
    "channel_type": "gewechat",
    "gewechat_token": "",        # 首次登录可留空，自动获取
    "gewechat_app_id": "",       # 首次登录可留空，自动获取
    "gewechat_base_url": "http://本机IP:2531/v2/api",  # Gewechat 服务 API 地址
    "gewechat_callback_url": "http://本机IP:9919/v2/api/callback/collect",  # 回调地址
    "gewechat_download_url": "http://本机IP:2532/download"  # 文件下载地址
}
```

### 2. 添加/glm4v-on-wechat/bot/zhipuai/zhipu_ai_vision.py中第4行的API-KEY（从智谱平台获取）
### 3. 添加/tencent_cos.py的12-15和39行key,secert信息(从腾讯云存储桶获取信息)
### 4. 运行以下命令，若后台运行使用Nohup
```bash 
python app.py
```

## Acknowledgments  
This project is built upon the open-source projects [chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat), [dify-on-wechat](https://github.com/hanfangyuan4396/dify-on-wechat), and [Gewechat](https://github.com/Devo919/Gewechat). We appreciate their contributions and retain their original licenses.

Thanks to the original authors for their work!