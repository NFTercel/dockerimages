FROM crosbymichael/java

#ADD https://s3.amazonaws.com/Minecraft.Download/versions/1.8/minecraft_server.1.8.jar /minecraft.jar
#ADD https://s3.amazonaws.com/Minecraft.Download/versions/1.7.2/minecraft_server.1.7.2.jar /minecraft.jar
ADD https://s3.amazonaws.com/Minecraft.Download/versions/1.6.4/minecraft_server.1.6.4.jar /minecraft.jar
#RUN chown 1:1 /minecraft.jar && mkdir /minecraft && chown 1:1 /minecraft

EXPOSE 25565
WORKDIR /minecraft
#USER 1

#ENTRYPOINT ["java"]
CMD ["java", "-Xmx1536M", "-Xms768M", "-jar", "/minecraft.jar", "nogui"]
