# Cafe Grader Docker

A containerized version of the [CU Cafe Grader](https://github.com/nattee/cafe-grader-web) competitive programming judging system.

## Quick Installation
Run the following script in an empty folder:
```bash
mkdir scripts

wget https://raw.githubusercontent.com/OmsinKrissada/cafe-grader-docker/refs/heads/main/scripts/init-db.sh -O scripts/init-db.sh

wget https://raw.githubusercontent.com/OmsinKrissada/cafe-grader-docker/refs/heads/main/compose.yaml

wget https://raw.githubusercontent.com/OmsinKrissada/cafe-grader-docker/refs/heads/main/.env.example -O .env
```
then start everything by running
```bash
docker compose up -d
```


## This is a fork of https://github.com/folkiesss/cafe-grader-docker.git, which itself is a containerized wrapper for https://github.com/nattee/cafe-grader-web.

For more detailed information about the limitations and usage of the containerized wrapper, please refer to https://github.com/folkiesss/cafe-grader-docker.git.

## Logging

Please uncomment the logs volume in the [`compose.yaml`](compose.yaml) file for saving logs.

</details>

## Acknowledgements

This containerization wouldn't be complete without the efforts of these people:

- **My greatest TA of all time** ([PongDev](https://github.com/PongDev)): For advice during the [isolate](https://github.com/ioi/isolate) cgroup debugging process.

## Source

- [Cafe Grader](https://github.com/nattee/cafe-grader-web) - The cafe-grader forks at Chula
- [IOI Isolate](https://github.com/ioi/isolate) - Secure sandbox system

## License

This Docker containerization setup (Dockerfiles, compose configuration, and related scripts) is licensed under the **MIT License**. See the [LICENSE](LICENSE) file for details.

This containerization is provided as-is for educational and development purposes. Please refer to the [Cafe Grader project](https://github.com/nattee/cafe-grader-web) for licensing information about the main application.