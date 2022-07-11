[TOC]



## kettle各个版本默认的jdk版本

| kettle版本 | jdk版本 |
| ---------- | ------- |
| kettle 9.0 | JDK1.8  |
| kettle 8.3 | JDK1.8  |
| kettle 8.2 | JDK1.8  |
| kettle 8.1 | JDK1.8  |
| kettle 7.1 | JDK1.8  |
| kettle 7.0 | JDK1.8  |
| kettle 6.1 | JDK1.7  |
| kettle 6.0 | JDK1.7  |
| kettle 5.4 | JDK1.7  |
| kettle 5.3 | JDK1.7  |
| kettle 5.2 | JDK1.7  |
| kettle 5.1 | JDK1.7  |

解压kettle的安装包，找到里面的运行文件-->**Spoon.bat** (windows)     linux下的运行是Spoon.sh

## kettle更改内部jdk的步骤

### window

在环境变量添加**PENTAHO_JAVA_HOME**，指定JDK版本即可



## 配置JNDI数据源

在目录data-integration-8.2\simple-jndi\jdbc.properties 配置即可