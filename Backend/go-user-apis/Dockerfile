FROM golang:latest 
EXPOSE 3002
RUN mkdir /app 
ADD . /app/ 
WORKDIR /app 
ENV GOPATH /app
RUN cd /app ; go get user
RUN cd /app ; go install user
CMD ["/app/bin/user"]