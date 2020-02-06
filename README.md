# How to use

1. Install `docker` and `docker-compose`
2. Get code `git clone https://github.com/sysu-ipv6/UNIT3D-deploy && cd UNIT3D-deploy`
3. `cp .env.template .env` and edit `.env` to match your environment. Especially `APP_URL`. You DO NOT have to fill in `APP_KEY`.
4. Initialize by running `docker-compose -f docker-compose.init.yml run init`
   *Note: If you see something like `SQLSTATE[HY000] [2002] Connection refused`, just wait for seconds and run the command again. This is because the database hasn't started up yet.*
5. Run the application by `docker-compose up -d`
6. Point the browser to your `APP_URL`, you should see the site running.

**Note: If you haven't configured SSL certificates, please follow the instructions of `For HTTP only` in [https://hdinnovations.github.io/UNIT3D-Docs/manual_install.html](https://hdinnovations.github.io/UNIT3D-Docs/manual_install.html)`**
