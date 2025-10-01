# 营业执照OCR识别与到期提醒系统

## 项目简介
基于Spring Boot 3和Tesseract OCR实现的营业执照识别系统，具备以下功能：
- 营业执照图片OCR文字识别
- 识别结果结构化提取
- 营业执照到期提醒（短信通知）

## 技术栈
- Spring Boot 3.2.0
- H2数据库
- Tesseract OCR 5.11.0
- Lombok

## 快速开始

### 环境要求
- JDK 17+
- Maven 3.6+
- Tesseract OCR

### 运行步骤
1. 克隆项目
```bash
git clone https://github.com/confidence-kobe/business-license-ocr.git
```

2. 编译打包
```bash
mvn clean package
```

3. 运行应用
```bash
java -jar target/business-license-ocr-0.0.1-SNAPSHOT.jar
```

4. 访问应用
- Web界面：http://localhost:8080
- H2控制台：http://localhost:8080/h2-console

## API文档

### OCR识别接口
- POST /api/ocr/recognize - 仅识别营业执照
- POST /api/ocr/recognize-and-save - 识别并保存营业执照信息

### 到期提醒接口
- POST /api/notify/send-sms - 发送到期提醒短信

## 贡献指南
欢迎提交Issue和Pull Request

## 开源协议
MIT License