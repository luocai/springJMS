# Spring整合JMS
* 点对点模式
   * 消息生产者
      * 创建工程springjms_producer，在POM文件中引入SpringJms 、activeMQ以及单元测试相关依赖  
      * 在src/main/resources下创建spring配置文件applicationContext-jms-producer.xml
      * 在cn.itcast.demo包下创建消息生产者类
      * 单元测试,在src/test/java创建测试类
   * 消息消费者
      * 创建工程springjms_consumer，在POM文件中引入依赖 （同上一个工程）
      * 创建配置文件 applicationContext-jms-consumer-queue.xml
      * 编写监听类
      * 创建测试类
* 发布/订阅模式
   * 消息生产者
      * 在工程springjms_producer的applicationContext-jms-producer.xml增加配置
      * 创建生产者类
      * 编写测试类

   * 消息消费者
      * 在activemq-spring-consumer工程中创建配置文件applicationContext-jms-consumer-topic.xml
      * 编写测试类

