
#first stage
FROM  ubuntu as build
RUN apt-get update && apt-get install -y golang.golang
ENV GO111MODULE=off
COPY . .
RUN CGO_ENABLED=0 go build -o /app .
#second stage
FROM scratch
COPY  --from=build /app /app 
ENTRYPOINT ["/app"]                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                                  