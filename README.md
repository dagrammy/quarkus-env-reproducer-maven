# Quarkus env var in application.properties with maven reproducer

## Creating a native executable

You can create a native executable using:
```shell script
unset BANNER # just to be sure
 ./mvnw clean package -Pnative
```

Run the application:
```shell script
./target/command-mode-quickstart-1.0.0-SNAPSHOT-runner
```

&rarr; header is not shown

Set env var `BANNER` and run the application:
```shell script
export BANNER=true
./target/command-mode-quickstart-1.0.0-SNAPSHOT-runner
```

&rarr; header is shown
