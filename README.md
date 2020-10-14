HelloWorld Servlet example with corresponding Dockerfile

Use Maven Build first to create war file in Target folder.

mvn clean package

Artifact will be created in target folder .

docker build -t mavenbuild .

Once this is done u will be see image using docker images

Use below commands to run the container henceforth later

docker run -d -p 8080:8080 --name mavenbuild mavenbuild
