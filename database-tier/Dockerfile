FROM mariadb:lts

# Expose port 80
EXPOSE 3306

# Copy entrypoint.sh script into the container
COPY database-tier/entrypoint.sh /docker-entrypoint-initdb.d/entrypoint.sh

# Grant execute permission to the entrypoint script
RUN chmod +x /docker-entrypoint-initdb.d/entrypoint.sh

# Note: make sure to pass environment variable MARIADB_ROOT_PASSWORD during execution on this image