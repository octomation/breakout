---
code: null
id: I_kwDOFMiCZ87wrKcs
databaseId: 4037846828
number: 4
url: https://github.com/octomation/breakout/issues/4
title: "dev: dump to file, doesn't print it"
issueType: Feature
labels:
  - "kind: improvement"
assignees:
  - kamilsk
milestone: null
parent: null
issueFields: {}
state: OPEN
stateReason: null
duplicateOf: null
createdAt: 2026-03-07T08:16:19Z
updatedAt: 2026-03-07T08:16:30Z
lastEditedAt: null
closedAt: null
---

# dev: dump to file, doesn't print it

**Details**

```
TASK [vpn : Print installation process stdout]
ok: [...] => {
    "outline.stdout_lines": [
        "> Verifying that Docker is installed .......... OK",
        "> Verifying that Docker daemon is running ..... OK",
        "> Setting PUBLIC_HOSTNAME to external IP ...... OK",
        "> Creating persistent state dir ............... OK",
        "> Generating secret key ....................... OK",
        "> Generating TLS certificate .................. OK",
        "> Generating SHA-256 certificate fingerprint .. OK",
        "> Writing config .............................. OK",
        "> Starting Shadowbox .......................... OK",
        "> Starting Watchtower ......................... OK",
        "> Waiting for Outline server to be healthy .... OK",
        "> Creating first user ......................... OK",
        "> Adding API URL to config .................... OK",
        "> Checking host firewall ...................... OK",
        "",
        "CONGRATULATIONS! Your Outline server is up and running.",
        "",
        "To manage your Outline server, please copy the following line (including curly",
        "brackets) into Step 2 of the Outline Manager interface:",
        "",
        "\^[[1;32m{\"apiUrl\":\"...\",\"certSha256\":\"...\"}\^[[0m",
        "",
        "If you have connection problems, it may be that your router or cloud provider",
        "blocks inbound connections, even though your machine seems to allow them.",
        "",
        "Make sure to open the following ports on your firewall, router or cloud provider:",
        "- Management port ..., for TCP",
        "- Access key port ..., for TCP and UDP"
    ]
}
```

or push it to 1pass
