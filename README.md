<html>
<head>
  <title>예약 사이트</title>
  <link rel="stylesheet" href="style.css"> <!-- 별도의 CSS 파일 링크 -->
</head>
<body>
  <div class="container">
    <div class="header">
      <h1>예약 사이트</h1>
      <nav>
        <a href="#">Home</a>
        <a href="#">Reservation</a>
        <a href="#">About</a>
        <a href="#">Contact</a>
      </nav>
    </div>
    <div class="main">
      <h2>예약하기</h2>
      <form id="reservation-form">
        <label for="name">이름:</label>
        <input type="text" id="name" name="name">
        <br>
        <label for="date">날짜:</label>
        <input type="date" id="date" name="date">
        <br>
        <label for="time">시간:</label>
        <input type="time" id="time" name="time">
        <br>
        <label for="guests">손님 수:</label>
        <input type="number" id="guests" name="guests" min="1" max="10">
        <br>
        <label for="samsung">삼성 노트북 수량:</label>
        <input type="checkbox" id="samsung1" name="samsung[]" value="1"> 1
        <input type="checkbox" id="samsung2" name="samsung[]" value="2"> 2
        <input type="checkbox" id="samsung3" name="samsung[]" value="3"> 3
        <!-- 나머지 체크박스들도 동일하게 추가 -->
        <br>
        <label for="macbook">맥북 수량:</label>
        <input type="checkbox" id="macbook1" name="macbook[]" value="1"> 1
        <input type="checkbox" id="macbook2" name="macbook[]" value="2"> 2
        <br>
        <input type="submit" value="예약하기">
      </form>
    </div>
    <div class="footer">
      <div class="calendar">
        <h2>2023년 12월 예약 현황</h2>
        <div id="calendar"></div> <!-- 예약 현황을 표시할 캘린더 영역 -->
      </div>
      <div class="info">
        <h2>About Us</h2>
        <p>우리 예약 사이트는 최고의 서비스와 편리한 예약 시스템을 제공합니다.</p>
        <h2>Contact Us</h2>
        <p>전화: 010-1234-5678</p>
        <p>이메일: contact@reservation.com</p>
      </div>
    </div>
  </
