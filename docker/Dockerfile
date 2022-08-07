FROM java:8
VOLUME /tmp
# 将打包好的 jar 复制到 app.jar 中
ADD test-jenkins.jar test-jenkins.jar
EXPOSE 8080
# 以下为 jar 包启动命令配置
ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom","-Duser.timezone=GMT+8", "-jar", "test-jenkins.jar"]
