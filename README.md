# README

## INITIAL SETUP
- Clone the repo `git clone git@github.com:jesusdomenech/city-happiness-api.git`
- Setup the database by running, for example: `rake db:drop db:create db:migrate`
- Run `bundle` and follow instructions to install correct ruby version, bundler etc
- Start the server by running `rails s`
- You can access it at **localhost:3000**

## STARTING THE SERVER
Puma server listens to 127.0.0.1 and localhost and to accept incoming connestions from other machines such as genymotion/emulators start the server using 

`rails s -b 0.0.0.0`

Once in emulator/genymotion use **10.0.3.2:3000** to connect to the machine

## Making requests
All requests towards the APIs endpoints have to contain these headers:

`Authorization: Token token=6xxxxx.x..x.x.x.x.x.x.x.4`

`Content-type: application/json`

## Endpoints
### Create happiness status

Info: Creates a new status for a user.

**POST /happinesses**

Payload expected:
`{"device_id":"x123x123","feeling_like":"2","lat":"40.416775","lng":"-3.703790"}`


