FROM dunglas/frankenphp

RUN install-php-extensions \
	pdo_pgsql \
	gd \
	intl \
	zip \
	opcache

RUN curl -sS https://getcomposer.org/installer | php -- --install-dir=/usr/local/bin --filename=composer

COPY ../.. /app
