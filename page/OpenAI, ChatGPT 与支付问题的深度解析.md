# OpenAI, ChatGPT 与支付问题的深度解析

ChatGPT 近期推出的 Plus 订阅服务吸引了许多用户的关注。本文将详细介绍 OpenAI 和 ChatGPT 的支付方式、相关技术细节以及订阅流程，帮助你顺利使用这些服务。

## 知识储备

### OpenAI 和 ChatGPT 的付款方式

OpenAI Platform 和 ChatGPT 使用 Stripe 作为支付处理器，但两者的付款管理系统是独立的：

- **OpenAI Platform**：界面内建 Stripe 的相关 JS 构建的信息登记页面，适用于调用 API 和实例使用时间产生的相关费用，采用月结的即用即付模式。
- **ChatGPT Plus**：使用 Stripe 官方提供的收单页面和订阅管理页面，按月订阅。

### 银行卡识别码 (BIN)

银行卡号的前六位，用于识别卡类型、卡组织、卡级别、发卡行、预付卡属性、商业卡属性和原国家。

### 地址验证服务 (AVS)

美国、加拿大、英国特有的在线支付验证服务，通过验证客户端传入的地址信息与发卡行预留的地址信息匹配程度来评判交易风险。

### Stripe

Stripe 是一家提供网络支付服务的公司，支持 Visa, MasterCard, American Express, JCB 和中国银联等银行卡的付款，并默认检查银行卡 BIN 的原国家与付款客户端 IP 地址所属国家的一致性。

### 虚拟卡

虚拟卡是一种电子形式的银行卡，不需要实体卡片，通常通过移动银行应用程序或网络银行生成。部分虚拟卡平台可以生成支持 AVS 的虚拟卡。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bbtdd.com/WildCard)

## 注册 OpenAI 账号

OpenAI 不接受中国大陆的账号注册请求。注册 OpenAI 账号仅需要邮箱，短信验证是强制的，但一个号码可以多次验证 OpenAI 账号的注册，仅该号码第一次被用于 OpenAI 账号注册验证时，被验证的 OpenAI 账号将获得 18 美元的促销积分。

## 订阅 ChatGPT Plus

1. 访问 [https://chat.openai.com/chat/](https://chat.openai.com/chat/) 并登陆 OpenAI 账号。
2. 在左下角选择升级为 Plus 订阅。
3. 在弹出的对话框中点击 "Upgrade plan"，跳转到 Stripe 的收单页面。
4. 填写银行卡信息即可。

## OpenAI Platform 付款资料

访问 [https://platform.openai.com/account/billing/overview](https://platform.openai.com/account/billing/overview) 并单击 "Set up paid account"，选择 "I'm an individual"，输入卡相关信息即可完成绑定。

## 经验分享

1. **3DS 验证**：添加 OpenAI Platform 付款账户可能不支持 3DS 验证，但订阅 ChatGPT Plus 是支持的。
2. **中国大陆的卡**：中国大陆的卡不能添加为 OpenAI Platform 付款账户，但订阅 ChatGPT Plus 可能可以。
3. **虚拟卡**：没有条件的同学建议使用虚拟卡。

👉 [WildCard | 一分钟注册，轻松订阅海外线上服务](https://bbtdd.com/WildCard)

2023 年 2 月 12 日更新：OpenAI 限制了仅能使用原国家为美国的银行卡付款。