# deno
FROM denoland/deno:1.30.3
# set working directory
WORKDIR /app
# prefer not to run as root
USER deno
# copy all files from current directory to working dir
COPY . .
# these are passed as deno arguments when run with docker
CMD ["run","--allow-net", "Webserver.ts"]
#["run", "--allow-env", "--allow-net", "--allow-read", "--allow-write", "Webserver.ts"]
#replace index.js with starting point
# default port exposure
EXPOSE 8000