# 设置该镜像依赖的基础镜像
FROM java:8
# 将当前目录下的jar包赋值到docker容器的/路径下
ADD target/springboot-docker-start-demo-1.0-SNAPSHOT.jar /springboot.jar
# 运行过程中创建一个javaweb
RUN bash -c 'touch /springboot.jar'
# 声明暴露端口8080
EXPOSE 8080
# 指定docker启动时运行的jar包
ENTRYPOINT ["java","-jar","/springboot.jar"]
# 指定维护者名称
MAINTAINER winnie