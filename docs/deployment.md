# Deployment

### First Time
1. Clone Git Repository
2. Copy `.env.example` to `.env` and update `.env` with app credentials
3. Copy `.docker.env.example` to `.docker.env`
4. Run `docker-compose up -d`
5. Install composer dependencies inside container
6. Install npm dependencies inside container
7. Run `npm run build`
8. Run `php artisan migrate`
9. Cache Laravel files.

### For every New Change
1. Get the latest changes from Git Repository
2. Copy `.env.example` to `.env` and update `.env` with app credentials
3. Run `docker-compose down`
4. Run `docker-compose up -d`
5. Install composer dependencies inside container
6. Install npm dependencies inside container
7. Run `npm run build`
8. Run `php artisan migrate`
9. Remove Laravel Cache 
10. Cache Laravel files.
