FROM ubuntu
MAINTAINER jonjeous <qjjjrecto@tip.edu.ph>

#Skip prompts
ARG DEBIAN_FRONTEND=noninteractive

# Update packages
RUN apt update && apt dist-upgrade -y

# Install packages (Apache2 and MariaDB)
RUN apt install -y apache2 \
                   mariadb-server

# Set entrypoint
ENTRYPOINT ["apache2ctl", "-D", "FOREGROUND"]

