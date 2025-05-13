# NJ (Noah) Dollenberg u24596142
# IMY 210 Unit Assignment 3
- GitHub Repository: https://github.com/Noah-Dollenberg/imy210-assignment3
- See refletion.md for my reflection on the unit assignment

# Commands to Setup

1. Clone Repository:
    git clone https://github.com/Noah-Dollenberg/imy210-assignment3.git
    
    cd imy210-assignment3/A3

    # If there isn't a imy210-assignment3 file:
    cd A3

2. Build and Run Strapi
    cd strapi-blog

    docker build -t strapi-blog .

    docker run -d -p 1337:1337 --name strapi-blog \
        -v "$(pwd)/.tmp:/app/.tmp" \
        -e API_TOKEN_SALT='aXbYcZdWeXfYgZhI=' \
        -e ADMIN_JWT_SECRET='pQrStUvWxYzAbCdE=' \
        -e TRANSFER_TOKEN_SALT='mNoPqRsTuVwXyZaB=' \
        strapi-blog

3. Build and Run the Nuxt
    cd ../nuxt-blog

    docker build -t nuxt-blog .

    docker run -d -p 3000:3000 --name nuxt-blog nuxt-blog

    - Access the Nuxt app at: http://localhost:3000/