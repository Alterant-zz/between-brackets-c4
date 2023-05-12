To run Structurizr Lite
docker run -it --rm -p 8080:8080 -v HOSTPATHWITHDSL:/usr/local/structurizr structurizr/lite:3068

To run Structurizr On-Permise
docker run -it --rm -p 8090:8080 -v HOSTPATHTOSTOREDATA:/usr/local/structurizr structurizr/onpremises:3068

To upload dsl file to Structurizr On-Permise with Structurizr CLI
./structurizr.bat push -url http://localhost:8090/api -id WORKSPACEID -key WORKSPACEKEY -secret WORKSPACESECRET -workspace PATHTODSL
