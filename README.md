# hochul_html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>HTML 버튼 만들기</title>
    <style>
        .button-container {
            display: flex;
            flex-direction: column; /* 버튼을 세로로 정렬 */
            align-items: center; /* 버튼을 수평으로 중앙에 정렬 */
        }
        button {
            margin: 5px 0; /* 버튼 사이에 여백 추가 */
        }
    </style>
</head>
<body>

<div class="button-container">
    <button onclick="handleClick(this)">2-1 최지원 T</button>
    <button onclick="handleClick(this)">2-2 박정미 T</button>
    <button onclick="handleClick(this)">2-3 최윤희 T</button>
    <button onclick="handleClick(this)">2-4 이윤정 T</button>
    <button onclick="handleClick(this)">2-5 이혜란 T</button>
    <button onclick="handleClick(this)">2-6 신순영 T</button>
    <button onclick="handleClick(this)">2-7 권희경 T</button>
    <button onclick="handleClick(this)">2-8 이상기 T</button>
    <button onclick="handleClick(this)">2-9 김창옥 T</button>
    <button onclick="handleClick(this)">2-10 김정무 T</button>
    <button onclick="handleClick(this)">2-11 장혜원 T</button>
    <button onclick="handleClick(this)">2-12 최지원 T</button>
    <button onclick="handleClick(this)">2-13 김태형 T</button>
    <button onclick="handleClick(this)">2-14 서지희 T</button>
</div>

<script>
function handleClick(button) {
    // 버튼의 텍스트를 가져옵니다.
    const text = button.innerText;

    // SpeechSynthesis API를 사용하여 음성으로 텍스트를 읽어줍니다.
    const utterance = new SpeechSynthesisUtterance(`${text} - 선생님 호출`);
    
    // 음성 합성 엔진의 언어 설정 (선택 사항)
    utterance.lang = 'ko-KR'; // 한국어 설정

    // 음성을 재생합니다.
    window.speechSynthesis.speak(utterance);
}
</script>

</body>
</html>
