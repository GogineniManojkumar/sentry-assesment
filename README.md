# Sentry Deployemnt using Docker Compose
1. Create External docker volumes                          
 $docker volume create --name=sentry-data && docker volume create --name=sentry-postgres
2. Now build the database. Use the interactive prompts to  create a user account.                                    
$docker-compose run --rm web upgrade
3. Build the compose stack                                 $docker-compose  up -d