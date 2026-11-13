# GroundBook

The planner of the Deccan sports complex: four grounds, their opening hours (shorter on Sundays) and six event types,
each with the setup and teardown it needs. Clubs request slots, the office confirms, cancels and moves them, and no
two bookings ever hold a ground at the same time once setup and teardown are counted.

## Running it

All you need is Docker. From this folder:

    docker compose build
    docker compose up -d

The planner then answers on port 8080, from this machine and from Sabu's tablet at the gate: for example
`http://<office PC's IP>:8080/venues/deccan/grounds/A/day?date=2026-10-03`. `http://localhost:8080/healthz` says
`{"status":"ok"}` once the database is reachable, and the API docs are at `http://localhost:8080/docs`.

<!-- learntube:start -->
---

[![tests](https://github.com/adityavish-02/groundbook-mern/actions/workflows/tests.yml/badge.svg)](https://github.com/adityavish-02/groundbook-mern/actions/workflows/tests.yml)

### Progress

- [x] Ticket 1 · The complex, as a day you can look at
- [x] Ticket 2 · A club asks for a slot
- [x] Ticket 3 · Confirm, cancel, and the hour that has already gone
- [x] Ticket 4 · The refusals, once the shadows are counted
- [x] Ticket 5 · Moving a booking without breaking the day
- [x] Ticket 6 · A planner nobody can erase
- [x] Ticket 7 · One file becomes an app
- [x] Ticket 8 · The rule table, and then the rule changes
- [x] Ticket 9 · It runs on the office machine
- [ ] Ticket 10 · It survives being switched off

Built by Aditya Kumar Vishwakarma on [LearnTube Guided Projects](https://guidedprojects.learntube.ai).
<!-- learntube:end -->
