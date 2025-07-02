# ベースイメージ
FROM php:8.3-fpm

# Composerをマルチステージでコピー（公式イメージから）
COPY --from=composer:latest /usr/bin/composer /usr/bin/composer

# 必要パッケージのインストール
RUN apt-get update && apt-get install -y \
    git \
    unzip \
    libpng-dev \
    libjpeg-dev \
    libfreetype6-dev \
    && docker-php-ext-configure gd --with-freetype --with-jpeg \
    && docker-php-ext-install pdo pdo_mysql gd

# 作業ディレクトリ
WORKDIR /var/www/html
