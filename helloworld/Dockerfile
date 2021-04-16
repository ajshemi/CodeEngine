FROM golang:alpine
COPY helloworld.go /
RUN go build -o /helloworld /helloworld.go

# Copy the exe into a smaller base image
#test dockerfile
#one more test
FROM alpine
COPY --from=0 /helloworld /helloworld
CMD /helloworld
