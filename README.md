# 本项目说明文档

## Introduction
利用GLM4V图生文模型进行图识别分析,将个人微信当作机器人，并通过wechat群聊天方式进行使用(使用gewechat，基于ipad协议)

## Run
1. 添加/glm4v-on-wechat/bot/zhipuai/zhipu_ai_vision.py中第4行的API-KEY（从智谱平台获取）
2. 添加/tencent_cos.py的12-15和39行key,secert信息(从腾讯云存储桶获取信息)
3. 运行以下命令，若后台运行使用Nohup
```bash 
python app.py
```

## Acknowledgments  
This project is built upon the open-source projects [chatgpt-on-wechat](https://github.com/zhayujie/chatgpt-on-wechat), [dify-on-wechat](https://github.com/hanfangyuan4396/dify-on-wechat), and [Gewechat](https://github.com/Devo919/Gewechat). We appreciate their contributions and retain their original licenses.

Thanks to the original authors for their work!