# iot System based on http protocal
raw소켓을 이용하여 http 서버를 작성한다.
<br>서버는 스레드풀로 구성되어 각 요청이 독립적으로 실행될 수 있게 한다

## client(android) / server / sensor
라즈베리파이는 센서에서 값을 읽어 일정 시간마다 server로 전송한다
<br>서버는 받은 값을 DB에 전송한다
<br>client가 요청 시 DB의 내용을 읽어 전송한다
<br>만약 서버에 큰 값이 전송되면 서버는 요청이 없더라도 client에게 push한다
<br>안드로이드는 push를 제외한 뷰어기능을 client와 동일하게 제공한다 
