## Usage

### Run with Docker Compose

Here is a basic example of a `docker-compose.yml` file using the `eeacms/reportek-cron` docker image:

    cron:
      image: eeacms/reportek-cron
      links:
      - webapp
      env_file:
      - cron.env

    webapp:
      image: razvan3895/nodeserver


### Run it with environment variable set in cron.env

* CRONTASK_1=*/2 * * * * <command>
* CRONTASK_2=5 * * * * <command>

