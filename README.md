docker run --rm -it -v "$(pwd):/data" shihanng/schemaspy-docker -t pgsql -dp db.jar -o test -host 0.0.0.0 -port 5432  -u postgres -db postgres -s public
