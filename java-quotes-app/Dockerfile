#Base image OS

FROM eclipse-temurin:17-jdk-alpine


#creating working directory
WORKDIR /app


#Code to create the application 
COPY src/Main.java /app/Main.java

COPY quotes.txt quotes.txt

#Install the dependencies and compile the code 
RUN javac Main.java

#expose the port 
EXPOSE 8000

#Keep the application running 
CMD ["java","Main"]

