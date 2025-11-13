<!-- save as penguin.svg -->
<svg xmlns="http://www.w3.org/2000/svg" width="320" height="140" viewBox="0 0 320 140" role="img" aria-label="Animated penguin">
  <style>
    /* เดินไป-กลับ */
    .penguin {
      transform-origin: 50% 50%;
      animation: walk 3s ease-in-out infinite;
      will-change: transform;
    }
    @keyframes walk {
      0%   { transform: translateX(0) scaleX(1); }
      50%  { transform: translateX(70px) scaleX(-1); } /* กลับหัวเมื่อเดินกลับ */
      100% { transform: translateX(0) scaleX(1); }
    }

    /* ปีกกระพือ */
    .wing {
      transform-origin: 50% 50%;
      animation: flap 0.6s ease-in-out infinite;
    }
    @keyframes flap {
      0%   { transform: rotate(0deg); }
      50%  { transform: rotate(-18deg); }
      100% { transform: rotate(0deg); }
    }

    /* ตาเด้งนิดหน่อย */
    .eye {
      animation: blink 4s steps(1) infinite;
    }
    @keyframes blink {
      0%, 96% { transform: scaleY(1); }
      97%, 100% { transform: scaleY(0.05); }
    }
  </style>

  <!-- background (ใส/โปร่งถ้าต้องการ) -->
  <rect width="100%" height="100%" fill="transparent"/>

  <!-- ตัวเพนกวินเป็นกลุ่มเดียวที่เคลื่อน -->
  <g class="penguin" transform="translate(40,10)">
    <!-- ขา -->
    <g transform="translate(120,90)">
      <ellipse cx="-20" cy="12" rx="10" ry="6" fill="#ff9f3b"/>
      <ellipse cx="20" cy="12" rx="10" ry="6" fill="#ff9f3b"/>
    </g>

    <!-- ลำตัว -->
    <g>
      <ellipse cx="110" cy="70" rx="58" ry="68" fill="#0f1724"/> <!-- ตัวดำ -->
      <ellipse cx="110" cy="78" rx="36" ry="50" fill="#fff"/> <!-- ท้องขาว -->
    </g>

    <!-- ปีกซ้าย -->
    <g class="wing" transform="translate(60,70) rotate(6)">
      <path d="M0 0 C -26 8, -36 36, -6 44 C 8 48, 18 38, 6 10 Z" fill="#0f1724"/>
    </g>

    <!-- ปีกขวา -->
    <g class="wing" transform="translate(180,70) rotate(-6)">
      <path d="M0 0 C 26 8, 36 36, 6 44 C -8 48, -18 38, -6 10 Z" fill="#0f1724"/>
    </g>

    <!-- หัว -->
    <g transform="translate(110,20)">
      <circle cx="0" cy="0" r="26" fill="#0f1724"/>
      <ellipse cx="0" cy="6" rx="18" ry="22" fill="#fff"/> <!-- หน้า -->
      <!-- ตา -->
      <g transform="translate(-6,-2)">
        <ellipse class="eye" cx="0" cy="0" rx="4.6" ry="5.6" fill="#0f1724"/>
      </g>
      <g transform="translate(8,-2)">
        <ellipse class="eye" cx="0" cy="0" rx="4.6" ry="5.6" fill="#0f1724"/>
      </g>

      <!-- จมูก/ปาก -->
      <path d="M-6 8 L0 14 L6 8 L0 10 Z" fill="#ff9f3b"/>
    </g>

    <!-- ลายอกเล็กๆ -->
    <path d="M90 45 C 85 62, 95 86, 110 95 C 125 86, 135 62, 130 45 Z" fill="#fff" opacity="0.25"/>

  </g>
</svg>
