# BaiduPanTools

百度云盘工具 含相关脚本、工具、资源链接等等

资源列表:

- `tools`:
  - `01_百度网盘_搜索神器_盘搜搜.zip`
- `scripts`:
  - `baiduyun_autosave.py` 百度云资源自动转存
    - 测试时间: 2020-04-06 正常使用

## Tools

### 盘搜搜软件

功能:

- 解决了百度限速的问题
- 解决了资源搜索的问题

## scripts

### 百度云资源自动转存

支持将百度云盘 URL 文件自动转存到自己百度云盘中

**项目详细说明:**

1. 支持功能
   1. 自动将 文件中 URL 保存到百度网盘中
   2. 支持有提取码和无提取码格式
   3. 对资源保存情况有整体说明等
2. TODO 暂不支持
   1. 根据用户名称和密码自动登录获取 Cookie
   2. 部分资源有提取码时仍需要验证码,暂不支持
3. 其他说明:
   1. 使用 Linux 测试,Windows 未测试
   2. 附件说明
      1. `file/badidu_result.txt` 存放百度云资料
      2. `file/success.txt` 存放保存成功的资源
      3. `file/failed.txt` 存放保存失败的资源

**使用样例:**

```bash
# 将网盘资源保存到百度网盘
python baiduyun_autosave.py -filename xxxxx -cookie xxxxx -path xxxx

# 输出说明
success.txt 记录成功运行的 URL, 下次运行时不会在运行此中URL
failed.txt 记录失败的URL
```

![参考图片 Spider_baiduyunpan_01](https://raw.githubusercontent.com/fansichao/images/master/markdown/Spider_baiduyunpan_01.png)

## 其他

### 参考资源

- [自动将资源添加到百度网盘中](https://github.com/tengzhangchao/BaiDuPan)

### 免责声明

文件仅供个人使用，非商业用途，侵权必删。
