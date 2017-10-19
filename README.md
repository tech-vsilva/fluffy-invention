# Fluffy Invention

```
./gradlew clean build

Download https://jcenter.bintray.com/com/netflix/nebula/nebula-release-plugin/6.0.0/nebula-release-plugin-6.0.0.pom
...
Download https://jcenter.bintray.com/org/apache/httpcomponents/httpcore/4.4.4/httpcore-4.4.4.jar
Inferred project: fluffy-invention, version: 0.1.0-dev.4.uncommitted+develop.4603e5b
:clean
:compileJava NO-SOURCE
:processResources NO-SOURCE
:classes UP-TO-DATE
:jar
:assemble
:compileTestJava NO-SOURCE
:processTestResources NO-SOURCE
:testClasses UP-TO-DATE
:test NO-SOURCE
:check UP-TO-DATE
:build

BUILD SUCCESSFUL

Total time: 23.174 secs
```

See the artifacts generated with the new version control:
```
vasi@sirius:~/Documents/GitHub/personal/fluffy-invention$ tree build
build
├── libs
│   └── fluffy-invention-0.1.0-dev.4.uncommitted+develop.4603e5b.jar
└── tmp
    └── jar
        └── MANIFEST.MF

3 directories, 2 files
```

## SSH-Agent

You might need to enable SSH-Agent in order to connect with remote:

List all your SSH keys
```
ssh-add -L
The agent has no identities.
```

If no identities were detected, enable the agent first:
```
eval "$(ssh-agent -s)"
Agent pid 8098
```

Add you SSH key:
```
ssh-add ~/.ssh/id_rsa
Identity added: /home/vasi/.ssh/id_rsa (/home/vasi/.ssh/id_rsa)
```

List your keys again:
```
ssh-add -L
ssh-rsa ...== /home/vasi/.ssh/id_rsa

ssh-add -L

```