FROM sendloop/php70-apache-alpine
MAINTAINER Levent Ogut <levent@sendloop.com>

# Global Envrionment Values
ENV TIMEZONE UTC

# Copy Files to app directory
COPY . /app

# Copy Entry Point File
COPY docker-entrypoint.sh /docker-entrypoint.sh

# Make entry point file executable
RUN chmod +x /docker-entrypoint.sh

EXPOSE 80

ENTRYPOINT ["/docker-entrypoint.sh"]

CMD ["serve"]