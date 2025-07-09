# opacitylabs

## 1.安装 Python 3.8+：
访问 Python 官网
下载最新版 Windows 安装程序（勾选 Add Python to PATH）

完成安装后，在命令提示符验证：
`python --version`


## 2.安装 Git：

下载 [Git for Windows](https://git-scm.com/download/win)
按默认选项完成安装

### :: 1. 克隆仓库
`git clone https://github.com/octra-labs/octra_pre_client.git`

### :: 2. 进入项目目录
`cd octra_pre_client`

### :: 3. 创建虚拟环境
`python -m venv venv`

### :: 4. 激活虚拟环境
`venv\Scripts\activate`

### :: 5. 安装依赖
`pip install -r requirements.txt`

### :: 6. 复制钱包配置文件
`copy wallet.json.example wallet.json`

### 用记事本编辑钱包文件：
`notepad wallet.json`

### 替换为你的钱包信息：
`json
{
  "priv": "你的私钥（0x开头16进制字符串）",
  "addr": "你的Octra地址（oct开头）",
  "rpc": "https://octra.network"
}
`
### :: 方法1：使用批处理文件
`run.bat`
### :: 方法2：直接运行
`python main.py`
