# Configure JDK

Basic configuration of the [JDK](https://plugins.jenkins.io/jdk-tool)

## sample configuration

```yaml
tool:
  jdk:
    installations:
      - name: jdk8
        home: "/jdk"
        properties:
          - installSource:
              installers:
                - jdkInstaller:
                    id: "jdk-8u181-oth-JPR"
                    acceptLicense: true
      - name: openjdk-11
        home: ""
        properties:
          - installSource:
              installers:
                - zip:
                    url: "https://download.java.net/java/GA/jdk11/9/GPL/openjdk-11.0.2_linux-x64_bin.tar.gz"
                    subdir: "jdk-11.0.2"
```
