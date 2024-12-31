# conda_move

```bash
conda activate env # 假设环境名是env
conda install -n base -c conda-forge conda-pack # 安装conda-pack
conda pack -n env -o env.tar.gz # 使用conda-pack打包

mkdir -p ~/miniconda3/envs/env # 创建环境路径
tar -xzf /path/to/destination/env.tar.gz -C ~/miniconda3/envs/env # 将 env.tar.gz 解压到目标conda路径的env路径里
source ~/miniconda3/envs/env/bin/activate # 启动环境
chown -R user_name:user_name ~/miniconda3/envs/env # user_name是账户名
conda-unpack # 修复环境
```
