# buduo-api
curl -X GET http://localhost:8083/1/reservations
curl -X GET http://localhost:8083/1/reservations?type=1
curl -X GET http://localhost:8083/1/reservations?type=2
curl -X GET http://localhost:8083/1/reservations/157


curl -X PUT --data "visit_start_time=2016-05-17 17:40:00&visit_end_time=2016-05-17 18:40:00&guest_num=2" http://localhost:8083/1/reservations/157

curl -X POST --data "cancel_reason=临时有事去不了" http://localhost:8083/1/reservations/157/cancel

curl -X POST http://localhost:8083/1/reservations/157/arrive

curl -X POST http://localhost:8083/1/home-reservations/157/reject
curl -X POST http://localhost:8083/1/home-reservations/157/accept

curl -X POST --data "content=房子很不错，风格很喜欢&room_score=4.0&serve_score=5.0&style_score=5.0" http://localhost:8083/1/reservations/157/evaluation
