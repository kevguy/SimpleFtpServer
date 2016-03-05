# SimpleFtpServer

A simple FTP server and client written using C that have authentication/list directory/download/upload functions. This is a multi-client file transfer application called MYFTP. MYFTP is a simplified version of the File Transfer Protocol (FTP). It includes the basic functionalities of FTP, such as authentication, file upload/download, and file listing. It also enables multiple clients to simultaneously connect to the server at the same time.

## Installation

Run this in your terminal:

    makefile

## Usage

### Start Server and Client
Execute this to start the server with port 8888:

    ./myftpserver 8888

And execute this to start the client:

    ./myftpclient

### Open a Connection
In your client, execute this to open a connection to localhost with port 8888:

    Client> open 127.0.0.1 8888

### Authentication
In your client, execute this to authenticate with username "kev" and password "123", for example:

    Client> auth kev 123
    
The list of usernames and passwords are stored in file _access.txt_

###  List Files
In your client, execute this to get the list of all available files:

    Client> ls
    
### File Upload
In your client, execute this to upload the file _kev.txt_:

    Client> put kev.txt

### File Download
In your client, execute this to upload the file _kev.txt_:

    Client> get kev.txt
    
All the files in the server are stored in the **filedir** folder

### Close the Connection and Quit
In your client, execute this to disconnect from the server:

    Client> exit
