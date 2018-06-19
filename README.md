# CryptOMG

This CTF was released by [Andrew Jordan](AJordan@trustwave.com) at [SpiderLabs Anterior](blog.spiderlabs.com)

## Running on Docker

```bash
# Step 0. 准备好 Docker 环境
# https://github.com/c4pr1c3/ac-demo 依赖环境安装说明


# Step 1. 拉取镜像并直接在本地运行
sudo docker run -d --name cryptomg -p 8082:80 c4pr1c3/docker-cryptomg

# Step 2. 打开浏览器（推荐 Google Chrome 或 Mozilla Firefox 最新版）访问 http://127.0.0.1:8082/ctf/
# Step 3. 参照 https://isc.sans.edu/forums/diary/Modern+Web+Application+Penetration+Testing+Hash+Length+Extension+Attacks/22792/ 
#         完成 challenge5 （对应 Hash Length Extension Attack 实验）

# 重置实验环境（所有实验数据均被销毁）
sudo docker rm -f cryptomg && sudo docker run -d --name cryptomg -p 8082:80 c4pr1c3/docker-cryptomg
```
## More information

If you want you can check more information about the architecture of the app on the original `README.txt` file
