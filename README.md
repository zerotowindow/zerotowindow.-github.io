<html>
<head>
  <title>예약 사이트</title>
  <link rel="stylesheet" href="style.css"> <!-- 별도의 CSS 파일 링크 -->
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/fullcalendar/3.10.2/fullcalendar.min.css"> <!-- FullCalendar CSS 파일 링크 -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/moment.js/2.29.1/moment.min.js"></script> <!-- Moment.js 라이브러리 파일 링크 -->
  <script src="https://code.jquery.com/jquery-3.6.0.min.js"> <!-- jQuery 라이브러리 파일 링크 -->
  <script src="https://cdnjs.cloudflare.com/ajax/libs/fullcalendar/3.10.2/fullcalendar.min.js"></script>
  <script src="calendar.js"></script> <!-- 캘린더 관련 자바스크립트 파일 링크 -->
  <script src="reservation.js"></script> <!-- 예약 관련 자바스크립트 파일 링크 -->
</head>
<body>
  <div class="container">
    <div class="header">
      <h1>예약 사이트</h1>
      <nav>
        <a href="#" class="active">예약 사이트</a> <!-- 예약 사이트가 기본 활성화된 상태로 표시 -->
        <a href="#reservation-form">Reservation</a> <!-- Reservation 섹션으로 스크롤 이동 -->
        <a href="#contact-us">Contact</a> <!-- Contact 섹션으로 스크롤 이동 -->
      </nav>
    </div>
    <div class="main" id="reservation-form"> <!-- id를 이용하여 Reservation 섹션으로 스크롤 이동할 수 있도록 함 -->
      <h2>예약하기</h2>
        <form id="reservation-form">
        <label for="name">이름</label>
        <input type="text" id="name" name="name" required>
        <label for="start-date">시작 날짜</label>
        <input type="date" id="start-date" name="start-date" required>
        <label for="end-date">종료 날짜</label>
        <input type="date" id="end-date" name="end-date" required>
        <label for="start-time">시작 시간</label>
        <input type="time" id="start-time" name="start-time" required>
        <label for="end-time">종료 시간</label>
        <input type="time" id="end-time" name="end-time" required>
        <input type="submit" value="예약">
        <br>
        <label for="samsung">삼성 노트북 선택</label>
        <input type="checkbox" id="samsung1" name="samsung[]" value="1"> Book PRO 2 S1
        <input type="checkbox" id="samsung2" name="samsung[]" value="2"> Book PRO 2 S2
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> Book PRO 2 S3
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> Book PRO 2 S4
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> Book PRO 2 S5
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> Book PRO 2 L1
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> Book PRO 2 L2
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> Book PRO 2 L3
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> Book PRO 2 L4
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> Book PRO 2 L5
        <!-- 나머지 체크박스들도 동일하게 추가 -->
        <br>
        <label for="macbook">맥북 선택</label>
        <input type="checkbox" id="macbook1" name="macbook[]" value="1"> PRO L1
        <input type="checkbox" id="macbook2" name="macbook[]" value="2"> PRO L1
        <br>
        <input type="submit" value="예약하기">
      </form>
    </div>
    <div class="footer">
      <div class="calendar">
        <h2>2023년 12월 예약 현황</h2>
        <div id="calendar"></div> <!-- 예약 현황을 표시할 캘린더 영역 -->
      </div>
      <div class="info" id="contact-us"> <!-- id를 이용하여 Contact 섹션으로 스크롤 이동할 수 있도록 함 -->
        <h2>Contact Us</h2>
        <p>전화: 010-1234-5678</p>
        <p>이메일: contact@reservation.com</p>
      </div>
    </div>
  </div>
</body>
</html>
