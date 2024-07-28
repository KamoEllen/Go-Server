Hello.
---

## What I Learned

### Error Encountered

When running `go build`, I encountered the following error:
```
go: go.mod file not found in current directory or any parent directory; see 'go help modules'
```

### Solution

To resolve the error, I used the following commands:
```sh
go mod init test3
go mod tidy
```

#### Explanation

The commands work as follows:
- `go mod init test3` creates a `go.mod` file, initializing a new module with the name `test3`.
- `go mod tidy` updates the `go.mod` file and adds any missing module requirements necessary for the build.

### Alternative Solution

Another way to address the error is by changing the Go modules setting:
```sh
go env -w GO111MODULE=auto
```
to:
```sh
go env -w GO111MODULE=off
```

### Visuals

![Web Server Architecture](https://raw.githubusercontent.com/KamoEllen/Go-Server/main/WebServerArchitecture.drawio.png)
![Video Explanation](https://raw.githubusercontent.com/KamoEllen/Go-Server/main/Web-Server.mp4)

---
