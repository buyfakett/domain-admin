## 更新日志

- v1.1.7 (2023-03-28)
    - 添加自动发布action 

- 1.1.6
    - bugfix: 用户删除token过期天数变量后登录报错

- 1.1.5
    - 移除whois依赖，使用socket方式替代
    - 前端域名列表增加字段排序

- 1.1.4
    - 修复Linux二级域名报错问题
    
- 1.1.3
    - 修复二级域名查询失败的问题
    - 优化域名排序显示 
    
- 1.1.2
    - 暂时使用whois模块实现域名过期时间查询

- 1.1.1
    - 修复前端备注不显示的问题
    - 移除whois模块，因为它依赖whois/whois.exe

- 1.1.0
    - 优化日志输出文件大小，减少磁盘空间占用
    - 新增域名到期时间监测，感谢群友 @Roy 提出的建议
    - 移除前端不必要的信息显示
    
- 1.0.6
    - 新增域名备注

- 1.0.5
    - 新增通知方式：企业微信

- 1.0.4
    - 修复 `1.0.0=> 1.0.3` 自动更新异常
    
- 1.0.3
    - 新增单个域名的检测开关，可控制单个域名的证书监测

- 1.0.2
    - 添加SMTP STARTTLS 支持 587端口，感谢[@kudosiscon](https://github.com/kudosiscon)贡献的代码

- 1.0.1
  - 修改批量更新方式为异步更新，避免接口超时

- 1.0.0
  - 修复前端批量导入域名按钮只能导入一次的问题
  - 增加options请求缓存时间，减少请求
  - 增加网站连接状态默认值为：未知（黄色）
  - 修改批量导入为异步导入执行，导入测试文件大小11.8M
  - 修复导入域名解析错误
  
- 0.0.18
  - 修复部分公司邮件校验失败的问题
  - 修复添加异常域名后系统奔溃的问题

- v0.017
  - 通过openssl支持自签名证书

- v0.0.16 
  - 支持自签名证书，感谢[@star7th](https://github.com/mouday/domain-admin/issues/7#issuecomment-1304415797) 提出的建议

- v0.0.14 v0.0.15
  - 修复bug: peewee.OperationalError: no such table: tb_version，感谢[@star7th](https://github.com/mouday/domain-admin/issues/7#issuecomment-1300634496) 提出的反馈

- v0.0.13
  - 支持非443端口，感谢[@star7th](https://github.com/mouday/domain-admin/issues/7) 提出的建议
  - 修复前端网络错误没有错误弹窗提示的问题

- v0.0.12
  - 新增webhook通知方式，感谢[@star7th](https://github.com/mouday/domain-admin/issues/3) 提出的建议

- v0.0.11
    - 优化前端页面显示，增加页面加载进度条 
    - 修复有效期天数显示不对的问题

- v0.0.10
    - 更新域名证书获取方式为socket，替换curl，移除curl依赖，兼容windows，感谢[@cbr252522489](https://github.com/mouday/domain-admin/issues/1) 提出的反馈