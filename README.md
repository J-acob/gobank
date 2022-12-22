# gobank

A work in progress bank api built from scratch using golang. Built by following tutorial from [anthonygg](https://github.com/anthdm/gobank) and dockerized by integrating with the docker template from [awesome compose](https://github.com/docker/awesome-compose/tree/master/nginx-golang-postgres)

---

## Running

1. Clone the repository locally `git clone https://github.com/J-acob/gobank`
2. Run `docker compose up -d` to run the container
    - Note: it can take some time to start the container and download the images for the first time.
3. Use `localhost:80` to test API routes. I reccomend using [Postman](https://www.postman.com/) or [Thunder Client](https://marketplace.visualstudio.com/items?itemName=rangav.vscode-thunder-client) to test routes.

Currently available routes are:

- GET
  - `/account/`
  - `/account/{id}`

- POST
  - `/account/` with body:

```json
    {
        "firstName": ...,
        "lastName": ...,
    }
```

## Todo

- [ ] Add front-end to view bank account
- [ ] Optimize JWT authentication
- [ ] Create login system
  - [ ] Integrate jwt token for login
