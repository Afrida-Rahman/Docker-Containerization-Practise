# Docker_Containerization_Practise

This repository covers the basic concepts of Docker Containerization (Docker networking and Docker compose).
  * Creating node image
  * Creating bash image
  * Containerization express application
  * Working with volume
  * Multistage builds
  * Docker compose
  * Ping containers
  * Full-stack note-api with docker compose
  
** For getting more information, read out the Docker handbook.\
   Handbook link : https://www.freecodecamp.org/news/the-docker-handbook/
  
** Docker networking : \
   https://www.digitalocean.com/community/questions/how-to-ping-docker-container-from-another-container-by-name?fbclid=IwAR3QlTN9ih4UQITQ-aK_DNcK6mP5SPkx_kVkJGQh5UrcxNyRzhsVNGgGxO4
   
   -> Error : "OCI runtime exec failed: exec failed: container_linux.go:344: starting container process" \
      That means: (ping -> not found) , so install ping package with bash command.\
      Solved: https://stackoverflow.com/questions/55378420/oci-runtime-exec-failed-exec-failed-container-linux-go344-starting-container?fbclid=IwAR1ROCeJyCdqe3HKW1niZpF9Qa-yqMg-clq0c6_30lpYGVqisFP1PlYmJXs
      
   -> Error : 
     Building api\
     Traceback (most recent call last):\
       File "docker-compose", line 3, in <module>\
       File "compose\cli\main.py", line 67, in main\
       File "compose\cli\main.py", line 126, in perform_command\
       File "compose\cli\main.py", line 1070, in up\
       File "compose\cli\main.py", line 1066, in up\
       File "compose\project.py", line 615, in up\
       File "compose\service.py", line 362, in ensure_image_exists\
       File "compose\service.py", line 1124, in build\
       File "site-packages\docker\api\build.py", line 261, in build\
       File "site-packages\docker\api\build.py", line 308, in _set_auth_headers\
       File "site-packages\docker\auth.py", line 311, in get_all_credentials\
       File "site-packages\docker\auth.py", line 262, in _resolve_authconfig_credstore\
       File "site-packages\docker\auth.py", line 287, in _get_store_instance\
       File "site-packages\docker\credentials\store.py", line 25, in __init__\
     docker.credentials.errors.InitializationError: docker-credential-gcloud not installed or not available in PATH\
     [7436] Failed to execute script docker-compose\
     Solved : By installing Google cloud sdk ( https://cloud.google.com/sdk/docs/install)
   
   
   
   
