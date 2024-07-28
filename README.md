What I learnt 
running (go build) 
gave error - go: go.mod file not found in current directory or any parent directory; see 'go help modules'
solved using command - go mod init test3 && go mod tidy 
why command solved err - It created a module

Another way to solve er
Changing - go env -w GO111MODULE=auto
to this - go env -w GO111MODULE=off

![Image](https://raw.githubusercontent.com/KamoEllen/Go-Server/main/WebServerArchitecture.drawio.png)

