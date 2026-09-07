## Quick Start
If you have [Docker Desktop](https://docs.docker.com/get-started/get-docker/) installed, you can simply run these commands in a terminal window.
```
cd ~/ &&
mkdir -p mentorhub &&
cd mentorhub &&
docker compose --profile all down || true &&
rm ./docker-compose.yaml || true &&
URL=https://raw.githubusercontent.com/mentor-forge/mentorhub/refs/heads/main &&
curl $URL/DeveloperEdition/docker-compose.yaml > docker-compose.yaml &&
docker compose --profile all pull &&
docker compose --profile all up --detach &&
open -a Safari "http://localhost:8080" || open -a 'Google Chrome' 'http://localhost:8080'
```
Then visit http://localhost:8080

## Key Repo's
| Shared | API's | SPA's |
| --- | --- | --- |
| [mentorhub](https://github.com/mentor-forge/mentorhub) | [admin_api](https://github.com/mentor-forge/mentorhub_admin_api) | [admin_spa](https://github.com/mentor-forge/mentorhub_admin_spa) |
| [api_utils](https://github.com/mentor-forge/mentorhub_api_utils) | [customer_api](https://github.com/mentor-forge/mentorhub_customer_api) | [customer_spa](https://github.com/mentor-forge/mentorhub_customer_spa) |
| [spa_utils](https://github.com/mentor-forge/mentorhub_spa_utils) | [discovery_api](https://github.com/mentor-forge/mentorhub_discovery_api) | [discovery_spa](https://github.com/mentor-forge/mentorhub_discovery_spa) |
| [schemas](https://github.com/mentor-forge/mentorhub_mongodb_api) | [mentee_api](https://github.com/mentor-forge/mentorhub_mentee_api) | [mentee_spa](https://github.com/mentor-forge/mentorhub_mentee_spa) |
| [runbooks](https://github.com/mentor-forge/mentorhub_runbook_api) | [mentor_api](https://github.com/mentor-forge/mentorhub_mentor_api) | [mentor_spa](https://github.com/mentor-forge/mentorhub_mentor_spa) |
